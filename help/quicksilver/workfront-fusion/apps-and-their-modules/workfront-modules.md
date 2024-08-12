---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Workfront
description: Puoi utilizzare il connettore Adobe Workfront Fusion Adobe Workfront per automatizzare i processi all’interno di Workfront. Se disponi di una licenza di Workfront Fusion for Work Automation and Integration, puoi utilizzarla anche per connettersi ad app e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 7c00ea85b4a03346cdb39c937a1cef970d409ef0
workflow-type: tm+mt
source-wordcount: '6280'
ht-degree: 2%

---

# [!DNL Adobe Workfront] moduli

È possibile utilizzare il connettore [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] per automatizzare i processi in [!DNL Workfront]. Se disponi di una licenza [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione del lavoro e l&#39;integrazione], puoi utilizzarla anche per connettersi ad app e servizi di terze parti.

Il connettore [!DNL Workfront] non viene conteggiato rispetto al numero di app attive disponibili per l&#39;organizzazione. Tutti gli scenari, anche se utilizzano solo l&#39;app [!DNL Workfront], vengono conteggiati rispetto al numero totale di scenari dell&#39;organizzazione.

Per ulteriori informazioni sulle app e sugli scenari disponibili per la tua organizzazione, consulta [Organizzazioni](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organizzazioni e team](../../workfront-fusion/organizations/organizations-and-teams.md).

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connetti [!DNL Workfront] a [!DNL Workfront Fusion]

Il connettore [!DNL Workfront] utilizza OAuth 2.0 per connettersi a [!DNL Workfront].

Puoi creare una connessione al tuo account [!DNL Workfront] direttamente da un modulo [!DNL Workfront Fusion].

1. In qualsiasi modulo di Adobe Workfront, fai clic su **Aggiungi** accanto al campo Connessione.
1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nome connessione]</td>
        <td>
          <p>Immettere un nome per la nuova connessione.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Seleziona se ti connetti a un ambiente di produzione o non di produzione.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo di connessione]</td>
        <td>
          <p>Specificare se ci si connette a un account di servizio o a un account personale.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti l'ID client [!DNL Workfront]. È disponibile nell’area Applicazioni OAuth2 dell’area Configura di Workfront. Apri l’applicazione specifica a cui ti stai connettendo per visualizzare l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti l'ID client [!DNL Workfront]. È disponibile nell’area Applicazioni OAuth2 dell’area Configura di Workfront. Apri l’applicazione specifica a cui ti stai connettendo per visualizzare l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL autenticazione]</td>
        <td>Questo può rimanere il valore predefinito, oppure puoi immettere l'URL dell'istanza Workfront, seguito da <code>/integrations/oauth2</code>. <p>Esempio: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Prefisso host]</td>
        <td>Nella maggior parte dei casi, questo valore deve essere <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Se non viene visualizzato un pulsante di accesso SAML, significa che l&#39;organizzazione non ha attivato il Single Sign-On (SSO). Puoi accedere con il tuo nome utente e la tua password.
>   
>   Per ulteriori informazioni sull&#39;SSO, vedere [Panoramica del Single Sign-On in [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* Le connessioni OAuth 2.0 all&#39;API [!DNL Workfront] non si basano più sulle chiavi API.

## [!DNL Workfront] moduli e relativi campi

Quando configuri [!DNL Workfront] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Workfront], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>* Se non trovi i campi più aggiornati in un modulo Workfront, potrebbe trattarsi di un problema di caching. Attendi un’ora e riprova.
>* I codici di stato HTTP 429 di Adobe Workfront non dovrebbero causare disattivazioni, ma attivare invece una breve pausa di esecuzione nello scenario.

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Guarda gli eventi]**

Questo modulo trigger esegue uno scenario in tempo reale quando in Workfront vengono aggiunti, aggiornati o eliminati oggetti di un tipo specifico

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

1. Fai clic su **[!UICONTROL Aggiungi]** a destra della casella **Webhook**.

