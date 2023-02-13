---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Acrobat Sign
description: Con la [!DNL Adobe Acrobat Sign] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] in base agli eventi nel [!DNL Adobe] Account Acrobat Sign, creazione, lettura o aggiornamento di accordi e altri record, ricerca di record utilizzando i criteri impostati e caricamento di documenti.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 8bb97b08bb5991fadbf2627f4ebfdaa25ae337ce
workflow-type: tm+mt
source-wordcount: '6579'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] moduli

Con la [!DNL Adobe Acrobat Sign] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] in base agli eventi nel [!DNL Adobe Acrobat Sign] creare, leggere o aggiornare accordi e altri record, cercare record utilizzando i criteri impostati e caricare documenti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe Acrobat Sign] raccomandazioni di utilizzo del connettore

La [!DNL Adobe Sign ]l’app automatizza i processi aziendali di eSignature in [!DNL Fusion] molto più semplice e potente.

Nuovi utenti a [!DNL Adobe Sign] dovrebbero prestare particolare attenzione ad alcuni dei vincoli relativi all&#39;aggiornamento degli accordi. I contratti non vengono generalmente modificati una volta avviati. Consigliamo ai nuovi utenti di [!DNL Adobe Sign] concentrarsi sulla creazione di nuovi accordi utilizzando il modulo di creazione dell&#39;accordo. Questo farà [!DNL Fusion] automazione più semplice e migliore con [!DNL Adobe Sign].

[!DNL Adobe Sign] Gli accordi devono avere un campo d&#39;azione. Sono disponibili alcune opzioni per eseguire questa operazione, ma la più semplice e comune è caricare un documento transitorio e quindi mappare tale documento al contratto.

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] moduli e relativi campi

Quando si configura [!DNL Adobe Acrobat Sign] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Acrobat Sign] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL Attento agli accordi]**

Questo modulo di attivazione avvia uno scenario quando un contratto viene creato o aggiornato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Selezionare se si desidera controllare i nuovi record, i record aggiornati o entrambi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record] </td> 
   <td>Selezionare il tipo di record che si desidera controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trova testo]</td> 
   <td> <p>Immettere i termini che si desidera cercare. Il modulo restituisce record che includono questi termini come valori di campo.</p> <p>Per ulteriori informazioni sulla ricerca di campi in [!DNL Adobe Acrobat Sign], vedere "Come funziona la ricerca di testo in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Ricerca Adobe Sign - Come funziona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di accordi restituiti]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Guarda gli eventi]**

Questo modulo di attivazione avvia uno scenario in cui si verifica un evento selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>Selezionare il webhook che si desidera utilizzare o fare clic su <b>[!UICONTROL Aggiungi]</b> e compila i campi seguenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>Immettere un nome per il webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ambiti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Account]</p> </li> 
     <li> <p>[!UICONTROL Group]</p> </li> 
     <li> <p>[!UICONTROL Utente]</p> </li> 
     <li> <p>[!UICONTROL Resource]</p> <p>Se si seleziona [!UICONTROL Resource], immettere l'ID risorsa e il tipo di risorsa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Livello risorsa]</td> 
   <td> <p>Seleziona il tipo di risorsa da visualizzare.</p> 
    <ul> 
     <li> <p>Accordi [!UICONTROL]</p> </li> 
     <li> <p>[!UICONTROL Widget]</p> </li> 
     <li> <p>[!UICONTROL Megasign]</p> </li> 
     <li> <p>[!UICONTROL Documentazione libreria]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook eventi di abbonamento]</td> 
   <td>Seleziona la [!DNL Adobe Sign] eventi che si desidera che il modulo visualizzi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome visualizzato applicazione]</td> 
   <td>Nome visualizzato dell'applicazione attraverso la quale viene creato il webhook.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome applicazione]</td> 
   <td>Nome visualizzato dell'applicazione attraverso la quale viene creato il webhook.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-mail di notifica dei problemi di [!UICONTROL]</td> 
   <td> <p>Questa impostazione funziona solo per gli account amministratore</p> <p>Per ogni indirizzo e-mail a cui si desidera inviare le e-mail di notifica dei problemi, fare clic su <b>[!UICONTROL Aggiungi]</b> e immetti l’indirizzo e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement Parametri condizionali]</td> 
   <td>Se desideri aggiungere parametri condizionali, seleziona <b>[!UICONTROL Sì]</b> nel tipo di record a cui si desidera aggiungere i parametri, quindi selezionare <b>[!UICONTROL Sì]</b> su eventuali parametri da attivare.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Azioni

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL Creare un record]**

