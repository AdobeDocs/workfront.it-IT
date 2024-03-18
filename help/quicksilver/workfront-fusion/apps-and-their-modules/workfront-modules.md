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
source-git-commit: 5110370fd934ac53e48d5993604d541c73ffdadf
workflow-type: tm+mt
source-wordcount: '5945'
ht-degree: 2%

---

# [!DNL Adobe Workfront] moduli

È possibile utilizzare [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] per automatizzare i processi in [!DNL Workfront]. Se si dispone di [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione e l&#39;integrazione del lavoro] , puoi utilizzarla anche per connettersi ad app e servizi di terze parti.

Il [!DNL Workfront] il connettore non viene conteggiato rispetto al numero di app attive disponibili per l’organizzazione. Tutti gli scenari, anche se utilizzano solo [!DNL Workfront] app, conteggio rispetto al conteggio totale degli scenari della tua organizzazione.

Per ulteriori informazioni sulle app e sugli scenari disponibili per la tua organizzazione, consulta [Organismi](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organizzazioni e team](../../workfront-fusion/organizations/organizations-and-teams.md).

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connetti [!DNL Workfront] a [!DNL Workfront Fusion]

Il [!DNL Workfront] Il connettore utilizza OAuth 2.0 per connettersi a [!DNL Workfront].

Puoi creare una connessione al tuo [!DNL Workfront] account direttamente dall&#39;interno di un [!DNL Workfront Fusion] modulo.

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
        <td>Immetti il [!DNL Workfront] ID client. È disponibile nell’area Applicazioni OAuth2 dell’area Configura di Workfront. Apri l’applicazione specifica a cui ti stai connettendo per visualizzare l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il [!DNL Workfront] ID client. È disponibile nell’area Applicazioni OAuth2 dell’area Configura di Workfront. Apri l’applicazione specifica a cui ti stai connettendo per visualizzare l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL autenticazione]</td>
        <td>Questo può rimanere il valore predefinito, oppure puoi immettere l’URL dell’istanza Workfront, seguito da <code>/integrations/oauth2</code>. <p>Esempio: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Prefisso host]</td>
        <td>Nella maggior parte dei casi, questo valore deve essere <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Se non viene visualizzato un pulsante di accesso SAML, significa che l&#39;organizzazione non ha attivato il Single Sign-On (SSO). Puoi accedere con il tuo nome utente e la tua password.
>   
>   Per ulteriori informazioni sull&#39;SSO, vedere [Panoramica del Single Sign-On [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* Connessioni OAuth 2.0 al [!DNL Workfront] Le API non si basano più sulle chiavi API.

## [!DNL Workfront] moduli e relativi campi

Quando si configura [!DNL Workfront] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Workfront] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Se non trovi i campi più aggiornati in un modulo Workfront, potrebbe trattarsi di un problema di caching. Attendi un’ora e riprova.

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
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

1. Clic **[!UICONTROL Aggiungi]** a destra del **Webhook** casella.

