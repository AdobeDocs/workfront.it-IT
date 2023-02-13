---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Creazione di attività e problemi dallo Slack
description: Dopo aver installato e configurato [!DNL Adobe Workfront] ad Slack, è possibile creare attività e problemi dallo Slack e associarli a progetti in Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Crea attività e problemi da [!DNL Slack]

Dopo aver installato e configurato [!DNL Adobe Workfront for Slack], puoi creare attività e problemi da [!DNL Slack] e associarli a progetti in [!DNL Workfront].

Per ulteriori informazioni sulla configurazione [!DNL Workfront] con [!DNL Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

È necessario disporre dell&#39;accesso per creare attività e problemi nel livello di accesso e disporre di [!UICONTROL Collaborare] autorizzazioni per il progetto a cui li stai associando.

Per ulteriori informazioni sui livelli di accesso, vedere [Panoramica dei livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Per ulteriori informazioni sulle autorizzazioni per gli oggetti, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.\

## Prerequisiti

Prima di creare attività e problemi da [!DNL Slack], devi

* Configura [!DNL Workfront] per Slack\
   Per istruzioni sulla configurazione [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Crea attività da [!DNL Slack]

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a Workfront da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo messaggio:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >I comandi sono sensibili all’uso di maiuscole e minuscole. Puoi avviare il comando con `/wf` anziché `/workfront`.
   >  
   >Il Nome attività deve essere immesso così come apparirà nella [!DNL Workfront] senza parentesi né virgolette.\
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)

1. (Facoltativo) Inizia a digitare il nome di un progetto a cui si desidera associare la nuova attività e selezionala quando viene visualizzata nell’elenco.\
   Viene visualizzata una conferma che indica che l’attività è stata aggiunta al progetto selezionato.
1. (Facoltativo) Fai clic sul nome dell’attività nel messaggio di conferma per aprirla in [!DNL Workfront], in una nuova scheda del browser.

## Crea problemi da [!DNL Slack]

1. Accedi al tuo [!DNL Slack] istanza ed accesso a [!DNL Workfront] da [!DNL Slack].\
   Per ulteriori informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare il seguente comando nel campo messaggio:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >I comandi sono sensibili all’uso di maiuscole e minuscole. Puoi avviare il comando con &#39;/wf&#39; invece di &#39;/workfront&#39;. \
   >Il nome del problema deve essere immesso così come apparirà nel [!DNL Workfront] senza parentesi né virgolette.\
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)

1. (Facoltativo) Inizia a digitare il nome di un progetto a cui desideri associare il nuovo problema e selezionalo quando viene visualizzato nell’elenco.\
   Ricevi una conferma che indica che il problema è stato aggiunto al progetto selezionato.
1. (Facoltativo) Fai clic sul nome del problema nel messaggio di conferma per aprirlo in [!DNL Workfront], in una nuova scheda del browser.