Questo modulo di azione crea un nuovo record del tipo selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Group]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Documento libreria]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Utente]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni sul gruppo]</td> 
   <td> <p>Immetti o mappa il [!UICONTROL Name] e l' [!UICONTROL ID] del gruppo e indica se questo è il gruppo predefinito per l'account.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni sul documento della libreria]</td> 
   <td> <p>Compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL File da inviare]</b> </p> <p>Per ogni file da aggiungere, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e compilare i campi.</p> 
      <ul> 
       <li><b>[!UICONTROL ID documento transitorio]</b> <p>Immettere l'ID del documento transitorio</p> </li> 
       <li> <p><b>[!UICONTROL URL trasferimento file]</b> </p> <p>Compila i campi seguenti:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Immettere il tipo di MIME del file originale. I tipi MIME (Multipurpose Internet Mail Extension) sono etichette che consentono al software di identificare diversi tipi di dati condivisi su Internet. I server web e i browser utilizzano il tipo MIME per determinare cosa deve essere fatto con un file. Ad esempio, un file con il tipo MIME <code>text/html</code> verrà elaborato in un browser in modo diverso rispetto a un file con tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere un nome per il file.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Immetti l’URL del file da inviare.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Selezionare se il documento deve essere notarizzato.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Nome modello libreria]</b> </p> <p>Immettere o mappare il nome del modello libreria</p> </li> 
     <li> <p><b>[!UICONTROL Modalità di condivisione]</b> </p> <p>Specifica gli utenti che devono avere accesso al documento della libreria.</p> </li> 
     <li> <p><b>[!UICONTROL Stato del documento della libreria]</b> </p> <p>Selezionare se il documento è in stato di authoring o attivo.</p> </li> 
     <li> <p><b>[!UICONTROL Tipo di modello libreria]</b> </p> <p>Per ogni tipo di modello libreria che desideri utilizzare, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e selezionare il tipo di modello.</p> </li> 
     <li> <p><b>[!UICONTROL Data ultimo evento]</b> </p> <p>Immettere l'ultima data in cui si è verificato un evento nel documento della libreria.</p> <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL Stato del documento della libreria]</b> </p> <p>Selezionare lo stato del documento della libreria.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni utente]</td> 
   <td> <p>Compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>E-MAIL [!UICONTROL]</b> </p> <p>Immetti l’indirizzo e-mail dell’utente.</p> </li> 
     <li> <p><b>[!UICONTROL È amministratore account]</b> </p> <p>Seleziona questa opzione se l’utente creato è un amministratore dell’account.</p> </li> 
     <li> <p><b>[!UICONTROL User ID]</b> </p> <p>Immetti l'ID univoco dell'utente</p> </li> 
     <li> <p><b>[!UICONTROL Account ID]</b> </p> <p>Immetti l’ID univoco della [!DNL Adobe Acrobat Sign] account associato a questo utente.</p> </li> 
     <li> <p><b>[!UICONTROL Nome]</b> </p> <p>Immettere il nome dell'utente.</p> </li> 
     <li> <p><b>[!UICONTROL Cognome]</b> </p> <p>Immettere il cognome dell'utente</p> </li> 
     <li> <p><b>[!UICONTROL Company]</b> </p> <p>Immetti il nome della società dell’utente.</p> </li> 
     <li> <p><b>[!UICONTROL Initials]</b> </p> <p>Immettere le iniziali dell'utente.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere le impostazioni internazionali dell'utente. Questo determina la lingua dell’interfaccia utente. </p> </li> 
     <li> <p><b>[!UICONTROL Phone]</b> </p> <p>Immettere il numero di telefono dell'utente</p> </li> 
     <li> <p><b>ID gruppo principale</b> </p> <p>Inserisci il gruppo a cui viene aggiunto il nuovo utente. Se non viene inserito nulla, l’utente verrà aggiunto al gruppo predefinito per l’account.</p> </li> 
     <li> <p><b>[!UICONTROL Job title]</b> </p> <p>Immettere il titolo del processo dell'utente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni modulo web]</td> 
   <td> <p>Compila i campi seguenti</p> 
    <ul> 
     <li> <p><b>[!UICONTROL File info]</b> </p> <p>Per ogni file da aggiungere al modulo Web, fare clic su Aggiungi e compilare i campi seguenti:</p> 
      <ul> 
       <li> <p>[!UICONTROL Tipo di file]</p> <p>[!UICONTROL Document]</p> </li> 
       <li> <p>[!UICONTROL Documento transitorio]</p> </li> 
       <li> <p>[!UICONTROL URL file info]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web form name]</b> </p> <p>Immettere un nome per il modulo web. Questo nome viene utilizzato per identificare il modulo web in luoghi come e-mail e siti web.</p> </li> 
     <li> <p><b>[!UICONTROL Stato modulo web]</b> </p> <p>Selezionare lo stato in cui creare il nuovo modulo web.</p> </li> 
     <li> <p><b>[!UICONTROL Informazioni sul set di partecipanti al modulo web]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Informazioni membro]</b> </p> <p>Per ogni membro che si desidera aggiungere al set di partecipanti, fare clic su <b>[!UICONTROL Aggiungi elemento]</b>. </p> 
        <ul> 
         <li> <p><b>E-MAIL [!UICONTROL]</b> </p> <p>Lascia questa opzione vuota.</p> </li> 
         <li> <p><b>[!UICONTROL Security option]</b> </p> <p>Se si desidera aggiungere un'opzione di protezione per l'autenticazione dell'utente, selezionare <b>[!UICONTROL Sì]</b>, quindi seleziona l’opzione di protezione e compila tutti i campi necessari.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Role]</b> </p> <p>Selezionare il ruolo. Tutti i membri del set di partecipanti condividono il ruolo.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Informazioni aggiuntive sui set di partecipanti al modulo web]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Informazioni membro]</b> </p> <p>Per ogni membro che si desidera aggiungere al set di partecipanti, fare clic su <b>[!UICONTROL Aggiungi elemento]</b>.</p> 
        <ul> 
         <li> <p><b>E-MAIL [!UICONTROL]</b> </p> <p>Lascia questa opzione vuota.</p> </li> 
         <li> <p><b>[!UICONTROL Security option]</b> </p> <p>Se si desidera aggiungere un'opzione di protezione per l'autenticazione dell'utente, selezionare <b>[!UICONTROL Sì]</b>, quindi seleziona l’opzione di protezione e compila tutti i campi necessari.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Role]</b> </p> </li> 
       <li> <p><b>ID partecipante al modulo web </b> </p> <p>Immettere l'ID del partecipante al modulo web.</p> </li> 
       <li> <p><b>[!UICONTROL Order]</b> </p> <p>Specificare l'ordine in cui il set di partecipanti deve interagire con il modulo web. Ad esempio, il gruppo di partecipanti che ha un valore di ordine pari a 1 deve andare per primo, 2 deve andare avanti e così via. I numeri d'ordine devono iniziare con uno e non devono presentare spazi vuoti nella serie. </p> </li> 
       <li> <p><b>[!UICONTROL Informazioni sul set di partecipanti al provider]</b> </p> <p>Se il partecipante è sconosciuto, specificare se il provider deve fornire i dettagli del partecipante e inserire un messaggio con i dettagli richiesti per il partecipante sconosciuto.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Informazioni sull'errore di autenticazione]</b> </p> <p>Se desideri fornire una pagina di errore o di errore per gli utenti, seleziona <b>[!UICONTROL Sì]</b>, quindi compila i campi seguenti:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Immetti l’URL della pagina di errore.</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Abilita questa opzione se desideri che la pagina di errore sia visualizzata all’interno del modulo web</p> </li> 
       <li> <p><b>[!UICONTROL Ritardo]</b> </p> <p>Immettere il ritardo, in secondi, prima che l'utente venga reindirizzato alla pagina di errore.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>Per ogni indirizzo e-mail che si desidera ricevere una e-mail al momento della firma dell’accordo finale sul modulo web, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti l’indirizzo e-mail.</p> </li> 
     <li> <p><b>[!UICONTROL Informazioni sul completamento]</b> </p> <p style="font-style: normal;">Se desideri fornire una pagina di successo ai tuoi utenti, seleziona <b>[!UICONTROL Sì]</b>, quindi compila i campi seguenti:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Inserisci l’URL per la pagina di successo</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Abilita questa opzione se desideri che la pagina di successo venga visualizzata all’interno del modulo web</p> </li> 
       <li> <p><b>[!UICONTROL Ritardo]</b> </p> <p>Inserisci il ritardo, in secondi, prima che l’utente venga reindirizzato alla pagina di successo.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Group ID]</b> </p> <p>Immettere l'ID del gruppo a cui appartiene il modulo web. Se non viene immesso nulla, il modulo web appartiene al gruppo principale dell’utente dell’account.</p> </li> 
     <li> <p><b>[!UICONTROL Data ultimo evento]</b> </p> <p>Immettere la data dell'ultimo evento sul modulo web. Usa il formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere le impostazioni internazionali dell'utente. Questo determina la lingua dell’interfaccia utente. </p> </li> 
     <li> <p><b>Opzione [!UICONTROL Security]n</b> </p> <p>Immettere la password utilizzata per proteggere il documento. Devi comunicare questa password separatamente a tutte le parti interessate.</p> </li> 
     <li> <p><b>[!UICONTROL Vaulting info]</b> </p> <p>Se l'account è impostato per l'archiviazione dei documenti e l'opzione per l'abilitazione per contratto, è possibile abilitare questa opzione per l'archiviazione del contratto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare un accordo]**