1. Configurare il webhook in **[!UICONTROL Aggiungi un hook]** che viene visualizzata.

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
      <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo di record]</td> 
      <td>Seleziona il tipo di [!DNL Workfront] registrare che si desidera che il modulo controlli.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Seleziona se desideri controllare lo stato precedente o quello nuovo.<ul><li><p><b>[!UICONTROL Nuovo stato]</b></p><p>Attiva uno scenario quando il record cambia <b>a</b> un determinato valore.</p><p>Ad esempio, se lo stato è impostato su [!UICONTROL Nuovo stato] e il filtro è impostato su [!UICONTROL Stato] [!UICONTROL È uguale a] [!UICONTROL In corso], il webhook attiva uno scenario quando lo stato [!UICONTROL Stato] diventa [!UICONTROL In corso], indipendentemente dallo stato precedente. </p></li><li><p><b>[!UICONTROL Old State]</b></p><p>Attiva uno scenario quando il record cambia <b>da</b> un determinato valore.</p><p>Ad esempio, se lo stato è impostato su [!UICONTROL Old State] e il filtro è impostato su [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In corso], il webhook attiva uno scenario quando uno stato [!UICONTROL Status] attualmente [!UICONTROL In corso] passa a un altro stato. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>È possibile impostare i filtri per controllare solo i record che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo che desideri che il filtro valuti, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND.</p> <p>Nota: non è possibile modificare i filtri esistenti [!DNL Workfront] webhook. Per impostare filtri diversi per [!DNL Workfront] sottoscrizioni di eventi, rimuovi il webhook corrente e creane uno nuovo.</p> <p>Per ulteriori informazioni sui filtri evento, consulta <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtri di abbonamento agli eventi in [!DNL Workfront] &gt; Moduli [!UICONTROL Watch Events]</a> in questo articolo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Escludi eventi creati da questa connessione</td> 
      <td>Abilita questa opzione per escludere gli eventi creati o aggiornati utilizzando lo stesso connettore utilizzato dal modulo di attivazione. Questo può evitare situazioni in cui uno scenario potrebbe attivarsi da solo, causandone la ripetizione in un ciclo infinito.<p><b>NOTA</b>Il tipo di record Assegnazione non include questa opzione.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origine record]</td> 
      <td> <p>Scegli se desideri che lo scenario sia visibile <strong>[!UICONTROL Solo Nuovi Record]</strong>, <strong>[!UICONTROL Aggiornato Solo Record]</strong>, <strong>[!UICONTROL Record nuovi e aggiornati]</strong>, o <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Nota: se si sceglie <strong>[!UICONTROL Record nuovi e aggiornati]</strong>, la creazione del webhook crea 2 abbonamenti evento (per lo stesso indirizzo del webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Dopo la creazione del webhook, puoi visualizzare l’indirizzo dell’endpoint a cui vengono inviati gli eventi.

Per ulteriori informazioni, consulta la sezione [Esempi di payload di eventi](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) nel [!DNL Workfront] Articolo della Guida [API di abbonamento agli eventi](../../wf-api/general/event-subs-api.md).

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] registrare che si desidera che il modulo controlli.</p> <p>Selezionare ad esempio [!UICONTROL Attività] se si desidera avviare l'esecuzione dello scenario ogni volta che viene aggiornato un campo record in un'attività.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Seleziona il campo che desideri che il modulo controlli per gli aggiornamenti. Questi campi riflettono i campi [!DNL Workfront] l'amministratore ha configurato per il tracciamento.</td> 
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

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Record di controllo]**

Questo modulo trigger esegue uno scenario quando vengono aggiunti, aggiornati o entrambi gli oggetti di un tipo specifico. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario. Nell’output, il modulo indica se ogni record è nuovo o aggiornato.

I record aggiunti e aggiornati nel periodo di tempo specificato vengono restituiti come nuovi record.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Scegli se desideri che lo scenario sia visibile <strong>[!UICONTROL Solo Nuovi Record]</strong>, <strong>[!UICONTROL Aggiornato Solo Record]</strong>, o <strong>[!UICONTROL Record nuovi e aggiornati]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>(Viene visualizzato dopo aver scelto un <strong>Filtro</strong>.) Seleziona il tipo di [!DNL Workfront] registrare che si desidera che il modulo controlli.</p> <p>Ad esempio, se si desidera avviare lo scenario ogni volta che viene creato un nuovo progetto, selezionare [!UICONTROL Progetto]</p> </td> 
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

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
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
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
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
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare un record (allegare moduli personalizzati)]**

