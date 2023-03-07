---
title: Configurare [!DNL SharePoint] integrazione
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: È possibile integrare [!DNL Workfront] con [!DNL SharePoint] Online, per consentire agli utenti di navigare, collegarsi e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altri [!DNL Workfront] ad esempio Google Drive, Box e Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2517'
ht-degree: 0%

---

# Configurare la versione precedente [!DNL SharePoint] integrazione

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
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

Devi disporre degli accessi o delle autorizzazioni necessari in [!DNL SharePoint] per modificare o configurare i [!DNL SharePoint].

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


## Configurare l’integrazione legacy di SharePoint per l’accesso continuo ai documenti

Per garantire agli utenti un accesso continuo ai documenti collegati a Workfront tramite l’integrazione legacy di SharePoint, devi riconfigurare l’accesso all’integrazione legacy di SharePoint e mantenere aggiornato SharePoint Client Secret.

* [Riconfigurare l’accesso alla versione precedente di [!DNL SharePoint] integrazione](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configura il segreto client per l’accesso continuo ai [!DNL SharePoint] integrazione](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Riconfigurare l’accesso alla versione precedente di [!DNL SharePoint] integrazione

Per garantire l&#39;accesso ai documenti collegati tramite [!DNL SharePoint] , assicurando al contempo che gli utenti non possano collegare nuovi documenti tramite tale integrazione, completa la procedura seguente.

>[!NOTE]
>
> * La versione precedente [!DNL SharePoint] l’integrazione è etichettata &quot;[!DNL SharePoint].&quot;
> * Il nuovo [!DNL SharePoint] l’integrazione è etichettata &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;


1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![Configurazione](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona quindi **[!UICONTROL Provider cloud]**.
1. Assicurati che il **[!DNL SharePoint]** opzione e **[!UICONTROL [!DNL SharePoint](Graph API)]** sono entrambe abilitate.
1. Fai clic su **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona quindi **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Seleziona il segno di spunta a sinistra dell’elenco per tutte le integrazioni esistenti, quindi seleziona **[!UICONTROL Disattiva]**.


### Configura il segreto client per l’accesso continuo ai [!DNL SharePoint] integrazione

Il tuo [!DNL SharePoint] Il segreto client scade una volta all’anno. Per garantire un accesso continuo ai documenti [!DNL SharePoint] integrazione, è necessario mantenere i [!DNL SharePoint] Segreto client aggiornato.

>[!IMPORTANT]
>
> Perché [!DNL SharePoint] I segreti client sono gestiti da [!DNL Microsoft], le funzioni e le procedure del segreto client possono cambiare in base agli aggiornamenti apportati a [!DNL SharePoint] creato da [!DNL Microsoft]. Controlla sempre [!DNL Microsoft] per informazioni aggiornate sulle procedure e le funzioni di [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genera un nuovo segreto client come descritto in [Sostituire un segreto client in scadenza in un [!DNL SharePoint] Componente aggiuntivo](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copia il segreto client in un percorso sicuro.
1. Accedi a [!DNL Workfront] come amministratore.
1. In Workfront, fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Fai clic sul pulsante [!DNL SharePoint] dell’integrazione da aggiornare, quindi fai clic su **[!UICONTROL Modifica]**.
1. Immetti il nuovo segreto client in **[!UICONTROL Segreto client]** campo.
1. Fai clic su **[!UICONTROL Salva]**.



## Istruzioni per la configurazione dell’integrazione legacy di SharePoint

>[!IMPORTANT]
>
>Questa integrazione è stata rimossa. Le istruzioni qui sono solo a scopo informativo e verranno rimosse a breve.


Workfront si connette a [!DNL SharePoint] Online utilizzando OAuth 2.0, uno standard utilizzato dalla maggior parte delle integrazioni basate sul web per l’autenticazione e l’autorizzazione degli utenti.

Per configurare OAuth, è necessario creare un [!DNL SharePoint] sito e un&#39;app del sito in [!DNL SharePoint]. Questo processo è descritto nelle sezioni seguenti.

Per ulteriori informazioni su OAuth, consulta [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Per semplificare la copia e l&#39;incollamento delle informazioni tra [!DNL Workfront] e [!DNL SharePoint] in questi passaggi si consiglia di mantenere entrambe le applicazioni aperte in schede separate.

* [Creare e configurare un [!DNL SharePoint] sito](#create-and-configure-a-sharepoint-site)
* [Concedere le autorizzazioni di scrittura all’app del sito](#grant-write-permissions-to-the-site-app)
* [Creare un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione](#create-a-workfront-sharepoint-integration-instance)
* [Completare l’integrazione](#complete-your-integration)
* [Aggiungi documenti](#add-documents)

### Creare e configurare un [!DNL SharePoint] sito  {#create-and-configure-a-sharepoint-site}

Per ottenere [!DNL Workfront] per eseguire l’autenticazione con [!DNL SharePoint], [!DNL Workfront] può utilizzare un sito principale in cui gli utenti dispongono di [!UICONTROL Controllo completo] livello di autorizzazione o autorizzazioni Manage specifiche. Il sito master funge da punto di ingresso di autenticazione per [!DNL Workfront].

Per creare e configurare un [!DNL SharePoint] Sito:

1. (Facoltativo) Se non si desidera utilizzare il sito principale dell&#39;organizzazione, è possibile creare un sito principale in [!DNL SharePoint].

   Per istruzioni, visita [Creare un sito](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) nel [!DNL Microsoft] Documentazione.

   * Seleziona la **[!UICONTROL Sito team]** durante la creazione del sito.

1. (Condizionale) Se hai creato un sito nel passaggio 1, passa al sito appena creato.

   Oppure

   Se non hai creato un sito nel passaggio 1, passa al sito principale della tua organizzazione.

1. Aggiungi `/_layouts/15/appregnew.aspx` alla fine dell’URL nella barra di ricerca nella parte superiore della finestra del browser.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL ID client]</p> </td> 
      <td> <p>Clic <strong>[!UICONTROL Genera]</strong> per generare un ID client. Copia questo ID in un percorso sicuro. La utilizzerai in seguito quando configurerai il [!DNL SharePoint] integrazione in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Segreto client]</p> </td> 
      <td> <p>Clic <strong>[!UICONTROL Genera]</strong> per generare un segreto client. Copia il segreto in una posizione sicura. La utilizzerai in seguito quando configurerai il [!DNL SharePoint] integrazione in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titolo</p> </td> 
      <td> <p>Inserisci un titolo, ad esempio [!DNL Workfront] App del sito. Gli utenti visualizzano questo titolo quando aggiungono documenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL URI reindirizzamento]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea]**
1. Continua con [Concedere le autorizzazioni di scrittura all’app del sito](#grant-write-permissions-to-the-site-app).

### Concedere le autorizzazioni di scrittura all’app del sito  {#grant-write-permissions-to-the-site-app}

A questo punto, hai creato correttamente un’app del sito e l’hai registrata in [!DNL Workfront]. Questa app del sito è nota anche come app principal in [!DNL SharePoint]. Risiede nel tuo tenant. Le nuove app del sito non hanno automaticamente accesso alle raccolte siti all’interno del tenant. Le autorizzazioni devono essere concesse in modo esplicito per ogni raccolta siti. Nei passaggi seguenti verrà illustrato come concedere l&#39;autorizzazione di scrittura alla nuova app del sito per una raccolta siti. Ripeti questi passaggi per ogni raccolta siti aggiunta in [!UICONTROL Raccolte siti visibili] nei passaggi precedenti.

Questa app del sito deve avere [!UICONTROL Scrittura] autorizzazioni per tutte le raccolte siti a cui gli utenti devono accedere tramite [!DNL Workfront].

1. Aggiungere &quot;/_layouts/15/appinv.aspx&quot; all’URL in [!DNL Sharepoint].

   **Esempio:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configura i campi seguenti

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID app]</td> 
      <td> <p>Aggiungi l'ID client creato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>e fai clic su <strong>Ricerca [!UICONTROL]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Queste impostazioni vengono compilate automaticamente quando si fa clic su [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copiare il codice XML seguente nel campo [!UICONTROL Permission Request XML]. Assicurati che venga aggiunto esattamente come mostrato, senza spazi aggiuntivi, ecc. per evitare errori.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Fai clic su **[!UICONTROL Crea]**.
1. Nella finestra di dialogo visualizzata, fai clic su **[!UICONTROL Fidati]**.
1. Verificare che l&#39;app del sito abbia accesso alla raccolta siti facendo clic sul pulsante **[!UICONTROL Autorizzazioni app per raccolta siti]** collegamento in [!UICONTROL Impostazioni sito].
1. Ripeti i passaggi precedenti per le altre raccolte siti, quindi continua con [Creare un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione](#create-a-workfront-sharepoint-integration-instance).

### Creare un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione {#create-a-workfront-sharepoint-integration-instance}

Quando hai creato un’app del sito in [!DNL SharePoint], ora puoi copiare le informazioni dall’app del sito in [!DNL Workfront]. L’app del sito è un’entità principale dell’app e funge da canale attraverso il quale vengono effettuate le richieste OAuth per accedere ai documenti all’interno delle raccolte siti.

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Clic **[!UICONTROL Aggiungi[!DNL SharePoint]]**.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Immetti un nome per [!DNL SharePoint] integrazione. Gli utenti visualizzano questo nome quando fanno clic su [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration' (Nome dell'integrazione). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Istanza host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Dominio di accesso]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Si riferisce al sito principale che gli utenti utilizzeranno per l’autenticazione tramite. È probabile che sia lo stesso dominio di [!UICONTROL [!DNL SharePoint] Istanza host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> Le raccolte siti vengono utilizzate solo nella versione precedente [!DNL SharePoint] Integrazione.
       <ul> 
        <li> <p><b>Se utilizzi il sito principale della tua organizzazione</b><b>:</b> </p> <p>Invio <code>/</code></p> </li> 
        <li> <p><b>Se si utilizza un sito principale e siti secondari:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] non consiglia più l'utilizzo dei siti secondari.</p> <p>Immettere il file dell'URL per la raccolta siti creata nella sezione precedente.</p> <p>Questa è la sezione dell’URL dopo .com.</p> <p>Esempio: per l’URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, lo stelo sarebbe <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID client]</td> 
      <td>Immetti l'ID client generato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Segreto client]</td> 
      <td>Immetti il segreto client generato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL raccolte siti visibili]</td> 
      <td> <b>Importante</b> Le raccolte siti vengono utilizzate solo nella versione precedente [!DNL SharePoint] integrazione.
       <ul> 
        <li> <p><b> Se utilizzi il sito principale della tua organizzazione</b><b>:</b> </p> <p>Invio <code>/</code></p> </li> 
        <li> <p><b>Se si utilizza un sito principale e siti secondari:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] non consiglia più l'utilizzo dei siti secondari.</p> <p>Per ogni sito secondario che si desidera aggiungere al [!DNL SharePoint] nell'integrazione, immettere lo stelo del sito secondario.</p> <p>Esempio: per l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, lo stelo sarebbe <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTA</b>:   <p>Se si desidera verificare solo la configurazione (nessun sito secondario), immettere lo stelo del sito principale. </p> <p>Esempio: per l’URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, lo stelo sarebbe <code>/sites/mysite</code>.</p> <p>Dopo aver testato la configurazione come descritto in <a href="#complete-your-integration" class="MCXref xref">Completare l’integrazione</a>, è necessario rimuovere il sito master e immettere i siti secondari.</p> 
          <ol> 
           <li value="1">Fai clic su <strong>Menu principale di [!UICONTROL]</strong> icona <img src="assets/main-menu-icon.png"> nell'angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Nel pannello a sinistra, fai clic su <strong>[!UICONTROL Documenti]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integrazione]</strong>.</p></li><li><p>Fai clic su [!DNL SharePoint] dell’integrazione che stai impostando, quindi fai clic su Modifica.</p></li><li><p>Eliminare lo stelo del sito master dal campo [!UICONTROL Raccolte siti visibili].</p></li><li><p>Per ogni sito secondario che si desidera aggiungere al [!DNL SharePoint] nell'integrazione, immettere lo stelo del sito secondario.</p></li><p>Esempio: per l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, lo stelo sarebbe <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**
1. Continua con [Completare l’integrazione](#complete-your-integration).

### Completare l’integrazione {#complete-your-integration}

La configurazione di base è quasi completa.

1. In Workfront, fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Documenti]** ![](assets/document-icon.png).
1. Clic **[!UICONTROL Aggiungi nuovo]**.
1. Clic **[!UICONTROL Da]`<title of your [!DNL SharePoint] site>`** nel menu a discesa.

   Verrà visualizzata una finestra di dialogo in cui si invita l&#39;utente a considerare attendibile il sito.

   >[!NOTE]
   >
   >Se questa finestra di dialogo non viene visualizzata, [!DNL SharePoint] L’integrazione di non è configurata correttamente.

1. Clic **[!UICONTROL Fidati]**.

### Aggiungi documenti {#add-documents}

È ora possibile aggiungere documenti da [!DNL SharePoint] sito.

Per istruzioni, consulta [Collega un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Se l’utente che ha collegato una cartella non ha più accesso all’applicazione esterna, [!DNL Workfront] non può più accedere al contenuto della cartella. Ciò può verificarsi, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda. Per garantire l’accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

## Risoluzione dei problemi

* [Problema: si verificano errori basati sull’autenticazione quando si utilizza [!DNL SharePoint] integrazione.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: as a [!DNL Workfront] utente, non è possibile effettuare il provisioning di un nuovo [!DNL SharePoint] dell&#39;istanza. Quando tento di farlo, viene visualizzato un errore.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: quando si tenta di esplorare [!DNL SharePoint] file in [!DNL Workfront], non viene visualizzata alcuna raccolta siti o tutte le raccolte siti.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: impossibile accedere a cartelle e documenti collegati in precedenza in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: si verificano errori basati sull’autenticazione quando si utilizza [!DNL SharePoint] integrazione. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluzioni:

Gli utenti devono essere membri di un gruppo che dispone delle autorizzazioni appropriate per [!DNL SharePoint] sito.

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

### Problema: as a [!DNL Workfront] utente, non è possibile effettuare il provisioning di un nuovo [!DNL SharePoint] dell&#39;istanza. Quando tento di farlo, viene visualizzato un errore. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluzioni:

Ciò può essere causato da una serie di elementi, provenienti da [!DNL Workfront] o [!DNL SharePoint]configurazione di. Verifica che:

* L’ID client, il segreto client, l’URL restituito e altri campi di configurazione sono mappati correttamente tra i [!DNL Workfront] [!DNL SharePoint] Istanza di integrazione e [!DNL SharePoint] App del sito.
* L’utente ha [!UICONTROL Controllo completo] autorizzazione per la raccolta siti utilizzata per l&#39;autenticazione.
* L’app del sito è elencata in [!UICONTROL Autorizzazioni app per siti] per [!UICONTROL Raccolta siti] utilizzato per l’autenticazione.

### Problema: quando si tenta di esplorare [!DNL SharePoint] file in [!DNL Workfront], non viene visualizzata alcuna raccolta siti o tutte le raccolte siti. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluzioni:

Per visualizzare una raccolta siti in [!DNL Workfront], devono essere soddisfatte le seguenti condizioni:

* La raccolta siti deve essere registrata nel [!DNL Workfront] [!DNL SharePoint] Istanza di integrazione.

   Per verificarlo in [!DNL Workfront]:

   1. Vai a [!UICONTROL Configurazione] > [!UICONTROL Documenti] > [!UICONTROL [!DNL SharePoint] Integrazione].
   1. Modifica il [!DNL SharePoint] Informazioni sull’istanza di integrazione.
   1. Verificare che la raccolta siti sia elencata in [!UICONTROL Raccolte siti visibili].

* L&#39;utente deve disporre dell&#39;accesso in visualizzazione alla raccolta siti in [!DNL SharePoint].
* Per verificarlo in [!DNL SharePoint], vai a [!DNL SharePoint], e aprire la raccolta siti > [!UICONTROL Impostazioni] > [!UICONTROL Autorizzazioni del sito].
* Il [!DNL SharePoint] L&#39;app del sito deve avere accesso alla raccolta siti.

   Per verificarlo in [!DNL SharePoint]:

   1. Vai alla raccolta siti > [!UICONTROL Impostazioni] > [!UICONTROL Autorizzazioni per l’app del sito].
   1. Assicurati che [!UICONTROL App del sito] utilizzato da [!DNL Workfront] è elencato qui.
   1. (Condizionale) Se l&#39;app del sito non è elencata, aggiungi alla raccolta siti utilizzando _layouts/15/appinv.aspx.

      Per informazioni sull&#39;aggiunta della raccolta siti, vedere Concessione di autorizzazioni di scrittura all&#39;app del sito.

### Problema: impossibile accedere a cartelle e documenti collegati in precedenza in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Soluzione:

Se l’utente che ha collegato [!DNL SharePoint] la cartella non può più eseguire l&#39;autenticazione, [!DNL Workfront] non può più accedere al contenuto della cartella. Ciò può verificarsi, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda.

Per garantire l’accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

Per informazioni sul collegamento di cartelle da provider esterni, consulta [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: viene visualizzato l&#39;errore &quot;404 not found&quot; quando si tenta di aggiungere un documento da [!DNL Sharepoint]

#### Soluzione:

Questo errore può verificarsi se uno dei siti è configurato in [!UICONTROL Raccolte siti visibili] è stato eliminato in Sharepoint. Controlla la [!UICONTROL Raccolte siti visibili] e rimuovere tutti i siti eliminati in Sharepoint.
