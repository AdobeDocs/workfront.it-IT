---
title: Inviare richieste di Adobe Workfront Planning
description: Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '1878'
ht-degree: 0%

---

# Inviare richieste di Adobe Workfront Planning per creare record

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Dopo che un responsabile dell&#39;area di lavoro crea un modulo di richiesta per un tipo di record in Adobe Workfront Planning, è possibile utilizzare il modulo per inviare richieste che creeranno record per il tipo di record associato al modulo.

È possibile inviare una richiesta di Workfront Planning dalle aree seguenti:

* Dall’area Richieste di Workfront.
* Da un collegamento diretto al modulo di richiesta condiviso.

  Questo articolo descrive come inviare una richiesta per aggiungere nuovi record a un tipo di record dall’area Richieste di Workfront o da un collegamento condiviso.
* <span class="preview">Dalla pagina del tipo di record, quando si aggiunge o si richiede un nuovo record. Per informazioni, vedere [Crea record](/help/quicksilver/planning/records/create-records.md).</span>

Gli utenti Workfront e gli utenti esterni possono inviare richieste ai tipi di record Planning e creare record. <!--double check on the external users-->

Per informazioni su come un manager area di lavoro può creare un modulo di richiesta e associarlo a un tipo di record, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotti</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td>
   <td>
<p>Uno dei seguenti piani di Workfront:</p>
<ul><li>Seleziona</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p>
   </td>
<tr>
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td>
   <td>
<p>Qualsiasi </p>  
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </td>
<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Licenza Esterna, Collaboratore, Light o Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <p>Visualizza o autorizzazioni superiori per un'area di lavoro <!--<span class="preview">and record type</span>-->, se sei un utente di Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>Per accedere all'area Planning in Workfront, è necessario disporre di un modello di layout che includa l'area Planning nel menu principale. </p>
   <p> Tuttavia, per inviare richieste a Workfront Planning non è necessario accedere all'area Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di inviare una richiesta a un modulo di richiesta Workfront Planning, è necessario disporre dei seguenti elementi:

* In Workfront Planning devono esistere gli elementi seguenti:

   * Un’area di lavoro
   * Un tipo di record.
   * Modulo di richiesta associato a un tipo di record.

     Per informazioni, vedere [Creare un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Il modulo di richiesta deve essere condiviso in modo da potervi accedere. Esistono i seguenti scenari:

   * Internamente, il modulo deve essere condiviso con utenti che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro.

     Gli utenti di Workfront possono accedere al modulo da un collegamento <span class="preview"> oppure trovare il modulo di richiesta nell&#39;area Richieste di Workfront.</span>

   * Se non disponi di un account Workfront, significa che un collegamento al modulo è stato condiviso con persone esterne.

     Gli utenti di Workfront possono anche accedere a un collegamento condiviso con persone esterne.

* Il collegamento al modulo non deve essere scaduto.

## Considerazioni sull&#39;invio di richieste a Workfront Planning

* Non è possibile modificare una richiesta in Workfront dopo averla inviata.
* Ogni richiesta sottomessa crea un record per il tipo di record associato al modulo utilizzato, se il modulo non è associato a un&#39;approvazione o se l&#39;approvazione è stata concessa da tutti gli approvatori.
* I record creati mediante l&#39;invio di moduli di richiesta non possono essere distinti dai record aggiunti tramite qualsiasi altro metodo in Workfront Planning.

  Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* Le richieste inviate vengono visualizzate nella scheda Pianificazione della sezione Inviate dell&#39;area Richieste di Workfront.
* Esistono limitazioni nella visualizzazione di determinati tipi di campo in un modulo di richiesta o nella pagina dei dettagli della richiesta dopo l’invio di un modulo.

  Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


<div class="preview">

## Inviare una richiesta a Workfront Planning nell&#39;area Richieste di Workfront

>[!NOTE]
>
>Dopo i rilasci mensili in Produzione, le funzioni descritte in questa sezione sono disponibili anche nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi.

{{step1-to-requests}}

1. Abilita **Passa a una nuova esperienza** nell&#39;angolo superiore destro dello schermo.
L&#39;abilitazione di questa impostazione rende disponibili i moduli di richiesta di Workfront Planning nell&#39;area **Richieste** di Workfront.

   >[!TIP]
   >
   >Questa impostazione è disponibile solo quando sono presenti le seguenti condizioni:
   >
   >* La società ha acquistato un pacchetto Workfront Planning.
   >* La tua istanza di Workfront è integrata in Adobe Unified Experience.
   >* Puoi accedere alla visualizzazione di almeno un’area di lavoro.
   >

1. Fai clic su **Nuova richiesta**.

   ![Nuova casella di richiesta con schede Workfront e Planning unificate](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   Viene visualizzata la casella **Nuova richiesta** con le seguenti informazioni:

   * Le 6 code di richieste Workfront e i moduli di richiesta Planning utilizzati più di recente vengono visualizzati nella sezione Recenti.
   * Nella sezione **Tutti i moduli di richiesta** vengono visualizzate in ordine alfabetico 50 code di richiesta Workfront e moduli di richiesta Planning aggiuntivi. Puoi cercare una coda di richieste che non viene visualizzata per impostazione predefinita.

1. Esegui una delle operazioni seguenti:

   * Fare clic sulla scheda di uno dei moduli di richiesta Planning nelle sezioni Moduli di richiesta recenti o Tutti
   * Inizia a digitare il nome di un modulo di richiesta Planning nella casella di ricerca, quindi fai clic sulla scheda quando viene visualizzata nell’elenco.

   Viene aperto il modulo di richiesta.

1. Aggiorna i campi disponibili nel modulo di richiesta. I campi con un asterisco rosso sono obbligatori.
1. Fai clic su **Invia**.

   Il modulo di richiesta si chiude e si torna all&#39;area **Richieste**.

   Il modulo viene inviato e si verificano gli eventi seguenti:

   * Se il modulo di richiesta non è stato associato a un&#39;approvazione, la richiesta viene aggiunta alla scheda Pianificazione della sezione Inviata dell&#39;area Richieste di Workfront e viene aggiunto un nuovo record al tipo di record associato al modulo.

   * Se il modulo di richiesta era associato a un’approvazione, la richiesta viene aggiunta alla scheda Pianificazione della sezione Inviata dell’area Richieste di Workfront. Un nuovo record viene aggiunto alla pagina del tipo di record solo dopo l&#39;approvazione di tutti gli approvatori.

     Per informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Area richieste con attivazione/disattivazione della scheda di pianificazione del flusso di lavoro unificato](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Tutti gli utenti che hanno accesso ad almeno un&#39;area di lavoro possono visualizzare la scheda Pianificazione nell&#39;area Richieste. Puoi visualizzare solo le richieste inviate da te o da altri utenti alle aree di lavoro per le quali disponi almeno delle autorizzazioni di visualizzazione. Gli amministratori di Workfront possono visualizzare tutte le richieste inviate a qualsiasi area di lavoro del sistema.

   * Ricevi una notifica in-app e un messaggio e-mail che informa che la richiesta è stata inviata correttamente o è stata inviata per la revisione.
   * Se il modulo di richiesta era associato a un’approvazione, gli approvatori ricevono una notifica in-app e un messaggio e-mail per rivedere e approvare la richiesta.

     >[!NOTE]
     >
     >Le notifiche e-mail e in-app sono visibili solo quando l’istanza di Workfront della tua organizzazione viene integrata in Adobe Unified Experience.

   1. (Facoltativo) Fai clic su **Visualizza la richiesta** nel messaggio di conferma, per aprire la richiesta, oppure fai clic sull&#39;icona **X** per chiudere la conferma.

1. (Facoltativo) Fai clic sulla scheda **Planning** nell&#39;area Richieste per visualizzare la richiesta, quindi fai clic sul nome della richiesta.

   Viene visualizzata la pagina dei dettagli della richiesta.

   ![Pagina dettagli richiesta](assets/request-details-page.png)

1. (Condizionale) Se il modulo di richiesta non è associato a un&#39;approvazione o se la richiesta è stata approvata, fare clic sul nome della richiesta, quindi sul nome del record nel campo **Record**.

   La pagina del record viene visualizzata in Workfront Planning.

   >[!TIP]
   >
   >* Se il campo principale del record non è stato aggiornato nel modulo di richiesta, il nome del record nel campo Record della richiesta viene visualizzato come **Senza titolo**.
   >
   >* Se il modulo di richiesta è associato a un’approvazione, questa deve essere concessa prima di poter accedere al record dalla pagina della richiesta.

1. (Facoltativo) Fare clic sul nome del tipo di record ****.

   La pagina del tipo di record viene visualizzata in Workfront Planning.

</div>

## Inviare una richiesta a Workfront Planning da un collegamento condiviso a un modulo di richiesta

1. Passare al collegamento condiviso con l&#39;utente da un tipo di record di Workfront Planning.

1. Aggiorna i campi disponibili nel modulo. I campi con un asterisco sono obbligatori.

   >[!TIP]
   >
   >   Se il campo **Oggetto** è disponibile, non sarà visibile in Workfront Planning dopo l&#39;invio della richiesta.
   >
   >È consigliabile aggiornare il maggior numero possibile di campi nella richiesta per rendere il nuovo record identificabile quando viene aggiunto al tipo di record in Workfront Planning.

1. Fai clic su **Invia**.

   Il modulo viene inviato e si verificano gli eventi seguenti:

   * Se il modulo di richiesta non è stato associato a un&#39;approvazione, la richiesta viene aggiunta alla scheda Pianificazione della sezione Inviata dell&#39;area Richieste di Workfront e viene aggiunto un nuovo record al tipo di record associato al modulo.

   * Se il modulo di richiesta era associato a un’approvazione, la richiesta viene aggiunta alla scheda Pianificazione della sezione Inviata dell’area Richieste di Workfront. Un nuovo record viene aggiunto alla pagina del tipo di record solo dopo l&#39;approvazione di tutti gli approvatori.

     Per informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Scheda Pianificazione nelle richieste](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Tutti gli utenti che hanno accesso ad almeno un&#39;area di lavoro possono visualizzare la scheda Pianificazione nell&#39;area Richieste. Puoi visualizzare solo le richieste inviate da te o da altri utenti alle aree di lavoro per le quali disponi almeno delle autorizzazioni di visualizzazione. Gli amministratori di Workfront possono visualizzare tutte le richieste inviate a qualsiasi area di lavoro del sistema. <!--ensure this is correct; asking team in slack-->

   * Ricevi una notifica in-app e un messaggio e-mail che informa che la richiesta è stata inviata correttamente o è stata inviata per la revisione.
   * Se il modulo di richiesta era associato a un’approvazione, gli approvatori ricevono una notifica in-app e un messaggio e-mail per rivedere e approvare la richiesta.

     >[!NOTE]
     >
     >Le notifiche e-mail e in-app sono visibili solo quando l’istanza di Workfront della tua organizzazione viene integrata in Adobe Unified Experience.

1. <span class="preview">(facoltativo) Fai clic su **Visualizza la richiesta** per aprire la richiesta in Workfront.</span>

   Oppure

   <span class="preview">Fare clic su [Invia un&#39;altra richiesta](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) per aprire il modulo di richiesta e aggiungere una nuova richiesta. </span>

1. (Facoltativo) Fai clic su **Menu principale** > **Richieste** > scheda **Pianificazione** per visualizzare la richiesta, quindi fai clic sul nome della richiesta.

   Viene visualizzata la pagina dei dettagli della richiesta.

   ![Pagina dettagli richiesta](assets/request-details-page.png)

1. (Condizionale) Se il modulo di richiesta non è associato a un&#39;approvazione o se la richiesta è stata approvata, fare clic sul nome della richiesta, quindi sul nome del record nel campo **Record**.

   La pagina del record viene visualizzata in Workfront Planning.

   >[!TIP]
   >
   >* Se il nome del record non è stato aggiunto al modulo di richiesta, il nome del record nel campo Record della richiesta viene visualizzato come **Senza titolo**.
   >
   >* Se il modulo di richiesta è associato a un’approvazione, questa deve essere concessa prima di poter accedere al record dalla pagina della richiesta.

1. (Facoltativo) Fare clic sul nome del tipo di record ****.

   La pagina del tipo di record viene visualizzata in Workfront Planning.