Questo modulo di azione crea un oggetto, ad esempio un progetto, un’attività o un problema in [!DNL Workfront]e consente di aggiungere un modulo personalizzato al nuovo oggetto. Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Ad esempio, puoi utilizzare questo modulo per creare un’attività in [!DNL Workfront] quando un client aggiunge una nuova riga in una [!DNL Google Sheets] elenco delle attività da eseguire.

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] che si desidera creare nel modulo.</p> <p>Ad esempio, se desideri creare un progetto, seleziona [!UICONTROL Progetto] dall’elenco a discesa, quindi accertati di avere accesso ai dati (dei moduli precedenti nello scenario) che popoleranno il progetto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</p> <p>Per i campi nei moduli personalizzati, utilizza <b>[!UICONTROL Allega Modulo Personalizzato]</b> campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Allega Modulo Personalizzato]</td> 
   <td>Selezionare i moduli personalizzati da aggiungere al nuovo oggetto, quindi immettere i valori per tali campi.</td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando si immette il testo per un campo personalizzato o un [!UICONTROL Nota] (Commento o risposta), è possibile utilizzare i tag HTML nella [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, consulta [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Crea record]**

Questo modulo di azione crea un oggetto, ad esempio un progetto, un’attività o un problema in Workfront. Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Ad esempio, puoi utilizzare questo modulo per creare un’attività in [!DNL Workfront] quando un client aggiunge una nuova riga in un elenco di attività di Google Sheets che devono essere eseguite.

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] che si desidera creare nel modulo.</p> <p>Ad esempio, se desideri creare un progetto, seleziona [!UICONTROL Progetto] dall’elenco a discesa, quindi accertati di avere accesso ai dati (dei moduli precedenti nello scenario) che popoleranno il progetto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando si immette il testo per un campo personalizzato o un [!UICONTROL Nota] (Commento o risposta), è possibile utilizzare i tag HTML nella [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, consulta [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Chiamata API personalizzata]**

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Workfront] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Workfront] moduli.

Il modulo restituisce le seguenti informazioni:

* **[!UICONTROL Codice di stato]** (numero): indica l’esito positivo o negativo della richiesta HTTP. Si tratta di codici standard che puoi cercare su Internet.
* **[!UICONTROL Intestazioni]** (oggetto): contesto più dettagliato per il codice di risposta/stato che non è correlato al corpo di output. Non tutte le intestazioni visualizzate in un’intestazione di risposta sono intestazioni di risposta, quindi alcune potrebbero non essere utili.

  Le intestazioni di risposta dipendono dalla richiesta HTTP scelta durante la configurazione del modulo.

* **[!UICONTROL Corpo]** (oggetto): a seconda della richiesta HTTP scelta durante la configurazione del modulo, alcuni dati potrebbero essere restituiti. Tali dati, ad esempio i dati di una richiesta GET, sono contenuti in questo oggetto.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Inserisci un percorso relativo a<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL versione API]</td> 
   <td>Seleziona la versione di [!DNL Workfront] API che desideri che il modulo utilizzi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Determina il tipo di contenuto della richiesta.</p> <p>Ad esempio:<code> {"Content-type":"application/json"}</code></p> <p>Nota: se ricevi errori ed è difficile determinarne l’origine, puoi modificare le intestazioni in base al [!DNL Workfront] documentazione. Se la chiamata API personalizzata restituisce un errore di richiesta HTTP 422, prova a utilizzare un <code>"Content-Type":"text/plain"</code> intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> <p>Suggerimento: è consigliabile inviare informazioni tramite il corpo JSON anziché come parametri di query.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forza eliminazione]</td> 
   <td>Abilita questa opzione per garantire che il record venga eliminato, anche se [!DNL Workfront] L’interfaccia utente richiede la conferma dell’eliminazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Immetti l’univoco [!DNL Workfront] ID del record che desideri eliminare dal modulo.</p> <p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL Workfront] che si desidera eliminare dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID documento]</td> 
   <td> <p>Mappa o immetti manualmente il codice univoco [!DNL Workfront] ID del documento che desideri scaricare dal modulo.</p> <p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Azione Varie]**

