---
title: Creazione di record di pianificazione dalle descrizioni dello spazio ideazione
description: Utilizzando Ideation Space, una nuova funzionalità di Adobe Workfront Planning, è possibile trasformare i resoconti in record di Planning. I resoconti esportati creano nuovi record o aggiornano quelli esistenti. In questo articolo viene descritto come creare o modificare i record di Planning esistenti utilizzando lo spazio ideazione.
role: User, Admin
author: Alina
source-git-commit: bef848df8b263de89bfa90b7fec74b14734dfeff
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%
---

# Crea record di Planning dalle descrizioni dello spazio ideazione

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Utilizzando Ideation Space, una nuova funzionalità di Adobe Workfront Planning, è possibile trasformare i resoconti in record di Planning. I resoconti esportati creano nuovi record o aggiornano quelli esistenti.

In questo articolo viene descritto come creare o modificare i record di Planning esistenti utilizzando lo spazio ideazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p></li>
Oppure
<li><p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p></li></ul>
   </td> 
    <!--
    <tr> 
    <td role="rowheader"><p>Additional products</p></td> 
    <td><ul>
    <li><p>Adobe GenStudio for Performance Marketing</p></li>
    <li><p>Adobe Customer Journey Analytics</p></li>
    </ul>
    </td> 
    </tr> 
    -->
  <tr> 
   <td role="rowheader"><p>Licenza flusso di lavoro Adobe</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> 
   <ul>
   <li><p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   </li>
   <li><p>L’impostazione Disattiva spazio ideazione nel livello di accesso deve essere deselezionata</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td> <p>Autorizzazioni Contribute o superiori per l'area di lavoro e il tipo di record in cui si desidera aggiungere record </p>
      <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
      <p>Visualizzare le autorizzazioni per gli oggetti Workfront per aggiungerli alle descrizioni <!--not sure if this is available--></p>
      <p>Autorizzazioni dell’editor per lo spazio ideazione per creare resoconti</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Considerazioni sull’utilizzo dello spazio Ideazione per creare record

* Durante la creazione o la modifica di record, è possibile avviare lo spazio di ideazione solo da Workfront Planning o dal menu principale di Workfront. Lo spazio ideazione non esiste al di fuori di Workfront.
* Per accedere allo spazio di ideazione, è necessario disporre di un&#39;area di lavoro e di un tipo di record in Workfront Planning.
* I nuovi record iniziano sempre con il contenuto segnaposto, indipendentemente dalla modalità di creazione.
* Quando si elimina un record di Planning collegato a una descrizione breve dell&#39;ideazione, la descrizione rimane nello spazio dell&#39;ideazione e l&#39;area di lavoro associata nello spazio dell&#39;ideazione non viene eliminata.
* La sincronizzazione delle informazioni avviene solo dallo spazio di ideazione a Workfront Planning. Non esiste alcuna sincronizzazione inversa o automatica da un record Planning alla descrizione dello spazio ideazione.
* Quando si creano, modificano o rimuovono campi in Workfront Planning, si verificano gli scenari seguenti:

  * Ogni giorno vengono aggiunti nuovi campi creati in record collegati a descrizioni idee. I nuovi campi vengono visualizzati vuoti nella descrizione ideazione.
  * I campi rimossi rimangono nella descrizione e mantengono i valori precedenti.
  * I campi rinominati aggiornano i nomi nella descrizione.
* È possibile aggiungere documenti come schede nello spazio Ideazione. Sono incluse anche le immagini.

  Sono supportati i seguenti tipi di file: PDF, Excel, CSV, PNG (e altri formati di immagine), Word, PowerPoint. Video non supportati.

  Tutti i documenti caricati vengono convertiti in PDF sul backend per l’elaborazione.
* È possibile trascinare i record direttamente da Workfront Planning nello spazio e visualizzarli come file caricati manualmente.

## Creare record utilizzando lo spazio ideazione

1. Nella pagina di destinazione di Workfront Planning fare clic sulla scheda relativa a un&#39;area di lavoro che è possibile gestire.
1. Fare clic sulla scheda per un tipo di record a cui è possibile aggiungere record.
1. Per creare un record, eseguire una delle operazioni seguenti:

   * Da qualsiasi visualizzazione della pagina del tipo di record, fare clic su **Nuovo record** nell&#39;angolo superiore destro della pagina e nella casella **Scegliere un metodo per aggiungere i record**, fare clic su **Apri lo spazio ideazione**, quindi fare clic su **Continua**.
   * Scorri fino alla parte inferiore della tabella dei record e fai clic su **Nuova riga**, quindi fai clic su **Apri lo spazio ideazione**.

     >[!TIP]
     >
     >Se si seleziona **Non mostrare**, il prompt futuro verrà chiuso definitivamente. Se si fa clic sull&#39;icona Chiudi **X**, la casella verrà chiusa, ma verrà visualizzata di nuovo alla successiva aggiunta di un record in linea.

   ![Nuova casella di record con pulsante Apri spazio ideazione](assets/new-record-creation-picker-with-ideation.png)

   Lo spazio ideazione viene aperto in una nuova scheda con un prompt vuoto.

   Il record viene creato immediatamente con il testo segnaposto.

