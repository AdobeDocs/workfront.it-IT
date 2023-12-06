---
title: Configurare [!DNL SharePoint] integrazione
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: È possibile integrare [!DNL Workfront] con [!DNL SharePoint] Online, per consentire agli utenti di navigare, collegarsi e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altri [!DNL Workfront] integrazioni di documenti.
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 3cc1745b33d645d37248185b4163a39c1bead60e
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%

---

# Configurare [!DNL SharePoint] integrazione

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Il nuovo [!DNL SharePoint] L’integrazione è stata rilasciata in produzione con la versione 22.3 (luglio 2022). Anche se gli utenti possono ancora accedere ai documenti collegati tramite il [!DNL SharePoint] , devono utilizzare il nuovo [!DNL SharePoint] per collegare documenti da SharePoint.
>
>* La nuova integrazione di SharePoint non richiede la configurazione da parte di un amministratore e può essere impostata da singoli utenti. Tuttavia, per garantire una transizione senza problemi alla nuova integrazione di SharePoint, un amministratore Workfront deve apportare alcune piccole modifiche alle impostazioni nell’area di configurazione di Workfront.
>
>    Per informazioni e istruzioni, consulta [Configurare l’integrazione legacy di SharePoint per l’accesso continuo ai documenti](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in questo articolo.
>    
>* È consigliabile che gli utenti colleghino i documenti attualmente collegati tramite il [!DNL SharePoint] tramite la nuova integrazione.
>    
>    Per istruzioni sul collegamento di documenti, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

È possibile integrare [!DNL Workfront] con [!DNL SharePoint Online], che consente agli utenti di navigare su, collegare e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altri [!DNL Workfront] integrazioni, come [!DNL Google Drive], [!DNL Box], e [!DNL Dropbox].

Questa integrazione è compatibile solo con [!DNL SharePoint Online]. Istanze locali di [!DNL SharePoint] non sono supportati.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

Devi disporre degli accessi o delle autorizzazioni necessari in [!DNL SharePoint] per modificare o configurare [!DNL SharePoint] integrazione.

## Collegare i documenti tramite la nuova integrazione SharePoint

I singoli utenti possono collegare i documenti tramite il nuovo [!DNL SharePoint] integrazione. L’integrazione non richiede la configurazione dell’amministratore. L’utente accede al proprio [!DNL Microsoft] quando si collega un documento, che consente all’integrazione di accedere ai documenti disponibili nel [!DNL SharePoint].

La prima volta che un utente connette [!DNL Workfront] [!DNL SharePoint] integrazione con il loro [!DNL SharePoint] , visualizzeranno e accetteranno tutte le autorizzazioni che [!DNL Workfront] utilizza quando si interagisce con i [!UICONTROL SharePoint] account. Autorizzazioni di lettura consentite [!DNL Workfront] per visualizzare e accedere ai file su [!DNL SharePoint], e le autorizzazioni di scrittura consentono all&#39;utente di caricare file in [!DNL SharePoint].

![Autorizzazioni di SharePoint](assets/sharepoint-permissions.png)

Per istruzioni su come collegare i documenti tramite il nuovo [!DNL SharePoint] integrazione, vedi [Collega un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] l’integrazione può connettersi a un singolo [!DNL SharePoint] dell&#39;istanza. Pertanto, un utente può impostare un’integrazione per uno [!DNL SharePoint], ma non può impostare un’integrazione per un secondo [!DNL SharePoint], anche se dispongono di autorizzazioni per e documenti sul secondo [!DNL SharePoint].
>
>* Un utente ha accesso agli stessi siti, raccolte, cartelle, sottocartelle e file tramite [!DNL Workfront] [!DNL SharePoint] l&#39;integrazione che hanno nel loro [!DNL SharePoint] account.

### Collega documenti da SharePoint

Per istruzioni sul collegamento di documenti da SharePoint tramite il nuovo [!DNL SharePoint] integrazione, vedi [Collega un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Inviare documenti a SharePoint

Per inviare un documento a SharePoint:

1. Fai clic su **Invia a** icona ![Invia a](assets/send-to-icon.png) e seleziona SharePoint (Graph API).
1. (Facoltativo) Cercare nella barra di ricerca il sito o la cartella in cui si desidera inviare il documento.
1. Selezionare il sito o la cartella dall&#39;elenco.

   * I siti sono contrassegnati con ![Icona del sito](assets/site-icon.png).

   * Le cartelle sono contrassegnate con ![Icona cartella](assets/folder-icon.png).

   * I file non sono contrassegnati da un&#39;icona.

1. Fai clic su **Salva**.


## Informazioni su sicurezza, accesso e autorizzazione per [!DNL SharePoint] integrazione

### Autenticazione e autorizzazione

[!DNL Workfront] utilizza OAuth2 per recuperare un token di accesso e un token di aggiornamento. Questo token di accesso viene utilizzato per l’autorizzazione con tutti [!DNL SharePoint] aree.

### Accesso e autorizzazioni

La prima volta che un utente aggiunge un documento a [!DNL Workfront] da [!DNL SharePoint], vengono indirizzati a una schermata che richiede le seguenti autorizzazioni:

| Accesso | Motivo |
|---|---|
| Accesso completo ai file | Consente [!DNL Workfront] per accedere ai file di un utente e collegare le risorse. Quando i documenti vengono inviati da [!DNL Workfront] a [!DNL SharePoint], [!DNL Workfront] richiede l’accesso per creare la risorsa. |
| Leggi elementi in tutte le raccolte siti | Consente [!DNL Workfront] leggere le risorse per abilitare la navigazione degli utenti. |
| Modifica o elimina elementi in tutte le raccolte siti | Consente [!DNL Workfront] per creare risorse in sites e raccolte siti. L’eliminazione viene utilizzata solo per la pulizia dopo tentativi di collegamento non riusciti. |
| Gestisci l&#39;accesso ai dati a cui hai dato accesso | Consente [!DNL Workfront] per generare un token di aggiornamento. |
| Accedi e leggi il profilo utente | Consente [!DNL Workfront] per utilizzare il token di accesso per agire per conto dell’utente, tramite il flusso di accesso OAuth2. |

* Questo accesso viene concesso dall’utente la prima volta che utilizza l’integrazione e può essere revocato in qualsiasi momento.
* Le autorizzazioni richieste per questa integrazione sono **delegato** autorizzazioni.
* [!DNL Workfront] richiede l’accesso minimo necessario per eseguire operazioni nell’integrazione.
* Accesso per visualizzare, modificare o eliminare un [!DNL Adobe Workfront] documento collegato a [!DNL SharePoint] si basa sull’accesso dell’utente in [!DNL Workfront]. Tuttavia, la navigazione, il download o la modifica di un [!DNL SharePoint] file o cartella richiede l&#39;accesso a [!DNL SharePoint]e l&#39;accesso a queste azioni è controllato da [!DNL SharePoint].
* Gli utenti possono visualizzare miniature e immagini in anteprima da cui provengono [!DNL SharePoint]e possono visualizzare i nomi di file e cartelle in [!DNL SharePoint], senza accedere a [!DNL SharePoint].
* Il token di accesso di un utente viene utilizzato solo quando l’utente è offline e un altro utente visualizza il contenuto di una cartella collegata a [!DNL Workfront]. Il token di accesso viene utilizzato per verificare se eventuali documenti nella cartella sono stati aggiunti, rimossi o modificati.

### Sicurezza

Tutte le comunicazioni tra [!DNL Workfront] e [!DNL SharePoint] viene eseguito tramite HTTPS, che crittografa le informazioni.

[!DNL Workfront] non memorizza, copia o duplica dati da [!DNL SharePoint]. L&#39;unica eccezione è che [!DNL Workfront] memorizza le miniature da [!DNL SharePoint] da visualizzare nella vista a elenco e in Anteprima.

Se una risorsa è stata caricata per la prima volta in [!DNL Workfront], e quindi inviato a [!DNL SharePoint], [!DNL Workfront] conserva i dati per il primo file perché gli utenti possono scaricare una versione precedente di un file [!DNL Workfront] documento. Se un documento è stato creato in [!DNL SharePoint], [!DNL Workfront] non memorizza i dati del file.

## Configurare la versione precedente di [!DNL SharePoint] integrazione per un accesso continuo ai documenti

Per garantire agli utenti un accesso continuo ai documenti collegati a Workfront tramite [!DNL SharePoint] dell&#39;integrazione, è necessario riconfigurare l&#39;accesso alla [!DNL SharePoint] e mantenere aggiornato il segreto client di SharePoint.

* [Riconfigurare l’accesso alla versione precedente di [!DNL SharePoint] integrazione](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Configura il segreto client per l’accesso continuo ai [!DNL SharePoint] integrazione](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Riconfigurare l’accesso alla versione precedente di [!DNL SharePoint] integrazione

Riconfigurazione della versione precedente [!DNL SharePoint] consente agli utenti di accedere ai documenti collegati tramite il [!DNL SharePoint] garantendo al tempo stesso che gli utenti non possano collegare nuovi documenti tramite tale integrazione.

>[!NOTE]
>
> * La versione precedente [!DNL SharePoint] l’integrazione è etichettata &quot;[!DNL SharePoint].&quot;
> * Il nuovo [!DNL SharePoint] l’integrazione è etichettata &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona quindi **[!UICONTROL Provider cloud]**.
1. Assicurati che il **[!DNL SharePoint]** opzione e **[!UICONTROL [!DNL SharePoint](Graph API)]** sono entrambe abilitate.
1. Fai clic su **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona quindi **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Seleziona il segno di spunta a sinistra dell’elenco per tutte le integrazioni esistenti, quindi seleziona **[!UICONTROL Disattiva]**.
   ![](assets/disable-old-sharepoint.png)


### Configura il segreto client per l’accesso continuo ai [!DNL SharePoint] integrazione

Il tuo [!DNL SharePoint] Il segreto client scade una volta all’anno. Per garantire un accesso continuo ai documenti [!DNL SharePoint] integrazione, è necessario mantenere i [!DNL SharePoint] Segreto client aggiornato.

>[!IMPORTANT]
>
> Perché [!DNL SharePoint] I segreti client sono gestiti da [!DNL Microsoft], le funzioni e le procedure del segreto client possono cambiare in base agli aggiornamenti apportati a [!DNL SharePoint] creato da [!DNL Microsoft]. Controlla sempre [!DNL Microsoft] per informazioni aggiornate sulle procedure e le funzioni di [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genera un nuovo segreto client come descritto in [Sostituire un segreto client in scadenza in un [!DNL SharePoint] Componente aggiuntivo](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Copia il segreto client in un percorso sicuro.
1. Accedi a [!DNL Workfront] come amministratore.
1. In Workfront, fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Configurazione]** ![Icona Configurazione](/help/_includes/assets/gear-icon-setup.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Fai clic sul pulsante [!DNL SharePoint] dell’integrazione da aggiornare, quindi fai clic su **[!UICONTROL Modifica]**.
1. Individua il **Informazioni di connessione** nella finestra di modifica, quindi inserisci il nuovo Segreto client nel **[!UICONTROL Segreto client SharePoint]** campo.
1. Fai clic su **[!UICONTROL Salva]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Risoluzione dei problemi

* [Problema: si verificano errori basati sull’autenticazione quando si utilizza [!DNL SharePoint] integrazione.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: quando si tenta di esplorare [!DNL SharePoint] file in [!DNL Workfront], non viene visualizzata alcuna raccolta siti o tutte le raccolte siti.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: impossibile accedere a cartelle e documenti collegati in precedenza in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: si verificano errori basati sull’autenticazione quando si utilizza [!DNL SharePoint] integrazione. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluzioni:

Gli utenti devono disporre delle autorizzazioni appropriate per [!DNL SharePoint] sito.

Utenti con [!UICONTROL Controllo completo] dispongono di tutte le autorizzazioni necessarie per [!DNL SharePoint] integrazione. Se non si desidera concedere l&#39;accesso Controllo completo agli utenti, è necessario concedere le seguenti autorizzazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Può visualizzare, aggiungere, aggiornare, eliminare, approvare e personalizzare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modifica]</p> </td> 
   <td> <p>Può aggiungere, modificare ed eliminare elenchi; può visualizzare, aggiungere, aggiornare ed eliminare voci e documenti di elenco</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Visualizzazione, aggiunta, aggiornamento ed eliminazione di voci di elenco e documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Solo visualizzazione]</p> </td> 
   <td> <p>Può visualizzare pagine, voci di elenco e documenti (i tipi di documenti con gestori di file lato server possono essere visualizzati nel browser ma non scaricati)</p> </td> 
  </tr> 
 </tbody> 
</table>

Per istruzioni sulla creazione e la modifica dei livelli di autorizzazione, vedere [Come creare e modificare i livelli di autorizzazione](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) nella documentazione di Microsoft.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problema: quando si tenta di esplorare [!DNL SharePoint] file in [!DNL Workfront], non viene visualizzata alcuna raccolta siti o tutte le raccolte siti. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluzioni:

Per visualizzare una raccolta siti in [!DNL Workfront], devono essere soddisfatte le seguenti condizioni:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* L&#39;utente deve disporre dell&#39;accesso in visualizzazione alla raccolta siti in [!DNL SharePoint].

  Per verificarlo in [!DNL SharePoint], controllare le autorizzazioni della raccolta siti in SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problema: impossibile accedere a cartelle e documenti collegati in precedenza in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Soluzione:

Se l’utente che ha collegato [!DNL SharePoint] la cartella non può più eseguire l&#39;autenticazione, [!DNL Workfront] non può più accedere al contenuto della cartella. Ciò può verificarsi, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda.

Per garantire l’accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

Per informazioni sul collegamento di cartelle da provider esterni, consulta [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->