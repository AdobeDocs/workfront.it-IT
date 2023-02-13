---
title: Configura le [!DNL SharePoint] integrazione
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: È possibile integrare [!DNL Workfront] con [!DNL SharePoint] Online, per fornire agli utenti la possibilità di navigare, collegare e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altre [!DNL Workfront] integrazioni, ad esempio Google Drive, Box e Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# Configurare la versione precedente [!DNL SharePoint] integrazione

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Il nuovo [!DNL SharePoint] l’integrazione è stata rilasciata in produzione con la versione 22.3 (luglio 2022). Anche se gli utenti possono comunque accedere ai documenti collegati tramite la versione precedente [!DNL SharePoint] integrazione, devono utilizzare il nuovo [!DNL SharePoint] integrazione per collegare documenti da SharePoint.
>
>* La nuova integrazione di SharePoint non richiede la configurazione da parte di un amministratore e può essere impostata dai singoli utenti. Tuttavia, per garantire una transizione senza problemi alla nuova integrazione di SharePoint, un amministratore Workfront deve apportare alcune piccole modifiche alle impostazioni nell’area Configurazione di Workfront.
   >
   >    Per informazioni e istruzioni, consulta [Configurare l’integrazione legacy di SharePoint per un accesso continuo ai documenti](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in questo articolo.
>    
>* È consigliabile che gli utenti colleghino i documenti attualmente collegati tramite la versione precedente di [!DNL SharePoint] integrazione attraverso la nuova integrazione.
   >    
   >    Per istruzioni sul collegamento dei documenti, consulta [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


È possibile integrare [!DNL Workfront] con [!DNL SharePoint Online], fornendo agli utenti la possibilità di navigare, collegare e aggiungere [!DNL SharePoint] documenti in Workfront. La funzionalità fornita è simile a quella di altre [!DNL Workfront] integrazioni, ad esempio [!DNL Google Drive], [!DNL Box]e [!DNL Dropbox].

Questa integrazione è compatibile solo con [!DNL SharePoint Online]. Istanze on-premise di [!DNL SharePoint] non sono supportati.

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

È necessario disporre di qualsiasi accesso o autorizzazione necessari in [!DNL SharePoint] per modificare o configurare i [!DNL SharePoint].

## Collegamento di documenti tramite la nuova integrazione SharePoint

I singoli utenti possono collegare i documenti attraverso i nuovi [!DNL SharePoint] integrazione. L&#39;integrazione non richiede la configurazione amministratore. Al contrario, l’utente accede al [!DNL Microsoft] quando si collega un documento, ciò consente all&#39;integrazione di accedere ai documenti disponibili nel [!DNL SharePoint].

La prima volta che un utente connette il [!DNL Workfront] [!DNL SharePoint] integrazione con i [!DNL SharePoint] , visualizzeranno e accetteranno tutte le autorizzazioni che [!DNL Workfront] utilizza durante l’interazione con i [!UICONTROL SharePoint] conto. Autorizzazioni di lettura consentite [!DNL Workfront] per visualizzare e accedere ai file su [!DNL SharePoint]e le autorizzazioni di scrittura consentono all’utente di caricare i file in [!DNL SharePoint].

Per istruzioni sul collegamento di documenti attraverso il nuovo [!DNL SharePoint] integrazione, vedi [Collegamento di un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] l&#39;integrazione può connettersi a un singolo [!DNL SharePoint] istanza. Pertanto, un utente può impostare un&#39;integrazione per un [!DNL SharePoint], ma non può impostare un&#39;integrazione su un secondo [!DNL SharePoint], anche se dispongono di autorizzazioni per e documenti nel secondo [!DNL SharePoint].
>
>* Un utente ha accesso agli stessi siti, raccolte, cartelle, sottocartelle e file tramite [!DNL Workfront] [!DNL SharePoint] l&#39;integrazione nella loro [!DNL SharePoint] conto.


## Configurare l’integrazione legacy di SharePoint per un accesso continuo ai documenti

Per garantire agli utenti l’accesso ai documenti collegati a Workfront tramite l’integrazione legacy di SharePoint, è necessario riconfigurare l’accesso all’integrazione legacy di SharePoint e mantenere aggiornato il segreto client di SharePoint.

* [Riconfigura l’accesso alle versioni precedenti [!DNL SharePoint] integrazione](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configurare il segreto client per un accesso continuo alla versione precedente [!DNL SharePoint] integrazione](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Riconfigura l’accesso alle versioni precedenti [!DNL SharePoint] integrazione

Per garantire l’accesso ai documenti collegati tramite la versione precedente [!DNL SharePoint] l&#39;integrazione, assicurando al tempo stesso che gli utenti non possano collegare nuovi documenti tramite tale integrazione, completa la seguente procedura.

>[!NOTE]
>
> * L&#39;eredità [!DNL SharePoint] l&#39;integrazione è contrassegnata &quot;[!DNL SharePoint].&quot;
> * Il nuovo [!DNL SharePoint] l&#39;integrazione è contrassegnata &quot;[!UICONTROL [!DNL SharePoint] (API grafico)].&quot;


1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![Configurazione](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona **[!UICONTROL Provider cloud]**.
1. Assicurati che il **[!DNL SharePoint]** opzione e **[!UICONTROL [!DNL SharePoint](API grafico)]** sono entrambe abilitate.
1. Fai clic su **[!UICONTROL Salva]**.
1. Seleziona **[!UICONTROL Documenti]** nel menu di navigazione a sinistra, seleziona **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Seleziona il segno di spunta a sinistra dell’elenco per tutte le integrazioni esistenti, quindi seleziona **[!UICONTROL Disattiva]**.


### Configurare il segreto client per un accesso continuo alla versione precedente [!DNL SharePoint] integrazione

Le [!DNL SharePoint] Il segreto client scade una volta all&#39;anno. Per garantire l’accesso continuo ai documenti della versione precedente [!DNL SharePoint] integrazione, è necessario mantenere [!DNL SharePoint] Segreto client aggiornato.

>[!IMPORTANT]
>
> Perché [!DNL SharePoint] I segreti client vengono gestiti da [!DNL Microsoft], le funzioni e le procedure Segreto client possono cambiare in base agli aggiornamenti apportati a [!DNL SharePoint] realizzato da [!DNL Microsoft]. Controlla sempre la [!DNL Microsoft] documentazione per informazioni aggiornate sulle procedure e le funzioni di [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genera un nuovo segreto client come descritto in [Sostituire un segreto client in scadenza in un [!DNL SharePoint] Componente aggiuntivo](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copia questo segreto client in una posizione sicura.
1. Accedi a [!DNL Workfront] come amministratore.
1. In Workfront, fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Fai clic sul pulsante [!DNL SharePoint] integrazione da aggiornare, quindi fare clic su **[!UICONTROL Modifica]**.
1. Immetti il nuovo segreto client nel **[!UICONTROL Segreto client]** campo .
1. Fai clic su **[!UICONTROL Salva]**.



## Istruzioni per la configurazione dell’integrazione legacy di SharePoint

>[!IMPORTANT]
>
>Questa integrazione è stata dichiarata obsoleta. Le istruzioni qui sono solo a scopo informativo e saranno rimosse nel prossimo futuro.


Workfront si connette a [!DNL SharePoint] Online con OAuth 2.0, standard utilizzato dalla maggior parte delle integrazioni basate su web per l’autenticazione e l’autorizzazione degli utenti.

Per configurare OAuth, devi creare un [!DNL SharePoint] sito e un’app del sito in [!DNL SharePoint]. Questo processo è descritto nelle sezioni seguenti.

Per ulteriori informazioni su OAuth, consulta [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Per semplificare la copia e l’incolla delle informazioni tra [!DNL Workfront] e [!DNL SharePoint] in questi passaggi, si consiglia di mantenere aperte entrambe le applicazioni in schede separate.

* [Creare e configurare un [!DNL SharePoint] sito](#create-and-configure-a-sharepoint-site)
* [Concedere autorizzazioni di scrittura all’app sito](#grant-write-permissions-to-the-site-app)
* [Crea un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione](#create-a-workfront-sharepoint-integration-instance)
* [Completa l’integrazione](#complete-your-integration)
* [Aggiungi documenti](#add-documents)

### Creare e configurare un [!DNL SharePoint] sito  {#create-and-configure-a-sharepoint-site}

Per [!DNL Workfront] per autenticare con [!DNL SharePoint], [!DNL Workfront] può utilizzare un sito master in cui gli utenti hanno [!UICONTROL Controllo completo] livello di autorizzazione o autorizzazioni di gestione specifiche. Questo sito master funge da punto di ingresso autenticazione per [!DNL Workfront].

Per creare e configurare un [!DNL SharePoint] Sito:

1. (Facoltativo) Se non desideri utilizzare il sito principale dell&#39;organizzazione, puoi creare un sito principale in [!DNL SharePoint].

   Per istruzioni, visita [Creare un sito](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in [!DNL Microsoft] Documentazione.

   * Seleziona la **[!UICONTROL Sito del team]** durante la creazione del sito.

1. (Condizionale) Se hai creato un sito nel passaggio 1, vai al sito appena creato.

   Oppure

   Se non hai creato un sito nel passaggio 1, vai al sito principale della tua organizzazione.

1. Aggiungi `/_layouts/15/appregnew.aspx` alla fine dell’URL nella barra di ricerca nella parte superiore della finestra del browser.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>ID client [!UICONTROL]</p> </td> 
      <td> <p>Fai clic su <strong>[!UICONTROL Generate]</strong> per generare un ID client. Copia questo ID in una posizione sicura. La utilizzerai in un secondo momento quando configurerai la [!DNL SharePoint] integrazione in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Segreto client]</p> </td> 
      <td> <p>Fai clic su <strong>[!UICONTROL Generate]</strong> per generare un segreto client. Copia questo segreto in una posizione sicura. La utilizzerai in un secondo momento quando configurerai la [!DNL SharePoint] integrazione in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titolo</p> </td> 
      <td> <p>Inserisci un titolo, ad esempio [!DNL Workfront] App del sito. Gli utenti visualizzano questo titolo quando aggiungono documenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Dominio app [!UICONTROL]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL URI di reindirizzamento]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea]**
1. Continua a [Concedere autorizzazioni di scrittura all’app sito](#grant-write-permissions-to-the-site-app).

### Concedere autorizzazioni di scrittura all’app sito  {#grant-write-permissions-to-the-site-app}

A questo punto, hai creato correttamente un’app del sito e l’hai registrata all’interno di [!DNL Workfront]. Questa app per sito è anche nota come entità principale dell&#39;app in [!DNL SharePoint]. Si trova all’interno del tenant. Le nuove app del sito non hanno automaticamente accesso alle raccolte siti all’interno del tenant. Le autorizzazioni devono essere concesse esplicitamente per ogni raccolta siti. I passaggi seguenti mostrano come concedere l’autorizzazione di scrittura alla nuova app del sito una raccolta siti. Ripeti questi passaggi per ciascuna raccolta siti aggiunta in [!UICONTROL Raccolte siti visibili] nei passaggi precedenti.

Questa app del sito deve avere [!UICONTROL Scrivi] autorizzazione a qualsiasi raccolta siti a cui gli utenti devono accedere tramite [!DNL Workfront].

1. Aggiungi &quot;/_layouts/15/appinv.aspx&quot; all’URL in [!DNL Sharepoint].

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
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Aggiungi l'ID client creato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>e fai clic su <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL URL di reindirizzamento]</p> </td> 
      <td> <p>Questi vengono compilati automaticamente quando fai clic su [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copia il seguente XML nel campo [!UICONTROL Permission Request XML] (XML richiesta di autorizzazione). Assicurati che venga aggiunto esattamente come mostrato senza spazi aggiuntivi, ecc. per evitare errori.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Fai clic su **[!UICONTROL Crea]**.
1. Nella finestra di dialogo visualizzata, fai clic su **[!UICONTROL Fidati di]**.
1. Verifica che l’app del sito abbia accesso alla raccolta siti facendo clic sul pulsante **[!UICONTROL Autorizzazioni per le app di raccolta siti]** collegare [!UICONTROL Impostazioni sito].
1. Ripeti i passaggi precedenti per le raccolte siti rimanenti, quindi continua con [Crea un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione](#create-a-workfront-sharepoint-integration-instance).

### Crea un [!DNL Workfront] [!DNL SharePoint] istanza di integrazione {#create-a-workfront-sharepoint-integration-instance}

Quando hai creato un’app sito in [!DNL SharePoint], ora puoi copiare le informazioni dall’app sito in [!DNL Workfront]. L’app sito è un’entità app e funge da canale tramite il quale vengono effettuate le richieste OAuth per accedere ai documenti all’interno delle raccolte siti.

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Fai clic su **[!UICONTROL Aggiungi[!DNL SharePoint]]**.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Immetti un nome per la [!DNL SharePoint] integrazione. Gli utenti visualizzano questo nome quando fanno clic su [!UICONTROL Aggiungi] &gt; [!UICONTROL Da] 'nome dell'integrazione'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Istanza host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Dominio di accesso]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Si riferisce al sito principale che gli utenti utilizzeranno per l’autenticazione tramite . È probabilmente lo stesso dominio del [!UICONTROL [!DNL SharePoint] Istanza host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> Le raccolte siti vengono utilizzate solo nella versione precedente [!DNL SharePoint] Integrazione.
       <ul> 
        <li> <p><b>Se utilizzi il sito principale dell’organizzazione</b><b>:</b> </p> <p>Invio <code>/</code></p> </li> 
        <li> <p><b>Se si utilizza un sito master e siti secondari:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] sconsiglia più l’utilizzo di siti secondari.</p> <p>Inserisci il fusto URL per la raccolta siti creata nella sezione precedente.</p> <p>Questa è la sezione dell'URL dopo .com.</p> <p>Esempio: per l’URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, lo stelo sarebbe <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID client]</td> 
      <td>Immetti l’ID client generato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Segreto client]</td> 
      <td>Inserisci il segreto client generato in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creare e configurare un [!DNL SharePoint] sito </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Raccolte siti visibili]</td> 
      <td> <b>Importante</b> Le raccolte siti vengono utilizzate solo nella versione precedente [!DNL SharePoint] integrazione.
       <ul> 
        <li> <p><b> Se utilizzi il sito principale dell’organizzazione</b><b>:</b> </p> <p>Invio <code>/</code></p> </li> 
        <li> <p><b>Se si utilizza un sito master e siti secondari:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] sconsiglia più l’utilizzo di siti secondari.</p> <p>Per ogni sito secondario che desideri aggiungere al tuo [!DNL SharePoint] integrazione, immettere il fusto del sito secondario.</p> <p>Esempio: per l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, lo stelo sarebbe <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTA</b>:   <p>Se si desidera testare solo la configurazione (nessun sito secondario), immettere lo stelo del sito principale. </p> <p>Esempio: per l’URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, lo stelo sarebbe <code>/sites/mysite</code>.</p> <p>Quando hai verificato la configurazione come descritto in <a href="#complete-your-integration" class="MCXref xref">Completa l’integrazione</a>, è necessario rimuovere il sito master e immettere i siti secondari.</p> 
          <ol> 
           <li value="1">Fai clic sul pulsante <strong>[!UICONTROL Menu principale]</strong> icona <img src="assets/main-menu-icon.png"> nell'angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Nel pannello a sinistra, fai clic su <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integrazione]</strong>.</p></li><li><p>Fai clic sul pulsante [!DNL SharePoint] integrazione da configurare, quindi fare clic su Modifica.</p></li><li><p>Elimina lo stelo per il sito principale dal campo [!UICONTROL Visible Site Collections] (Raccolte siti visibili).</p></li><li><p>Per ogni sito secondario che desideri aggiungere al tuo [!DNL SharePoint] integrazione, immettere il fusto del sito secondario.</p></li><p>Esempio: per l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, lo stelo sarebbe <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**
1. Continua a [Completa l’integrazione](#complete-your-integration).

### Completa l’integrazione {#complete-your-integration}

La configurazione di base è quasi completa.

1. In Workfront, fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Documenti]** ![](assets/document-icon.png).
1. Fai clic su **[!UICONTROL Aggiungi nuovo]**.
1. Fai clic su **[!UICONTROL Da]`<title of your [!DNL SharePoint] site>`** nel menu a discesa .

   Viene visualizzata una finestra di dialogo che ti invita a Considerare attendibile il sito.

   >[!NOTE]
   >
   >Se questa finestra di dialogo non viene visualizzata, la [!DNL SharePoint] integrazione non configurata correttamente.

1. Fai clic su **[!UICONTROL Fidati di]**.

### Aggiungi documenti {#add-documents}

È ora possibile aggiungere documenti dal [!DNL SharePoint] sito.

Per istruzioni, consulta [Collegamento di un documento esterno a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Se l’utente che ha collegato una cartella non ha più accesso all’applicazione esterna, [!DNL Workfront] non può più accedere al contenuto della cartella. Questo può accadere, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda. Per garantire un accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

## Risoluzione dei problemi

* [Problema: Gli utenti rilevano errori basati sull’autenticazione quando utilizzano [!DNL SharePoint] integrazione.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: Come [!DNL Workfront] utente, impossibile eseguire il provisioning di un nuovo [!DNL SharePoint] istanza. Quando provo a farlo, vedo un errore.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: Quando si tenta di sfogliare [!DNL SharePoint] file in [!DNL Workfront], non visualizzo nessuna o tutte le raccolte siti.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: Non è possibile accedere a cartelle e documenti precedentemente collegati in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Gli utenti rilevano errori basati sull’autenticazione quando utilizzano [!DNL SharePoint] integrazione. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluzioni:

Gli utenti devono essere membri di un gruppo che dispone delle autorizzazioni appropriate per [!DNL SharePoint] sito.

Utenti con [!UICONTROL Controllo completo] accedere dispone di tutte le autorizzazioni necessarie per [!DNL SharePoint] integrazione. Se non desideri concedere l&#39;accesso a Controllo completo agli utenti, devi concedere le seguenti autorizzazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Può visualizzare, aggiungere, aggiornare, eliminare, approvare e personalizzare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Edit]</p> </td> 
   <td> <p>Può aggiungere, modificare ed eliminare elenchi; può visualizzare, aggiungere, aggiornare ed eliminare elementi e documenti dell’elenco</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Può visualizzare, aggiungere, aggiornare ed eliminare elementi e documenti dell’elenco</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Solo visualizzazione]</p> </td> 
   <td> <p>Può visualizzare pagine, elementi di elenco e documenti (i tipi di documenti con gestori di file lato server possono essere visualizzati nel browser ma non scaricati)</p> </td> 
  </tr> 
 </tbody> 
</table>

Per istruzioni su come creare e modificare i livelli di autorizzazione, consulta [Come creare e modificare i livelli di autorizzazione](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) nella documentazione di Microsoft.

### Problema: Come [!DNL Workfront] utente, impossibile eseguire il provisioning di un nuovo [!DNL SharePoint] istanza. Quando provo a farlo, vedo un errore. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluzioni:

Ciò può essere causato da una serie di elementi, provenienti da [!DNL Workfront] o [!DNL SharePoint]Configurazione di . Verifica che:

* I campi ID client, Segreto client, URL di ritorno e altri campi di configurazione sono correttamente mappati tra [!DNL Workfront] [!DNL SharePoint] L&#39;istanza di integrazione e [!DNL SharePoint] App del sito.
* L&#39;utente ha [!UICONTROL Controllo completo] autorizzazione alla raccolta siti utilizzata per l&#39;autenticazione.
* L’app del sito è elencata in [!UICONTROL Autorizzazioni per le app per siti] per [!UICONTROL Raccolta siti] utilizzato per l&#39;autenticazione.

### Problema: Quando si tenta di sfogliare [!DNL SharePoint] file in [!DNL Workfront], non visualizzo nessuna o tutte le raccolte siti. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluzioni:

Per visualizzare una raccolta siti in [!DNL Workfront], devono essere soddisfatte le seguenti condizioni:

* La raccolta siti deve essere registrata nel [!DNL Workfront] [!DNL SharePoint] Istanza di integrazione.

   Per verificare questo in [!DNL Workfront]:

   1. Vai a [!UICONTROL Configurazione] > [!UICONTROL Documenti] > [!UICONTROL [!DNL SharePoint] Integrazione].
   1. Modifica le [!DNL SharePoint] Informazioni sull’istanza di integrazione.
   1. Verifica che la raccolta siti sia elencata in [!UICONTROL Raccolte siti visibili].

* L&#39;utente deve avere accesso alla raccolta siti in [!DNL SharePoint].
* Per verificare questo in [!DNL SharePoint], vai a [!DNL SharePoint], quindi apri la raccolta siti > [!UICONTROL Impostazioni] > [!UICONTROL Autorizzazioni del sito].
* La [!DNL SharePoint] L&#39;app del sito deve avere accesso alla raccolta siti.

   Per verificare questo in [!DNL SharePoint]:

   1. Vai alla raccolta siti > [!UICONTROL Impostazioni] > [!UICONTROL Autorizzazioni per le app per siti].
   1. Assicurati che [!UICONTROL App sito] utilizzato da [!DNL Workfront] è elencato qui.
   1. (Condizionale) Se l&#39;app del sito non è elencata, aggiungi alla raccolta siti utilizzando _layouts/15/appinv.aspx.

      Per informazioni sull&#39;aggiunta della raccolta siti, consulta Concessione di autorizzazioni di scrittura all&#39;app sito.

### Problema: Non è possibile accedere a cartelle e documenti precedentemente collegati in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Soluzione:

Se l’utente che ha collegato un [!DNL SharePoint] la cartella non può più essere autenticata, [!DNL Workfront] non può più accedere al contenuto della cartella. Questo può accadere, ad esempio, se l’utente che ha collegato originariamente la cartella lascia l’azienda.

Per garantire un accesso continuo, un utente con accesso alla cartella deve ricollegare la cartella.

Per informazioni sul collegamento di cartelle da fornitori esterni, consulta [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: Viene visualizzato un errore &quot;404 non trovato&quot; quando si tenta di aggiungere un documento da [!DNL Sharepoint]

#### Soluzione:

Questo errore potrebbe verificarsi se uno dei siti configurati nel [!UICONTROL Raccolte siti visibili] elenco eliminato in Sharepoint. Controlla la [!UICONTROL Raccolte siti visibili] e rimuovere i siti che sono stati eliminati in Sharepoint.
