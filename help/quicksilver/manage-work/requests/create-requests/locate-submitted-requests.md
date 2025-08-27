---
product-area: requests
navigation-topic: create-requests
title: Individuare le richieste inviate
description: Scopri le aree di Adobe Workfront in cui puoi individuare le richieste che hai inviato o che un altro utente ha inviato o le richieste che non hai mai inviato e che sono state salvate come bozze.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 0ffae8ed285f6e9164a239552feb90465bea3cca
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 2%

---

# Individuare le richieste inviate

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Puoi individuare i seguenti tipi di richieste inviate da te o da un altro utente oppure richieste avviate ma non ancora inviate. Puoi individuare queste richieste nelle seguenti aree di Adobe Workfront:

* Scheda **Workfront** dell&#39;area Richieste in Workfront: individuare le richieste inviate alle code di richieste di Workfront nelle sezioni seguenti:
   * **Sezione inviata**: tutte le richieste inviate da te o da un altro utente e a cui hai accesso sono almeno View.
   * **Sezione bozza**: tutte le richieste avviate ma non completate e non inviate. Per ulteriori informazioni sulle bozze di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!TIP]
  >
  >È possibile visualizzare solo le proprie bozze di richieste.

* Scheda **Planning** dell&#39;area Richieste in Workfront: individuare le richieste inviate ai moduli di richiesta di Workfront Planning. L&#39;organizzazione deve acquistare un pacchetto Workfront Planning. Per informazioni, vedere i seguenti articoli:

   * [Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
   * [Inviare richieste di Adobe Workfront Planning per creare record](/help/quicksilver/planning/requests/submit-requests.md)


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   Oppure
   <p>Corrente: richiesta o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>Modifica l'accesso alle Issues</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Visualizza autorizzazioni o versioni successive nelle richieste</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Prodotto</td> 
   <td> <ul><li>Adobe Workfront</li><li>È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Individuare le richieste inviate

Per individuare le richieste inviate da te o da altri utenti:

{{step1-to-requests}}

1. (Condizionale) Se la tua organizzazione ha acquistato un pacchetto Workfront Planning, fai clic sulla scheda **Workfront** per visualizzare le richieste di Workfront.
1. Fai clic su **Inviato** nel pannello a sinistra per visualizzare tutte le richieste inviate.

   È possibile visualizzare fino a 2.000 richieste, che possono essere visualizzate su più pagine.

   >[!TIP]
   >
   >Non è possibile personalizzare le colonne nell’elenco delle richieste inviate.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. Per impostazione predefinita, vengono visualizzate le seguenti colonne:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Nome</td> 
         <td> <p>Nome della richiesta.</p> <p>Fai clic sul nome di una richiesta per aprirla. </p> <p><b>SUGGERIMENTO</b>

   Se il problema non è stato mantenuto durante la conversione in un’attività o un progetto, il nome del problema viene visualizzato in grigio e non è più possibile fare clic su di esso. Per informazioni sulla conversione dei problemi, vedere <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Panoramica sulla conversione dei problemi in Adobe Workfront</a>. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">Convertito in</td> 
         <td> <p>Nome dell'oggetto di risoluzione, che può essere un'attività o un progetto a cui è stata convertita la richiesta. </p> <p>Fare clic sul nome dell'attività o del progetto per aprirli. </p> <p>Se la richiesta non è stata convertita, questo campo è vuoto. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Percorso</td> 
         <td>Il nome della coda di richieste, dei gruppi di argomenti e degli argomenti della coda in cui la richiesta è stata inviata in origine. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Stato</td> 
         <td>Stato corrente della richiesta o dell'oggetto di risoluzione (attività o progetto)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Data inserimento</td> 
         <td>La data in cui la richiesta è stata inviata o la data in cui è stato creato l’oggetto di risoluzione se la richiesta è stata eliminata al momento della conversione. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Data ultimo aggiornamento</td> 
         <td> <p>Data dell’ultimo aggiornamento della richiesta.</p> <p>Per impostazione predefinita, l’elenco delle richieste inviate è ordinato in base a questo campo. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Facoltativo) Fai clic sull’intestazione di una colonna per ordinarla.

   >[!TIP]
   >
   >Quando ci si sposta dall’elenco Richieste inviate, l’opzione di ordinamento selezionata viene mantenuta.

