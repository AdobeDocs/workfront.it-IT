---
title: Inviare richieste di Adobe Workfront Planning
description: Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Inviare richieste di Adobe Workfront Planning per creare record

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.

Gli utenti Workfront e gli utenti esterni possono inviare richieste ai tipi di record Planning e creare record. <!--double check on the external users-->

Questo articolo descrive come inviare una richiesta per aggiungere nuovi record a un tipo di record.

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
   <p>Visualizza o autorizzazioni superiori per un’area di lavoro, se sei un utente di Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
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
   * Tipo di record associato a un modulo di richiesta. Per informazioni, vedere [Creare un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Il modulo di richiesta deve essere condiviso con un collegamento in modo da potervi accedere. Esistono i seguenti scenari:

   * Se disponi di un account Workfront, il collegamento è stato condiviso solo con persone interne e puoi contribuire o accedere più facilmente all’area di lavoro. Gli utenti esterni a Workfront non possono accedere a un collegamento condiviso internamente.
   * Se non disponi di un account Workfront, il collegamento è stato condiviso con persone esterne. Gli utenti di Workfront possono anche accedere a un collegamento condiviso con persone esterne.

* Il collegamento al modulo non deve essere scaduto.

## Considerazioni sull&#39;invio di richieste a Workfront Planning

* È possibile accedere a un modulo di richiesta per le richieste di Workfront Planning solo da un collegamento specifico al modulo.
* Una richiesta inviata a Workfront Planning non può essere modificata.
* Ogni richiesta inviata crea un record per il tipo di record associato al modulo utilizzato <span class="preview">se il modulo non è associato a un&#39;approvazione o se l&#39;approvazione è stata concessa da tutti gli approvatori.</span>
* I record creati con l’invio di moduli di richiesta non possono essere differenziati dai record aggiunti tramite qualsiasi altro metodo. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Le richieste inviate vengono visualizzate nella scheda Pianificazione della sezione Inviate nell&#39;area Richieste di Workfront </span>.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Inviare una richiesta a Workfront Planning

1. Passare al collegamento condiviso con l&#39;utente da un tipo di record di Workfront Planning.

1. Aggiorna i campi disponibili nel modulo. I campi con un asterisco sono obbligatori.

   >[!TIP]
   >
   >   Se il campo **Oggetto** è disponibile, non sarà visibile in Workfront Planning dopo l&#39;invio della richiesta.
   >
   >È consigliabile aggiornare il maggior numero possibile di campi nella richiesta per rendere il nuovo record identificabile quando viene aggiunto al tipo di record in Workfront Planning.

1. Fai clic su **Invia**.

   Il modulo viene inviato e si verificano gli eventi seguenti:

   * Se il modulo di richiesta non è stato associato a un&#39;approvazione o <span class="preview">se l&#39;approvazione è stata concessa da tutti gli approvatori</span>, viene aggiunto un nuovo record al tipo di record associato al modulo.

   * Se il modulo di richiesta non è associato a un&#39;approvazione, la richiesta <span class="preview"> viene aggiunta alla scheda Pianificazione della sezione Inviata dell&#39;area Richieste Workfront e viene aggiunto un nuovo record alla pagina del tipo di record.</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Tutti gli utenti che hanno accesso ad almeno un&#39;area di lavoro possono visualizzare la scheda Pianificazione nell&#39;area Richieste. Puoi visualizzare solo le richieste inviate da te o da altri utenti alle aree di lavoro per le quali disponi almeno delle autorizzazioni di visualizzazione. Gli amministratori di Workfront possono visualizzare tutte le richieste inviate a qualsiasi area di lavoro del sistema. </span> <!--ensure this is correct; asking team in slack-->

   * <span class="preview">Se il modulo di richiesta era associato a un&#39;approvazione, la richiesta viene temporaneamente salvata nella scheda Pianificazione nella sezione Inviata dell&#39;area Richieste Workfront. Nessun record creato per il tipo di record associato al modulo di richiesta.</span>

     <span class="preview">Per informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>
   * <span class="preview">Ricevi una notifica in-app e un messaggio e-mail che informa che la richiesta è stata inviata correttamente o è stata inviata per la revisione.</span>
   * <span class="preview">Se il modulo di richiesta era associato a un&#39;approvazione, gli approvatori ricevono una notifica in-app e un messaggio di posta elettronica per rivedere e approvare la richiesta.</span>

     >[!NOTE]
     >
     ><span class="preview">Le notifiche e-mail e in-app sono visibili solo quando l&#39;istanza di Workfront dell&#39;organizzazione è integrata in Adobe Unified Experience.</span>




