---
mode: agent
description: 'Rimozione del frame della documentazione di sola anteprima di Workfront per GA: anteprima di snippet boilerplate, class="preview" HTML e paralleli passaggi o sezioni in-preview vs in-production.'
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%
---

# Rimuovi evidenziazione anteprima

Esegui questo flusso di lavoro solo quando viene chiesto di &quot;rimuovere l’evidenziazione dell’anteprima&quot; (o chiaramente
stesso intento). Converte procedure/riferimenti creati da Courtney e con tag di anteprima
argomenti nei contenuti pronti per GA.

## Ambito

Applica solo quando **tutti** sono true:

1. Ho richiamato questo flusso di lavoro.
2. Il percorso del file **non** contiene `product-announcements` (esclude l&#39;intero
tree: note sulla versione, beta, annunci).
3. Il file non è elencato in **Percorsi esclusi**.
4. La riga `author:` dell&#39;argomento principale include **`Courtney`** (autore unico o coautore).
5. L&#39;articolo include almeno uno dei seguenti elementi:
   - Linguaggio dell’ambiente di anteprima nella prosa del corpo o nei paragrafi di frammenti reali
     (&quot;informazioni evidenziate&quot;, &quot;Ambiente di anteprima&quot;, &quot;non ancora in generale
     disponibile&quot;, note sulla versione rapida) — **not** una corrispondenza dal solo testo del collegamento su un
     sommario/pagina indice;
   - Qualsiasi elemento di HTML con `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`...);
   - Variabile frammento di anteprima come `{{highlighted-preview}}` o
     `{{highlighted-preview-article-level}}`.

Se l’ambito non è chiaro, conferma prima di modificare.

**Sommario/pagine di indice - ignora sempre** quando l&#39;unica dicitura di anteprima si trova all&#39;interno di un
il testo visualizzato del collegamento markdown che punta a un altro articolo e il file non contiene
`class="preview"`, nessuna variabile frammento e nessuna anteprima boilerplate in prosa
al di fuori dei collegamenti.

### Percorsi esclusi

Non fare l&#39;inventario o modificare questi elementi a meno che non venga esplicitamente ignorato:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Flusso di lavoro richiesto (human in the loop)

Non eseguire la modifica in serie senza approvazione.

1. **Inventario** — crea un elenco ordinato di percorsi nell&#39;ambito (ricerca `help/`). Ometti
   `product-announcements`, percorsi esclusi e riferimenti a sommario e solo indice.
2. **Inizio** — chiedere se iniziare con il primo articolo (o con un percorso denominato).
3. **Per articolo — mostra prima, modifica dopo OK** — leggi il file, propone modifiche come
prima/dopo gli estratti o una differenza mirata, quindi attendi l’approvazione esplicita.
4. **Dopo ogni file** — chiedere se si desidera passare al successivo (oppure interrompere/saltare).

## Regole di contenuto (il contenuto dell’anteprima diventa il documento)

Obiettivo: mantieni il comportamento documentato per Anteprima, elimina &quot;in produzione&quot; obsoleto
i rami, quindi rimuovere etichette di sola anteprima e wrapper.

- **Passaggi paralleli**: rimuovi il passaggio &quot;in produzione&quot;; mantieni &quot;in anteprima&quot;
La fase è sostanziale, ma devi modificarla in modo che non sia specifica per l’anteprima. Correggi la numerazione. Se
nessun parallelo chiaro, fermarsi e chiedere quale blocco mantenere.
- **Sezioni parallele**: rimuovere la sezione ambiente di produzione; sostituirla
con il contenuto della sezione anteprima, quindi neutralizza la formulazione dell’anteprima e rimuovi
  `class="preview"` wrapper.
- **Frammenti e avvisi principali**: rimuovere la boilerplate di sola anteprima e
frasi il cui unico scopo è la disponibilità dell’anteprima.
- **`class="preview"`**: rimuovere i tag di apertura e chiusura, mantenere il contenuto interno.
Mantieni struttura elenco/tabella; correggi gli elenchi interrotti o gli spazi vuoti inattivi.
- **Sezioni con commenti (`<!-- … -->`)**: non modificare a meno che non venga specificato esplicitamente
dica così. Se il contenuto dell’anteprima viene visualizzato solo all’interno di commenti, richiamalo e chiedi.
Impostazione predefinita: lascia invariati i commenti.

## Do not

- Esecuzione su `product-announcements` percorsi o percorsi esclusi.
- Modifica automatica dei blocchi di commento.
- Rimuovi &quot;Anteprima&quot; quando si tratta di un nome di prodotto in un contesto non correlato (ad esempio, Anteprima
ambiente sandbox) — in caso di dubbi,
- Cambia `author:` o materiale non correlato.
- Ignora il passaggio Mostra → approva.

## Controlli di qualità prima di presentare modifiche

- Nessun `class="preview"` rimanente nell&#39;ambito concordato.
- Nessuna intestazione duplicata orfana o numero di passaggi interrotti.
- L’introduzione viene letta correttamente per GA (non &quot;solo in anteprima&quot; per le funzioni fornite).