1. Configura il webhook nella casella **[!UICONTROL Aggiungi un hook]** visualizzato.

   Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome webhook]</td> 
      <td>(Facoltativo) Digita un nuovo nome per il webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo di record]</td> 
      <td>Selezionare il tipo di record [!DNL Workfront] che si desidera controllare nel modulo.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Seleziona se desideri controllare lo stato precedente o quello nuovo.<ul><li><p><b>[!UICONTROL Nuovo stato]</b></p><p>Attiva uno scenario quando il record cambia <b>in</b> un valore specificato.</p><p>Ad esempio, se lo stato è impostato su [!UICONTROL Nuovo stato] e il filtro è impostato su [!UICONTROL Stato] [!UICONTROL È uguale a] [!UICONTROL In corso], il webhook attiva uno scenario quando lo stato [!UICONTROL Stato] diventa [!UICONTROL In corso], indipendentemente dallo stato precedente. </p></li><li><p><b>[!UICONTROL Old State]</b></p><p>Attiva uno scenario quando il record cambia <b> da</b> a un determinato valore.</p><p>Ad esempio, se lo stato è impostato su [!UICONTROL Old State] e il filtro è impostato su [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In corso], il webhook attiva uno scenario quando uno stato [!UICONTROL Status] attualmente [!UICONTROL In corso] passa a un altro stato. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>È possibile impostare i filtri per controllare solo i record che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo che desideri che il filtro valuti, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND.</p> <p>Nota: non è possibile modificare i filtri nei webhook [!DNL Workfront] esistenti. Per impostare filtri diversi per le sottoscrizioni di eventi [!DNL Workfront], rimuovere il webhook corrente e crearne uno nuovo.</p> <p>Per ulteriori informazioni sui filtri eventi, vedere <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtri di sottoscrizione eventi nei moduli [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> in questo articolo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Escludi eventi creati da questa connessione</td> 
      <td>Abilita questa opzione per escludere gli eventi creati o aggiornati utilizzando lo stesso connettore utilizzato dal modulo di attivazione. Questo può evitare situazioni in cui uno scenario potrebbe attivarsi da solo, causandone la ripetizione in un ciclo infinito.<p><b>NOTA</b>Il tipo di record Assegnazione non include questa opzione.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origine record]</td> 
      <td> <p>Scegliere se si desidera che lo scenario controlli <strong>[!UICONTROL Solo nuovi record]</strong>, <strong>[!UICONTROL Solo record aggiornati]</strong>, <strong>[!UICONTROL Record nuovi e aggiornati]</strong> o <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Nota: se si sceglie <strong>[!UICONTROL Record nuovi e aggiornati]</strong>, la creazione del webhook crea 2 sottoscrizioni di eventi (per lo stesso indirizzo del webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Dopo la creazione del webhook, puoi visualizzare l’indirizzo dell’endpoint a cui vengono inviati gli eventi.

Per ulteriori informazioni, vedere la sezione [Esempi di payload evento](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) nell&#39;articolo della Guida [!DNL Workfront] [API sottoscrizione evento](../../wf-api/general/event-subs-api.md).

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Campo di controllo]**

Questo modulo trigger esegue uno scenario quando viene aggiornato un campo specificato. Il modulo restituisce sia il vecchio che il nuovo valore del campo specificato. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] che si desidera controllare nel modulo.</p> <p>Selezionare ad esempio [!UICONTROL Attività] se si desidera avviare l'esecuzione dello scenario ogni volta che viene aggiornato un campo record in un'attività.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Seleziona il campo che desideri che il modulo controlli per gli aggiornamenti. Questi campi riflettono i campi configurati dall'amministratore [!DNL Workfront] per il tracciamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Output]</td> 
   <td>Seleziona le informazioni da includere nel bundle di output per questo modulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Osserva record]**

