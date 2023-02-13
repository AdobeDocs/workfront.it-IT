---
navigation-topic: notifications
title: Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima
description: Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente quando hai effettuato l’accesso a Anteprima.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima

[!UICONTROL Adobe Workfront] disabilita tutte le comunicazioni e-mail dagli ambienti Preview e Custom Refresh Sandbox. Per informazioni sull’ambiente Sandbox di anteprima, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Per informazioni sull’ambiente Sandbox di aggiornamento personalizzato, consulta [Ambiente Sandbox di aggiornamento personalizzato di Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Se desideri ricevere le seguenti notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente mentre sei connesso a Anteprima:

* Notifiche e-mail attivate dalle notifiche degli eventi
* Notifiche promemoria
* Notifiche di promemoria automatiche in ritardo o in anticipo
* Inviti e-mail

Puoi eseguire questa operazione autonomamente o per qualsiasi utente a cui hai accesso per la modifica. Per ulteriori informazioni sull&#39;accesso necessario per modificare gli utenti, vedi [Concedere l’accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Le notifiche di consegna dei rapporti e push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di anteprima. Né tu né il [!DNL Workfront] L’amministratore può abilitare la consegna dei rapporti o le notifiche push per l’app mobile quando accedi all’ambiente Sandbox di anteprima.
>
>Per informazioni sulle consegne dei rapporti, vedi [Panoramica sulla consegna dei rapporti](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>[!UICONTROL Request] o superiore per modificare la tua impostazione</p> <p>Pianificare per modificare l’impostazione per altri utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso [!UICONTROL System Administrator].</p> <p> Per informazioni su questo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p>Nel tuo livello di accesso, [!UICONTROL Edit] deve essere selezionato per l’impostazione [!UICONTROL Users]. E, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , l’opzione [!UICONTROL Crea] e almeno una delle due opzioni [!UICONTROL User Admin] devono essere abilitate. </p> <p>Se utilizzi l’opzione [!UICONTROL User Admin (Group Users)] , devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Per informazioni sull'impostazione [!UICONTROL Users] in un livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima

1. Accedi al tuo ambiente Sandbox di anteprima.
1. Fai clic sull’immagine del profilo nell’angolo superiore destro di [!DNL Adobe Workfront]. Quindi, fai clic sul pulsante **[!UICONTROL Altro]** menu e seleziona **[!UICONTROL Modifica]**.

   Oppure

   Cerca un utente in [!DNL Workfront] e fare clic sul loro nome. Quindi, fai clic sul pulsante **[!UICONTROL Altro]** menu e seleziona **[!UICONTROL Modifica]**.

   Oppure

   Per più utenti: Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **[!UICONTROL Utenti]** ![](assets/users-icon-in-main-menu.png).  Quindi, seleziona più utenti e fai clic su **[!UICONTROL Modifica]**.

1. Fai clic su **[!UICONTROL Preferenze]**.
1. Seleziona **[!UICONTROL Ricevi e-mail da questo ambiente di test]**.

   >[!NOTE]
   >
   >Questa opzione non è disponibile se ti trovi in un ambiente di produzione.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