Questo modulo di azione crea un accordo, lo invia per la firma e restituisce l’ID del contratto.

>[!NOTE]
>
>È consigliabile caricare il documento per firmare come documento transitorio, quindi mapparlo sul [!UICONTROL File da inviare] nel campo [!UICONTROL Creare un accordo] modulo . Per un esempio, consulta &quot;Carica documento&quot; in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File da inviare]</td> 
   <td> <p>Per ogni elemento che si desidera includere nel contratto, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL File Type]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Document]</b> </p> <p>Compila i campi seguenti:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Data di creazione]</b> </p> <p>Immettere o mappare la data di creazione del documento nel formato <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. Ad esempio: <code>2016-02-25T18:46:19Z</code> rappresenta l’ora UTC.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Immettere o mappare l'ID del documento.</p> </li> 
         <li> <p><b>[!UICONTROL Label]</b> </p> <p>Immetti o mappa un’etichetta univoca per il file. In caso di flusso di lavoro personalizzato, questo eseguirà la mappatura di un file all’elemento corrispondente nella definizione del flusso di lavoro. Questo deve essere specificato nel caso di richiesta di creazione di un accordo di flusso di lavoro personalizzato.</p> </li> 
         <li> <p><b>[!UICONTROL Numero di pagine]</b> </p> <p>Immettere o mappare il numero di pagine nel documento.</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Immetti o mappa il tipo di MIME del file originale. I tipi MIME (Multipurpose Internet Mail Extension) sono etichette che consentono al software di identificare diversi tipi di dati condivisi su Internet. I server web e i browser utilizzano il tipo MIME per determinare cosa deve essere fatto con un file. Ad esempio, un file con il tipo MIME <code>text/html</code> verrà elaborato in un browser in modo diverso rispetto a un file con tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere o mappare un nome per il documento.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL ID documento libreria]</b> </p> <p>Immettere l'ID del documento della libreria</p> </li> 
       <li> <p><b>[!UICONTROL ID documento transitorio]</b> </p> <p>Immettere l'ID del documento transitorio</p> </li> 
       <li> <p><b>[!UICONTROL URL trasferimento file]</b> </p> <p>Compila i campi seguenti:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>Immettere il tipo di MIME del file originale. I tipi MIME (Multipurpose Internet Mail Extension) sono etichette che consentono al software di identificare diversi tipi di dati condivisi su Internet. I server web e i browser utilizzano il tipo MIME per determinare cosa deve essere fatto con un file. Ad esempio, un file con il tipo MIME <code>text/html</code> verrà elaborato in un browser in modo diverso rispetto a un file con tipo MIME <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere un nome per il file.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Immetti l’URL del file da inviare.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>Immetti un’etichetta per il file.</p> </li> 
     <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Abilita questa opzione per indicare che il file deve essere notarizzato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement name]</td> 
   <td>Immettere un nome per il nuovo contratto. Questo nome viene utilizzato per identificare il contratto in luoghi come e-mail e siti web.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni sui set di partecipanti]</td> 
   <td> <p>Per ogni set di partecipanti che si desidera aggiungere, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Members]</b> </p> <p>Per ogni persona che si desidera aggiungere al set di partecipanti, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e inserisci l'indirizzo e-mail della persona.</p> </li> 
     <li> <p><b>[!UICONTROL Order]</b> </p> <p>Specifica l'ordine in cui il set di partecipanti deve firmare il contratto. Ad esempio, il gruppo di partecipanti che ha un valore di ordine pari a 1 deve firmare per primo, 2 deve firmare per successivo e così via. I numeri d'ordine devono iniziare con uno e non devono presentare spazi vuoti nella serie. </p> </li> 
     <li> <p><b>[!UICONTROL Role]</b> </p> <p>Selezionare un ruolo per il set di partecipanti. Tutti i partecipanti al set ricevono questo ruolo.</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>Immettere o mappare l'ID del set di partecipanti.</p> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>Immettere o mappare un'etichetta univoca per il set di partecipanti. Per i flussi di lavoro personalizzati, l’etichetta specificata nel set di partecipazione deve essere associata alla fase di partecipazione nel flusso di lavoro personalizzato.</p> </li> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere un nome per il set di partecipanti. Questo nome deve essere univoco all'interno del contratto.</p> </li> 
     <li> <p><b>[!UICONTROL Messaggio privato]</b> </p> <p>Immettere o mappare un messaggio per il set di partecipanti. Tutti i partecipanti al set ricevono questo messaggio.</p> </li> 
     <li> <p><b>[!UICONTROL Pagine visibili]</b> </p> <p>Se per questo contratto è abilitata la visibilità limitata dei documenti, specifica quali file sono visibili a questo set di partecipanti. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Signature type]</td> 
   <td> <p>Selezionare il tipo di firma richiesto dal contratto.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-sign]</b> </p> <p>L'accordo deve essere firmato per via elettronica.</p> </li> 
     <li> <p><b>[!UICONTROL Scritto]</b> </p> <p>L'accordo deve essere firmato a mano e il contratto firmato deve essere analizzato e caricato.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td> <p>Selezionare uno stato per il contratto.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Authoring]</b> </p> <p>È comunque possibile modificare o aggiungere campi al contratto.</p> </li> 
     <li> <p><b>[!UICONTROL Bozza]</b> </p> <p>È possibile creare questo accordo in modo incrementale prima di inviarlo.</p> </li> 
     <li> <p><b>[!UICONTROL In Processo]</b> </p> <p>Questo accordo sarà inviato immediatamente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>Puoi inviare questo accordo alle parti interessate che non devono firmare, come le parti interessate. Essi ricevono un’e-mail all’inizio del processo di firma e un’altra quando viene ricevuta la firma finale. Essi ricevono anche una copia PDF dell'accordo. </p> <p>Per ogni persona che desideri utilizzare per CC su questo accordo, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>E-MAIL [!UICONTROL]</b> </p> <p>Immetti o mappa l'indirizzo e-mail che desideri inserire in CC sul contratto.</p> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>Immetti o mappa un’etichetta per questo indirizzo e-mail, come mostrato nella descrizione del flusso di lavoro</p> </li> 
     <li> <p><b>[!UICONTROL Pagine visibili]</b> </p> </li> 
     <li> <p>Se per questo contratto è abilitata la visibilità limitata dei documenti, specifica quali file sono visibili a questo set di partecipanti. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opzione e-mail]</td> 
   <td> <p>Per ogni tipo di e-mail, seleziona se tale tipo di e-mail viene inviata a tutti i partecipanti o non viene inviata alcuna.</p> 
    <ul> 
     <li> <p><b>E-mail di completamento di [!UICONTROL]</b> </p> <p>Invia un'e-mail quando il contratto viene completato, annullato, scaduto o rifiutato.</p> </li> 
     <li> <p><b>E-mail in volo</b> </p> <p>Invia un'e-mail quando il contratto viene delegato o sostituito.</p> </li> 
     <li> <p><b>E-mail di apertura dell’accordo di [!UICONTROL]</b> </p> <p>Invia un messaggio e-mail quando viene creato il contratto o quando viene richiesta un'azione su di esso.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td> <p>Immetti o mappa un ID per questo contratto. È possibile specificarlo al momento della creazione del contratto e utilizzarlo per individuare il contratto in moduli o query successive.</p> <p>Nota: Il valore External ID è visibile a tutti i partecipanti tramite l’API, quindi non deve essere utilizzato per contenere un token sensibile.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni campo unione]</td> 
   <td> <p>Per ogni campo del contratto per il quale si desidera inserire un valore predefinito, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immettere il valore predefinito e il nome del campo.</p> <p>I valori verranno presentati ai firmatari per i campi modificabili Per i campi di sola lettura i valori forniti non saranno modificabili durante il processo di firma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni notaio]</td> 
   <td> <p>Compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Appuntamento]</b> </p> <p>Immettere o mappare un'ora e una data proposte per l'appuntamento per la notarizzazione del presente contratto.</p> </li> 
     <li> <p><b>[!UICONTROL Note]</b> </p> <p>Inserisci o mappa le note da includere nella sessione notaia.</p> </li> 
     <li> <p><b>[!UICONTROL Payment]</b> </p> <p>Seleziona se il notaio è pagato dal firmatario o dal mittente del contratto.</p> </li> 
     <li> <p><b>[!UICONTROL Tipo di notaio]</b> </p> <p>Selezionare il tipo di notaio</p> 
      <ul> 
       <li> <p>[!UICONTROL Provider noary]</p> <p>Il notaio è fornito dal notaio.</p> </li> 
       <li> <p>[!UICONTROL BYON noary]</p> <p>Il notaio è fornito dal cliente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opzione di firma del post]</td> 
   <td> <p>Seleziona se desideri indirizzare i firmatari a una pagina di successo dopo la firma del contratto. Se si seleziona <b>[!UICONTROL Sì]</b>, compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Ritardo di reindirizzamento]</b> </p> <p>Immettere o mappare un numero che rappresenta il numero di secondi prima che il firmatario venga reindirizzato alla pagina di successo. Se questo valore è maggiore di 0, l'utente vedrà prima lo standard [!DNL Adobe Sign] il messaggio di successo e quindi dopo un ritardo verrà reindirizzato alla pagina di successo.</p> </li> 
     <li> <p><b>[!UICONTROL URL di reindirizzamento]</b> </p> <p>Immettere o mappare un URL accessibile al pubblico a cui verrà inviato l’utente dopo aver completato correttamente il processo di firma.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Security option]</td> 
   <td> <p>Immettere o mappare la password secondaria da utilizzare per proteggere il documento PDF. </p> <p>Importante: [!DNL Adobe Sign] non condividerà mai questa password, quindi devi comunicarla separatamente a tutte le parti interessate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vaulting info]</td> 
   <td>Se l'account è impostato per l'archiviazione dei documenti e l'opzione per l'abilitazione per contratto, è possibile abilitare questa opzione per l'archiviazione del contratto.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creazione di record correlati]**