Questo modulo trigger esegue uno scenario quando vengono aggiunti, aggiornati o entrambi gli oggetti di un tipo specifico. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario. Nell’output, il modulo indica se ogni record è nuovo o aggiornato.

I record aggiunti e aggiornati nel periodo di tempo specificato vengono restituiti come nuovi record.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Scegliere se si desidera che lo scenario controlli <strong>[!UICONTROL Solo nuovi record]</strong>, <strong>[!UICONTROL Solo record aggiornati]</strong> o <strong>[!UICONTROL Record nuovi e aggiornati]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>(Visualizza dopo aver scelto un <strong>filtro</strong>.) Selezionare il tipo di record [!DNL Workfront] che si desidera controllare nel modulo.</p> <p>Ad esempio, se si desidera avviare lo scenario ogni volta che viene creato un nuovo progetto, selezionare [!UICONTROL Progetto]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro facoltativo]</td> 
   <td> <p>(Avanzata) Digita una stringa di codice API per definire eventuali parametri o codice aggiuntivi che definiranno meglio i criteri. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++


### Azioni

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Converti oggetto]**

Questo modulo di azione effettua una delle seguenti conversioni:

* Converti problema in progetto
* Converti problema in attività
* Converti attività in progetto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo di oggetto]</td> 
   <td> <p>Selezionare il tipo di oggetto da convertire. Questo è il tipo di oggetto prima della conversione.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Converti in]</td> 
   <td>Selezionare l'oggetto in cui si desidera convertirlo. Questo è il tipo di oggetto dopo la conversione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;ID Oggetto&gt;]</td> 
   <td> <p>Immettere l'ID dell'oggetto. </p> <p>Nota: quando si immette l'ID di un oggetto, è possibile iniziare a digitare il nome dell'oggetto, quindi selezionarlo dall'elenco. Il modulo immette quindi l’ID appropriato nel campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID modello [!UICONTROL]</td> 
   <td> <p>Per la conversione in progetto, seleziona l’ID modello da utilizzare per il progetto.</p> <p>Nota: quando si immette l'ID di un oggetto, è possibile iniziare a digitare il nome dell'oggetto, quindi selezionarlo dall'elenco. Il modulo immette quindi l’ID appropriato nel campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Moduli personalizzati]</td> 
   <td>Seleziona i moduli personalizzati da aggiungere all’oggetto appena convertito, quindi immetti i valori per i campi del modulo personalizzato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>Abilitare le opzioni desiderate durante la conversione dell'oggetto. Sono disponibili opzioni a seconda dell’oggetto da o verso il quale si sta eseguendo la conversione.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copia campi nativi]</td> 
   <td> <p>Abilita questa opzione per copiare tutti i campi nativi dall’oggetto originale al nuovo oggetto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copia moduli personalizzati]</td> 
   <td> <p>Abilita questa opzione per copiare tutti i campi nativi dall’oggetto originale al nuovo oggetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crea un record (allegando moduli personalizzati)]**

Questo modulo di azione crea un oggetto, ad esempio un progetto, un&#39;attività o un problema in [!DNL Workfront], e consente di aggiungere un modulo personalizzato al nuovo oggetto. Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

