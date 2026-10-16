---
title: Creazione o modifica di record di pianificazione dalle descrizioni dello spazio di ideazione
description: Utilizzando Ideation Space, una nuova funzionalità di Adobe Workfront Planning, è possibile trasformare i resoconti in record di Planning. I resoconti esportati creano nuovi record o aggiornano quelli esistenti. In questo articolo viene descritto come creare o modificare i record di Planning esistenti utilizzando lo spazio ideazione.
role: User, Admin
author: Alina
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b81918ef8da7c7a4eeb9797b65a5af964db93911
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%
---

# Creare o modificare record di Planning dalle descrizioni dello spazio ideazione

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
<!--
Not available for beta:
Or
<li><p>Any Planning package when purchased as a standalone product</p></li>
-->
</ul>
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

## Considerazioni sull&#39;utilizzo dello spazio Ideazione per creare o modificare record di Planning

* Per poter creare o modificare un record di Planning, è necessario avviare lo spazio Ideazione da Workfront Planning. L&#39;accesso allo spazio delle ideazioni dal menu principale di Workfront non consente di collegare un&#39;ideazione a un record di Planning.
* Per utilizzare lo spazio di ideazione per creare o modificare record, è necessario disporre di un&#39;area di lavoro e di un tipo di record in Workfront Planning.
* I nuovi record iniziano sempre con il contenuto segnaposto, indipendentemente dalla modalità di creazione.
* Quando si elimina un record di Planning collegato a una descrizione breve dell&#39;ideazione, la descrizione rimane nello spazio dell&#39;ideazione e il relativo spazio associato non viene eliminato.
* La sincronizzazione delle informazioni avviene solo dallo spazio di ideazione a Workfront Planning. Non esiste alcuna sincronizzazione inversa o automatica da un record Planning alla descrizione dello spazio ideazione. <!--this might change?-->
* Quando si creano, modificano o rimuovono campi in Workfront Planning, si verificano gli scenari seguenti:

  * Ogni giorno vengono aggiunti nuovi campi creati in record collegati a descrizioni idee. I nuovi campi vengono visualizzati vuoti nella descrizione ideazione.
  * I campi rimossi rimangono nella descrizione e mantengono i valori precedenti.
  * I campi rinominati aggiornano i nomi nella descrizione.
* È possibile aggiungere documenti come schede nello spazio Ideazione. Sono incluse anche le immagini.

  È possibile aggiungere i seguenti tipi di file: PDF, Excel, CSV, PNG (e altri formati di immagine), Word, PowerPoint. Video non supportati.

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

   Lo spazio ideazione viene aperto in una nuova scheda.

   CX Coworker si apre nel pannello di destra.

   Il record viene creato immediatamente con un nome segnaposto.

   <!--
    1. (Optional) Click the **Open previous canvases** icon ![Open existing briefs icon](assets/open-existing-briefs-icon.png) in the upper-right corner of the prompt box, to open existing briefs
    -->

1. Aggiungere un prompt nella finestra di dialogo **CX Coworker**, quindi premere Invio.

   Più dettagli condividi, più utili saranno le informazioni fornite dallo spazio di ideazione. Ad esempio, digita una descrizione della campagna che stai pianificando: &quot;torna alla campagna scolastica per un’agenzia di marketing&quot;.

1. Continuare a creare la descrizione come descritto nell&#39;articolo [Creare descrizioni nello spazio ideazione](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md).

   <!--
    1. Click **Start ideating**.
        The Ideation space works through the following steps while it builds your idea: 
        1. Understand your goal and context
        2. Review your space and selected materials
        3. Gather evidence from documents, web, and data
        4. Synthesize findings into a research summary
        5. Create and refine cards with citations
        During this process you'll see the Ideation space actively searching connected Workfront Planning data or information available on the web.
        For example, it might search for existing programs, products, personas, or regions, as well as for similar concepts available online. 
        When the ideation completes, the following things are added to the Ideation space:  
        * A summary of the AI findings which is linked to several cards with detailed information about things to consider. The details cards display in a new section. A connector indicates which card section belongs to which summary.  
        * A **Brief** file in the lower-left corner of the ideation space. The brief is a draft of the future record and it displays as a record's Details page. 
        ![Ideation card with branches](assets/ideation-card-with-branched-off-additional-cards.png)      
    1. Continue to add information to the ideation space to complete creating your brief. 
    -->

1. (Condizionale) Al termine della descrizione, fare clic sull&#39;immagine di anteprima nell&#39;angolo inferiore sinistro, quindi fare clic su **Esporta in Workfront Planning** per creare un record di Planning.

   In questo modo, si completa la creazione del record con le informazioni aggiuntive e lo si aggiunge al tipo di record selezionato in origine.

## Modificare i record esistenti utilizzando lo spazio ideazione

Puoi aprire lo spazio ideazione da record esistenti per aggiornarli.

Non è possibile modificare in blocco i record nello spazio ideazione.

1. Passare a un record esistente in Workfront Planning e aprire la relativa pagina dei dettagli.

1. Fai clic su **Apri nello spazio ideazioni** ![](assets/open-in-ideation-space.png). Verrà aperto lo spazio Ideazione in una nuova scheda.

   Se esiste già un&#39;idea per il record, lo spazio viene aperto.

   Se non esiste alcuna ideazione, viene creato uno spazio di ideazione e un breve.

   >[!TIP]
   >
   >Non è possibile modificare in blocco i record utilizzando lo spazio ideazione.
1. Continua a modificare il resoconto come descritto nella sezione [Crea record utilizzando lo spazio di ideazione](#create-records-using-the-ideation-space) in questo articolo.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->


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


