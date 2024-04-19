---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Visualizzazione e gestione di applicazioni OAuth2 personalizzate
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di Workfront, che consentono ad altre applicazioni di accedere a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Visualizzazione e gestione di applicazioni OAuth2 personalizzate

Come un [!DNL Adobe Workfront] amministratore, puoi visualizzare e gestire le applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono l&#39;accesso ad altre applicazioni [!UICONTROL Workfront].

>[!NOTE]
>
>* Nel contesto di OAuth2, &quot;applicazione OAuth2&quot; si riferisce a questo tipo di collegamento di accesso tra un&#39;app e un server come [!DNL Workfront]. Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Puoi avere fino a un totale di dieci applicazioni OAuth2 alla volta.

* Per informazioni sulla creazione di applicazioni OAuth2 personalizzate, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite l’autenticazione del server (flusso JWT), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite PKCE, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> Devi essere un [!DNL Workfront] amministratore. </p>
    <p>Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

È necessario creare [!UICONTROL OAuth2] per la tua organizzazione prima di visualizzarle o gestirle.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gestione di applicazioni OAuth2 personalizzate

* [Visualizzare e modificare applicazioni OAuth2 personalizzate](#view-and-edit-custom-oauth2-applications)
* [Elimina applicazioni OAuth2 personalizzate](#delete-custom-oauth2-applications)

### Visualizzare e modificare applicazioni OAuth2 personalizzate {#view-and-edit-custom-oauth2-applications}

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.
1. Passa il puntatore sull’applicazione e fai clic su **[!UICONTROL Modifica]** ![](assets/edit-icon.png) quando appare all&#39;estrema destra.
1. (Facoltativo) Modificare i dettagli dell&#39;applicazione.

   Per i campi relativi alle app OAuth2 e JWT, consulta [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Elimina applicazioni OAuth2 personalizzate {#delete-custom-oauth2-applications}

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su ** **.
1. Passa il puntatore sull’applicazione e fai clic su **[!UICONTROL Elimina]** ![](assets/delete.png) quando appare all&#39;estrema destra.

## Gestire i segreti client nelle applicazioni OAuth2

* [Visualizza dettagli segreto client](#view-client-secret-details)
* [Aggiungi o modifica note per Segreto client](#add-or-edit-notes-for-client-secret)
* [Elimina segreto client](#delete-client-secret)

### Visualizza dettagli segreto client {#view-client-secret-details}

>[!IMPORTANT]
>
>Non è possibile visualizzare il segreto client stesso. Se hai perso il segreto client, devi eliminarlo e crearne uno nuovo.
>
>* Per eliminare un segreto client, vedi [Elimina segreto client](#delete-client-secret) in questo articolo.
>* Per creare un nuovo segreto client, consulta [Creare un’applicazione OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. Fai clic su *[!UICONTROL *Menu principale]* Icona * ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Passa il puntatore del mouse sull’applicazione e fai clic su **[!UICONTROL Modifica]** quando viene visualizzata all’estrema destra.
1. Visualizza dettagli nell&#39;area Segreto client:

   * Data di creazione
   * Data ultimo utilizzo
   * Note

     Per aggiungere note a un segreto client, vedi [Aggiungi o modifica note per Segreto client](#add-or-edit-notes-for-client-secret).

### Aggiungi o modifica note per Segreto client {#add-or-edit-notes-for-client-secret}

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.
1. Passa il puntatore del mouse sull’applicazione e fai clic su **[!UICONTROL Modifica]** quando viene visualizzata all’estrema destra.
1. Individua il segreto client per il quale desideri aggiungere o modificare una nota.
1. Fai clic sulla casella contenente i dettagli del segreto client.

   È ora possibile aggiungere testo di nota o modificare il testo di nota esistente.

   >[!NOTE]
   >
   >Il testo della nota può contenere un massimo di 64 caratteri.

1. Fare clic all&#39;esterno dell&#39;apparecchio o premere **[!UICONTROL Invio]** per salvare il testo della nota.

### Elimina segreto client {#delete-client-secret}

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.
1. Passa il puntatore del mouse sull’applicazione e fai clic su **[!UICONTROL Modifica]** quando viene visualizzata all’estrema destra.
1. Individua il segreto client da eliminare.
1. Fai clic su **[!UICONTROL Elimina]** icona ![](assets/delete.png) accanto a Segreto client.