È possibile utilizzare questo modulo, ad esempio, per creare un&#39;attività in [!DNL Workfront] quando un client aggiunge una nuova riga in un elenco [!DNL Google Sheets] di attività da eseguire.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Assicurati di fornire il numero minimo di campi di input. Ad esempio, se desideri creare un problema, devi fornire un ID progetto principale valido nel campo ID progetto per indicare dove il problema dovrebbe risiedere in Workfront. Puoi utilizzare il pannello di mappatura per mappare queste informazioni da un altro modulo dello scenario, oppure puoi immetterle manualmente digitando il nome e selezionandolo dall’elenco.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] che si desidera venga creato dal modulo.</p> <p>Ad esempio, se desideri creare un progetto, seleziona [!UICONTROL Progetto] dall’elenco a discesa, quindi accertati di avere accesso ai dati (dei moduli precedenti nello scenario) che popoleranno il progetto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</p> <p>Per i campi nei moduli personalizzati, utilizza il campo <b>[!UICONTROL Allega modulo personalizzato]</b>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Allega Modulo Personalizzato]</td> 
   <td>Selezionare i moduli personalizzati da aggiungere al nuovo oggetto, quindi immettere i valori per tali campi.</td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando immetti il testo per un campo personalizzato o un oggetto [!UICONTROL Note] (Commento o risposta), puoi utilizzare i tag HTML nel campo [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, vedere [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Crea record]**

Questo modulo di azione crea un oggetto, ad esempio un progetto, un’attività o un problema in Workfront. Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

È possibile utilizzare questo modulo, ad esempio, per creare un&#39;attività in [!DNL Workfront] quando un client aggiunge una nuova riga in un elenco di attività di Google Sheets.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Assicurati di fornire il numero minimo di campi di input. Ad esempio, se desideri creare un problema, devi fornire un ID progetto principale valido nel campo ID progetto per indicare dove il problema dovrebbe risiedere in Workfront. Puoi utilizzare il pannello di mappatura per mappare queste informazioni da un altro modulo dello scenario, oppure puoi immetterle manualmente digitando il nome e selezionandolo dall’elenco.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] che si desidera venga creato dal modulo.</p> <p>Ad esempio, se desideri creare un progetto, seleziona [!UICONTROL Progetto] dall’elenco a discesa, quindi accertati di avere accesso ai dati (dei moduli precedenti nello scenario) che popoleranno il progetto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando immetti il testo per un campo personalizzato o un oggetto [!UICONTROL Note] (Commento o risposta), puoi utilizzare i tag HTML nel campo [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, vedere [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Chiamata API personalizzata]**

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata all&#39;API [!DNL Workfront]. In questo modo è possibile creare un&#39;automazione del flusso di dati che non può essere eseguita dagli altri moduli [!DNL Workfront].

Il modulo restituisce le seguenti informazioni:

* **[!UICONTROL Codice di stato]** (numero): indica il completamento o l&#39;errore della richiesta HTTP. Si tratta di codici standard che puoi cercare su Internet.
* **[!UICONTROL Intestazioni]** (oggetto): contesto più dettagliato per il codice di risposta/stato che non è correlato al corpo dell&#39;output. Non tutte le intestazioni visualizzate in un’intestazione di risposta sono intestazioni di risposta, quindi alcune potrebbero non essere utili.

  Le intestazioni di risposta dipendono dalla richiesta HTTP scelta durante la configurazione del modulo.

* **[!UICONTROL Corpo]** (oggetto): a seconda della richiesta HTTP scelta durante la configurazione del modulo, è possibile che alcuni dati vengano restituiti. Tali dati, ad esempio i dati di una richiesta GET, sono contenuti in questo oggetto.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Immettere un percorso relativo a <code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL versione API]</td> 
   <td>Selezionare la versione dell'API [!DNL Workfront] che si desidera venga utilizzata dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Determina il tipo di contenuto della richiesta.</p> <p>Ad esempio:<code> {"Content-type":"application/json"}</code></p> <p>Nota: se ricevi errori ed è difficile determinarne l'origine, puoi modificare le intestazioni in base alla documentazione di [!DNL Workfront]. Se la chiamata API personalizzata restituisce un errore di richiesta HTTP 422, provare a utilizzare un'intestazione <code>"Content-Type":"text/plain"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> <p>Suggerimento: è consigliabile inviare informazioni tramite il corpo JSON anziché come parametri di query.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Elimina record]**