Questo modulo di azione crea record collegati a un modulo selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record del record originale con cui si desidera associare i record creati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Immettere o mappare l'ID dell'oggetto a cui si desidera associare il record creato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campo relativo al contratto]</td> 
   <td> <p>Selezionare il tipo di campo correlato che si desidera creare</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Campi modulo]</b> </p> <p>Immetti l’ID modello del modello che contiene i campi da creare</p> </li> 
     <li> <p><b>[!UICONTROL Promemoria]</b> </p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Recipient Participent ID]</b> </p> <p>Per ogni partecipante che si desidera ricevere un promemoria, fare clic su [!UICONTROL Aggiungi elemento] e immettere l'ID del partecipante.</p> </li> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Per i nuovi record, lo stato deve essere [!UICONTROL Active].</p> </li> 
       <li> <p><b>[!UICONTROL Ritardo primo promemoria]</b> </p> <p>Immettere il ritardo in ore prima dell'invio del primo promemoria. Il valore minimo consentito è 1 ora e il valore massimo non può essere superiore alla differenza tra la creazione dell'accordo e la scadenza dell'accordo in ore. Se questo ritardo non viene impostato, il primo promemoria verrà basato sulla frequenza.</p> </li> 
       <li> <p><b>[!UICONTROL Frequenza promemoria]</b> </p> <p>Imposta la frequenza con cui desideri inviare il promemoria. Se non viene fornita la frequenza, il promemoria verrà inviato una volta.</p> </li> 
       <li> <p><b>[!UICONTROL Data ultimo invio]</b> </p> <p>Questo campo è impostato dal sistema.</p> </li> 
       <li> <p><b>[!UICONTROL Data di invio successiva]</b> </p> <p>Questo campo deve essere vuoto o impostato su [!UICONTROL ONCE].</p> </li> 
       <li> <p><b>[!UICONTROL Note]</b> </p> <p>Inserire una nota da includere nel promemoria. Questo è utile per spiegare al partecipante perché è richiesta la loro partecipazione.</p> </li> 
       <li> <p><b>[!UICONTROL Avvia contatore promemoria da]</b> </p> <p>Seleziona se il promemoria viene inviato in base a quando il contratto viene creato quando diventa disponibile.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Rapporto sull’identità del firmatario]</b> </p> <p>Immettere la password utilizzata per proteggere il documento PDF.</p> </li> 
     <li> <p><b>[!UICONTROL Visualizzazioni]</b> </p> <p>Inserisci i campi seguenti</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Seleziona il nome della visualizzazione da creare.</p> </li> 
       <li> <p><b>[!UICONTROL Accesso automatico utente]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per accedere automaticamente all'URL restituito.</p> </li> 
       <li> <p><b>[!UICONTROL Frame Parent]</b> </p> <p>Inserisci o mappa un elenco di URL del dominio padre separati da virgole in cui gli URL restituiti possono essere incorniciati. Se lasciato vuoto, il [!DNL Adobe Acrobat Sign] le pagine non sono visualizzabili in iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere la lingua in cui si desidera creare la visualizzazione. </p> </li> 
       <li> <p><b>[!UICONTROL Nessun flag chrome]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per visualizzare la pagina incorporata senza intestazione o piè di pagina di navigazione.</p> </li> 
       <li> <p><b>[!UICONTROL Può modificare i file]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri modificare la sezione di caricamento file aggiungendo o rimuovendo file. Non si tratta di un meccanismo di controllo degli accessi. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>[!UICONTROL Documento libreria]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se si desidera rendere visibili i collegamenti ai documenti di libreria. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>[!UICONTROL File locale]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri che venga visualizzato il pulsante di caricamento file locale. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>[!UICONTROL Connettori web]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se si desidera che vengano visualizzati i collegamenti per allegare documenti da origini Web. Il valore predefinito è Sì.</p> </li> 
       <li> <p><b>[!UICONTROL È selezionata l’anteprima]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per impostare la pagina Componi in modalità Creazione.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>Per ogni membro con cui si desidera condividere il contratto, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e inserire l'indirizzo e-mail del membro e un messaggio a tale membro.</p> </li> 
     <li> <p>[!UICONTROL Delega set di partecipanti]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Participant set ID]</b> </p> <p>Immettere l'ID del set di partecipanti</p> </li> 
       <li> <p><b>[!UICONTROL Informazioni membro]</b> </p> <p>Per ogni membro che si desidera aggiungere, fare clic su [!UICONTROL Aggiungi elemento] e inserire l'indirizzo e-mail e le informazioni telefoniche per il membro.</p> </li> 
       <li> <p><b>[!UICONTROL Messaggio privato]</b> </p> <p>Immetti un messaggio. Tutti i membri del set di partecipanti ricevono questo messaggio.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni sulla vista Libreria]</td> 
   <td> <p>Compila i campi seguenti:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immetti un nome per il modello libreria. Questo nome viene utilizzato nelle e-mail e nei siti web.</p> </li> 
     <li> <p><b>[!UICONTROL Accesso automatico utente]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per accedere automaticamente all'URL restituito.</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Inserisci o mappa un elenco di URL del dominio padre separati da virgole in cui gli URL restituiti possono essere incorniciati. Se lasciato vuoto, il [!DNL Adobe Acrobat Sign] le pagine non sono visualizzabili in iframe.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere la lingua in cui si desidera creare la visualizzazione. </p> </li> 
     <li> <p><b>[!UICONTROL Nessun flag chrome]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per visualizzare la pagina incorporata senza intestazione o piè di pagina di navigazione.</p> </li> 
     <li> <p><b>[!UICONTROL Send view configuration]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri configurare la visualizzazione [!UICONTROL Send] , compila i campi seguenti.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Agreement name]</b> </p> <p>Immettere o mappare il nome del contratto per il documento della libreria nella pagina di composizione.</p> </li> 
       <li> <p><b>[!UICONTROL Può modificare i file]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri modificare la sezione di caricamento file aggiungendo o rimuovendo file. Non si tratta di un meccanismo di controllo degli accessi. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>[!UICONTROL File locale]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se si desidera rendere visibili i collegamenti ai documenti di libreria. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>[!UICONTROL Connettori web]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se si desidera che vengano visualizzati i collegamenti per allegare documenti da origini Web. Il valore predefinito è [!UICONTROL Sì].</p> </li> 
       <li> <p><b>Anteprima selezionata</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per impostare la pagina Componi in modalità Creazione.</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Informazioni sulla visualizzazione utente]</td> 
   <td> <p>Compila i campi seguenti</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Selezionare il nome della visualizzazione utente richiesta.</p> </li> 
     <li> <p><b>[!UICONTROL Accesso automatico utente]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per accedere automaticamente all'utente. Seleziona <b>[!UICONTROL No]</b> per richiedere le credenziali. Il valore predefinito è [!UICONTROL No].</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Inserisci o mappa un elenco di URL del dominio padre separati da virgole in cui gli URL restituiti possono essere incorniciati. Se lasciato vuoto, il [!DNL Adobe Acrobat Sign] le pagine non sono visualizzabili in iframe.</p> </li> 
     <li> <p><b>Nessun flag di chrome</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per visualizzare la pagina incorporata senza intestazione o piè di pagina di navigazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi correlati al widget]</td> 
   <td> <p>Selezionare il record correlato che si desidera creare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Visualizzazioni]</p> <p>Compila i campi seguenti.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Selezionare il nome della visualizzazione modulo Web richiesta</p> </li> 
       <li> <p><b>[!UICONTROL Accesso automatico utente]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per accedere automaticamente all'utente. Seleziona <b>[!UICONTROL No]</b> per richiedere le credenziali. Il valore predefinito è [!UICONTROL No].</p> </li> 
       <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Inserisci o mappa un elenco di URL del dominio padre separati da virgole in cui gli URL restituiti possono essere incorniciati. Se lasciato vuoto, il [!DNL Adobe Acrobat Sign] le pagine non sono visualizzabili in iframe.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere la lingua in cui si desidera creare la visualizzazione. </p> </li> 
       <li> <p><b>[!UICONTROL Nessun flag chrome]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per visualizzare la pagina incorporata senza intestazione o piè di pagina di navigazione.</p> </li> 
       <li> <p>[!UICONTROL Configurazione personalizzata della vista firma]</p> <p>Per configurare una visualizzazione di firma personalizzata, selezionare <b>[!UICONTROL Sì]</b> e compila i campi seguenti:</p> 
        <ul> 
         <li> <p><b>E-MAIL [!UICONTROL]</b> </p> <p>Immettere l'indirizzo e-mail della persona che riceve il modulo web appena creato</p> </li> 
         <li> <p><b>[!UICONTROL Commento]</b> </p> <p>Immetti un commento che descriva come il chiamante API abbia stabilito l’identità del firmatario. Queste informazioni vengono visualizzate nella sezione [!DNL Adobe Acrobat Sign] audit trail.</p> </li> 
         <li> <p><b>[!UICONTROL Scadenza]</b> </p> <p>Immettere una data di scadenza per la personalizzazione del modulo web. </p> <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Riutilizzabile]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> se si desidera che il firmatario designato possa firmare il modulo più di una volta.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>Per ogni membro con cui si desidera condividere il contratto, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e inserire l'indirizzo e-mail del membro e un messaggio a tale membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Chiamata API personalizzata]**
Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>Nota: Per l’elenco degli endpoint disponibili, consulta [!DNL Adobe Sign] Riferimento API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Immetti la stringa di query della richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caricare un documento transitorio]</td> 
   <td> <p>Se si desidera caricare un documento transitorio, immettere il file di origine del documento da caricare.</p> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Elencare record]**

