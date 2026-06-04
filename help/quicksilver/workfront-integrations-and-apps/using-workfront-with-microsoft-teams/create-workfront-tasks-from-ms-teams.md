---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Crea [!DNL Adobe Workfront] attività da [!DNL Microsoft] Team
description: Puoi creare attività personali in Adobe [!DNL Workfront] da Microsoft Teams se un proprietario del team ha installato e configurato [!DNL Workfront] Microsoft Teams per il tuo team e hai effettuato l'accesso a Workfront da Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
TQID: https://experienceleague.adobe.com/EGXeEO-HU8813eA-dyVAuKSv6rAQg8tsDiDT5leVee0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: a7ef0b24-c866-4849-a368-53678af2dfe5
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 31%

---

# Crea [!DNL Adobe Workfront] attività da [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Poiché [Microsoft sta eseguendo la transizione al nuovo client Teams](https://learn.microsoft.com/it-it/microsoftteams/teams-classic-client-end-of-availability), il client Teams classico non sarà più disponibile dopo il 1° luglio 2025. Per continuare a utilizzare Microsoft Teams e le app integrate come Workfront, è necessario effettuare la transizione al nuovo client Teams prima di tale data.
>
>L’integrazione aggiornata di Workfront è ora disponibile e completamente compatibile con la nuova esperienza Teams. Nella maggior parte dei casi, Workfront verrà visualizzato automaticamente dopo la transizione degli utenti. In caso contrario, l’integrazione potrà essere installata manualmente dall’App Store di Microsoft Teams. Per installare o verificare l’integrazione di Workfront nel nuovo client Teams, consulta [Installare  [!DNL Adobe Workfront]  per Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).



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
   <td> <p>Standard</p>
   <p>Work o successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È possibile creare attività personali in [!DNL Adobe Workfront] da [!DNL Microsoft Teams] se sono soddisfatte le seguenti condizioni:

* Il proprietario del team ha installato e configurato [!DNL Workfront for Microsoft Teams] per il team.
* Sei connesso a [!DNL Workfront] da [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] non supporta più [!DNL Internet Explorer]. Per utilizzare l&#39;integrazione di [!DNL Adobe Workfront for Microsoft Teams], è necessario utilizzare un browser Web diverso da [!DNL Internet Explorer].

Per informazioni sull&#39;installazione di [!DNL Workfront for Microsoft Teams] e l&#39;accesso a [!UICONTROL Workfront] da [!DNL Microsoft Teams], vedere [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Crea attività personali da [!DNL Microsoft Teams]

1. Accedere a [!DNL Workfront] da [!DNL Microsoft Teams].

   Per informazioni sull&#39;accesso a [!DNL Workfront], vedere [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Per aprire una scheda **[!UICONTROL Nuova attività]**:

   * Se sei nel canale di chat bot [!DNL Workfront], digita **[!UICONTROL Nuova attività]** nel campo [!UICONTROL conversazione] per creare una nuova attività.
   * Se ti trovi in un canale di chat diverso dal canale di chat bot [!DNL Workfront]:

      * Inizia a digitare **[!DNL @workfront]** nel campo [!UICONTROL conversazione], quindi seleziona il canale bot [!DNL Workfront] desiderato.
      * Continua a digitare **[!UICONTROL Nuova attività]** nel campo [!UICONTROL conversazione] per creare una nuova attività.

        La scheda [!UICONTROL Nuova attività] viene visualizzata nel canale bot [!DNL Workfront].

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. Nel canale bot [!UICONTROL Workfront], specifica le seguenti informazioni sulla scheda [!UICONTROL Nuova attività]:

   * Nome attività nel campo **[!UICONTROL Scrivi il titolo dell&#39;attività]**.
   * Descrizione attività nel campo **[!UICONTROL Scrivi la descrizione dell&#39;attività]**.
   * La data entro la quale l&#39;attività deve essere completata, nel campo **[!UICONTROL Data di scadenza]**.

1. Fai clic su **[!UICONTROL Salva].**

   La nuova attività personale viene creata in [!DNL Workfront]. È stato assegnato un [!UICONTROL numero di riferimento], che è visibile nella scheda [!UICONTROL nuova attività].

   Per informazioni sui numeri di riferimento, vedere la sezione [[!UICONTROL Numeri di riferimento] di oggetti](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) nell&#39;articolo [Comprendere gli oggetti in [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facoltativo) Fai clic su **[!UICONTROL Modifica]** per modificare ulteriormente le informazioni sull&#39;attività.
1. (Facoltativo) Fare clic su **[!UICONTROL Visualizza in[!DNL Workfront]]** per aprire l&#39;attività in una nuova scheda in [!DNL Workfront] e modificare ulteriormente l&#39;attività, spostarla in un progetto o assegnarla a un altro utente.
