---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Visualizzare e gestire applicazioni OAuth2 personalizzate
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di Workfront, che consente ad altre applicazioni di accedere a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 1%

---

# Visualizzare e gestire applicazioni OAuth2 personalizzate

Come [!DNL Adobe Workfront] amministratore, puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono l&#39;accesso ad altre applicazioni [!UICONTROL Workfront].

>[!NOTE]
>
>Nel contesto di OAuth2, &quot;applicazione Oauth2&quot; fa riferimento a questo tipo di collegamento di accesso tra un’app e un server come [!DNL Workfront]. Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* Per informazioni sulla creazione di applicazioni OAuth2 personalizzate, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 con le credenziali utente (flusso di codice di autorizzazione), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando l’autenticazione server (flusso JWT), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando PKCE, consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> Devi essere un [!DNL Workfront] amministratore. </p>
    <p>Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Devi creare [!UICONTROL OAuth2] le applicazioni per la tua organizzazione prima di poterle visualizzare o gestire.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gestione di applicazioni OAuth2 personalizzate

* [Visualizzare e modificare applicazioni OAuth2 personalizzate](#view-and-edit-custom-oauth2-applications)
* [Eliminare applicazioni OAuth2 personalizzate](#delete-custom-oauth2-applications)

### Visualizzare e modificare applicazioni OAuth2 personalizzate {#view-and-edit-custom-oauth2-applications}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Passa il puntatore sull’applicazione e fai clic su **[!UICONTROL Modifica]** ![](assets/edit-icon.png) quando appare all&#39;estrema destra.
1. (Facoltativo) Modificare i dettagli dell&#39;applicazione.

   Per i campi relativi alle app OAuth2 e JWT, vedi [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Eliminare applicazioni OAuth2 personalizzate {#delete-custom-oauth2-applications}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Clic **  **.
1. Passa il puntatore sull’applicazione e fai clic su **[!UICONTROL Elimina]** ![](assets/delete.png) quando appare all&#39;estrema destra.

## Gestire i segreti client nelle applicazioni OAuth2

* [Visualizza dettagli segreto client](#view-client-secret-details)
* [Aggiungi o modifica note per Segreto client](#add-or-edit-notes-for-client-secret)
* [Eliminare il segreto client](#delete-client-secret)

### Visualizza dettagli segreto client {#view-client-secret-details}

>[!IMPORTANT]
>
>Non è possibile visualizzare il segreto client stesso. Se hai perso il segreto client, devi eliminarlo e crearne uno nuovo.
>
>* Per eliminare un segreto client, vedi [Elimina segreto client](#delete-client-secret) in questo articolo.
>* Per creare un nuovo segreto client, vedi [Creare un’applicazione OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. Fai clic sul pulsante *[!UICONTROL *Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Passa il puntatore sull’applicazione e fai clic sul pulsante **[!UICONTROL Modifica]** quando appare all&#39;estrema destra.
1. Visualizza i dettagli nell&#39;area Segreto client:

   * Data creazione
   * Data ultimo utilizzo
   * Note

      Per aggiungere note a un segreto client, consulta [Aggiungi o modifica note per Segreto client](#add-or-edit-notes-for-client-secret).

### Aggiungi o modifica note per Segreto client {#add-or-edit-notes-for-client-secret}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Passa il puntatore sull’applicazione e fai clic sul pulsante **[!UICONTROL Modifica]** quando appare all&#39;estrema destra.
1. Individua il segreto client di cui desideri aggiungere o modificare una nota.
1. Fare clic sulla casella contenente i dettagli del segreto client.

   È ora possibile aggiungere testo della nota o modificare il testo della nota esistente.

   >[!NOTE]
   >
   >Il testo della nota può contenere un massimo di 64 caratteri.

1. Fare clic fuori dalla casella o premere **[!UICONTROL Invio]** per salvare il testo della nota.

### Eliminare il segreto client {#delete-client-secret}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Passa il puntatore sull’applicazione e fai clic sul pulsante **[!UICONTROL Modifica]** quando appare all&#39;estrema destra.
1. Individua il segreto client da eliminare.
1. Fai clic sul pulsante **[!UICONTROL Elimina]** icona ![](assets/delete.png) accanto al segreto client.
