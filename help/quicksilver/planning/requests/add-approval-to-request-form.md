---
title: Aggiungere un’approvazione a un modulo di richiesta in Adobe Workfront Planning
description: È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un'approvazione per ogni richiesta sottomessa, prima di creare un record.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: de568156315ff9094d938600c91b55e185d53765
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 2%

---

# Aggiungere un’approvazione a un modulo di richiesta in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un&#39;approvazione per ogni richiesta sottomessa, prima di creare un record.

Questo articolo descrive come un manager dell&#39;area di lavoro può aggiungere un&#39;approvazione a un modulo di richiesta associato a un tipo di record.

Per informazioni sulla creazione di un modulo di richiesta in Workfront Planning, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Per informazioni sull&#39;invio di una richiesta a un tipo di record per la creazione di un record, vedere [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p>
Oppure
<p>Qualsiasi pacchetto del flusso di lavoro e qualsiasi pacchetto Planning</p>

<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro e tipo di record</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull’aggiunta di approvazioni a un modulo di richiesta

* È possibile aggiungere uno o più approvatori a un modulo di richiesta. È possibile aggiungere solo utenti come approvatori.
* È possibile visualizzare le informazioni sull&#39;approvazione in un record creato inviando un modulo di richiesta nei campi Approvato da e Data approvata. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).
* Quando si aggiungono più approvatori a un modulo di richiesta, tutti gli approvatori devono accettare la richiesta prima di creare un record in Workfront Planning.
* Se tutti gli approvatori approvano la richiesta, viene creato un record per il tipo di record associato al modulo di richiesta.
* Se almeno un approvatore rifiuta la richiesta e tutti gli altri la approvano, viene creata una richiesta per l&#39;area Richieste di Workfront, ma non viene creato alcun record per il tipo di record associato al modulo di richiesta.
* L’aggiunta di approvazioni a un modulo di richiesta è facoltativa. Workfront Planning crea immediatamente un record quando viene sottomessa una richiesta, se il modulo di richiesta non è associato a un&#39;approvazione.

## Aggiungere un’approvazione a un modulo di richiesta

1. Iniziare a creare un modulo di richiesta per un tipo di record, come descritto in [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Fare clic su **Configurazione**.

   Viene visualizzata l&#39;area **Configurazione**.

   ![Scheda Configurazione](assets/configuration-tab.png)
1. Nel campo **Approvatori**, inizia a digitare il nome di un utente o team che desideri impostare come approvatore, quindi selezionalo quando viene visualizzato nell&#39;elenco.
1. (Facoltativo e condizionale) Se hai impostato più di un approvatore e hai bisogno di un solo approvatore per prendere una decisione, abilita l&#39;opzione **È richiesta una sola decisione**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Puoi aggiungere uno o più approvatori a un modulo di richiesta.
   >
   >* Se si aggiungono più approvatori e l&#39;opzione È necessaria una sola decisione non è abilitata, tutti gli approvatori devono approvare la richiesta prima che Workfront Planning crei un record.
   >
   >* Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il record non viene creato. La richiesta rimane nella scheda Pianificazione della sezione Inviata nell&#39;area Richieste di Workfront.
   >
   >* Se si aggiungono più approvatori e l&#39;opzione È necessaria una sola decisione non è abilitata, tutti gli approvatori devono prendere una decisione prima che una richiesta venga approvata o rifiutata.
   >
   >* Se un team è impostato come approvatore, è necessaria una sola decisione del team.


1. (Facoltativo) Fai clic su **Pubblica** se non hai mai condiviso il modulo di richiesta in precedenza

   Oppure

   Fai clic su **Condividi** per condividere il modulo, quindi su **Copia collegamento**.
1. (Facoltativo) Dopo che un utente utilizza il collegamento condiviso e invia una richiesta, Workfront Planning invia una notifica in-app di approvazione e un messaggio e-mail agli approvatori.

   >[!NOTE]
   >
   >   Per consentire agli utenti di ricevere notifiche e-mail e in-app, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.


   Per informazioni sull&#39;approvazione delle richieste, vedere [Approvare una richiesta](/help/quicksilver/planning/requests/approve-request.md).
