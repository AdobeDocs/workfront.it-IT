---
name: update-for-release
description: ""
source-git-commit: 4c2305da7635694d9d7bc174b5837a0d57fb7ac0
workflow-type: tm+mt
source-wordcount: '2009'
ht-degree: 0%

---


# Aggiornamento per versione (Workfront)

Questa abilità spiega come aggiornare gli articoli della guida di Workfront per una prossima versione di funzioni. Il flusso di lavoro è l&#39;inverso di `remove-preview-highlighting`: è in corso l&#39;aggiunta di un nuovo comportamento agli articoli, contrassegnati come Anteprima e (in seguito, in GA) eliminati dall&#39;altra abilità.

## Ambito

Applica quando **tutti** sono true:

1. L’utente sta aggiornando gli articoli della guida di Workfront per una funzione in fase di spedizione (in genere prima l’anteprima).
2. La modifica introduce un nuovo comportamento o una nuova interfaccia utente, non una pulizia GA. Per la pulizia GA, utilizza invece **remove-preview-highlighting**.
3. Il file è **non** una nota sulla versione. Per le note sulla versione, utilizza invece **release-notes-formatter**.
4. L’utente ha fornito un contesto della funzione: almeno una breve descrizione e uno screenshot; idealmente un URL PRD (Adobe Wiki).

Se l&#39;ambito non è chiaro, confermare prima di iniziare.

## Flusso di lavoro richiesto (human in the loop)

**not** modifica in blocco l&#39;archivio. Sposta un articolo alla volta. Dopo ogni articolo, chiedi se continuare con il successivo.

### &#x200B;1. Raccogliere il contesto della funzione

Conferma con l’utente:

- **Modifiche** (riepilogo di 1-2 frasi del nuovo comportamento o interfaccia utente).
- **Schermate** della nuova interfaccia utente. Se fornito, salva nella cartella `assets/` dell&#39;articolo di destinazione con un nome di file Kebab-Case descrittivo (esempio: `add-custom-message.png`). Se non specificato, chiedere se attenderne uno o procedere con un riferimento segnaposto.
- **URL PRD** (Adobe Wiki), se disponibile. Recuperalo con lo strumento MCP `user-Adobe Wiki Confluence` `get_wiki_content`. Leggilo per trovare comportamenti che l’utente non può vedere nell’interfaccia utente: effetti collaterali delle notifiche, cosa accade quando qualcosa viene modificato o aggiunto in un secondo momento, limiti dei caratteri non visualizzati, autorizzazioni, ecc.
- **Disponibilità**: solo anteprima, anteprima + rilascio rapido o già disponibilità generale. Questo guida la scelta dello snippet nel passaggio 3.
- **Esclusioni esplicite**: tutti gli articoli che l&#39;utente desidera saltare (ad esempio, &quot;questa funzione non è nei modelli&quot;).

### &#x200B;2. Articoli interessati dall’inventario

Cerca nel repository con le parole chiave dell&#39;area funzionale (ad esempio `approval workflow`, `document approval`, l&#39;etichetta del campo specifico). Creare un elenco candidati:

