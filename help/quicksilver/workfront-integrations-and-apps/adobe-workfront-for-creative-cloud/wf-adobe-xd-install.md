---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installare e aprire Adobe Workfront for XD
description: Puoi installare il plug-in Adobe Workfront for XD da Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: c21e1c1d8e45b7c6407e8741b31055bfed9f4717
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 2%

---

# Installa e apri [!DNL Adobe Workfront for XD]

È possibile installare il plug-in [!DNL Adobe Workfront for XD] da Adobe Marketplace. Il plug-in supporta le seguenti lingue:

* Inglese
* Francese
* Tedesco
* Italiano
* Spagnolo
* Portoghese
* Giapponese
* Cinese semplificato
* Cinese tradizionale
* Coreano

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package/td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Standard</p>
    <p>Work or higher</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td><p>È necessario disporre di una licenza [!DNL Adobe Creative Cloud] oltre a una licenza [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* È necessario installare l&#39;app [!DNL Adobe XD] prima di installare il plug-in Workfront.

## Installa il plug-in [!DNL Adobe Workfront for XD] per la tua organizzazione

Se sei un amministratore di [!DNL Adobe Admin Console], puoi includere il plug-in nei pacchetti di distribuzione di [!DNL Creative Cloud]. Per ulteriori informazioni, vedere [Inclusione di plug-in nel pacchetto](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Visualizza un&#39;esercitazione video qui](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Gli amministratori di [!DNL Adobe Admin Console] possono anche creare pacchetti di solo plug-in da distribuire agli utenti. Per ulteriori informazioni, consulta [Creare [!UICONTROL [!DNL Adobe Workfront] per [!DNL Creative Cloud]] pacchetti per i tuoi utenti in [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Installa il plug-in [!DNL Adobe Workfront for XD] singolarmente

È possibile installare il plug-in [!DNL Adobe Workfront for XD] da [!DNL Adobe Exchange].

1. Vai alla [pagina di installazione di Adobe Workfront for XD](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&workflow=share) in Adobe Exchange.
1. Nella finestra di dialogo visualizzata, fai clic su **Apri [!DNL Adobe Creative Cloud] app desktop**.
1. Una volta aperto Gestione plug-in [!DNL Adobe XD], fare clic su **[!UICONTROL Installa]**.
1. Leggere le informazioni nella finestra di dialogo, quindi fare clic su **[!UICONTROL OK]**.
1. Per informazioni su come aprire il plug-in, consulta la sezione seguente.

## Apri il plug-in [!DNL Adobe Workfront for XD]

1. Apri [!DNL Adobe XD].

1. Creare un nuovo file o aprirne uno esistente.

1. Nell&#39;angolo in basso a sinistra, fai clic sull&#39;icona **Plugin**.

![Finestra del plug-in di XD](assets/xd-plugin-window-350x620.png)

1. Nel **[!UICONTROL pannello Plugin]**, trovare **[!UICONTROL Adobe Workfront per XD]**.

1. Per informazioni su come accedere al plug-in, consulta la sezione seguente.

## Accedi a [!DNL Adobe Workfront for XD]

1. Verificare che il pannello del plug-in sia aperto, quindi fare clic su **[!DNL Adobe Workfront for XD]**.
1. Immetti il dominio, quindi fai clic su **[!UICONTROL Accedi]**. Viene visualizzata una pagina del browser.

   >[!TIP]
   >
   >* Per trovare il dominio, aprire un browser, accedere all&#39;istanza [!DNL Workfront] e copiare la prima parte dell&#39;URL:\
   >![Individua dominio](assets/domain-350x50.png)
   >
   >* Se l&#39;istanza di Workfront è integrata con Experience Cloud e il dominio inizia con `experience.adobe.com`, chiedi all&#39;amministratore di fornirti il dominio di Workfront che si trova in Prodotto > Workfront in Admin Console.

1. Nel browser, immetti le tue credenziali di [!DNL Adobe], quindi fai clic su **[!DNL Log in]**. Se l&#39;azienda utilizza un Single Sign-On (SSO), verrà visualizzata la pagina del provider SSO per l&#39;accesso.

   >[!NOTE]
   >
   >Non ti verrà richiesto di immettere le credenziali di [!DNL Workfront] se hai effettuato l&#39;accesso di recente.

1. Seguire le istruzioni per accedere a [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] si connette a [!DNL Adobe Creative Cloud] utilizzando OAuth 2.0, uno standard sicuro utilizzato dalla maggior parte delle integrazioni basate sul Web per l&#39;autenticazione e l&#39;autorizzazione degli utenti.

1. Fai clic su **[!UICONTROL Consenti ad Access]** di completare l&#39;accesso e torna a [!DNL Adobe XD] per visualizzare il tuo lavoro.

### Risoluzione dei problemi di accesso

**Errore &quot;Si è verificato un errore&quot; durante il tentativo di accesso**


Non puoi usare un URL che inizia con `experience.adobe.com` per accedere al plug-in.

![log in error](assets/plugin-log-in-error.png) ![dominio](assets/incorrect-domain.png)


Per risolvere il problema:

1. Disinstalla e reinstalla il plug-in Adobe Workfront for XD per cancellare il dominio e l’errore.

1. Immetti il dominio Workfront. Il dominio deve essere `company-name.my.workfront.com` e non `experience.adobe.com`.

Per trovare il tuo dominio Workfront se usi Adobe Unified Experience, vai a
