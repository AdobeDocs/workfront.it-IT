---
title: Creare slip nello spazio di ideazione
description: Questo articolo descrive come sviluppare un brainstorming e definire una strategia nello spazio Ideazione per creare delle descrizioni. È possibile esportare i resoconti delle idee finiti in un file o in Workfront Planning per creare o aggiornare i record.
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 1%

---


# Creare slip nello spazio ideazione

<!-- add to TOC and miniTOC-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Utilizzando Ideation Space, una nuova funzionalità di Adobe Workfront Planning, è possibile trasformare i resoconti in record di Planning. I resoconti esportati creano nuovi record o aggiornano quelli esistenti.

Questo articolo descrive come sviluppare un brainstorming e definire una strategia nello spazio Ideazione per creare delle descrizioni. Per creare o aggiornare i record, esportare le descrizioni delle idee completate in un file o in Workfront Planning.

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

<tr> 
   <td role="rowheader"><p>Prodotti aggiuntivi</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
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
   <tr> 
   <td role="rowheader"><p>Ruoli utente di Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualsiasi ruolo utente di GenStudio per accedere a Campagne, Prodotti e Utenti tipo</li>
   <li>GenStudio System Manager per accedere alle attivazioni <!--and Events--></li></ul>
   Per informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Ruoli utente e autorizzazioni</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Crea descrizione breve spazio ideazione

