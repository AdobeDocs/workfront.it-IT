---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Visualizzazione e gestione di applicazioni OAuth2 personalizzate
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di Workfront, che consentono ad altre applicazioni di accedere a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Visualizzazione e gestione di applicazioni OAuth2 personalizzate

In qualità di amministratore di [!DNL Adobe Workfront], puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono ad altre applicazioni di accedere a [!UICONTROL Workfront].

>[!NOTE]
>
>* Nel contesto di OAuth2, &quot;applicazione OAuth2&quot; fa riferimento a questo tipo di collegamento di accesso tra un&#39;app e un server come [!DNL Workfront]. Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Puoi avere fino a un totale di dieci applicazioni OAuth2 alla volta.

* Per informazioni sulla creazione di applicazioni OAuth2 personalizzate, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Per istruzioni sulla configurazione e l&#39;utilizzo dell&#39;applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), vedere [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della propria organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni sulla configurazione e l&#39;utilizzo dell&#39;applicazione OAuth2 tramite l&#39;autenticazione del server (flusso JWT), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione tramite il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni sulla configurazione e l&#39;utilizzo dell&#39;applicazione OAuth2 tramite PKCE, vedere [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della propria organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> Devi essere un amministratore [!DNL Workfront]. </p>
    <p>Per informazioni sugli amministratori di [!DNL Workfront], vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

+++

## Prerequisiti

È necessario creare [!UICONTROL applicazioni OAuth2] per l&#39;organizzazione prima di visualizzarle o gestirle.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gestione di applicazioni OAuth2 personalizzate

* [Visualizzare e modificare applicazioni OAuth2 personalizzate](#view-and-edit-custom-oauth2-applications)
* [Elimina applicazioni OAuth2 personalizzate](#delete-custom-oauth2-applications)

### Visualizzare e modificare applicazioni OAuth2 personalizzate {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Crea integrazione app]**.
1. Passa il puntatore del mouse sull&#39;applicazione e fai clic sull&#39;icona **[!UICONTROL Modifica]** ![Modifica](assets/edit-icon.png) quando viene visualizzata all&#39;estrema destra.
1. (Facoltativo) Modificare i dettagli dell&#39;applicazione.

   Per i campi relativi alle app OAuth2 e JWT, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Elimina applicazioni OAuth2 personalizzate {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Passa il puntatore del mouse sull&#39;applicazione e fai clic su **[!UICONTROL Elimina]** ![Elimina](assets/delete.png) quando viene visualizzato all&#39;estrema destra.

## Gestire i segreti client nelle applicazioni OAuth2

* [Visualizza dettagli segreto client](#view-client-secret-details)
* [Aggiungi o modifica note per Segreto client](#add-or-edit-notes-for-client-secret)
* [Elimina segreto client](#delete-client-secret)

### Visualizza dettagli segreto client {#view-client-secret-details}

>[!IMPORTANT]
>
>Non è possibile visualizzare il segreto client stesso. Se hai perso il segreto client, devi eliminarlo e crearne uno nuovo.
>
>* Per eliminare un segreto client, vedere [Elimina segreto client](#delete-client-secret) in questo articolo.
>* Per creare un nuovo segreto client, vedi [Creare un&#39;applicazione OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Passa il puntatore del mouse sull&#39;applicazione e fai clic sull&#39;icona **[!UICONTROL Modifica]** quando viene visualizzata all&#39;estrema destra.
1. Visualizza dettagli nell&#39;area Segreto client:

   * Data di creazione
   * Data ultimo utilizzo
   * Note

     Per aggiungere note a un segreto client, vedere [Aggiungere o modificare le note per il segreto client](#add-or-edit-notes-for-client-secret).

### Aggiungi o modifica note per Segreto client {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Crea integrazione app]**.
1. Passa il puntatore del mouse sull&#39;applicazione e fai clic sull&#39;icona **[!UICONTROL Modifica]** quando viene visualizzata all&#39;estrema destra.
1. Individua il segreto client per il quale desideri aggiungere o modificare una nota.
1. Fai clic sulla casella contenente i dettagli del segreto client.

   È ora possibile aggiungere testo di nota o modificare il testo di nota esistente.

   >[!NOTE]
   >
   >Il testo della nota può contenere un massimo di 64 caratteri.

1. Fare clic all&#39;esterno della casella o premere **[!UICONTROL Invio]** per salvare il testo della nota.

### Elimina segreto client {#delete-client-secret}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Crea integrazione app]**.
1. Passa il puntatore del mouse sull&#39;applicazione e fai clic sull&#39;icona **[!UICONTROL Modifica]** quando viene visualizzata all&#39;estrema destra.
1. Individua il segreto client da eliminare.
1. Fai clic sull&#39;icona **[!UICONTROL Elimina]** ![Elimina](assets/delete.png) accanto al segreto client.
