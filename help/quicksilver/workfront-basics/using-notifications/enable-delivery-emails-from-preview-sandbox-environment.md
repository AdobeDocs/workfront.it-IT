---
navigation-topic: notifications
title: Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima
description: Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente mentre sei connesso all’ambiente di anteprima.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '522'
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

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o versione successiva per modificare l'impostazione</p> <p>[!UICONTROL Plan] per modificare l'impostazione per altri utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso [!UICONTROL System Administrator].</p> <p> Per informazioni su questo livello di accesso, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Nel livello di accesso, è necessario selezionare [!UICONTROL Edit] per l'impostazione [!UICONTROL Users]. Per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , è necessario abilitare l'opzione [!UICONTROL Create] e almeno una delle due opzioni [!UICONTROL User Admin]. </p> <p>Se si utilizza l'opzione [!UICONTROL User Admin (Group Users)], è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Per informazioni sull'impostazione [!UICONTROL Users] in un livello di accesso, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
    </ul> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

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