Questo modulo di azione elenca tutti i record del tipo selezionato a cui l&#39;account ha accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record per il quale si desidera recuperare i record correlati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td> <p>Immettere le impostazioni internazionali dell'utente. Questo determina la lingua dell’interfaccia utente. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td>Immetti o mappa l’ID esterno (un ID assegnato al di fuori di [!DNL Adobe Acrobat Sign]) per i contratti che desideri restituire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group ID]</td> 
   <td>Immettere l'ID del gruppo associato ai record che si desidera elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra nascosti (record)]</td> 
   <td>Abilita questa opzione se desideri includere i record nascosti nei risultati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Start index]</td> 
   <td> <p>Immettere il numero del primo record che il modulo deve restituire. </p> <p>Nota: Questo campo viene combinato con il campo [!UICONTROL Numero massimo di record restituiti] per l’impaginazione. Ad esempio, se il [!UICONTROL Numero massimo di eventi restituiti] è 100 e l’ [!UICONTROL Start index] è 101, il modulo restituisce record 101-200 o la seconda pagina di risultati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di record restituiti]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo [action] venga utilizzato durante ogni ciclo di esecuzione di uno scenario.</p> <p>Nota: Questo campo viene combinato con il campo [!UICONTROL Cursor] o [!UICONTROL Start Index] per l’impaginazione. Ad esempio, se il [!UICONTROL Numero massimo di eventi restituiti] è 100 e l’ [!UICONTROL Start index] è 101, il modulo restituisce record 101-200 o la seconda pagina di risultati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL del dominio principale]</td> 
   <td> <p>Inserisci o mappa un elenco di URL del dominio padre separati da virgole in cui gli URL restituiti possono essere incorniciati. Se lasciato vuoto, il [!DNL Adobe Acrobat Sign] le pagine non sono visualizzabili in iframe.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leggi un record]**