Questo modulo di azione elimina un oggetto, ad esempio un progetto, un’attività o un problema in Workfront.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forza eliminazione]</td> 
   <td>Abilita questa opzione per garantire che il record venga eliminato, anche se l'interfaccia utente [!DNL Workfront] richiede la conferma dell'eliminazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Immettere l'ID [!DNL Workfront] univoco del record che si desidera eliminare dal modulo.</p> <p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record [!DNL Workfront] da eliminare dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Per evitare che i record vengano eliminati a causa di operazioni asincrone, è consigliabile effettuare la configurazione dello scenario seguente.
>
>1. Eliminare il record in modo sincrono.
>1. Aggiungi la gestione degli errori al modulo Elimina record per ignorare l’errore causato dal timeout di 40 secondi.


+++

+++ **[!UICONTROL Scarica documento]**

Questo modulo di azione scarica un documento da Workfront.

Specifica l’ID del record.

Il modulo restituisce il contenuto, il nome, l&#39;estensione e la dimensione del file del documento. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID documento]</td> 
   <td> <p>Mappare o immettere manualmente l'ID [!DNL Workfront] univoco del documento che si desidera scaricare dal modulo.</p> <p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Azione Varia]**

Questo modulo di azione consente di eseguire azioni sull’API.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] con cui si desidera interagire il modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Selezionare l'azione che si desidera venga eseguita dal modulo.</p> <p>Potrebbe essere necessario compilare ulteriori campi, a seconda del tipo di record [!UICONTROL] e dell'azione [!UICONTROL] scelti. Alcune combinazioni di queste due impostazioni possono richiedere solo un ID record, mentre altre (come Project per il tipo di record <strong>[!UICONTROL]</strong> e [!UICONTROL Allega modello] per l'azione <strong>[!UICONTROL]</strong>) richiedono informazioni aggiuntive (ad esempio un ID oggetto e un ID modello).</p> <p>Per informazioni dettagliate sui singoli campi, consulta la <a href="http://developer.workfront.com/">documentazione per gli sviluppatori di Workfront</a>. <p><strong>Nota</strong>: il sito della documentazione per gli sviluppatori include informazioni solo tramite la versione 14 dell'API, ma contiene comunque informazioni importanti per le chiamate API. </p> 
    <ol> 
     <li value="1"> <p>Selezionare il tipo di record dalla barra di navigazione a sinistra nella pagina della documentazione per gli sviluppatori [!DNL Workfront]. I seguenti tipi hanno pagine proprie:</p> 
      <ul> 
       <li> <p>[!UICONTROL Progetti]</p> </li> 
       <li> <p>[!UICONTROL Attività]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Utenti]</p> </li> 
       <li> <p>[!UICONTROL Documenti]</p> </li> 
      </ul> <p>Per tutti gli altri tipi di record, selezionare <b>[!UICONTROL Altri oggetti ed endpoint]</b> e individuare il tipo di record nelle pagine ordinate alfabeticamente.</p> </li> 
     <li value="2"> <p>Nella pagina del tipo di record appropriato, cercare l'azione (Ctrl+F o Comando+F).</p> </li> 
     <li value="3"> <p>Visualizza le descrizioni dei campi disponibili nell'azione selezionata.</p> </li> 
    </ol> <p>Nota:  <p>Durante la creazione di una bozza tramite il modulo [!DNL Workfront] [!UICONTROL Misc Action], è consigliabile creare una bozza senza opzioni avanzate, quindi aggiornare la bozza utilizzando l'API SOAP [!DNL Workfront Proof].</p> <p>Per ulteriori informazioni sulla creazione di una bozza con l'API [!DNL Workfront] (utilizzata da questo modulo), vedere <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Aggiungere opzioni di bozza avanzate durante la creazione di una bozza tramite l'API [!DNL Adobe Workfront]</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID [!DNL Workfront] univoco del record con cui si desidera interagire con il modulo.<p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Leggi un record]**

Questo modulo di azione recupera i dati da un singolo record.

Specifica l’ID del record. È inoltre possibile specificare quali record correlati si desidera che vengano letti dal modulo.

