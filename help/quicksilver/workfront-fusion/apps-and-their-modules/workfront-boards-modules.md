---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli delle schede madri Adobe Workfront
description: Puoi utilizzare il connettore per schede madri Adobe Workfront per automatizzare i processi all’interno delle schede Workfront e collegarlo ad app e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
source-git-commit: 074bcf15c61f9c0c75cebf774b15baf7fe383f35
workflow-type: tm+mt
source-wordcount: '2118'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Moduli per schede madri

>[!NOTE]
>
>Questo connettore è attualmente in versione beta.

Le bacheche Adobe Workfront sono strumenti flessibili che consentono la collaborazione in team fornendo l’accesso a una bacheca condivisa contenente colonne e schede.

Puoi utilizzare i moduli Schede Adobe Workfront per leggere o aggiornare i record, effettuare una chiamata API all’API delle schede Workfront o attivare uno scenario quando si verifica un’azione su una scheda.

Per informazioni generali sulle schede madri Workfront, consulta [Panoramica delle schede](/help/quicksilver/agile/boards-overview.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td>
  <td> <p>Qualsiasi</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td>
   <td> <p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: [!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza</td> 
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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).
Moduli delle schede madri Adobe Workfront e relativi campi

## Prerequisiti

È necessario aver configurato una bacheca in Adobe Workfront prima di potersi connettere ad essa.

## Creare una connessione alle schede madri Workfront

>[!NOTE]
>
>È possibile utilizzare una connessione Workfront per connettersi alle schede madri Workfront oppure creare una connessione separata alle schede madri Workfront.

Per creare una connessione alle schede madri Workfront:

1. In qualsiasi [!DNL Adobe Workfront Boards] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

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
            <p>Immettere un nome per la connessione.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Seleziona se ti connetti a un ambiente di produzione o non di produzione.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Seleziona se ti interessa la connessione a un account di servizio o a un account personale.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID client]<p>(Facoltativo)</p></td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL ID client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segreto client]<p>(Facoltativo)</p></td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL Segreto Client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL autenticazione]<p>(Facoltativo)</p></td>
          <td>Immetti l’URL che verrà utilizzato dall’istanza di Workfront per autenticare questa connessione. <p>Il valore predefinito è <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Prefisso host]</td>
          <td>Immetti il prefisso host.<p>Il valore predefinito è <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## Moduli delle schede madri Adobe Workfront e relativi campi