Questo modulo di azione recupera le informazioni da un singolo record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record per il quale si desidera recuperare i record correlati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID record]</td> 
   <td>Immettere o mappare l'ID del record che si desidera recuperare.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leggere i record correlati]**

Leggi ulteriori informazioni relative a un singolo record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record per il quale si desidera recuperare i record correlati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record ID] (Esempio: [!UICONTROL Account ID])</td> 
   <td>Immettere o mappare l'ID del record per il quale si desidera recuperare i record correlati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altri campi]</td> 
   <td>Immettere le informazioni in campi specifici in base al tipo di record e ai campi correlati.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Aggiornare un record]**

Questo modulo di azione aggiorna un singolo record in [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* Come best practice, se si prevede di apportare modifiche sostanziali a un accordo, si consiglia di creare un nuovo accordo invece di aggiornarlo.
>* Alcuni aggiornamenti presentano campi obbligatori. Quando configuri l’aggiornamento, assicurati di compilare tutti i campi obbligatori. I campi obbligatori sono in grassetto [!DNL Workfront Fusion] moduli.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID record] </td> 
   <td>Immettere o mappare l'ID del record che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record da aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altri campi]</td> 
   <td> <p>Immettere le informazioni in campi specifici in base al tipo di record e ai campi correlati.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Come best practice, se si prevede di apportare modifiche sostanziali a un accordo, si consiglia di creare un nuovo accordo invece di aggiornarlo.</p> </li> 
     <li> <p><b>[!UICONTROL Documento libreria]</b> </p> <p>Seleziona i campi da aggiornare, quindi compila i campi selezionati:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Selezionare il nuovo stato per il documento della libreria.</p> </li> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere o mappare il nome del modello libreria</p> </li> 
       <li> <p><b>[!UICONTROL Modalità di condivisione]</b> </p> <p>Specifica gli utenti che devono avere accesso al documento della libreria.</p> </li> 
       <li> <p><b>[!UICONTROL Tipo di modello libreria]</b> </p> <p>Per ogni tipo di modello libreria che desideri utilizzare, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e selezionare il tipo di modello.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Utente]</b> </p> <p>Seleziona i campi da aggiornare, quindi compila i campi selezionati:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Nome]</b> </p> <p>Immettere il nome dell'utente.</p> </li> 
       <li> <p><b>[!UICONTROL Cognome]</b> </p> <p>Immettere il cognome dell'utente</p> </li> 
       <li> <p><b>[!UICONTROL Company]</b> </p> <p>Immetti il nome della società dell’utente.</p> </li> 
       <li> <p><b>[!UICONTROL Phone]</b> </p> <p>Immettere il numero di telefono dell'utente</p> </li> 
       <li> <p><b>[!UICONTROL ID gruppo primario]</b> </p> <p>Inserisci il gruppo a cui viene aggiunto il nuovo utente. Se non viene inserito nulla, l’utente verrà aggiunto al gruppo predefinito per l’account.</p> </li> 
       <li> <p><b>[!UICONTROL Job title]</b> </p> <p>Immettere il titolo del processo dell'utente.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL widget])</b> </p> <p>Immettere le informazioni in campi specifici in base al tipo di record e ai campi correlati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Aggiorna record correlato]**

