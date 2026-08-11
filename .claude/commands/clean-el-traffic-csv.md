---
name: clean-el-traffic-csv
description: Pulisce un file CSV non elaborato relativo al traffico Experience League/Adobe Analytics da esportare in pagine solo Workfront, ordinate in base alle visualizzazioni di pagina. Da utilizzare quando l’utente fornisce un CSV del traffico pagina di Experience League (colonne come "URL della pagina generico", "Visitatori univoci", "Visite", "Visualizzazioni pagina") e chiede di pulirlo, filtrarlo o elaborarlo, oppure cita i fogli di calcolo di "tracciamento della documentazione"/"articoli più visualizzati".
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# Pulisci CSV traffico Experience League

Trasforma un’esportazione non elaborata della tabella a forma libera Adobe Analytics del traffico di pagina di Experience League in un file CSV deduplicato, pulito e solo per Workfront, ordinato in base alle visualizzazioni di pagina, sovrascrivendo il file originale e salvando una copia datata sul desktop.

## Forme di input

L&#39;input può essere costituito da una delle due forme seguenti:

1. **Esportazione non elaborata** — inizia con le righe di commento dei metadati (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"`, ecc.), seguite da una tabella gerarchica di suddivisione (ad esempio `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → singole righe di URL). La cella letterale `Page URL Generic (v33)` (o un&#39;etichetta `Page URL Generic ...` simile) viene visualizzata in parte giù nella seconda colonna.
2. **CSV già pulito**. La prima riga è già un&#39;intestazione semplice come `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, senza righe di metadati o colonne iniziali aggiuntive.

Rileva quale forma si ha prima di iniziare: se la riga 1 è una riga di intestazione semplice che corrisponde alla forma 2, salta direttamente al passaggio 2 (non sarà disponibile alcun intervallo di date, quindi salta anche il passaggio 7 a meno che l’utente non fornisca un intervallo di date separatamente).

## Flusso di lavoro

### Passaggio 0: acquisisci l’intervallo di date (solo esportazione non elaborata, prima di eliminare qualsiasi cosa)

Trovare la riga dei metadati vicino alla parte superiore corrispondente di `# Date: <range>` (esempio: `"# Date: Jul 1, 2026 - Jul 31, 2026"`). Record `<range>` (ad esempio `Jul 1, 2026 - Jul 31, 2026`) — necessario più avanti nel passaggio 7. Eseguire questa operazione prima di eliminare le righe.

### Passaggio 1: riduci l’esportazione non elaborata a una tabella semplice (solo esportazione non elaborata)

1. Trovare la riga contenente la cella `Page URL Generic (...)` (nella seconda colonna dell&#39;esportazione standard).
2. Elimina ogni riga al di sopra di tale riga, incluse le righe dei commenti dei metadati e le righe dei subtotali `Solution (v2)` / `workfront`.
3. Eliminare ogni colonna a sinistra della cella `Page URL Generic` (nell&#39;esportazione standard questa è solo la colonna A).
4. Sulla stessa riga (ora riga di intestazione), sostituire i valori dei subtotali numerici a destra di `Page URL Generic (...)` con le intestazioni letterali, nell&#39;ordine: `Unique Visitors`, `Visits`, `Page Views`. Lasciare la cella `Page URL Generic (...)` invariata.

Risultato: un file CSV semplice con intestazione `Page URL Generic (v33),Unique Visitors,Visits,Page Views` seguito da una riga per URL.

### Passaggio 2: mantenere solo le righe Workfront

Per ogni riga di dati, verificare se l&#39;URL contiene la sottostringa letterale `/workfront/` (barra su entrambi i lati). Il prefisso delle impostazioni internazionali non ha importanza (`/en/`, `/zh-hans/`, ecc. — rimangono tutti fintanto che il segmento di prodotto corrisponde).

- Eliminare la riga se l&#39;URL **non** contiene `/workfront/` come segmento del percorso. In questo modo verranno rimossi altri prodotti come `workfront-fusion`, `workfront-learn`, `proofhqpapi` e così via (una sottostringa come `tutorials-workfront` contiene **non** conteggio; la corrispondenza deve essere esattamente il segmento `/workfront/`).
- In caso contrario, conserva la riga.

### Passaggio 3: ritagliare l’URL

Per ogni riga superstite, trovare `/using` nell&#39;URL e mantenere solo la parte da `/` che la segue (inclusa), ignorando tutto ciò che precede e include `/using`.

Esempio: `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

Se `/using` non viene trovato nell&#39;URL di una riga Workfront, lasciare invariato tale URL e contrassegnarlo per l&#39;utente anziché indovinarlo.

### Passaggio 4: suffissi di frammento di striscia/query

Se l&#39;URL ritagliato contiene `#` o `?`, eliminare il carattere e tutto ciò che segue.

Esempio: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Passaggio 5: unire i duplicati

Dopo il ritaglio, più righe possono ora condividere lo stesso URL (ad esempio, due righe delle impostazioni internazionali diverse che si riducono allo stesso percorso). Combinare tutte le righe con un URL identico in una riga, sommando `Unique Visitors`, `Visits` e `Page Views` in modo indipendente.

Esempio: `/home,2,2,3` e `/home,5,6,7` → `/home,7,8,10`

### Passaggio 6: ordinare per visualizzazioni pagina

Ordina tutte le righe di dati per `Page Views` in ordine decrescente (prima la più grande). La riga di intestazione rimane fissa nella parte superiore, sopra i dati ordinati.

### Passaggio 7: aggiungi la riga dell’intervallo di date (solo esportazione non elaborata, se acquisita nel passaggio 0)

Prima di inserirlo, elimina eventuali virgole dall&#39;intervallo di date acquisito (ad esempio `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`). L&#39;intervallo non elaborato contiene virgole che altrimenti verrebbero lette in modo errato come separatori di colonna CSV sulla riga.

Inserisci una nuova riga nella parte superiore, sopra la riga di intestazione, contenente solo l’intervallo di date rimosso da virgole.

Ordine righe finale: riga intervallo di date → riga di intestazione → righe di dati ordinate.

### Passaggio 8: salvare

Sovrascrivi il file di input originale con il risultato pulito.

### Passaggio 9: salva una copia datata sul desktop (solo esportazione raw, se è stato acquisito un intervallo di date nel passaggio 0)

Creare una versione non crittografata dell&#39;intervallo di date: rimuovere le virgole e sostituire `\ / : * ? " < > |` con `-` (questi caratteri non sono validi nei nomi di file di Windows e potrebbero essere visualizzati in un intervallo di date a seconda delle impostazioni locali/del formato di esportazione).

Salva una copia aggiuntiva del file CSV pulito (lo stesso contenuto del passaggio 8) sul desktop dell’utente corrente, denominata:

`Documentation tracking report <filename-safe date range>.csv`

Esempio: un intervallo acquisito di `Apr 1, 2026 - Apr 30, 2026` diventa `Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`.

Ignorare questo passaggio per un file CSV già pulito (forma 2) a meno che l&#39;utente non fornisca separatamente un intervallo di date.

## Fuori ambito

La pubblicazione o la condivisione del file CSV pulito (ad esempio in Slack) è un passaggio separato e non ancora definito. Non tentare di allegare o caricare il file in alcun punto nell’ambito di questa abilità.

## Implementazione (esportazione non elaborata)

Per un’esportazione non elaborata, esegui i passaggi da 0 a 8 con questo script di PowerShell testato anziché modificare manualmente le righe, in modo più rapido e meno soggetto a errori per i file con centinaia di righe. Sostituire il percorso del file reale con `$path`.

Prima di eseguire, verificare se il file è bloccato (ad esempio, aperto in Excel). Se `Set-Content` non riesce e &quot;viene utilizzato da un altro processo&quot;, chiedere all&#39;utente di chiuderlo, quindi eseguirlo nuovamente.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

Per un CSV già pulito (forma di input 2), ignora la logica di trasferimento dell’intestazione, dell’intervallo di date e il passaggio 9: esegui i passaggi 2-6 e 8 sull’intestazione o sulle righe esistenti così come sono.