Questo modulo di azione consente di eseguire azioni sull’API.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] che si desidera che il modulo interagisca con.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Selezionare l'azione che si desidera venga eseguita dal modulo.</p> <p>Potrebbe essere necessario compilare ulteriori campi, a seconda del tipo di record [!UICONTROL] e dell'azione [!UICONTROL] scelti. Alcune combinazioni di queste due impostazioni possono richiedere solo un ID record, mentre altre (come Project per <strong>[!UICONTROL Tipo di record]</strong> e [!UICONTROL Allega modello] per <strong>[!UICONTROL Action]</strong>) richiedono informazioni aggiuntive (ad esempio un ID oggetto e un ID modello).</p> <p>Per informazioni dettagliate sui singoli campi, vedere <a href="http://developer.workfront.com/">Documentazione per sviluppatori Workfront</a>. <p><strong>Nota</strong>: il sito della documentazione per sviluppatori include informazioni solo tramite la versione 14 dell’API, ma contiene ancora informazioni importanti per le chiamate API. </p> 
    <ol> 
     <li value="1"> <p>Selezionare il tipo di record dalla barra di navigazione a sinistra nella [!DNL Workfront] pagina della documentazione per gli sviluppatori. I seguenti tipi hanno pagine proprie:</p> 
      <ul> 
       <li> <p>[!UICONTROL Progetti]</p> </li> 
       <li> <p>[!UICONTROL Attività]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Utenti]</p> </li> 
       <li> <p>[!UICONTROL Documenti]</p> </li> 
      </ul> <p>Per tutti gli altri tipi di record, selezionare <b>[!UICONTROL Altri oggetti ed endpoint]</b>e individuare il tipo di record nelle pagine ordinate alfabeticamente.</p> </li> 
     <li value="2"> <p>Nella pagina del tipo di record appropriato, cercare l'azione (Ctrl+F o Comando+F).</p> </li> 
     <li value="3"> <p>Visualizza le descrizioni dei campi disponibili nell'azione selezionata.</p> </li> 
    </ol> <p>Nota:  <p>Durante la creazione di una bozza tramite il [!DNL Workfront] Nel modulo [!UICONTROL Misc Action], la procedura consigliata consiste nel creare una bozza senza opzioni avanzate, quindi aggiornarla utilizzando [!DNL Workfront Proof] API SOAP.</p> <p>Per ulteriori informazioni sulla creazione di una bozza con [!DNL Workfront] API (utilizzata da questo modulo), consulta <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Aggiungi opzioni di verifica avanzate durante la creazione di una bozza tramite [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL Workfront] ID del record con cui vuoi che il modulo interagisca.<p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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

<td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo di record]</td>

<td>Scegli la [!DNL Workfront] tipo di oggetto che si desidera venga letto dal modulo.</td> 
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
   <td> <p>Immetti l’univoco [!DNL Workfront] ID del record che desideri che il modulo legga.</p> <p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Immetti l’univoco [!DNL Workfront] ID del record che desideri aggiornare nel modulo.</p> <p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] che desideri aggiornare il modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selezionare i campi che si desidera rendere disponibili per l'immissione dei dati. Questo consente di utilizzare questi campi senza dover scorrere quelli non necessari.</td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Quando si immette l&#39;ID di un oggetto, è possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo dall&#39;elenco. Il modulo immette quindi l’ID appropriato nel campo.
>* Quando si immette il testo per un campo personalizzato o un [!UICONTROL Nota] (Commento o risposta), è possibile utilizzare i tag HTML nella [!UICONTROL Testo nota] per creare testo RTF, ad esempio testo in grassetto o corsivo.
>
>  Per ulteriori informazioni sul testo RTF negli aggiornamenti, consulta [Aggiungere un aggiornamento a un elemento di lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Carica documento]**

Questo modulo di azione carica un documento in un [!DNL Workfront] oggetto, ad esempio un progetto, un’attività o un problema.

È possibile specificare la posizione del documento, il file da caricare e un nuovo nome facoltativo per il file.

Il modulo restituisce l’ID del documento e dei campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID record correlato]</td> 
   <td>Immetti l’univoco [!DNL Workfront] ID del record in cui desideri caricare il documento.</td> 
  </tr> 
  <tr> 
   <td>Tipo di record correlato a [!UICONTROL]</td> 
   <td>Seleziona il tipo di [!DNL Workfront] registra dove desideri che il modulo carichi il documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record padre (oggetto Workfront) di cui si desidera leggere i record associati.</p> <p>Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo</a> in questo articolo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID record padre]</td> 
   <td> <p>Immettere o mappare l'ID del record padre di cui si desidera leggere i record associati.</p> <p>Per ottenere l’ID, apri la [!DNL Workfront] nel browser e copia il testo alla fine dell'URL dopo "ID=". Ad esempio: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Workfront] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Workfront] record che si desidera cercare nel modulo.</p> </td> 
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
   <td> <p>Immettere il campo in base al quale si desidera eseguire la ricerca, l'operatore che si desidera utilizzare nella query e il valore ricercato nel campo.</p> <p>Nota: non usi <code>username </code>nei criteri di ricerca. Inclusione <code>username </code>in una query API a [!DNL Workfront] accede a Workfront e la ricerca non avrà esito positivo.</p> <p>Nota: <code>In</code> e <code>NotIn</code>utilizzare gli array. Gli input devono essere in formato array.</p></td> 
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

