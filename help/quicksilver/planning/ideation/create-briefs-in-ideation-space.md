---
title: Creare slip nello spazio di ideazione
description: Questo articolo descrive come sviluppare un brainstorming e definire una strategia nello spazio Ideazione per creare delle descrizioni. È possibile esportare i resoconti delle idee finiti in un file o in Workfront Planning per creare o aggiornare i record.
feature: Workfront Planning
role: User, Admin
author: Alina
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 1%
---

# Creare slip nello spazio ideazione

<!--add to TOC and miniTOC-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Utilizzando lo spazio ideazione, una nuova funzionalità di Adobe Workfront Planning, è possibile trasformare i resoconti in record di Planning o salvarli come file esterno. I resoconti esportati creano nuovi record o aggiornano quelli esistenti.

Questo articolo descrive come sviluppare un brainstorming e definire una strategia nello spazio Ideazione per creare delle descrizioni.

È possibile effettuare le seguenti operazioni:

* Per creare o aggiornare i record, esportare le descrizioni ideazione completate in Workfront Planning.

* Per utilizzare le informazioni di un breve documento in un&#39;altra applicazione, esportarlo in uno dei seguenti tipi di file:

  * PDF
  * Parola
  * PowerPoint
  * Modello di PowerPoint

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
Add this at GA - not available in beta:
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
      <!--
      not available right now:
      <p>View permissions to Workfront objects to add them to briefs </p>
      -->
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

## Crea descrizione breve spazio ideazione

È possibile creare resoconti brevi per creare o modificare record di Planning oppure per creare file che è possibile esportare in altre applicazioni.