Questo modulo di azione aggiorna i record relativi a un oggetto specifico.

>[!IMPORTANT]
>
>* Come best practice, se si prevede di apportare modifiche sostanziali a un accordo, si consiglia di creare un nuovo accordo invece di aggiornarlo.
>* Alcuni aggiornamenti presentano campi obbligatori. Quando configuri l’aggiornamento, assicurati di compilare tutti i campi obbligatori. I campi obbligatori sono in grassetto [!DNL Workfront Fusion] moduli.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record a cui sono associati i campi correlati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Immettere o mappare l'ID dell'oggetto a cui si desidera associare il record creato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altri campi]</td> 
   <td> <p>Immettere le informazioni in campi specifici in base al tipo di record e ai campi correlati.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Come best practice, se si prevede di apportare modifiche sostanziali a un accordo, si consiglia di creare un nuovo accordo invece di aggiornarlo.</p> </li> 
     <li> <p><b>[!UICONTROL Documento libreria]</b> </p> <p>Seleziona i campi da aggiornare, quindi compila i campi selezionati:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>Selezionare il nuovo stato per il documento della libreria.</p> </li> 
       <li> <p><b>[!UICONTROL Note]</b> </p> <p>Inserisci o mappa il testo della nota.</p> </li> 
       <li> <p><b>[!UICONTROL Visibility]</b> </p> <p>Selezionare se il documento della libreria viene visualizzato o visualizzato.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Utente]</b> </p> <p>Seleziona i campi da aggiornare, quindi compila i campi selezionati:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Elenco informazioni gruppo]</b> </p> <p>Compila i campi seguenti</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Status]</b> </p> <p>Seleziona il nuovo stato per l’utente.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Immetti l’ID univoco del gruppo</p> </li> 
         <li> <p><b>[!UICONTROL È amministratore di gruppo]</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per rendere questo utente un amministratore di gruppo.</p> </li> 
         <li> <p><b>È un gruppo primario</b> </p> <p>Seleziona <b>[!UICONTROL Sì]</b> per aggiornare questo gruppo al gruppo principale dell'utente.</p> </li> 
         <li> <p><b>[!UICONTROL Data di creazione]</b> </p> <p>Immettere la data di creazione del gruppo.</p> <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Digitare la coercizione in Adobe Workfront Fusion</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Immettere o mappare il nome del gruppo.</p> </li> 
         <li> <p><b>[!UICONTROL Creazione documento libreria visibile]</b> </p> <p>Queste impostazioni determinano se l'utente può creare documenti della libreria</p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>Consenti</p> </li> 
           <li> <p>[!UICONTROL Ereditato]</p> <p>Eredita impostazione gruppo da gruppo o account</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Invia limitato ai flussi di lavoro]</b> </p> <p>Queste impostazioni determinano se l'utente può creare accordi solo utilizzando flussi di lavoro.</p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>Consenti</p> </li> 
           <li> <p>[!UICONTROL Ereditato]</p> <p>Eredita impostazione gruppo da gruppo o account</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL L Utente può inviare]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>Consenti</p> </li> 
           <li> <p>[!UICONTROL Ereditato]</p> <p>Eredita impostazione gruppo da gruppo o account</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>Seleziona il nuovo stato per l’utente e inserisci un commento sul motivo per cui desideri attivare o disattivare l’utente.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Immettere le impostazioni internazionali dell'utente. Questo determina la lingua dell’interfaccia utente. </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web form] ([!UICONTROL widget])</b> </p> <p>Immettere le informazioni in campi specifici in base al tipo di record e ai campi correlati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Carica documento]**

