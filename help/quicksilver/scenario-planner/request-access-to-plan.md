---
product-area: enterprise-scenario-planner-product-area
keywords: piano,autorizzazioni,condivisione,iniziative,scenari,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Richiedere l'accesso a un piano nella Pianificazione scenario
description: È possibile richiedere l'accesso a un piano in Adobe Workfront Scenario Planner quando il collegamento al piano viene condiviso con l'utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Richiedi accesso a un piano in [!DNL Scenario Planner]

È possibile richiedere l&#39;accesso a un piano in [!DNL Adobe Workfront Scenario Planner] quando il collegamento al piano viene condiviso con l&#39;utente.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o versione successiva</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza [!DNL Adobe Workfront]<b>*</b> </p> </td> 
   <td> <p>[!UICONTROL Review], [!UICONTROL Work] o [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Prodotto*</strong> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso di visualizzazione o superiore al [!DNL Scenario Planner]</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il livello di accesso, vedere <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone oppure se la società ha acquistato [!DNL Workfront Scenario Planner], contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

Prima di poter richiedere l&#39;accesso a un piano in [!DNL Scenario Planner], è necessario disporre dei seguenti elementi:

* Un link al piano.

>[!NOTE]
>
>Se non si dispone dei diritti di livello di accesso per [!DNL Scenario Planner] e si tenta di accedere a un piano da un collegamento, non è possibile richiedere l&#39;accesso al piano. Viene invece visualizzata una schermata che ti informa di contattare l&#39;amministratore [!DNL Workfront].

## Richiedi accesso per i piani in [!DNL Workfront Scenario Planner]

Se non si dispone già delle autorizzazioni per un piano e si passa a tale piano da un collegamento condiviso con l&#39;utente, viene visualizzata una schermata che informa che non si dispone delle autorizzazioni necessarie per visualizzare il piano. Viene richiesto di richiedere le autorizzazioni al creatore del piano.

>[!TIP]
>
>È possibile richiedere le autorizzazioni solo al proprietario o al creatore di un piano. Non è possibile richiedere le autorizzazioni ad altri utenti che hanno accesso al piano.

Per richiedere le autorizzazioni:

1. Fare clic su un collegamento a un piano.

   ![](assets/request-access-to-plan-350x277.png)

1. Nel menu a discesa **[!UICONTROL Richiedi accesso a]**, indica il livello di autorizzazioni che desideri concedere. Selezionare una delle opzioni seguenti:

   * [!UICONTROL Visualizza]
   * [!UICONTROL Gestisci]

   Impossibile richiedere un&#39;autorizzazione superiore al proprio livello di accesso a [!DNL Scenario Planner]. Ad esempio, non è possibile richiedere le autorizzazioni [!UICONTROL Gestisci] se si dispone dell&#39;accesso di visualizzazione a [!DNL Scenario Planner].

   Per informazioni sui diversi livelli di autorizzazioni, vedere [Condividere un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Per informazioni su come un amministratore di Workfront può gestire l&#39;accesso a [!DNL Scenario Planner], vedere [Concedere l&#39;accesso a  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facoltativo) Immetti un commento o una richiesta nella **[!UICONTROL Casella Lascia commento]**, quindi fai clic su **[!UICONTROL Richiedi accesso]**.

   Si verifica quanto segue:

   * [!DNL Workfront] invia una notifica e-mail al proprietario del piano in cui può concedere le autorizzazioni richieste.\
     ![](assets/request-access-to-plan-email-350x156.png)

   * Dopo che il proprietario del piano ha concesso le autorizzazioni richieste, si riceve un messaggio e-mail che informa che le autorizzazioni sono state concesse se l&#39;amministratore [!DNL Workfront] ha abilitato la condivisione oggetto per la notifica all&#39;utente nel sistema e se si abilita la notifica e-mail [!UICONTROL Qualcuno condivide un oggetto con me] nel profilo.

     ![](assets/access-granted-to-plan-email-350x172.png)

   * Puoi anche concedere autorizzazioni ai piani dall&#39;area [!UICONTROL Home] e dall&#39;app mobile [!DNL Workfront].

   Per informazioni sull&#39;attivazione delle notifiche di sistema, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Per informazioni sull&#39;attivazione delle notifiche nel profilo, vedere [Notifiche: informazioni varie](../workfront-basics/using-notifications/notifications-misc-information.md).