1. (Facoltativo) Selezionare una richiesta nell&#39;elenco, quindi fare clic sull&#39;icona **Apri riepilogo** ![](assets/open-summary-with-text-nwe.png) per aprire il pannello Riepilogo e visualizzare ulteriori informazioni sulla richiesta, aggiungere commenti, documenti o assegnarla. Per informazioni sul pannello Riepilogo, vedere [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >Se il pannello Riepilogo è già aperto, l&#39;icona Apri riepilogo diventa Chiudi riepilogo.

1. (Facoltativo e condizionale) Fai clic sull&#39;icona **X** in alto a destra o sull&#39;icona **Chiudi riepilogo** ![](assets/close-summary-with-text-nwe.png) per chiudere il pannello Riepilogo.

   Se un problema è stato convertito in un’attività o un progetto e successivamente eliminato nel processo di conversione, il pannello Riepilogo risulta vuoto. Per informazioni sulla conversione dei problemi, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Dall&#39;icona **Filtro** ![](assets/filter-nwepng.png) in alto a destra dell&#39;elenco, selezionare uno dei filtri elencati nella tabella seguente.

   >[!TIP]
   >
   >Non è possibile modificare i filtri nella sezione Inviato dell’area Richieste.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutto</td> 
      <td>Tutte le richieste inviate, indipendentemente dallo stato o da chi le ha inviate.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>Tutte le richieste inviate che sono attualmente aperte, indipendentemente da chi le ha inviate. Solo le richieste per le quali disponi almeno delle autorizzazioni di visualizzazione vengono visualizzate qui se non le hai inviate personalmente. </p> <p>Le richieste senza una data di completamento effettiva o il cui oggetto di risoluzione non dispone di una data di completamento effettiva sono elencate nella scheda secondaria Apri.</p> <p><b>SUGGERIMENTO</b>

   Le richieste con uno stato diverso da Chiuso vengono considerate aperte.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Le mie richieste</td> 
      <td>Richieste inviate indipendentemente dal loro stato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le mie richieste aperte</td> 
      <td> <p>Richieste inviate ancora aperte. </p> <p>Le richieste senza una data di completamento effettiva o il cui oggetto di risoluzione non dispone di una data di completamento effettiva sono elencate nella scheda secondaria Richieste personali aperte. </p> <p><b>SUGGERIMENTO</b>

   Le richieste che non si trovano in uno stato che equivale a Chiuso vengono considerate aperte.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic sull&#39;icona **del filtro** Pagina![](assets/search-icon.png) nella parte superiore dell&#39;elenco per cercare una richiesta in base al nome. L’elenco viene aggiornato con risultati che corrispondono ai criteri di ricerca.

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Fai clic su **Bozze** per visualizzare tutte le richieste bozze. Workfront salva un numero illimitato di bozze per ogni coda di richieste in questa cartella. Quando si immette una nuova richiesta per un argomento della coda che presenta già una bozza, viene richiesto di utilizzare una bozza esistente. Per ulteriori informazioni, vedere [Creare richieste dalle bozze](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

1. (Facoltativo e condizionale) Se la tua organizzazione ha acquistato un pacchetto Workfront Planning, fai clic sulla scheda **Planning**, quindi fai clic su **Inviato** nel pannello a sinistra per visualizzare le richieste di Workfront Planning.

   Utilizzare **Filtri** e **Colonne** per aggiornare le informazioni nell&#39;elenco delle richieste di Planning.

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).


