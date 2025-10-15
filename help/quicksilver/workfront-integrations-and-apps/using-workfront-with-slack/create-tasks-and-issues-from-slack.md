---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Creazione di attività e problemi da Slack
description: Dopo aver installato e configurato [!DNL Adobe Workfront] per Slack, puoi creare attività e problemi da Slack e associarli ai progetti in Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Crea attività e problemi da [!DNL Slack]

Dopo aver installato e configurato [!DNL Adobe Workfront for Slack], puoi creare attività e problemi da [!DNL Slack] e associarli ai progetti in [!DNL Workfront].

Per ulteriori informazioni sulla configurazione di [!DNL Workfront] con [!DNL Slack], vedere [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Devi avere accesso per creare attività e problemi nel tuo livello di accesso e devi disporre di [!UICONTROL autorizzazioni Contribute] sul progetto a cui stai associando.

Per ulteriori informazioni sui livelli di accesso, vedere [Panoramica sui livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Per ulteriori informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/it/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].\

## Prerequisiti

Prima di poter creare attività e problemi da [!DNL Slack], è necessario

* Configura [!DNL Workfront] per Slack\
   Per istruzioni sulla configurazione di [!DNL Workfront for Slack], vedere [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Crea attività da [!DNL Slack]

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a Workfront da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo del messaggio:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >I comandi distinguono tra maiuscole e minuscole. Puoi avviare il comando con `/wf` invece di `/workfront`.
   >  
   >È necessario immettere il nome dell&#39;attività così come verrà visualizzato nell&#39;interfaccia [!DNL Workfront], senza parentesi quadre o virgolette.

1. (Facoltativo) Iniziare a digitare il nome di un progetto a cui si desidera associare la nuova attività e selezionarlo quando viene visualizzato nell&#39;elenco.\
   Viene visualizzata una conferma che indica che l&#39;attività è stata aggiunta al progetto selezionato.
1. (Facoltativo) Fare clic sul nome dell&#39;attività nel messaggio di conferma per aprirla in [!DNL Workfront], in una nuova scheda del browser.

## Crea problemi da [!DNL Slack]

1. Accedi all&#39;istanza [!DNL Slack] e accedi a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedere la sezione &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo del messaggio:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >I comandi distinguono tra maiuscole e minuscole. È possibile avviare il comando con &#39;/wf&#39; invece di &#39;/workfront.&#39; \
   >Il Nome problema deve essere immesso così come verrà visualizzato nell&#39;interfaccia [!DNL Workfront], senza parentesi quadre o virgolette.

1. (Facoltativo) Inizia a digitare il nome di un progetto a cui vuoi associare il nuovo problema e selezionalo quando viene visualizzato nell’elenco.\
   Viene visualizzata una conferma che indica che il problema è stato aggiunto al progetto selezionato.
1. (Facoltativo) Fai clic sul nome del problema nel messaggio di conferma per aprirlo in [!DNL Workfront], in una nuova scheda del browser.