Ad esempio, se il record che il modulo sta leggendo è un progetto, è possibile specificare che si desidera che le attività del progetto vengano lette.

Il modulo restituisce un array di dati dai campi standard per l’output specificato.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo di record]</td>

<td>Scegliere il tipo di oggetto [!DNL Workfront] che si desidera venga letto dal modulo.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Output]</td>

<td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Riferimenti]</td>
   <td>Selezionare i campi di riferimento da includere nell'output.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Raccolte]</td>
   <td>Selezionare i campi di riferimento da includere nell'output.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Immettere l'ID [!DNL Workfront] univoco del record che si desidera venga letto dal modulo.</p> <p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Aggiorna record]**

Questo modulo di azione aggiorna un oggetto, ad esempio un progetto, un’attività o un problema. Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo.

Specifica l’ID del record.

Il modulo restituisce l’ID dell’oggetto ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Immettere l'ID [!DNL Workfront] univoco del record che si desidera aggiornare nel modulo.</p> <p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] da aggiornare nel modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando immetti il testo per un campo personalizzato o un oggetto [!UICONTROL Note] (Commento o risposta), puoi utilizzare i tag HTML nel campo [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, vedere [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Carica documento]**

Questo modulo di azione carica un documento in un oggetto [!DNL Workfront], ad esempio un progetto, un&#39;attività o un problema.

È possibile specificare la posizione del documento, il file da caricare e un nuovo nome facoltativo per il file.

Il modulo restituisce l’ID del documento e dei campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID record correlato]</td> 
   <td>Immettere l'ID [!DNL Workfront] univoco del record in cui si desidera caricare il documento.</td> 
  </tr> 
  <tr> 
   <td>Tipo di record correlato a [!UICONTROL]</td> 
   <td>Selezionare il tipo di record [!DNL Workfront] in cui si desidera che il modulo carichi il documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Ricerche

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Leggi record correlati]**

Questo modulo di ricerca legge i record corrispondenti alla query di ricerca specificata, in un particolare oggetto padre.

È possibile specificare quali campi includere nell&#39;output. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record padre (oggetto Workfront) di cui si desidera leggere i record associati.</p> <p>Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo nei tipi di oggetto <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] disponibili per ogni modulo [!DNL Workfront]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID record padre]</td> 
   <td> <p>Immettere o mappare l'ID del record padre di cui si desidera leggere i record associati.</p> <p>Per ottenere l'ID, apri l'oggetto [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Raccolte]</td> 
   <td>Selezionare o mappare il tipo di record figlio che si desidera leggere nel modulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ricerca]**

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Workfront] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] da cercare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Selezionare un'opzione per specificare se si desidera che il modulo ottenga il primo risultato corrispondente ai criteri di ricerca o tutti i risultati corrispondenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL max]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campi criteri di ricerca]</td> 
   <td> <p>Selezionare i campi da utilizzare per i criteri di ricerca. Questi campi saranno quindi disponibili nel menu a discesa Criteri di ricerca.</p></td> 
  </tr> 
  <tr> 
   <td>Criteri di ricerca di [!UICONTROL]</td> 
   <td> <p>Immettere il campo in base al quale si desidera eseguire la ricerca, l'operatore che si desidera utilizzare nella query e il valore ricercato nel campo.</p> <p>Nota: non utilizzare <code>username </code> nei criteri di ricerca. L'inclusione di <code>username </code> in una query API per [!DNL Workfront] comporta l'accesso dell'utente a Workfront e la ricerca non avrà esito positivo.</p> <p>Nota: <code>In</code> e <code>NotIn</code> funzionano con gli array. Gli input devono essere in formato array.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Riferimenti]</td> 
   <td>Selezionare i campi di riferimento da includere nella ricerca.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Raccolte]</td> 
   <td>Seleziona le raccolte che desideri aggiungere alla ricerca.</td> 
  </tr> 
 </tbody> 
</table>
+++