1. Iniziare in Workfront Planning e creare o modificare un record utilizzando lo spazio ideazione.

   Per ulteriori informazioni, vedere [Creare record di Planning dalle descrizioni dello spazio ideazione](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
1. All&#39;apertura dello **spazio ideazione**, utilizzare il prompt fornito per descrivere il tipo di descrizione da creare.

   Ad esempio, digita &quot;Creare una campagna di ritorno a scuola per gli studenti delle scuole medie fino al mese di agosto, per genitori e insegnanti negli Stati Uniti&quot;.  Per rendere il resoconto il più completo possibile, indica quante più informazioni hai a disposizione per quale tipo di campagna, la timeline, le parti interessate e altri dettagli.

1. Fai clic su **Inizia ideazione**.

   Una volta aperto, l’agente spazio ideazione esegue i seguenti passaggi:

   1. **Acquisizione e sintesi dei dati**: richiama le informazioni rilevanti dalle origini connesse. Ad esempio:

      * Tipi di record esistenti o il tipo di record esistente da cui si è iniziato.
      * Documenti recenti che potresti aver caricato nello spazio delle ideazioni.
      * Informazioni Web corrispondenti ai criteri di richiesta.

        >[!TIP]
        >
        >Per poter cercare informazioni sul web, è necessario attivare l’impostazione di ricerca Web.\
        >Per informazioni, vedere la sezione [Configurare lo spazio ideazione](#configure-the-ideation-space)in questo articolo.
        >
   1. **Definizione del pubblico**: identifica o consiglia i parametri del pubblico di destinazione in base a modelli cronologici
   1. **Inquadramento strategico**: struttura il resoconto strategico della campagna
   1. **Messaggistica e ideazione di concetti**: genera opzioni di messaggio iniziali e indicazioni di concetti creativi
   1. **Breve generazione e handoff di pianificazione**: produce un resoconto strutturato che viene reindirizzato all&#39;area di lavoro di Workfront Planning

      Quando l&#39;agente ideazione termina il processo di raccolta di tutte le informazioni, si verificano le seguenti situazioni:

      * Vengono create cinque schede organizzate per informazioni pertinenti e simili.

        Il titolo delle schede è suddiviso in vari passaggi durante la creazione del record richiesto, per facilitarne il riconoscimento.

        Ad esempio, possono essere denominati:

        * Piano
        * Timeline
        * Segmenti
        * Meccanica
        * Messaggi

      I titoli delle schede sono personalizzati per ogni scheda nell’ideazione.

      * Le schede sono posizionate all&#39;interno dello stesso frame, a indicare che questo è il risultato di un&#39;idea.

      * Viene creata una breve descrizione che viene visualizzata in un&#39;immagine di anteprima nell&#39;angolo inferiore sinistro dello spazio ideazione. <!--add screen shot??-->

      Il documento contiene i campi suggeriti che il sistema considera pertinenti alle idee che state esaminando.

1. (Facoltativo) Fai clic sull&#39;icona **Help** ![](assets/more-information-icon.png) nell&#39;angolo superiore destro per visualizzare un elenco di scelte rapide da tastiera che ti aiuteranno a navigare nello spazio delle idee.

1. (Facoltativo) Fai clic su **Origini** nella parte inferiore di ogni scheda per capire da dove sono state raccolte le informazioni.

   Le informazioni possono essere importate da Workfront Planning o dal Web.
1. (Facoltativo) Utilizza le icone miniature in alto o miniature in basso su una scheda per fornire un feedback.<!--is this still available??-->
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
   1. Fare clic sull&#39;icona **Aggiungi scheda tassonomia WF** ![Aggiungi da Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> e selezionare un tipo di record connesso, quindi un record di ogni tipo per aggiungere le informazioni del record al tipo di record selezionato.

      Viene creata una scheda per il record selezionato da aggiungere allo spazio. Il tipo di record viene visualizzato nell&#39;angolo superiore sinistro della scheda del record.
   1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) e fai clic su **Visualizza in Workfront**.

      La pagina dei dettagli del record viene visualizzata in un&#39;altra scheda del browser in Workfront Planning.
   1. (Facoltativo) Seleziona la cornice di ideazione o una scheda, fai clic sull’icona Elimina, quindi fai clic su Elimina per confermare. La scheda viene rimossa dallo spazio ideazione.

      Quando si eliminano schede corrispondenti a un documento o a un record memorizzato, gli elementi vengono rimossi dallo spazio Ideazione ma rimangono nelle rispettive applicazioni.

1. (Facoltativo) Usa la casella **Chiedi qualsiasi cosa** nell&#39;angolo in basso a destra in qualsiasi momento per perfezionare la tua idea.

   Ad esempio, digita `regenerate` per una scheda specifica in modo che AI ripristini la scheda utilizzando il contesto aggiornato. Lo spazio di ideazione esegue nuovamente i passaggi di ragionamento (ricerca, sintesi, citazione) e aggiorna le schede interessate.

1. (Facoltativo) Nella casella **Chiedi a qualsiasi cosa**, fai una nuova domanda per iniziare una nuova idea.

   Viene generato un nuovo set di schede, dopo che lo spazio esegue nuovamente i passaggi di ragionamento.

1. (Facoltativo) Fai clic su uno dei connettori viola da qualsiasi set di schede di ideazione, quindi fai clic sull&#39;icona **Copia nella barra dei prompt** per rieseguire il ragionamento dell&#39;ideazione.

   ![Icona Copia nella barra dei prompt](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Facoltativo) Fai clic sulle icone **Annulla** o **Ripristina** ![Annulla e ripristina](assets/undo-redo-icons.png) nella parte superiore della pagina per annullare o annullare un&#39;azione.
1. Zoom indietro per visualizzare il quadro completo: l’obiettivo originale della campagna, tutte le schede di concetti generate dall’intelligenza artificiale con citazioni, documenti aggiuntivi, i record reali di Workfront Planning inseriti (prodotti, utenti tipo, ecc.). La scheda di riepilogo **Brief** nell&#39;angolo inferiore sinistro raccoglie tutto.

1. Fai clic sulla breve immagine di anteprima in basso a sinistra e rivedi la descrizione, quindi fai clic su una delle seguenti opzioni:

   * **Esporta nel file**. È possibile esportare il documento nei seguenti tipi di file:

     * PDF
     * Parola
     * PowerPoint (con o senza modello)
   * **Esporta in Workfront Planning**. L&#39;esportazione sovrascrive tutti i dati di campo esistenti nel record in Workfront Planning.

   In questo modo, si completa la creazione del record con le informazioni aggiuntive e lo si aggiunge al tipo di record selezionato in origine.

   Per ulteriori informazioni sull&#39;aggiornamento dei record di Planning mediante le descrizioni, vedere la sezione &quot;Considerazioni sull&#39;utilizzo dello spazio di ideazione per creare record&quot; nell&#39;articolo [Creare record di Planning dalle descrizioni dello spazio di ideazione](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configurare lo spazio ideazione

Sono disponibili controlli per lo spazio di ideazione che consentono di configurare gli elementi visualizzati sullo schermo e di spostarsi con facilità nello spazio.

1. Fai clic sull&#39;icona **Impostazioni** ![Impostazioni](assets/setting-icon.png) per controllare da dove IA richiama le informazioni, quindi scegli uno dei seguenti **Tipi di Source**:

   * **Documenti** — documenti caricati nello spazio selezionato
   * **Ricerca sul Web** — ricerca sul Web esterna
   * **CJA** — Adobe Customer Journey Analytics

1. Fai clic su **Salva**.

1. Fai clic sull&#39;icona **Aiuto** ![Icona Aiuto](assets/more-information-icon.png) per esaminare le scelte rapide da tastiera che puoi utilizzare per navigare nello spazio di ideazione o selezionare un altro valore di zoom.

   Scegli uno dei seguenti livelli di zoom:

   * Zoom 100%
   * Zoom 200%
   * Zoom per adattare

   In alternativa, per spostarsi nella pagina utilizzare una delle seguenti scelte rapide:

   | Azione | Scelta rapida |
   |---|---|
   | Zoom in/out | Ctrl/⌘ + / − |
   | Zoom per adattare/adattare la selezione | — |
   | Zoom al cursore | Ctrl/⌘ + scorrimento |
   | Sposta l’area di lavoro | Pressione prolungata di spazio + trascinamento |
   | Mostra/nascondi griglia punti | G |

1. Fai clic sull’icona Ricerca per cercare gli elementi nello spazio delle idee, quindi fai clic su quando viene visualizzato nell’elenco per individuarlo.








