---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporare una coda richieste in una dashboard
description: È possibile incorporare una nuova coda richieste in una dashboard per fornire accesso diretto alla coda richieste agli utenti, senza dover accedere all'area Richieste.
author: Courtney
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 6%

---

# Incorporare una coda richieste in una dashboard

<!-- Audited: 1/2025 -->

È possibile incorporare una nuova coda richieste in una dashboard per fornire accesso diretto alla coda richieste agli utenti, senza dover accedere all&#39;area Richieste.

Ad esempio, se disponi di una coda di richieste aperta all&#39;intera organizzazione, ad esempio una coda dell&#39;help desk o una coda di richieste PTO a cui tutti devono accedere regolarmente, potrebbe essere utile inserire la coda di richieste direttamente in uno dei dashboard per un accesso rapido e semplice. Il processo di impostazione di questa impostazione è simile a quello della creazione di una pagina esterna su un dashboard.

In primo luogo, è necessario ottenere un URL per la coda richieste. In secondo luogo, puoi incorporare l’URL in un dashboard aggiungendo una pagina esterna.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard e calendari</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per il dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Prerequisiti

Prima di poter incorporare una coda di richieste in un dashboard, è necessario creare entrambe le operazioni seguenti:

* **Dashboard**: per informazioni sulla creazione dei dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