Consulta l’elenco dei [!DNL Workfront] tipi di oggetto per i quali è possibile utilizzare questo modulo in [[!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipi di oggetto disponibili per ogni [!DNL Workfront] modulo

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipi di oggetto disponibili per ogni [!DNL Workfront] modulo trigger**

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
   <td>Tipo di Spesa</td> 
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

+++**Tipi di oggetto disponibili per ogni [!DNL Workfront] modulo azione**

>[!NOTE]
>
>Il [!UICONTROL Scarica documento] modulo non è incluso in questa tabella perché [!DNL Workfront] i tipi di oggetto non fanno parte della relativa configurazione.

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
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
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
   <td>Tipo di Spesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td>✓</td> 
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

+++**Tipi di oggetto disponibili per ogni [!DNL Workfront] modulo di ricerca**

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
   <td>Tipo di Spesa</td> 
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

## Filtri di abbonamento agli eventi in [!DNL Workfront] > [!UICONTROL Guarda gli eventi] moduli

>[!NOTE]
>
>Si consiglia vivamente di utilizzare i filtri di abbonamento agli eventi nel [!UICONTROL Guarda gli eventi] moduli.

Il [!DNL Workfront] [!UICONTROL Guarda gli eventi] Il modulo attiva scenari basati su un webhook che crea un abbonamento evento nel [!DNL Workfront] API. L’abbonamento a un evento è un set di dati che determina quali eventi vengono inviati al webhook. Ad esempio, se imposti un [!UICONTROL Guarda gli eventi] modulo che sta monitorando la presenza di problemi, l’abbonamento all’evento invia solo gli eventi relativi ai problemi.

Utilizzando i filtri di abbonamento agli eventi, gli utenti di Fusion possono creare sottoscrizioni agli eventi più adatte ai loro casi d’uso. Ad esempio, puoi impostare una sottoscrizione di evento nel [!DNL Workfront] API per inviare al webhook solo i problemi presenti in un progetto specifico, assicurando che [!UICONTROL Guarda gli eventi] Il modulo verrà attivato solo per i problemi di quel progetto. La possibilità di creare trigger più piccoli migliora la progettazione dello scenario riducendo il numero di trigger irrilevanti.

Questa operazione è diversa dalla configurazione di un filtro in [!DNL Workfront Fusion] scenario. Senza un filtro di abbonamento agli eventi, il webhook riceve tutti gli eventi relativi al tipo di oggetto selezionato. La maggior parte di questi eventi sarebbe irrilevante per lo scenario e deve essere filtrata prima che lo scenario possa continuare.

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
   * Quando si utilizza `Changed`, seleziona **Solo eventi aggiornati** nel **Origine record** campo.

>[!IMPORTANT]
>
>Non è possibile modificare i filtri esistenti [!DNL Workfront] webhook. Per impostare filtri diversi per [!DNL Workfront] sottoscrizioni di eventi, rimuovi il webhook corrente e creane uno nuovo.

>[!INFO]
>
>**Esempio:** Considera uno scenario che elabora i nuovi problemi assegnati a un utente specifico, Ana.
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
>Per filtrare gli eventi in modo che vengano elaborati solo i problemi assegnati ad Ana, puoi creare un filtro dopo [!UICONTROL Guarda gli eventi] modulo.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Se vengono creati 100 problemi in un giorno, ma solo due di essi sono assegnati ad Ana, lo scenario verrebbe eseguito 100 volte. 98 esecuzioni si fermerebbero al filtro, ma il modulo trigger consuma ancora dati ed esegue operazioni in tutte le esecuzioni.

Per ulteriori informazioni sugli abbonamenti agli eventi, consulta [Domande frequenti - Abbonamenti agli eventi](../../wf-api/general/event-subs-faq.md).

Per ulteriori informazioni sui webhook, consulta [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Per ulteriori informazioni sui filtri negli scenari, consulta [Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