1. (Facoltativo) Fare clic su **Utilizza descrizione esistente** nella casella di richiesta per sfogliare e aggiungere un documento esistente che verrà utilizzato dallo spazio ideazione per creare la descrizione e il record futuro. <!--CORRECT THIS PART: this is possible ONLY when you launch Ideation from the Main Menu, not from a record-->

   ![Prompt breve per ideazione vuoto](assets/empty-ideation-prompt.png)

1. (Facoltativo) Fai clic sull&#39;icona ![Apri tele precedenti **<!--accurate??--> {icona Apri slip esistenti](assets/open-existing-briefs-icon.png) nell&#39;angolo superiore destro della casella del prompt, per aprire gli slip esistenti**

1. In **Su cosa stai lavorando?** , descrivere il tipo di record che si desidera creare.

   Più dettagli condividi, più utili saranno le informazioni fornite dallo spazio di ideazione. Ad esempio, digita una descrizione della campagna che stai pianificando: &quot;torna alla campagna scolastica per un’agenzia di marketing&quot;.

1. Fai clic su **Inizia ideazione**.

   Durante la creazione dell&#39;idea, lo spazio ideazione funziona come segue: <!--check some of these in the UI - there might have been UI text changes-->

   1. Comprendere obiettivo e contesto
   2. Verifica lo spazio e i materiali selezionati
   3. Raccogliere prove da documenti, web e dati
   4. Sintetizzare i risultati in un riepilogo di ricerca
   5. Creare e perfezionare le schede con le citazioni

   Durante questo processo verrà visualizzato lo spazio di ideazione che consente di eseguire ricerche attive nei dati o nelle informazioni di Workfront Planning collegate disponibili sul Web.

   Ad esempio, potrebbe cercare programmi, prodotti, utenti tipo o aree geografiche esistenti, nonché concetti simili disponibili online. <!--check on this with Et-->

   Al termine dell’ideazione, vengono aggiunti i seguenti elementi allo spazio Ideazione:

   * Una sintesi dei risultati dell’intelligenza artificiale, collegata a diverse schede, con informazioni dettagliate sugli aspetti da considerare. Le schede dei dettagli vengono visualizzate in una nuova sezione. Un connettore indica la sezione della scheda a cui appartiene il riepilogo.

   * Un file **Brief** nell&#39;angolo inferiore sinistro dello spazio di ideazione. La bozza è una bozza del record futuro e viene visualizzata come pagina Dettagli del record.

   ![Scheda ideazione con rami](assets/ideation-card-with-branched-off-additional-cards.png)

1. Continua ad aggiungere informazioni allo spazio delle idee per completare la creazione del resoconto.

1. (Condizionale) Al termine della breve, fai clic sull’immagine di anteprima nell’angolo in basso a sinistra, quindi fai clic su una delle seguenti opzioni:

   * **Esporta nel file** per creare un file
   * **Esporta in Workfront Planning** per creare un record di Planning

   Per informazioni sull&#39;aggiunta e l&#39;esportazione di elementi al documento, vedere [Creare documenti nello spazio ideazione](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md).

   In questo modo, si completa la creazione del record con le informazioni aggiuntive e lo si aggiunge al tipo di record selezionato in origine.

## Modificare i record esistenti nello spazio ideazione

Puoi aprire lo spazio ideazione da record esistenti per aggiornarli.

Non è possibile modificare in blocco i record nello spazio ideazione.

1. Passare a un record esistente in Workfront Planning e aprire la relativa pagina dei dettagli.

1. Fai clic su **Apri nello spazio ideazioni**. Verrà aperto lo spazio Ideazione in una nuova scheda.

   Se esiste già un&#39;idea per il record, lo spazio viene aperto.

   Se non esiste alcuna ideazione, viene creato uno spazio di ideazione e un breve.

   >[!TIP]
   >
   >Non è possibile modificare i record in blocco utilizzando lo spazio delle ideazioni.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. Continua a modificare il resoconto come descritto nella sezione [Crea record utilizzando lo spazio di ideazione](#create-records-using-the-ideation-space) in questo articolo.






<!--
this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