+++ **[!UICONTROL Ricerca (legacy)]**

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Workfront] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'app [!DNL Workfront] a [!DNL Workfront Fusion], vedere <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record [!DNL Workfront] da cercare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Selezionare un'opzione per specificare se si desidera che il modulo ottenga il primo risultato corrispondente ai criteri di ricerca o tutti i risultati corrispondenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL max]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>Criteri di ricerca di [!UICONTROL]</td> 
   <td> <p>Immettere il campo in base al quale si desidera eseguire la ricerca, l'operatore che si desidera utilizzare nella query e il valore ricercato nel campo.</p> <p>Nota: non utilizzare <code>username </code> nei criteri di ricerca. L'inclusione di <code>username </code> in una query API per [!DNL Workfront] comporta l'accesso dell'utente a Workfront e la ricerca non avrà esito positivo.</p> <p>Nota: <code>In</code> e <code>NotIn</code> funzionano con gli array. Gli input devono essere in formato array.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Riferimenti]</td> 
   <td>Selezionare i campi di riferimento da includere nella ricerca.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Raccolte]</td> 
   <td>Seleziona le raccolte che desideri aggiungere alla ricerca.</td> 
  </tr> 
 </tbody> 
</table>

Visualizzare un elenco dei tipi di oggetto [!DNL Workfront] per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipi di oggetto disponibili per ogni modulo [!DNL Workfront]

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipi di oggetto disponibili per ogni modulo trigger [!DNL Workfront]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Osserva Record]</th> 
   <th>[!UICONTROL Watch Field]</th> 
   <th>[!UICONTROL Osserva Eventi]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo di approvazione</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Assegnazione</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Linea di base</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Fatturazione </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tariffa di fatturazione</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Azienda</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Cartella documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Richiesta documento</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Versione documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Spesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo di spesa</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ora</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo di ora</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iterazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Voce del diario</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Percorso milestone</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tag nota</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utente Progetto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approvazione bozza</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tempo riservato* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporto</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Rischio</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo Rischio</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approvatore passaggio</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modello</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Attività modello</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Scheda orario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aggiorna</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipi di oggetto disponibili per ogni modulo azione [!DNL Workfront]**

>[!NOTE]
>
>Il modulo [!UICONTROL Scarica documento] non è incluso in questa tabella perché i tipi di oggetto [!DNL Workfront] non fanno parte della relativa configurazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Crea record]</th> 
   <th>[!UICONTROL Aggiorna un record]</th> 
   <th>[!UICONTROL Elimina record]</th> 
   <th>[!UICONTROL Carica documento]</th> 
   <th>[!UICONTROL Leggi un record]</th> 
   <th>Chiamata API personalizzata [!UICONTROL]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo di approvazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Assegnazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Linea di base</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>Fatturazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tariffa di fatturazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Azienda</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Cartella documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versione documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tasso di cambio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Spesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo di spesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documento esterno</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gruppo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo di ora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iterazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Voce del diario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Percorso milestone</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tag nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utente Progetto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo riservato* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rischio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo Rischio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approvatore passaggio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modello</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività modello</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Scheda orario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aggiorna</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipi di oggetto disponibili per ogni modulo di ricerca [!DNL Workfront]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL - Ricerca]</th> 
   <th>[!UICONTROL Leggi record correlati]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo di approvazione</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Assegnazione</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Fatturazione</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tariffa di fatturazione</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Azienda</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Cartella documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versione documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Spesa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo di spesa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo di ora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iterazione</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Voce del diario</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Percorso milestone</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tag nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utente Progetto</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo riservato* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rischio</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo Rischio</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approvatore passaggio</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modello</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Attività modello</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Scheda orario</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delega utente</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Si consiglia di verificare che questo funzioni come previsto.

+++

## Filtri di sottoscrizione eventi nei moduli [!DNL Workfront] > [!UICONTROL Osserva eventi]

