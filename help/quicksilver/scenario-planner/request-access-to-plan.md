---
product-area: enterprise-scenario-planner-product-area
keywords: piano,autorizzazioni,condivisione,iniziative,scenari,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Richiedere l'accesso a un piano nella Pianificazione scenario
description: È possibile richiedere l'accesso a un piano in Adobe Workfront Scenario Planner quando il collegamento al piano viene condiviso con l'utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Richiedi accesso a un piano in [!DNL Scenario Planner]

È possibile richiedere l&#39;accesso a un piano in [!DNL Adobe Workfront Scenario Planner] quando il collegamento al piano viene condiviso con l&#39;utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per il nuovo piano Workfront Select o Workfront. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td>  <p>Accesso di [!UICONTROL View] o versione successiva al [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
