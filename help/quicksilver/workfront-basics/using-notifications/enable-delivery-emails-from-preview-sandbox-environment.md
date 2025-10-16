---
navigation-topic: notifications
title: Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima
description: Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente mentre sei connesso all’ambiente di anteprima.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima

[!UICONTROL Adobe Workfront] disabilita tutte le comunicazioni e-mail dagli ambienti Sandbox Anteprima e Aggiornamento personalizzato. Per informazioni sull&#39;ambiente Sandbox di anteprima, vedere [Ambiente Sandbox di anteprima Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Per informazioni sull&#39;ambiente Sandbox di aggiornamento personalizzato, vedere [Ambiente Sandbox di aggiornamento personalizzato di Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Se desideri ricevere le seguenti notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente durante l’accesso in Anteprima:

* Notifiche e-mail attivate da notifiche di eventi
* Notifiche promemoria
* Notifiche automatiche di promemoria in ritardo o anticipato
* Inviti e-mail

Puoi eseguire questa operazione per te stesso o per qualsiasi utente con accesso da modificare. Per ulteriori informazioni sull&#39;accesso necessario per modificare gli utenti, vedere [Concedere l&#39;accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>La consegna dei rapporti e le notifiche push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di anteprima. Né l&#39;utente né l&#39;amministratore [!DNL Workfront] possono abilitare la consegna dei rapporti o le notifiche push per l&#39;app mobile quando si accede all&#39;ambiente Sandbox di anteprima.
>
>Per informazioni sulle consegne dei report, vedi [Panoramica sulla consegna dei report](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> 
   <p>Collaboratore o versione successiva per modificare la propria impostazione</p> <p>Standard per modificare l'impostazione per altri utenti</p> 
   Oppure
   <p> Richiedi o superiore di modificare la tua impostazione</p> <p>Pianifica la modifica dell’impostazione per altri utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso [!UICONTROL System Administrator].</p> </li> 
     <li> <p>Nel livello di accesso, è necessario selezionare [!UICONTROL Edit] per l'impostazione [!UICONTROL Users]. Per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , è necessario abilitare l'opzione [!UICONTROL Create] e almeno una delle due opzioni [!UICONTROL User Admin]. </li> 
     <li>Se si utilizza l'opzione [!UICONTROL User Admin (Group Users)], è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima

1. Accedi all’ambiente Sandbox di anteprima.
1. Fai clic sull&#39;immagine del tuo profilo nell&#39;angolo superiore destro di [!DNL Adobe Workfront]. Quindi fare clic sul menu **[!UICONTROL Altro]** e selezionare **[!UICONTROL Modifica]**.

   Oppure

   Cercare un utente in [!DNL Workfront] e fare clic sul nome. Quindi fare clic sul menu **[!UICONTROL Altro]** e selezionare **[!UICONTROL Modifica]**.

   Oppure

   Per più utenti: fare clic sull&#39;icona **[!UICONTROL Menu principale]** ![Icona menu principale](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Workfront, quindi fare clic sull&#39;icona **[!UICONTROL Utenti]** ![Icona utente](assets/users-icon-in-main-menu.png).  Quindi, selezionare più utenti e fare clic su **[!UICONTROL Modifica]**.

1. Fai clic su **[!UICONTROL Preferenze]**.
1. Seleziona **[!UICONTROL Ricevi e-mail da questo ambiente di test]**.

   >[!NOTE]
   >
   >Questa opzione non è disponibile se ti trovi in un ambiente di produzione.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