Quando si configurano i moduli delle schede madri Workfront, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, possono essere visualizzati campi aggiuntivi per le Schede Workfront, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Schede](#cards)
* [Bacheche](#boards)
* [Colonne](#columns)
* [Tag](#tags)
* [Altro](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### Schede

* [Aggiungi voce elenco di controllo](#add-checklist-item)
* [Aggiungi sottoattività](#add-subtask)
* [Creare una scheda](#create-a-card)
* [Spostare una scheda](#move-a-card)
* [Leggi una scheda](#read-a-card)
* [Aggiornare una scheda](#update-a-card)

#### Aggiungi voce elenco di controllo

Questo modulo di azione aggiunge una voce dell’elenco di controllo alla scheda specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Inserisci o mappa l’ID della carta a cui desideri aggiungere una voce all’elenco di controllo.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL elementi dell'elenco di controllo]</td> 
   <td>Per ogni voce dell'elenco di controllo che si desidera aggiungere, fare clic su Aggiungi voce, immettere il nome della voce dell'elenco di controllo e selezionare se la voce è stata completata.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Aggiungi sottoattività

Questo modulo di azione aggiunge una sottoattività a una scheda in Bacheche. La scheda deve essere collegata. L’attività secondaria viene aggiunta anche all’attività Workfront rappresentata dalla scheda.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda padre]</td> 
   <td>Inserisci o mappa l’ID della scheda a cui desideri aggiungere una sottoattività.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca contenente la scheda a cui desideri aggiungere un’attività secondaria.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Immettere o associare un nome per la nuova sottoattività.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Creare una scheda

Questo modulo di azione crea una nuova scheda su una scheda Workfront.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca a cui desideri aggiungere una scheda.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column ID]</td> 
   <td>Immettere o mappare l'ID della colonna a cui si desidera aggiungere una sottoattività.<p>Puoi trovare l’ID tag nelle informazioni restituite dal modulo Read a board.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Immettere o mappare un nome per la nuova scheda.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Spostare una scheda

Questo modulo di azione sposta una scheda in una colonna diversa sulla stessa bacheca.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Inserisci o mappa l’ID della carta da spostare.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca che contiene la scheda da spostare.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID colonna di destinazione]</td> 
   <td>Inserisci o mappa l’ID della colonna in cui desideri spostare la scheda.<p>Puoi trovare l’ID tag nelle informazioni restituite dal modulo Read a board.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A indice]</td> 
   <td>Immetti o mappa la posizione della scheda nella nuova colonna.<p>La posizione superiore nella colonna nell'indice 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Leggi una scheda

Questo modulo di azione recupera informazioni su una scheda specifica.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Inserisci o mappa l’ID della carta da leggere.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Aggiornare una scheda

Questo modulo di azione aggiorna le informazioni relative a una scheda specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Immetti o mappa l’ID della carta da aggiornare.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca che contiene la scheda da aggiornare.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Immetti o mappa un nuovo nome per la scheda.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Inserisci o mappa una nuova descrizione per la scheda/\.</p></td> 
  </tr> 
 </tbody> 
</table>

### Bacheche

* [Creare una bacheca](#create-a-board)
* [Leggi una bacheca](#read-a-board)

#### Creare una bacheca

Questo modulo di azione crea una scheda in Workfront. Puoi specificare il tipo di bacheca da creare.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bacheca]</td> 
   <td>Inserisci o mappa un nome per la nuova bacheca.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td>Seleziona il tipo di bacheca da creare.</td> 
  </tr> 
 </tbody> 
</table>

#### Leggi una bacheca

Questo modulo di azione restituisce informazioni su una singola bacheca, ad esempio schede, colonne, tag e membri della bacheca.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Immetti o mappa l’ID della bacheca per la quale desideri recuperare informazioni.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

### Colonne

#### Creare una colonna

Questo modulo di azione crea una nuova colonna sulla bacheca specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca a cui desideri aggiungere una colonna.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome colonna]</td> 
   <td>Immettere o mappare un nome per la nuova colonna.</td> 
  </tr> 
 </tbody> 
</table>

### Tag

* [Aggiungere un tag a una scheda](#add-card-tag)
* [Creare un tag](#create-a-tag)

#### Aggiungere un tag a una scheda

Questo modulo di azione aggiunge un tag a una scheda.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID scheda]</td> 
   <td>Inserisci o mappa l’ID della scheda a cui desideri aggiungere un tag.<p>Puoi trovare l’ID della scheda nell’URL quando la visualizzi in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca contenente la scheda a cui desideri aggiungere un tag.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID tag]</td> 
   <td>Inserisci o mappa l’ID del tag da aggiungere.<p>Puoi trovare l’ID tag nelle informazioni restituite dal modulo Read a board.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Creare un tag

Questo modulo di azione crea un nuovo tag e gli assegna un colore.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bacheca]</td> 
   <td>Inserisci o mappa l’ID della bacheca per cui desideri creare un tag.<p>Puoi trovare l’ID della bacheca nell’URL quando visualizzi la bacheca in Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag name]</td> 
   <td>Immetti o mappa il nome del nuovo tag.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag Color]</td> 
   <td>Seleziona il colore per questo tag.</td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### Effettuare una chiamata API personalizzata

Questo modulo di azione effettua una chiamata personalizzata all’API delle schede madri Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
      <td> <p>È possibile utilizzare una connessione Workfront esistente per connettersi alle schede madri Workfront oppure una connessione specifica alle schede madri Workfront. </p><p>Per istruzioni sulla connessione [!DNL Workfront] app a [!DNL Workfront Fusion], vedi <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creare una connessione alle schede madri Workfront</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Inserisci un percorso relativo a<code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p><p>Per la maggior parte delle chiamate alle bacheche il metodo è POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Determina il tipo di contenuto della richiesta.</p> <p>Ad esempio:<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Per le bacheche Workfront, in genere questa sezione viene lasciata vuota.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di Graphql incorporato JSON </p> <p>Esempio:</p><p>In questo esempio viene aggiornato il nome di una colonna. È possibile includere <code>boardId</code> e <code>columnId</code> come GUID hardcoded o mappati da un modulo precedente.<p><pre>{

  &quot;query&quot;: &quot;mutazione { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>se</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