- Articoli pratici nella struttura `help/quicksilver/.../` pertinente.
- Articoli di panoramica e domande frequenti che menzionano l’area funzionale.
- **Escludi** `product-announcements/` (le note sulla versione utilizzano un&#39;abilità diversa).
- **Escludi** le pagine di sommario/indice in cui l&#39;unica menzione è il testo di collegamento a un altro articolo.
- **Escludi** articoli che l&#39;utente ha detto di saltare nel passaggio 1.

Presentare l&#39;elenco candidati all&#39;utente. Chiedi quali aggiornare e quali saltare. Riferimento incrociato `help/quicksilver/TOC.md` se un articolo di pari livello sembra mancante.

### &#x200B;3. Scegli lo snippet di anteprima

Leggi `help/_includes/snippets.md` e scegli in base alla disponibilità:

| Disponibilità | Frammento |
| --- | --- |
| Solo anteprima: il contenuto evidenziato è una novità in un articolo altrimenti in versione GA | `{{highlighted-preview}}` |
| Solo anteprima: l&#39;intero articolo è nuovo | `{{highlighted-preview-article-level}}` |
| Anteprima + rilascio rapido clienti, generale | `{{preview-fast-release-general}}` |

Se per il trimestre corrente esiste già uno snippet specifico per la versione, preferiscilo a quello generico. Conferma la scelta con l’utente prima di applicare.

### &#x200B;4. Per articolo — mostra prima, modifica dopo OK

Per ogni articolo nell’elenco confermato dall’utente:

1. **Leggi il file.**

2. **Determinare il pattern di evidenziazione.** Chiedi all’utente quale rientri in questo articolo (la risposta può differire per articolo):

   - **Duplicazione per sezione**: aggiungi `in Production` all&#39;intestazione di sezione esistente. Aggiungi una nuova sezione con `in Preview` aggiunta, racchiusa in `<div class="preview"> ... </div>`. Utilizzare quando il nuovo comportamento modifica in modo significativo la routine stessa, ovvero passaggi aggiuntivi o riordinati, una nuova immagine o un testo diverso. Tipico per procedure guidate.
   - **Duplicazione per riga**: per una descrizione di campo basata su tabella in cui viene modificata una sola riga e il resto della tabella/routine rimane invariato, lasciare invariata la riga esistente byte per byte e aggiungere un nuovo `<tr class="preview">` direttamente dopo di essa. Non intrecciare nuove frasi nella riga originale. Per le convenzioni esatte, consulta &quot;Duplicazione per riga&quot; in Regole di contenuto.
   - **Ritorno a capo per riga**: aggiungi le nuove frasi in linea all&#39;interno della sezione esistente, racchiuse in `<span class="preview"> ... </span>`. Da utilizzare quando l’aggiunta è una frase o due che si adattano naturalmente a un paragrafo esistente o a una risposta FAQ (non a una riga di tabella, utilizza la duplicazione per riga per tali righe).
   - **Misto**: alcune sezioni nello stesso articolo utilizzano modelli diversi per contenuti diversi. Utilizza questa opzione quando l’articolo combina tabelle procedurali, sezioni in stile FAQ e paragrafi normali.

3. **Posizionare il frammento** sulla propria riga immediatamente dopo l&#39;intestazione H1, con una riga vuota sopra e sotto. Lo snippet si trova **prima** del paragrafo dell&#39;introduzione.

4. **Nuovi dettagli bucket in &quot;includi sempre&quot; rispetto a &quot;in revisione&quot;.** Questo è il passaggio più importante.

   - **Includi sempre** (applica automaticamente, nessun prompt): comportamenti invisibili che l&#39;utente non può osservare durante l&#39;interazione con l&#39;interfaccia utente. Esempi:
     - Effetti indesiderati (ad esempio, &quot;la modifica invia nuovamente l’e-mail a tutti i partecipanti&quot;)
     - Comportamento tra altri oggetti o eventi successivi
     - Prerequisiti e autorizzazioni
     - Limiti non visualizzati nell’interfaccia utente
     - Tutto ciò che l’utente può imparare solo dal PRD, dai documenti o dal team di prodotto
   - **In attesa di revisione** (presente all&#39;utente con `AskQuestion` come selezione multipla): fatti che l&#39;utente può visualizzare sullo schermo durante l&#39;utilizzo della funzione. Esempi:
     - Contatore di caratteri già visualizzato nell&#39;interfaccia utente (esempio: `0 / 500`)
     - Stato predefinito di un campo espanso/compresso
     - Stato selezionato predefinito di una casella di controllo visibile
     - Etichette dei pulsanti accanto al campo
     - Messaggi di convalida visualizzati in linea

   Per ogni elemento &quot;in revisione&quot;, fornisci una motivazione di una frase (&quot;Aiuta i principianti a pianificare un messaggio più lungo&quot;, &quot;Aiuta gli utenti che non lo vedono in fasi successive a saperlo espandere&quot;). Includi solo gli elementi scelti dall&#39;utente. Il principio predefinito è &quot;se l’utente può visualizzarlo sullo schermo mentre sta eseguendo l’attività, non ripeterla&quot;, ma l’utente riceve la chiamata finale.

   **Quando si redigono le frasi effettive** per uno dei bucket, applicare `~/.cursor/skills/writing-quality/SKILL.md` regole di voce e tono durante la scrittura, ovvero una descrizione di un campo o di un comportamento normale, non una voce del registro delle modifiche (&quot;è stata rimossa&quot;, &quot;è stata aggiunta&quot;) e non aggiornare un&#39;istruzione invariata solo per allegarvi una nota di anteprima. Sformarlo correttamente la prima volta invece di fissare il tono in un passaggio successivo.

5. **Eseguire un passaggio finale di qualità di scrittura** sul testo scritto prima di visualizzarlo. Questa è una rete di sicurezza, non è la prima volta che queste regole si applicano — prendere qualsiasi cosa di passaggio 4 mancato (ridondanza, tono, la voce non combacia con le righe circostanti).

6. **Modifiche proposte.** Mostra gli estratti prima/dopo (o una descrizione mirata in stile diff) dell&#39;articolo, inclusi: posizionamento degli snippet, ridenominazioni delle intestazioni, nuovo contenuto in-Preview e dove si trova, riferimento della schermata ed eventuali wrapping in linea di `class="preview"`.

7. **Attendere l&#39;approvazione esplicita** (&quot;ok&quot;, &quot;apply&quot;, &quot;yes&quot;) prima di scrivere il file.

8. **Convalida.** Dopo aver scritto, esegui `ReadLints` sul file e segnala eventuali problemi. Leggi nuovamente la sezione modificata per confermare la struttura.

### &#x200B;5. Dopo ogni articolo

Chiedi se passare all’articolo successivo, interrompere, saltare o rivedere quello corrente.

### &#x200B;6. Fine della sessione — nota sulla versione di copia/incolla

Quando l’utente si conclude per la sessione (dice &quot;completato&quot;, &quot;basta&quot;, &quot;stop&quot; o rifiuta di continuare con l’articolo successivo), chiedi:

> &quot;Desideri una voce di nota sulla versione di copia/incolla per la pagina di miglioramento?&quot;

In caso affermativo, generate una bozza utilizzando il contesto della feature del passaggio 1 e l&#39;articolo della guida principale aggiornato in questa sessione. **Non scriverlo in alcun file**. Fornirlo solo come testo da copiare o incollare.

Formattare la voce in modo che corrisponda alla struttura della pagina dell&#39;area di prodotto dall&#39;abilità **release-notes-formatter**:

```markdown
## {Feature name}

>[!NOTE]
>
>Preview: {date or TBD}
>Production fast release: {date or TBD}
>Production for everyone: {date or TBD}

{1–3 sentences describing what changed and why it helps users. Lead with the benefit, not the UI action.}

For more information, see [{Primary article title}](/help/quicksilver/{path-to-article}.md).
```

Regole:

- Utilizza `TBD` per qualsiasi data non ancora nota; chiedi all&#39;utente se ha le date.
- Il nome della funzione è una frase maiuscola (solo la prima parola e i sostantivi corretti).
- La descrizione deve concentrarsi su ciò che gli utenti possono ora fare, non sui dettagli di implementazione.
- È stato aggiornato il collegamento all’articolo tutorial più specifico, non una pagina di panoramica.
- Non includere un blocco di data `>[!NOTE]` se tutte le date sono sconosciute e l&#39;utente non desidera utilizzare segnaposto. Ometterlo e notare che sarà necessario aggiungerlo in un secondo momento.

## Regole di contenuto

### Intestazioni

- Aggiungi esattamente **`in Production`** alle intestazioni di sezione esistenti che rimangono come riferimento lato produzione.
- Aggiungi esattamente **`in Preview`** ai nuovi titoli di sezione.
- Mantieni il resto dell&#39;intestazione in lettere maiuscole/minuscole (per `writing-quality`).

### Anteprima wrapper

- **Livello sezione**: a capo automatico in `<div class="preview"> ... </div>`. Posiziona i tag di apertura e chiusura sulle proprie righe, con una riga vuota sopra e sotto ogni tag, in modo che le intestazioni e gli elenchi Markdown all’interno continuino a essere visualizzati.
- **In linea (a livello di frase)**: racchiudi `<span class="preview"> ... </span>` all&#39;interno del paragrafo esistente, della cella della tabella o della risposta alle domande frequenti.
- Non nidificare mai `<span class="preview">` in un `<div class="preview">`.

### Duplicazione per riga

Per una descrizione di campo basata su tabella in cui cambia solo il *comportamento* del campo (non la procedura circostante):

- Lascia `<tr>` esistente completamente invariato: ora corrisponde al comportamento corrente/produzione. Non inserire mai nuove frasi o estendersi in esso.
- Aggiungi una nuova riga subito dopo:

  ```html
  <tr class="preview">
  <td><span class="preview"><strong>{new label} in preview</strong></span></td>
  <td><span class="preview">{self-contained description}</span></td>
  </tr>
  ```

- **Etichetta**: non prendere solo l&#39;etichetta del campo originale e aggiungere `(in Preview)`. Scrivere un&#39;etichetta breve e naturale per la nuova funzionalità (ad esempio, l&#39;etichetta originale &quot;Aggiungi nomi o e-mail&quot; → nuova etichetta &quot;Aggiungi persone o team&quot;), quindi aggiungere `in preview` in minuscolo senza parentesi: &quot;Aggiungi persone o team in anteprima&quot;.
- **Descrizione**: scrivi una nuova descrizione di 1-3 frasi solo del nuovo comportamento, nella voce esistente dell&#39;articolo. Non riutilizzare le frasi della riga originale come base e inserirvi delle aggiunte; la nuova riga deve essere letta come una descrizione completa e autonoma.
- **Note aggiuntive**: aggiungere con un&#39;interruzione di riga `<br>` seguita da `Note:` nella riga successiva, all&#39;interno dello stesso `<span class="preview">`. Non nidificare `<p>Note: ...</p>`. Poiché la nuova riga è isolata, ripeti brevemente qui qualsiasi fatto ancora rilevante dalla nota della riga originale, invece di supporre che lo abbia visto anche il lettore (ad esempio, una restrizione in modalità avanzata &quot;uno stadio aperto alla volta&quot; che si applica ugualmente alla nuova riga).
- **Più varianti**: se lo stesso campo viene aggiornato in più di una procedura nello stesso articolo (Basic vs. Advanced, legacy vs. ESM e così via) e il comportamento sottostante differisce effettivamente tra loro (ad esempio, legacy mantiene un consenso predefinito mentre ESM si espande sempre), scrivi ogni riga per corrispondere al comportamento effettivo della variante. Non copiare il testo di una variante nella riga di un’altra.

### Posizionamento snippet

- La linea dello snippet va immediatamente dopo la H1, con una linea vuota sopra e sotto.
- Lo snippet si trova **prima** del paragrafo dell&#39;introduzione, del callout `>[!IMPORTANT]` e di qualsiasi blocco dei requisiti di accesso.
- Un frammento per articolo.

### Schermate

- Salvare le nuove schermate nella cartella `assets/` dell&#39;articolo con un nome di file descrittivo con maiuscole/minuscole.
- Fai riferimento alla nuova schermata dall’interno della nuova sezione in-Preview. Se lo screenshot di una sezione in-produzione non riflette più la funzione con precisione, lasciala in posizione; rappresenta comunque il comportamento di produzione fino a GA.
- Non creare nomi di file di screenshot; se non è stato ancora fornito uno screenshot, chiedi all&#39;utente.
- **Segnaposto per uno screenshot che non esiste ancora**: se l&#39;utente desidera procedere senza attendere la risorsa, aggiungi un commento HTML direttamente dopo il riferimento dello screenshot esistente (di produzione), riutilizzando il nome file con il suffisso `-v2`:

  ```html
  <!--
  preview screen![{same alt text}](assets/{existing-filename}-v2.png)
  -->
  ```

  Sostituisci il riferimento reale (e rimuovi il commento) una volta fornita la schermata.

### Note e suggerimenti

- Un massimo di `>[!NOTE]` (o `>[!TIP]`, `>[!IMPORTANT]`, `>[!WARNING]`) per sezione. Se la sezione esistente contiene già una nota, combinare il nuovo contenuto correlato nella stessa nota come elenco puntato anziché sovrapporlo.

### Cosa non fare

- Non modificare gli articoli in `product-announcements/`.
- Non modificare in blocco: un articolo alla volta, con approvazione esplicita ogni volta.
- Non includere fatti dell’interfaccia utente osservabili senza prima mostrarli all’utente.
- Non modificare il contenuto all&#39;interno di `<!-- ... -->` commenti di HTML a meno che l&#39;utente non lo dica esplicitamente.
- Non modificare `author:` o campi di argomento non correlati.

## Controlli di qualità prima di presentare modifiche

Esegui questa lista di controllo completa per **ogni** articolo nella sessione, inclusi gli articoli secondari in cui stai &quot;aggiungendo solo un punto elenco&quot;, non solo il primo/principale.

- Lo snippet viene visualizzato una volta, sulla propria linea, dopo la H1, con righe vuote sopra e sotto.
- I titoli di sezione esistenti terminano con `in Production`.
- Le nuove intestazioni di sezione terminano con `in Preview` e la sezione si trova all&#39;interno di `<div class="preview">`.
- Le aggiunte in linea si trovano in `<span class="preview">`.
- Duplicazioni per riga: il `<tr>` originale è byte per byte invariato; il nuovo `<tr class="preview">` ha entrambe le celle racchiuse in `<span class="preview">`; l&#39;etichetta è una nuova etichetta breve + minuscola &quot;in anteprima&quot; (non l&#39;etichetta originale + &quot;(in Anteprima)&quot;); qualsiasi nota supplementare utilizza `<br>` + `Note:` in linea, non un `<p>` nidificato.
- Se lo stesso campo viene visualizzato in più varianti di procedura (Basic/Advanced, legacy/ESM), il testo di ogni nuova riga corrisponde al comportamento effettivo della variante, anziché essere copiato e incollato da un&#39;altra variante.
- La nuova prosa contrassegnata da anteprima è simile a una descrizione di campo o comportamento semplice, non a una voce del registro delle modifiche e non aggiorna in modo ridondante un&#39;istruzione invariata.
- `ReadLints` è pulito nel file modificato.
- L’articolo viene letto correttamente in entrambi gli stati (con il contenuto di anteprima mostrato e nascosto).

## Riferimenti

- Stile della documentazione di Workfront: vedi l&#39;abilità **write-quality** in `~/.cursor/skills/writing-quality/SKILL.md`.
- Catalogo snippet: `help/_includes/snippets.md` nell&#39;archivio documenti.
- Pulizia GA (flusso di lavoro inverso): consulta l&#39;abilità **remove-preview-highlighting** in `.cursor/skills/remove-preview-highlighting/SKILL.md`.
- Adobe Wiki MCP per PRD: server `user-Adobe Wiki Confluence`, strumento `get_wiki_content`.