Carica un documento transitorio. Un documento transitorio è disponibile per 7 giorni dopo il caricamento.

>[!NOTE]
>
>È consigliabile caricare il documento per firmare come documento transitorio, quindi mapparlo al campo File da inviare nel modulo Crea un accordo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID record]</td> 
   <td>Immettere o mappare l'ID del record che si desidera aggiornare</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td>Immettere il tipo di MIME del file originale. I tipi MIME (Multipurpose Internet Mail Extension) sono etichette che consentono al software di identificare diversi tipi di dati condivisi su Internet. I server web e i browser utilizzano il tipo MIME per determinare cosa deve essere fatto con un file. Ad esempio, un file con il tipo MIME <code>text/html</code> verrà elaborato in un browser in modo diverso rispetto a un file con tipo MIME <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** In questo flusso di lavoro, il documento da firmare (scaricato in precedenza da Workfront) viene caricato come documento transitorio.

![](assets/sign-example-1-350x308.png)

La [!UICONTROL Carica documento] il modulo fornisce al documento un [!DNL Adobe Acrobat Sign] ID a cui è possibile fare riferimento in moduli successivi. Quando il contratto viene creato, l&#39;ID del documento caricato viene incluso nel [!UICONTROL File da inviare] campo .

![](assets/sign-example-2-350x356.png)

+++

### Ricerche

+++ **[!UICONTROL Accordi di ricerca]**

Questo modulo di ricerca cerca gli accordi in base ai criteri forniti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Acrobat Sign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro testo]</td> 
   <td> <p>Cerca testo nei metadati del contratto. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Trova testo]</b> </p> <p>Immetti il testo che desideri trovare nei metadati del contratto. Ogni parola viene trattata come un elemento di testo separato. </p> </li> 
     <li> <p><b>[!UICONTROL Trova testo in]</b> </p> <p>Selezionare i campi di metadati in cui si desidera trovare il testo. Se non si seleziona nulla, i moduli ricercano tutti i metadati.</p> </li> 
    </ul> <p>Il modulo restituisce qualsiasi accordo contenente uno qualsiasi del testo immesso in uno qualsiasi dei campi selezionati. Esempio: l’inserimento di "primavera campagna" e la selezione delle opzioni Titolo e Nota restituiscono eventuali accordi con le parole "primavera" o "Campagna" in Titolo o Nota.</p> <p>Per ulteriori informazioni sulla ricerca di campi in [!DNL Adobe Acrobat Sign], vedere "Come funziona la ricerca di testo in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] Ricerca - Come funziona</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di creazione]</td> 
   <td>Selezionare le date. Il modulo restituisce solo i record in cui la data creata corrisponde a questo criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di scadenza]</td> 
   <td>Selezionare le date. Il modulo restituisce solo i record in cui la data di scadenza corrisponde a questo criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Data di modifica]</p> </td> 
   <td>Selezionare le date. Il modulo restituisce solo i record in cui la data modificata corrisponde a questo criterio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td> <p> L'ID esterno è un ID assegnato al mittente dell'accordo che può essere di qualsiasi forma, ma in genere sotto forma di "&lt;groupid&gt;:&lt;id&gt;".</p> <p>Per ogni ID esterno che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l’ID esterno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group ID]</td> 
   <td> <p>L'ID gruppo è un identificatore assegnato al momento della creazione del gruppo.</p> <p>Per ogni ID esterno che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l’ID esterno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Questo è l'ID assegnato al contratto specifico. </p> <p>Per ogni ID esterno che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l’ID esterno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent ID]</td> 
   <td> <p>Questo è l'ID assegnato all'oggetto principale del contratto. </p> <p>Per ogni ID esterno che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l’ID esterno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-mail del partecipante:</td> 
   <td> <p>Indirizzo e-mail di un partecipante. </p> <p>Per ogni ID esterno che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l’ID esterno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Role]</td> 
   <td>Selezionare i ruoli che si desidera includere nei risultati restituiti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td>Se si desidera che il modulo ordini i risultati, selezionare il campo in base al quale si desidera ordinare i risultati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordinamento [!UICONTROL]r</td> 
   <td>Se si desidera che il modulo ordini i risultati, selezionare se si desidera ordinare in ordine crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Selezionare gli stati da includere nei risultati restituiti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Selezionare i tipi di accordo che si desidera includere nei risultati restituiti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subtypes]</td> 
   <td>Selezionare i sottotipi di contratto che si desidera includere nei risultati restituiti. Solo gli accordi di modelli libreria presentano sottotipi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> <p>L'ID utente dell'utente con cui è condiviso il contratto.</p> <p>Per ogni ID utente che desideri aggiungere, fai clic su <b>[!UICONTROL Aggiungi]</b> e immetti o mappa l'ID utente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Selezionare il livello di visibilità che si desidera includere nei risultati restituiti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start index]</td> 
   <td> <p>Immettere la posizione del primo risultato che si desidera restituire. Combina questo con i [!UICONTROL risultati massimi restituiti] per impaginare i risultati</p> <p>Esempio: se si restituiscono 100 risultati alla volta, immettere 100 per restituire i risultati 100-200.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo [action] venga utilizzato durante ogni ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
