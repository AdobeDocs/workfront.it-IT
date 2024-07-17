---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Adobe Workfront Planning
description: Con i  [!DNL Adobe Workfront Planning] moduli, puoi avviare uno  [!DNL Adobe Workfront Fusion] scenario basato sugli eventi nel tuo [!DNL Adobe] account Workfront Planning, creare, leggere o aggiornare contratti e altri record, cercare i record utilizzando i criteri impostati e caricare i documenti.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: e067c5ff34c31060ca6fd392289d845f53a5ef3a
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] moduli

Con i moduli [!DNL Adobe Workfront Planning] è possibile attivare uno scenario quando si verificano eventi in Workfront Planning. È inoltre possibile creare, leggere, aggiornare ed eliminare record oppure eseguire una chiamata API personalizzata all&#39;account [!DNL Adobe Workfront Planning].

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
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

## Crea una connessione a [!DNL Adobe Workfront Planning]

Puoi creare una connessione al tuo account [!DNL Workfront Planning] direttamente da un modulo [!DNL Workfront Fusion].

1. In qualsiasi modulo app [!DNL Workfront Planning], fai clic su **[!UICONTROL Aggiungi]** accanto alla casella [!UICONTROL Connessione].
1. Immettere un nome per la connessione.
1. Seleziona se desideri connetterti a un ambiente di produzione o non di produzione.
1. Specificare se ci si connette a un account di servizio o a un account personale.
1. Fai clic su **[!UICONTROL Accesso SAML]** per creare la connessione e tornare al modulo.

## [!DNL Adobe Workfront Planning] moduli e relativi campi

### Guarda gli eventi

Questo modulo di attivazione avvia uno scenario quando un record, un tipo di record o un&#39;area di lavoro viene creata, aggiornata o eliminata in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Selezionare il webhook che si desidera utilizzare o fare clic su Aggiungi per crearne uno nuovo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di oggetto]</td>
      <td>Specificare se si desidera controllare record, tipi di record o aree di lavoro.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>È possibile impostare i filtri per controllare solo i record che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo che desideri che il filtro valuti, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND.</p> <p>Nota: non è possibile modificare i filtri nei webhook [!DNL Workfront] esistenti. Per impostare filtri diversi per le sottoscrizioni di eventi [!DNL Workfront], rimuovere il webhook corrente e crearne uno nuovo.</p> <p>Per ulteriori informazioni sui filtri eventi, vedere <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtri di sottoscrizione eventi nei moduli [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> nell'articolo Moduli di Workfront.</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL Oggetti da controllare]</td>
      <td>Seleziona se desideri controllare le nuove. record aggiornati, nuovi e aggiornati o eliminati.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Escludi aggiornamenti effettuati da questa connessione]</p>
      </td>
      <td>Abilita questa opzione per impedire che lo scenario venga attivato quando viene apportata una modifica dalla connessione utilizzata da questo modulo. Questo impedisce l’attivazione di un’altra istanza dello scenario se questo esegue un’azione di attivazione.</td> 
      </tr>
  </tbody>
</table>

### Eliminare un tipo di record

Questo modulo di azione elimina un singolo tipo di record in Workfront Planning dal relativo ID.

>[!WARNING]
>
>L&#39;eliminazione di un tipo di record in Workfront Planning comporta anche l&#39;eliminazione di tutti i record nella tabella dei tipi di record.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID tipo di record]</p>
      </td>
      <td>Immetti o mappa l’ID del campo da eliminare.</td> 
      </tr>
  </tbody>
</table>

### Effettuare una chiamata API personalizzata

Questo modulo effettua una chiamata API personalizzata all&#39;API [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Immetti un percorso relativo a https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL versione API]</p>
      </td>
      <td>
        <p>Seleziona la versione API da utilizzare. Se non selezioni una versione, per impostazione predefinita verrà utilizzata la versione più recente.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Immetti un percorso relativo a https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stringa Di Query]  </td>
      <td>
        <p>Per ogni coppia chiave/valore che si desidera aggiungere alla stringa di query, fare clic su <b>Aggiungi elemento</b> e immettere la chiave e il valore.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Creare un record

Questa azione consente di creare un singolo record in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID tipo di record]</p>
      </td>
      <td>Immettere o mappare il tipo di record che si desidera creare. I tipi di record disponibili sono basati sull'account Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Altri campi</p>
      </td>
      <td>Questi campi si basano sul tipo di record selezionato.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Eliminare un record

Questo modulo di azione elimina il record specificato in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID record]</p>
      </td>
      <td>Immettere o mappare l'ID del record che si desidera eliminare.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Ottieni un record

Questo modulo azioni recupera un singolo record da [!DNL Adobe Workfront Planning], specificato dal relativo ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID record]</td>
      <td>Immettere o mappare l'ID del record che si desidera recuperare.</td>
    </tr>
  </tbody>
</table>

### Ottieni record per tipo di record

Questo modulo di azione recupera tutti i record del tipo specificato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Selezionare o mappare l'area di lavoro contenente i record da recuperare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di record]</td>
      <td>Selezionare il tipo di record da recuperare.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Numero massimo di record restituiti]</p>
      </td>
      <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tbody>
</table>

### Recupera tipi di record

Questo modulo di azione recupera un elenco di tipi di record in un account [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
  </tbody>
</table>

### Aggiorna record

Questa azione aggiorna un singolo record in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Workfront Planning], vedere <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Creare una connessione a [!DNL Adobe Workfront Planning]</a> in questo articolo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID record]</p>
      </td>
      <td>Immettere o mappare il tipo di record che si desidera aggiornare. I tipi di record disponibili sono basati sull'account Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Altri campi</p>
      </td>
      <td>Questi campi si basano sul tipo di record selezionato.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Cerca record

Questo modulo di azione recupera un elenco di record in base ai criteri specificati.

>[!NOTE]
>
>Questo modulo è in costruzione.
