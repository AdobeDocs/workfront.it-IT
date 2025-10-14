---
title: 'Configura l''integrazione  [!DNL SharePoint] '
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Puoi integrare [!DNL Workfront] con [!DNL SharePoint] Online, consentendo agli utenti di accedere ai documenti di Workfront, collegarli e aggiungerli.  [!DNL SharePoint]  La funzionalità fornita è simile a quella di altre [!DNL Workfront] integrazioni di documenti.
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# Configurare l&#39;integrazione di [!DNL SharePoint]

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La nuova integrazione di [!DNL SharePoint] è stata rilasciata in produzione con la versione 22.3 (luglio 2022).
>
>* Anche se gli utenti possono ancora accedere ai documenti collegati tramite l&#39;integrazione legacy di [!DNL SharePoint], non possono collegare i documenti attraverso di essa. devono utilizzare la nuova integrazione [!DNL SharePoint] per collegare documenti da SharePoint.
>
>* Se non hai configurato un’integrazione legacy di SharePoint, non puoi aggiungerla. Per collegare i documenti a SharePoint è necessario utilizzare la nuova integrazione SharePoint.
>
>* La nuova integrazione di SharePoint potrebbe non richiedere la configurazione da parte di un amministratore e potrebbe essere impostata da singoli utenti. Tuttavia, per garantire una transizione senza problemi alla nuova integrazione di SharePoint, un amministratore Workfront deve apportare alcune piccole modifiche alle impostazioni nell’area di configurazione di Workfront.
>
>    Per informazioni e istruzioni, vedere [Configurare l&#39;integrazione legacy di SharePoint per l&#39;accesso continuo ai documenti](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in questo articolo.
>    
>* È consigliabile che gli utenti colleghino i documenti attualmente collegati tramite l&#39;integrazione legacy di [!DNL SharePoint] tramite la nuova integrazione.
>    
>    Per istruzioni sul collegamento di documenti, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

È possibile integrare [!DNL Workfront] con [!DNL SharePoint Online], consentendo agli utenti di navigare, collegare e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altre integrazioni [!DNL Workfront], ad esempio [!DNL Google Drive], [!DNL Box] e [!DNL Dropbox].

Questa integrazione è compatibile solo con [!DNL SharePoint Online]. Le istanze locali di [!DNL SharePoint] non sono supportate.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td>Nuovo: Standard <p>Oppure</p><p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td>Devi essere un amministratore [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per modificare o configurare l&#39;integrazione di [!DNL SharePoint], è necessario disporre dell&#39;accesso o delle autorizzazioni necessarie in [!DNL SharePoint].

## Collegare i documenti tramite la nuova integrazione SharePoint

I singoli utenti possono collegare i documenti tramite la nuova integrazione [!DNL SharePoint]. L’integrazione non richiede la configurazione dell’amministratore. Al contrario, l&#39;utente accede al proprio account [!DNL Microsoft] quando collega un documento, il che consente all&#39;integrazione di accedere ai documenti disponibili in [!DNL SharePoint] dell&#39;utente.

La prima volta che un utente connette l&#39;integrazione [!DNL Workfront] [!DNL SharePoint] al proprio account [!DNL SharePoint], vedrà e accetterà tutte le autorizzazioni utilizzate da [!DNL Workfront] durante l&#39;interazione con il proprio account [!UICONTROL SharePoint] oppure potrà richiedere le autorizzazioni all&#39;amministratore di Microsoft. Le autorizzazioni di lettura consentono a [!DNL Workfront] di visualizzare e accedere ai file in [!DNL SharePoint] e le autorizzazioni di scrittura consentono all&#39;utente di caricare i file in [!DNL SharePoint].

![Autorizzazioni di Sharepoint](assets/sharepoint-permissions.png)

Per istruzioni sul collegamento di documenti tramite la nuova integrazione [!DNL SharePoint], vedere [Collegare un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A seconda della configurazione Microsoft dell’organizzazione, gli utenti possono visualizzare una pagina &quot;Approvazione richiesta&quot; invece di una pagina &quot;Autorizzazioni richieste&quot;. In questo caso, gli utenti possono utilizzare questa pagina per richiedere che l’amministratore Microsoft dell’organizzazione conceda le autorizzazioni per l’integrazione di Sharepoint.
>
>* Un&#39;integrazione [!DNL SharePoint] può connettersi a una singola istanza [!DNL SharePoint]. Pertanto, un utente può impostare un&#39;integrazione per un [!DNL SharePoint], ma non può impostare un&#39;integrazione per un secondo [!DNL SharePoint], anche se dispone delle autorizzazioni per e documenti sul secondo [!DNL SharePoint].
>
>* Un utente ha accesso agli stessi siti, raccolte, cartelle, sottocartelle e file tramite l&#39;integrazione [!DNL Workfront] [!DNL SharePoint] come nel proprio account [!DNL SharePoint].

### Collega documenti da SharePoint

Per istruzioni sul collegamento di documenti da SharePoint tramite la nuova integrazione [!DNL SharePoint], vedere [Collegare un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Inviare documenti a SharePoint

Per inviare un documento a SharePoint:

1. Fai clic sull&#39;icona **Invia a** ![Invia a](assets/send-to-icon.png) e seleziona SharePoint (Graph API).
1. (Facoltativo) Cercare nella barra di ricerca il sito o la cartella in cui si desidera inviare il documento.
1. Selezionare il sito o la cartella dall&#39;elenco.

   * I siti sono contrassegnati con ![icona sito](assets/site-icon.png).

   * Le cartelle sono contrassegnate con ![Icona cartella](assets/folder-icon.png).

   * I file non sono contrassegnati da un&#39;icona.

1. Fai clic su **Salva**.


## Informazioni su sicurezza, accesso e autorizzazione per l&#39;integrazione di [!DNL SharePoint]

### Autenticazione e autorizzazione

[!DNL Workfront] utilizza OAuth2 per recuperare un token di accesso e un token di aggiornamento. Questo token di accesso viene utilizzato per l&#39;autorizzazione con tutte le [!DNL SharePoint] aree.

### Accesso e autorizzazioni

La prima volta che un utente aggiunge un documento a [!DNL Workfront] da [!DNL SharePoint], viene indirizzato alla pagina Autorizzazioni richieste, in cui può concedere le autorizzazioni per l&#39;integrazione con SharePoint.

>[!NOTE]
>
>A seconda della configurazione Microsoft dell’organizzazione, gli utenti possono visualizzare una pagina &quot;Approvazione richiesta&quot; invece di una pagina &quot;Autorizzazioni richieste&quot;. In questo caso, gli utenti possono utilizzare questa pagina per richiedere che l’amministratore Microsoft dell’organizzazione conceda le autorizzazioni per l’integrazione di Sharepoint.

Sono richieste le seguenti autorizzazioni:

| Accesso | Motivo |
|---|---|
| Accesso completo ai file | Consente a [!DNL Workfront] di accedere ai file di un utente per collegare le risorse. Quando i documenti vengono inviati da [!DNL Workfront] a [!DNL SharePoint], [!DNL Workfront] richiede l&#39;accesso per creare la risorsa. |
| Leggi elementi in tutte le raccolte siti | Consente a [!DNL Workfront] di leggere le risorse per abilitare la navigazione degli utenti. |
| Modifica o elimina elementi in tutte le raccolte siti | Consente a [!DNL Workfront] di creare risorse nei siti e nelle raccolte siti. L’eliminazione viene utilizzata solo per la pulizia dopo tentativi di collegamento non riusciti. |
| Gestisci l&#39;accesso ai dati a cui hai dato accesso | Consente a [!DNL Workfront] di generare un token di aggiornamento. |
| Accedi e leggi il profilo utente | Consente a [!DNL Workfront] di utilizzare il token di accesso per agire per conto dell&#39;utente tramite il flusso di accesso OAuth2. |

* Questo accesso viene concesso dall’utente la prima volta che utilizza l’integrazione e può essere revocato in qualsiasi momento.
* Le autorizzazioni richieste per questa integrazione sono **autorizzazioni delegate**.
* [!DNL Workfront] richiede l&#39;accesso minimo necessario per eseguire operazioni nell&#39;integrazione.
* L&#39;accesso per visualizzare, modificare o eliminare un documento [!DNL Adobe Workfront] collegato a [!DNL SharePoint] si basa sull&#39;accesso dell&#39;utente in [!DNL Workfront]. Tuttavia, qualsiasi spostamento, download o modifica di un file o di una cartella [!DNL SharePoint] richiede l&#39;accesso a [!DNL SharePoint] e l&#39;accesso a queste azioni è controllato da [!DNL SharePoint].
* Gli utenti possono visualizzare miniature e immagini di anteprima provenienti da [!DNL SharePoint] e visualizzare i nomi di file e cartelle in [!DNL SharePoint], senza effettuare l&#39;accesso a [!DNL SharePoint].
* Il token di accesso di un utente viene utilizzato solo quando l&#39;utente è offline e un altro utente visualizza il contenuto di una cartella collegata a [!DNL Workfront]. Il token di accesso viene utilizzato per verificare se eventuali documenti nella cartella sono stati aggiunti, rimossi o modificati.

### Sicurezza

Tutte le comunicazioni tra [!DNL Workfront] e [!DNL SharePoint] vengono eseguite tramite HTTPS, che crittografa le informazioni.

[!DNL Workfront] non archivia, copia o duplica dati da [!DNL SharePoint]. L&#39;unica eccezione è che [!DNL Workfront] memorizza le miniature di [!DNL SharePoint] da visualizzare nella vista a elenco e in Anteprima.

Se una risorsa è stata caricata per la prima volta in [!DNL Workfront] e quindi inviata a [!DNL SharePoint], [!DNL Workfront] mantiene i dati per il primo file perché gli utenti possono scaricare una versione precedente di un documento [!DNL Workfront]. Se un documento è stato creato in [!DNL SharePoint], [!DNL Workfront] non memorizza i dati del file.

## Configura l&#39;integrazione legacy di [!DNL SharePoint] per l&#39;accesso continuo ai documenti

Per garantire agli utenti un accesso continuo ai documenti collegati a Workfront tramite l&#39;integrazione legacy di [!DNL SharePoint], è necessario riconfigurare l&#39;accesso all&#39;integrazione legacy di [!DNL SharePoint] e mantenere aggiornato il segreto client di SharePoint.

* [Riconfigura l&#39;accesso all&#39;integrazione legacy [!DNL SharePoint] &#x200B;](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Configura il segreto client per l&#39;accesso continuo all&#39;integrazione legacy [!DNL SharePoint] &#x200B;](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Riconfigura l&#39;accesso all&#39;integrazione legacy di [!DNL SharePoint]

La riconfigurazione dell&#39;integrazione legacy di [!DNL SharePoint] consente agli utenti di accedere ai documenti collegati tramite l&#39;integrazione legacy di [!DNL SharePoint], garantendo al contempo che gli utenti non possano collegare nuovi documenti tramite tale integrazione.

>[!NOTE]
>
> * L&#39;integrazione legacy di [!DNL SharePoint] è etichettata come &quot;[!DNL SharePoint]&quot;.
> * La nuova integrazione [!DNL SharePoint] è etichettata &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Seleziona **[!UICONTROL Documenti]** nell&#39;area di navigazione a sinistra, quindi seleziona **[!UICONTROL Provider di cloud]**.
1. Verificare che l&#39;opzione **[!DNL SharePoint]** e l&#39;opzione **[!UICONTROL [!DNL SharePoint] (Graph API)]** siano entrambe abilitate.
1. Fai clic su **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, quindi seleziona **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Seleziona il segno di spunta a sinistra dell&#39;elenco per tutte le integrazioni esistenti, quindi seleziona **[!UICONTROL Disattiva]**.



### Configura il segreto client per l&#39;accesso continuo all&#39;integrazione legacy di [!DNL SharePoint]

Il segreto client [!DNL SharePoint] scade una volta all&#39;anno. Per garantire l&#39;accesso continuo ai documenti nell&#39;integrazione legacy di [!DNL SharePoint], è necessario mantenere aggiornato il relativo segreto client [!DNL SharePoint].

>[!IMPORTANT]
>
> Poiché [!DNL SharePoint] segreti client sono gestiti da [!DNL Microsoft], le funzionalità e le procedure del segreto client potrebbero cambiare in base agli aggiornamenti a [!DNL SharePoint] effettuati da [!DNL Microsoft]. Consultare sempre la documentazione di [!DNL Microsoft] per informazioni aggiornate sulle procedure e sulle funzionalità in [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Generare un nuovo segreto client come descritto in [Sostituire un segreto client in scadenza in un  [!DNL SharePoint] componente aggiuntivo](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Copia il segreto client in un percorso sicuro.
1. Accedere a [!DNL Workfront] come amministratore.
1. In Workfront, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro del **[!UICONTROL Main Menu]**, quindi fai clic sull&#39;icona **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > Integrazione **[!UICONTROL [!DNL SharePoint]]**.
1. Fai clic sull&#39;integrazione di [!DNL SharePoint] che desideri aggiornare, quindi fai clic su **[!UICONTROL Modifica]**.
1. Individua la sezione **Informazioni connessione** della finestra di modifica, quindi immetti il nuovo segreto client nel campo **[!UICONTROL Segreto client SharePoint]**.
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
1. Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

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

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![Document icon](assets/document-icon.png).
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

* [Problema: gli utenti rilevano errori basati sull&#39;autenticazione quando utilizzano l&#39;integrazione  [!DNL SharePoint] .](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: quando si tenta di sfogliare [!DNL SharePoint] i file in [!DNL Workfront], non viene visualizzata alcuna raccolta siti o tutte le raccolte siti.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: non è possibile accedere alle cartelle e ai documenti collegati in precedenza in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: gli utenti rilevano errori basati sull&#39;autenticazione durante l&#39;utilizzo dell&#39;integrazione [!DNL SharePoint]. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluzioni:

Gli utenti devono disporre delle autorizzazioni appropriate per il sito [!DNL SharePoint].

Gli utenti con l&#39;accesso [!UICONTROL Controllo completo] dispongono di tutte le autorizzazioni necessarie per l&#39;integrazione di [!DNL SharePoint]. Se non si desidera concedere l&#39;accesso Controllo completo agli utenti, è necessario concedere le seguenti autorizzazioni:

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

### Problema: quando si tenta di sfogliare [!DNL SharePoint] file in [!DNL Workfront], non vengono visualizzate alcune o tutte le raccolte siti. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluzioni:

Per visualizzare una raccolta siti in [!DNL Workfront], è necessario soddisfare le seguenti condizioni:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* L&#39;utente deve disporre dell&#39;accesso in visualizzazione alla raccolta siti in [!DNL SharePoint].

  Per verificare questa situazione in [!DNL SharePoint], controllare le autorizzazioni della raccolta siti in SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problema: impossibile accedere alle cartelle e ai documenti collegati in precedenza in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Soluzione:

Se l&#39;utente che ha collegato una cartella [!DNL SharePoint] non è più in grado di eseguire l&#39;autenticazione, [!DNL Workfront] non potrà più accedere al contenuto della cartella. Ciò può verificarsi, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda.

Per garantire l’accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

Per informazioni sul collegamento di cartelle da provider esterni, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
