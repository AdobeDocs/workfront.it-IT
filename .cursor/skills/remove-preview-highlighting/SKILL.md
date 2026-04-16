---
name: remove-preview-highlighting
description: ""
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---


# Rimuovi evidenziazione anteprima (Workfront)

## Limite

Applica solo quando **tutti** sono true:

1. L&#39;utente ha richiamato questo flusso di lavoro (ad esempio, dice **&quot;rimuovi evidenziazione anteprima&quot;** o chiaramente lo stesso intento).
2. Il percorso del file Markdown **non** contiene **`product-announcements`** (esclude l&#39;intera struttura di cartelle, ad esempio note sulla versione, beta, annunci in `help/quicksilver/product-announcements/`).
3. Il file Markdown è **non** elencato in **[Percorsi esclusi](#excluded-paths)**.
4. Il frontmatter del file Markdown include **`Courtney`** nella riga `author:` (autore unico o coautore).
5. L&#39;articolo contiene **almeno uno** di:
   - Anteprima-ambiente **lingua nella prosa del corpo o frammento reale paragrafi** (pattern tipici: &quot;informazioni evidenziate&quot;, &quot;ambiente di anteprima&quot;, &quot;non ancora disponibile a livello generale&quot;, note sulla versione rapida)—**non** una corrispondenza da **testo di collegamento** in una pagina sommario/indice (vedi sotto); o
   - Qualsiasi elemento di HTML con **`class="preview"`** (ad esempio `<span class="preview">`, `<div class="preview">`); o
   - Frammento di anteprima **variabile** come **`{{highlighted-preview}}`** o **`{{highlighted-preview-article-level}}`**.

Se l’ambito non è chiaro, conferma prima di modificare.

**SOMMARIO/pagine indice - ignora sempre questo caso:** **Mai** inserire un file nell&#39;inventario quando la dicitura relativa all&#39;anteprima **solo** è **all&#39;interno** Il testo visualizzato di un collegamento Markdown che punta a **un altro** articolo (ad esempio *Invia un report nell&#39;ambiente Sandbox di anteprima*) **e** il file contiene **no** `class="preview"`, **no** variabili snippet e **no** anteprima boilerplate in **prose al di fuori dei collegamenti**. Non si tratta dell’evidenziazione in anteprima su quella pagina, ma solo di una menzione del sommario. Si applica a qualsiasi indice/sommario, non a un solo file.

### Percorsi esclusi

Non aggiungerli mai all’inventario o modificarli in questo flusso di lavoro, a meno che l’utente non sostituisca esplicitamente:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md` — i limiti di produzione e anteprima parallela richiedono una decisione editoriale deliberata al di fuori dell&#39;automazione.
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md` — rapporti TOC; l&#39;unico segnale di &quot;anteprima&quot; è il collegamento all&#39;articolo di consegna Sandbox di anteprima.

## Flusso di lavoro richiesto (human in the loop)

**not** modifica in blocco l&#39;archivio senza approvazione.

1. **Inventario**\
   Crea un elenco ordinato di percorsi che soddisfano le regole di ambito di cui sopra (cerca nell&#39;archivio; preferisci `help/` strutture). **Ometti** qualsiasi percorso in **`product-announcements`**, qualsiasi percorso in **[Percorsi esclusi](#excluded-paths)** e qualsiasi **TOC/index** pagina corrispondente a **TOC/pagine indice** nell&#39;ambito. Se l’utente dice che un file elencato non presenta evidenziazioni in anteprima, rimuovilo dall’esecuzione e stringi i criteri invece di forzare le modifiche.

2. **Inizio**\
   Chiedi se iniziare con l&#39;articolo **first** nell&#39;elenco (o un percorso con i nomi utente).

3. **Per articolo — mostra prima, modifica dopo OK**
   - Leggi il file.
   - Suggerisci modifiche in modo chiaro: **prima/dopo estratti** o una descrizione di tipo differenze mirata di ciò che cambierà.
   - **Attendi** l&#39;approvazione esplicita (ad esempio &quot;ok&quot;, &quot;apply&quot;, &quot;yes&quot;) prima di scrivere il file.

4. **Dopo ogni file**\
   Chiedi se passare all&#39;articolo **next** (o interrompere/saltare).

## Regole di contenuto (GA: l’anteprima del contenuto diventa il documento)

Quando si rimuove l&#39;evidenziazione dell&#39;anteprima per la **disponibilità generale**, l&#39;obiettivo è: **mantenere il comportamento documentato per l&#39;anteprima**, eliminare **rami obsoleti &quot;in produzione&quot; / vecchio processo**, quindi **rimuovere etichette e wrapper di sola anteprima** in modo che l&#39;argomento venga letto come corrente per tutti i clienti.

### Passaggi paralleli

- Se l&#39;articolo ha un passaggio (o un elemento numerato) **incorniciato come &quot;in produzione&quot;** (o equivalente: produzione corrente / comportamento di produzione esistente) **e** un passaggio **parallelo** denominato come **&quot;in anteprima&quot;** (o ambiente di anteprima):
   - **Rimuovi** il passaggio in produzione (il vecchio percorso).
   - **Mantieni** la **sostanza** del passaggio nell&#39;anteprima, ma **reword** per cui è **non** specifica per l&#39;anteprima (rimuovi &quot;nell&#39;anteprima&quot;, &quot;Ambiente anteprima&quot;, ecc.). Regola la numerazione in modo che l&#39;elenco rimanga coerente.

Se la struttura è ambigua (nessun chiaro parallelo), **arresta** e mostra entrambi i candidati; chiedi all&#39;utente quale blocco mantenere.

### Sezioni parallele

- Se una **sezione** (intestazione e corpo) è **informazioni su &quot;nell&#39;ambiente di produzione&quot;** ed è presente una **sezione parallela** **informazioni su &quot;nell&#39;ambiente di anteprima&quot;**:
   - **Rimuovi** la sezione dell&#39;ambiente di produzione (il contenuto sostituito).
   - **Sostituisci** con il contenuto della sezione di anteprima, quindi **rimuovi** il testo dell&#39;ambiente di anteprima ed eventuali wrapper **`class="preview"`** in modo che la sezione sia neutra (pronta per GA).

### Frammenti e avvisi di contenuto

- Rimuovi **blocchi boilerplate** di sola anteprima (span/divs o paragrafi che spiegano solo che il contenuto evidenziato è Solo anteprima, rilascio rapido, sandbox, ecc.) una volta che la funzione è GA.
- Rimuovi collegamenti o frasi il cui scopo **only** è la disponibilità dell&#39;anteprima, a meno che l&#39;utente non dica di mantenere un avviso diverso.

### HTML `class="preview"`

- Rimuovi i **tag di apertura e chiusura** per gli elementi che utilizzano **`class="preview"`**, **contenuto interno** (markdown/HTML all&#39;interno del tag).
- Gestisci sia **`<span class="preview">`** che **`<div class="preview">`** e lo stesso pattern su altri tag (ad esempio **`<p class="preview">`**, **`<li class="preview">`**) quando sono visualizzati nel contenuto del corpo di **visible** (senza commenti).
- Mantieni struttura elenco/tabella; correggi gli elenchi interrotti o gli spazi vuoti inattivi dopo l’apertura.

### Sezioni con commenti (commenti di HTML)

- **Non** eliminare, decomprimere o in altro modo **modificare** il contenuto all&#39;interno di **`<!-- … -->`** commenti di HTML **a meno che l&#39;utente non indichi esplicitamente** come procedere (ad esempio eliminare l&#39;intero commento, eliminare le classi di anteprima solo all&#39;interno del commento, rimuovere il commento per GA).
- Se il contenuto correlato all&#39;anteprima o **`class="preview"`** appare **only** all&#39;interno di commenti, **richiamalo** quando rivedi l&#39;articolo: pronunciati sul contenuto del commento e **chiedi** cosa fare. **Impostazione predefinita: lascia invariate le sezioni commentate.**

### Cosa non fare

- Non eseguire questo flusso di lavoro sui percorsi in **`product-announcements`** (note sulla versione e correlate). L&#39;inventario deve escluderli.
- Non inventariare o modificare i percorsi elencati in **[Percorsi esclusi](#excluded-paths)** a meno che l&#39;utente non chieda esplicitamente di includerne uno.
- **Non** rimuovere o modificare automaticamente **blocchi esclusi** (`<!-- … -->`); segui **sezioni esclusi** sopra.
- Non rimuovere &quot;Anteprima&quot; quando è **not** su questo pattern di disponibilità delle funzionalità (ad esempio [Anteprima ambiente sandbox](·) come **nome prodotto** in un contesto non correlato); utilizza il giudizio e chiedi se non sei sicuro.
- Non modificare `author:` o elementi di primo piano non correlati a meno che l&#39;utente non lo richieda.
- Non saltare il passaggio **mostra → approva**.

## Controlli di qualità prima di presentare modifiche

- Nessun **`class="preview"`** rimanente nell&#39;ambito di modifica concordato.
- Nessuna intestazione duplicata orfana o numero di passaggi interrotti.
- L&#39;introduzione legge correttamente **senza** contraddicendo la disponibilità generale (nessuna &quot;solo in anteprima&quot; per le funzionalità fornite).

## Riferimenti

- Abbina **[Stile documentazione Workfront](https://experienceleague.adobe.com/?lang=it)** e convenzioni archivio (regole commit/PR se l&#39;utente esegue il commit).