* **Coda richieste**: per informazioni sulla creazione delle code richieste, vedere [Creare una coda richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Ottenere l&#39;URL della coda di richieste {#obtain-the-url-of-the-request-queue}

È possibile ottenere l&#39;URL di una coda di richieste in diversi modi, a seconda della parte della coda di richieste che si desidera esporre agli utenti quando vi accedono da un dashboard.

* [Ottenere un collegamento a un argomento della coda specifico con la possibilità di modificare il tipo di richiesta](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [Ottenere un collegamento a una coda di richieste e la possibilità di modificare il tipo di richiesta](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [Ottenere un collegamento a una coda di richieste senza possibilità di modificare il tipo di richiesta](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Ottenere un collegamento a un argomento della coda specifico con la possibilità di modificare il tipo di richiesta {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Quando si condivide un collegamento a un argomento della coda specifico con altri utenti, il modulo di richiesta viene aperto in corrispondenza dell&#39;argomento della coda esatto necessario per inviare la richiesta. Ciò è utile quando gli utenti potrebbero non essere sicuri di quale argomento della coda scegliere quando registrano le richieste per una coda di richieste specifica.

Gli utenti possono modificare il tipo di richiesta o scegliere un altro argomento, se necessario. Viene visualizzata anche la navigazione dell&#39;area Richieste.

1. Fai clic sul **menu principale** > **richieste** > **nuova richiesta**.
1. Se si desidera condividere una coda specifica, continuare a selezionare i gruppi di argomenti e gli argomenti della coda fino a raggiungere la coda che si desidera condividere nel dashboard. Per informazioni sull&#39;invio di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >La selezione dei gruppi di argomenti e degli argomenti della coda è facoltativa.

1. Fai clic su **Condividi percorso** nell&#39;angolo superiore destro dell&#39;area Nuova richiesta.

   In questo modo il collegamento viene copiato nella coda richieste o nell&#39;argomento della coda mentre viene visualizzato sullo schermo. Gli utenti possono aggiornare il Tipo di richiesta o uno qualsiasi dei gruppi di argomenti e degli argomenti della coda disponibili.

   ![Coda richieste con percorso condivisione](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Ottenere un collegamento a una coda di richieste e la possibilità di modificare il tipo di richiesta {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Quando condividi un collegamento a un tipo di richiesta, questo viene selezionato per l’utente. Questa funzione è utile quando gli utenti devono scegliere tra più gruppi di argomenti o argomenti in coda per lo stesso tipo di richiesta. Gli utenti possono modificare il tipo di richiesta e sceglierne un altro. Viene visualizzata anche la navigazione dell&#39;area Richieste.

1. Passa a un progetto designato come coda di richieste.

   Per informazioni sulla creazione di una coda di richieste da un progetto, passare a [Crea una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vai a **Dettagli coda**.
1. Copiare il codice trovato nel campo **URL di accesso diretto**.

   Il codice dovrebbe essere simile al seguente:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Collegamento alla coda di richieste associata al progetto selezionato. Tipo di richiesta preselezionato.

   Gli utenti possono selezionare qualsiasi gruppo di argomenti o argomento di coda di cui hanno bisogno oppure scegliere un altro tipo di richiesta.

   ![URL coda richieste](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Ottenere un collegamento a una coda di richieste senza possibilità di modificare il tipo di richiesta {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Quando condividi un collegamento a un tipo di richiesta preselezionato, il tipo di richiesta viene selezionato per l’utente e non può essere modificato (è disattivato). Gli utenti possono scegliere i gruppi di argomenti o gli argomenti in coda necessari. Questa funzione è utile quando non si desidera che gli utenti visualizzino e selezionino altri tipi di richiesta. La navigazione dell’area Richieste non viene visualizzata.

1. Passa a un progetto designato come coda di richieste.

   Per informazioni sulla creazione di una coda di richieste da un progetto, passare a [Crea una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vai a **Dettagli coda**.
1. Copiare il codice trovato nel campo **Codice incorporato**.

   Il codice dovrebbe essere simile al seguente:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Modifica il codice per mantenere solo le informazioni seguenti:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Puoi aggiungere un tag `<samp>iframe </samp>` quando incorpori il codice in un&#39;applicazione diversa da Workfront.

   Collegamento alla coda di richieste associata al progetto selezionato. Il tipo di richiesta è preselezionato e non può essere modificato.

   Gli utenti possono selezionare qualsiasi gruppo di argomenti o argomento della coda di cui hanno bisogno per il tipo di richiesta selezionato. Gli utenti non possono selezionare un altro tipo di richiesta.

   ![Codice coda richieste](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Incorporare una coda richieste in una dashboard

È possibile incorporare un collegamento alla coda delle richieste o a un argomento della coda nidificato sotto una coda delle richieste in un dashboard per consentire agli utenti di accedere direttamente all&#39;immissione delle richieste.

1. Ottenere un URL della coda richieste utilizzando uno dei metodi descritti nella sezione [Ottenere l&#39;URL della coda richieste](#obtain-the-url-of-the-request-queue) di questo articolo.

1. Fai clic sul **menu principale** > **dashboard** > **Nuovo dashboard**.

1. Digitare un **Nome** per il dashboard. Questo è un campo obbligatorio.

1. Fare clic su **Aggiungi pagina esterna**.

   ![Pagina esterna](assets/add-external-page-highlighted---nwe-350x214.png)

1. Nella casella **Aggiungi pagina esterna** modificare i campi seguenti:

   * **Nome**: immettere il nome della coda di richieste che si desidera visualizzare nel dashboard. Questo è un campo obbligatorio.

   * **Descrizione**: immettere una descrizione per la visualizzazione di questa pagina esterna. Questo campo non è obbligatorio ed è importante solo per scopi di reporting. Non viene visualizzato nel dashboard.

   * **URL**: incolla l&#39;URL ottenuto utilizzando uno dei metodi descritti nel passaggio 1.

   * **Altezza**: immettere l&#39;altezza della pagina esterna. Questo definisce quanto spazio occupa nel dashboard la pagina esterna contenente la coda di richieste. Questo campo è obbligatorio e il valore predefinito è 500.

1. Fai clic su **Salva**.

1. Fai clic su **Salva e Chiudi**.

   La coda di richieste viene visualizzata nel dashboard come un componente del dashboard separato.

1. (Facoltativo) Fare clic su **Azioni dashboard**, quindi su **Modifica** per aggiungere report, calendari o altre pagine esterne allo stesso dashboard.

   Per informazioni sull&#39;aggiunta di componenti a un dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