1. Accedere a Workfront con Planning in cui è stato attivato Collaboratore ed eseguire una delle operazioni seguenti:

   * Vai al **menu principale** > **spazio ideazione**
   * Vai a **Menu principale** > **Planning** > fai clic su un&#39;area di lavoro > fai clic su un tipo di record > **Nuovo record** > **Avvia spazio ideazione**

     Per ulteriori informazioni sulla creazione di record utilizzando lo spazio ideazione, vedere [Creare record di Planning dalle descrizioni dello spazio ideazione](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
   * Vai a **Menu principale** > **Planning** > fai clic su un&#39;area di lavoro > fai clic su un tipo di record > fai clic su un record esistente > **Apri in Spazio ideazione**

   Viene aperto lo spazio ideazione e per impostazione predefinita viene creata una nuova ideazione con il seguente formato:

   `catalyze-canvas-< number > - Month date, year at time` <!--submitted bug to change the default name to "Untitled ideation"-->

   Se si apre un&#39;ideazione da un record esistente, il nome dell&#39;ideazione corrisponde al nome del record.

1. (Consigliato) Fai clic sul nome dell’idea per modificarlo.

1. (Condizionale e facoltativo) Per aprire un altro spazio ideazione esistente, fai clic sul menu a discesa a destra del nome dell’ideazione, cercalo per nome, quindi fai clic sull’ideazione quando viene visualizzata nell’elenco.

1. All&#39;apertura dello **spazio ideazione**, il CX Coworker si apre a destra. Utilizza il prompt di Collaborator per descrivere il tipo di resoconto che desideri creare.

   Ad esempio, digita &quot;Creare una campagna di ritorno a scuola per gli studenti delle scuole medie fino al mese di agosto, per genitori e insegnanti negli Stati Uniti&quot;.  Per rendere il resoconto il più completo possibile, indica quante più informazioni hai a disposizione per quale tipo di campagna, la timeline, le parti interessate, i punti di controllo per le approvazioni e altri dettagli.

1. Fai clic su Invio.

1. Rispondi alle domande di Collaboratore per continuare l&#39;ideazione, quindi fai clic su **Invia**

   Oppure

   Fai clic su **Ignora questionario** per saltare ulteriori domande.

1. (Condizionale) Quando Collaboratore offre di creare schede per l&#39;ideazione, rispondi **Sì**.

   Le schede vengono aggiunte allo spazio di ideazione e puoi visualizzare le sorgenti di ogni scheda e decidere quale aggiungere alla descrizione.

1. Fai clic sull&#39;icona **Ricerca** ![Icona Ricerca](assets/search-icon.png) per cercare elementi nello spazio delle idee, quindi fai clic su quando viene visualizzato nell&#39;elenco per passare a tale spazio.

1. (Facoltativo) Fai clic su **Origini** nella parte inferiore di ogni scheda per capire da dove sono state raccolte le informazioni.

   Le informazioni possono essere importate da Workfront Planning o dal Web.

   È inoltre possibile fare clic sull&#39;icona **Origini** ![Origini](assets/sources-icon.png) nell&#39;angolo superiore destro dello spazio per visualizzare un elenco delle origini per tutte le schede dello spazio.
1. (Facoltativo) Fai clic su **Commenti** ![Icona Commento](assets/comments-icon.png) nell&#39;angolo superiore destro dello spazio e **@** assegna altri tag per iniziare il brainstorming all&#39;interno dello spazio.

   Gli utenti riceveranno una notifica e-mail relativa al tag.
1. (Facoltativo) Fai clic sull&#39;icona **Filtro** ![](assets/filter-comments-icon.png) all&#39;interno della scheda dei commenti per filtrare i commenti in base ai seguenti criteri:

   * Revisori
   * Ora di aggiunta del commento
   * Stato (in cui il commento è stato risolto o è in sospeso)
   * Non letto (mostra solo i commenti non letti)
1. (Facoltativo) Utilizza le icone **Miniature in alto** o **Miniature in basso** su una scheda ![Icone in alto o in basso](assets/thumbs-up-and-down-icons.png) per fornire feedback sulla precisione delle informazioni sulla scheda.
1. Fai clic su una scheda o sulla cornice contenente tutte le schede, quindi fai clic su **Aggiungi alla descrizione** per aggiungere le relative informazioni alla descrizione.

   Workfront abbina ogni informazione con il campo in cui è più probabile memorizzarla.

   Ad esempio, le timeline vengono aggiunte ai campi di tipo data e alle descrizioni dei campi di tipo paragrafo.

1. (Condizionale) Fai clic su una scheda, quindi fai clic su **Chiedi IA a ...** per avere idee sul passaggio successivo, prima di aggiungere le informazioni alla descrizione. Le risposte si trovano nel contesto delle informazioni di ciascuna carta.
1. Fai clic sull&#39;icona **Aggiungi documenti** ![Aggiungi documenti](assets/add-documents-in-ideation-space.png) nell&#39;angolo superiore sinistro dello spazio di ideazione per caricare i documenti nello spazio. È possibile aggiungere nuovi documenti o documenti già aggiunti allo spazio in precedenza.

   >[!TIP]
   >
   >Per poter accedere ai documenti e caricarli nello spazio, è necessario attivare l&#39;impostazione Documenti.
   >Per informazioni, vedere la sezione [Configurare lo spazio ideazione](#configure-the-ideation-space) in questo articolo.
   > 
1. Fare clic sull&#39;icona **Aggiungi scheda tassonomia WF** ![Aggiungi da Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--asked to change this tooltip--> e selezionare un tipo di record connesso, quindi un record di ogni tipo per aggiungere le informazioni del record al tipo di record selezionato.

   Viene creata una scheda per il record selezionato da aggiungere allo spazio. Il tipo di record viene visualizzato nell&#39;angolo superiore sinistro della scheda del record.

   >[!TIP]
   >
   >L&#39;icona <!--check UI name--> della scheda **Aggiungi tassonomia WF** non è disponibile quando si accede allo spazio di ideazione dal menu principale e la descrizione non è connessa a un record di Planning.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) sulla scheda record connessa e fai clic su **Visualizza in Workfront**.

   La pagina dei dettagli del record viene visualizzata in un&#39;altra scheda del browser in Workfront Planning.
1. (Facoltativo) Seleziona la cornice di ideazione o una scheda, fai clic sull&#39;icona **Elimina**, quindi fai clic su **Elimina** per confermare. La scheda viene rimossa dallo spazio ideazione.

   Quando si eliminano schede corrispondenti a un documento o a un record memorizzato, gli elementi vengono rimossi dallo spazio Ideazione ma rimangono nelle rispettive applicazioni.

1. (Facoltativo) Utilizza la casella **Chiedi qualsiasi cosa al collega** nell&#39;angolo in basso a destra in qualsiasi momento per perfezionare la tua idea.

   Ad esempio, digita `regenerate` per una scheda specifica in modo che AI ripristini la scheda utilizzando il contesto aggiornato. Lo spazio di ideazione esegue nuovamente i passaggi di ragionamento (ricerca, sintesi, citazione) e aggiorna le schede interessate.

1. (Facoltativo) Fai clic su uno dei connettori viola da qualsiasi set di schede di ideazione, quindi fai clic sull&#39;icona **Copia prompt completo** per copiare negli Appunti il prompt che ha generato la scheda, quindi incollala nella casella del prompt di Collaborator.

   ![Icona Copia nella barra dei prompt](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Facoltativo) Fai clic sulle icone **Annulla** o **Ripristina** ![Annulla e ripristina](assets/undo-redo-icons.png) nella parte superiore dello spazio delle ideazioni per annullare o annullare un&#39;azione.
1. Zoom indietro per visualizzare il quadro completo: l’obiettivo originale della campagna, tutte le schede di concetti generate dall’intelligenza artificiale con citazioni, documenti aggiuntivi, i record reali di Workfront Planning inseriti (prodotti, utenti tipo, ecc.). La scheda di riepilogo **Brief** nell&#39;angolo inferiore sinistro raccoglie tutto.

1. Fai clic sulla breve immagine di anteprima in basso a sinistra e rivedi la descrizione, quindi fai clic su una delle seguenti opzioni:

   * **Esporta nel file**. È possibile esportare il documento nei seguenti tipi di file:

     * PDF
     * Parola
     * PowerPoint (con o senza modello)
   * **Esporta in Workfront Planning**. L&#39;esportazione sovrascrive tutti i dati di campo esistenti nel record Planning corrispondente all&#39;ideazione.

   >[!TIP]
   >
   >**L&#39;esportazione in Workfront Planning** è disattivata quando si accede allo spazio ideazione dal menu Principale e la descrizione non è connessa a un record di Planning.

   In questo modo si completa la creazione del record o del file con le informazioni aggiuntive. Se si è iniziato da un record esistente, le informazioni contenute nella descrizione vengono aggiunte al record. Se si inizia con un nuovo record, il record viene creato con le informazioni riportate nella descrizione.

   Per ulteriori informazioni sull&#39;aggiornamento dei record di Planning mediante le descrizioni, vedere la sezione &quot;Considerazioni sull&#39;utilizzo dello spazio di ideazione per creare record&quot; nell&#39;articolo [Creare record di Planning dalle descrizioni dello spazio di ideazione](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configurare lo spazio ideazione

Sono disponibili controlli per lo spazio di ideazione che consentono di configurare gli elementi visualizzati sullo schermo e di spostarsi con facilità nello spazio.

1. Fai clic sull&#39;icona **Impostazioni** ![Impostazioni](assets/setting-icon.png) per controllare da dove IA richiama le informazioni, quindi scegli uno dei seguenti **Tipi di Source**:

   * **Documenti** — documenti caricati nello spazio selezionato
   * **Ricerca sul Web** — ricerca sul Web esterna
   <!--
     **CJA** — Adobe Customer Journey Analytics
    -->
1. Fai clic su **Salva**.

1. Fai clic sull&#39;icona a discesa **livello di zoom** a sinistra dell&#39;icona **Guida** o dell&#39;icona **Guida** ![Guida](assets/more-information-icon.png) per selezionare un&#39;opzione o rivedere le scelte rapide da tastiera che è possibile utilizzare per spostarsi nello spazio delle idee o selezionare un valore di zoom diverso.

   Scegli uno dei seguenti livelli di zoom:

   * Zoom 100%
   * Zoom 200%
   * Zoom per adattare

   In alternativa, per spostarsi nella pagina utilizzare una delle seguenti scelte rapide:

   | Azione | Scelta rapida |
   | --- | --- |
   | Zoom in/out | Ctrl/⌘ + / − |
   | Zoom per adattare/adattare la selezione | — |
   | Zoom al cursore | Ctrl/⌘ + scorrimento |
   | Sposta l’area di lavoro | Pressione prolungata di spazio + trascinamento |
   | Mostra/nascondi griglia punti | Gig Byt |



<!--

    Once opened, the Ideation space agent goes through the following steps:

    1. **Data ingestion and synthesis**:  Pulls relevant information from connected sources. For example: 
    
        * Existing record types or the existing record type that you started from. 
        * Recent documents you might have uploaded in the ideation space. 
        * Web information that matches your prompt criteria.

            >[!TIP]
            >
            >The Web search setting must be turned on for AI to be able to look for information on the web.  
            >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
            >
    1. **Audience definition**: Identifies or recommends target audience parameters based on historical patterns
    1. **Strategy framing**: Structures the strategic narrative for the campaign
    1. **Messaging and concept ideation**: Generates initial message options and creative concept directions
    1. **Brief generation and planning handoff**: Produces a structured brief that feeds back into the Workfront Planning workspace

        When the Ideation agent finishes the process of collecting all the information, the following things occur: 
    
        * Five cards are created and are organized by relevant and like-information. 

            The cards are titled using various steps in the creation of the requested record, for easy recognition. 
    
            For example, they could be named:

            * Plan
            * Timeline
            * Segments
            * Mechanics  
            * Messaging 

        The cards titles are custom to each card in the ideation. 

        * The cards are placed inside the same frame indicating this is the result of one ideation. 

        * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!
    
        The brief contains suggested fields that the system considers pertinent to the ideas you are exploring. 
-->