>[!NOTE]
>
>Si consiglia vivamente di utilizzare i filtri di abbonamento agli eventi nei moduli [!UICONTROL Osserva eventi].

Il modulo [!DNL Workfront] [!UICONTROL Osserva eventi] attiva scenari basati su un webhook che crea una sottoscrizione evento nell&#39;API [!DNL Workfront]. L’abbonamento a un evento è un set di dati che determina quali eventi vengono inviati al webhook. Ad esempio, se imposti un modulo [!UICONTROL Osserva eventi] che sta monitorando la presenza di problemi, l&#39;abbonamento all&#39;evento invia solo gli eventi correlati ai problemi.

Utilizzando i filtri di abbonamento agli eventi, gli utenti di Fusion possono creare sottoscrizioni agli eventi più adatte ai loro casi d’uso. Ad esempio, è possibile impostare una sottoscrizione evento nell&#39;API [!DNL Workfront] per inviare al webhook solo i problemi che si trovano in un progetto specifico, assicurandosi che il modulo [!UICONTROL Osserva eventi] venga attivato solo per i problemi del progetto. La possibilità di creare trigger più piccoli migliora la progettazione dello scenario riducendo il numero di trigger irrilevanti.

Questa operazione è diversa dalla configurazione di un filtro nello scenario [!DNL Workfront Fusion]. Senza un filtro di abbonamento agli eventi, il webhook riceve tutti gli eventi relativi al tipo di oggetto selezionato. La maggior parte di questi eventi sarebbe irrilevante per lo scenario e deve essere filtrata prima che lo scenario possa continuare.

Nel filtro Workfront > Osserva eventi sono disponibili i seguenti operatori:

* Uguale a
* Non è uguale a
* Maggiore di
* Minore di
* Maggiore o uguale a
* Minore o uguale a
* Contiene
* Esiste
   * Questo operatore non richiede un valore e il campo del valore è assente.
* Non esiste
   * Questo operatore non richiede un valore e il campo del valore è assente.
* Cambiato
   * Questo operatore non richiede un valore e il campo del valore è assente.
   * Questo operatore ignora il campo Stato.
   * Quando utilizzi `Changed`, seleziona **Solo eventi aggiornati** nel campo **Origine record**.

>[!IMPORTANT]
>
>Impossibile modificare i filtri nei webhook [!DNL Workfront] esistenti. Per impostare filtri diversi per le sottoscrizioni di eventi [!DNL Workfront], rimuovere il webhook corrente e crearne uno nuovo.

>[!INFO]
>
>**Esempio:** considera uno scenario che elabora nuovi problemi assegnati a un utente specifico, Ana.
>
>### Filtrare gli eventi utilizzando un filtro di abbonamento agli eventi (scelta consigliata)
>
>Utilizzando il filtro eventi, puoi impostare il webhook per attivare lo scenario quando un problema viene assegnato ad Ana al momento della creazione. Ana ha l’ID utente b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Se vengono creati 100 problemi in un giorno, ma solo due di essi sono assegnati ad Ana, lo scenario verrebbe eseguito due volte.
>
>### Filtra gli eventi all’interno dello scenario (scelta non consigliata)
>
>Per filtrare gli eventi in modo che vengano elaborati solo i problemi assegnati ad Ana, puoi creare un filtro dopo il modulo [!UICONTROL Osserva eventi].
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Se vengono creati 100 problemi in un giorno, ma solo due di essi sono assegnati ad Ana, lo scenario verrebbe eseguito 100 volte. 98 esecuzioni si fermerebbero al filtro, ma il modulo trigger consuma ancora dati ed esegue operazioni in tutte le esecuzioni.

Per ulteriori informazioni sulle sottoscrizioni di eventi, vedere [Domande frequenti - Sottoscrizioni eventi](../../wf-api/general/event-subs-faq.md).

Per ulteriori informazioni sui webhook, vedere [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Per ulteriori informazioni sui filtri negli scenari, vedere [Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

