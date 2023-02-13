---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Figma
description: Con la [!DNL Adobe Workfront Fusion] Moduli Figma, è possibile recuperare elenchi di commenti, file, versioni di file o progetti. Puoi anche pubblicare un commento o effettuare una chiamata all’API Figma.
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] Moduli

Con la [!DNL Adobe Workfront Fusion] [!DNL Figma] è possibile recuperare elenchi di commenti, file, versioni di file o progetti. Puoi anche pubblicare un commento o effettuare una chiamata al [!DNL Figma] API.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
      <td>
        <p>[!UICONTROL Pro] o superiore</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Prodotto</td>
      <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td>
    </tr>
  </tbody>
</table>


Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Figma] moduli, è necessario disporre di un [!DNL Figma] conto.

## [!DNL Figma] moduli e relativi campi

Quando si configura [!DNL Figma] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Figma] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Commenti](#comments)

* [Progetti e file](#projects-and-files)

* [Componenti e stili](#components-and-styles)

* [Altro](#other)


### Commenti

* [Eliminare un commento](#delete-a-comment)

* [Elencare commenti](#list-comments)

* [Pubblica un commento](#post-a-comment)


#### [!UICONTROL Eliminare un commento]

Questo modulo di azione elimina un singolo commento da un file.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Immettere o mappare l'ID file del file da cui si desidera aggiungere l'eliminazione di un commento. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Commento]</td>
      <td>Inserisci il testo del commento da eliminare.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare commenti]

Questo modulo di ricerca elenca tutti i commenti allegati a un singolo file in [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Immettere o mappare l'ID file del file per il quale si desidera recuperare i commenti. </p>
        <ul>
          <li>
            <p>Se non conosci l'ID, fai clic su <b>[!UICONTROL Trova file]</b> e immetti o mappa l’ID del progetto a cui è associato il file, quindi seleziona il file .</p>
          </li>
          <li>
            <p>Se non conosci l’ID del progetto, fai clic su <b>[!UICONTROL Trova progetti]</b> e immetti o mappa l’ID del team a cui è associato il progetto, quindi seleziona il progetto e il file.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di commenti che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Pubblica un commento]

Questo modulo di azione pubblica un commento in un file Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Immettere o mappare l'ID file del file a cui si desidera inviare un commento. </p>
        <ul>
          <li>
            <p>Se non conosci l’ID del file, fai clic su <b>[!UICONTROL Trova file]</b> e immetti o mappa l’ID del progetto a cui è associato il file, quindi seleziona il file .</p>
          </li>
          <li>
            <p>Se cerchi di trovare l’ID del file e non conosci l’ID del progetto, fai clic su <b>[!UICONTROL Trova progetti]</b> e immetti o mappa l’ID del team a cui appartiene il progetto a cui è associato il file. Seleziona il progetto, quindi seleziona il file .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Commento]</td>
      <td>Inserisci il testo del commento.</td>
    </tr>
  </tbody>
</table>


### Progetti e file

* [Ottenere un file o un&#39;immagine](#get-a-file-or-image)

* [Cronologia delle versioni del file di elenco](#list-file-version-history)

* [Elencare file di progetto](#list-project-files)

* [Elencare progetti](#list-projects)


#### [!UICONTROL Ottenere un file o un&#39;immagine]

Questo modulo di azione recupera un singolo file o immagine da una libreria Figma

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di oggetto]</td>
      <td>
        <p>Selezionare il tipo di oggetto che si desidera recuperare.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>Il modulo restituisce il documento a cui fa riferimento [!UICONTROL Key] come oggetto JSON. La chiave file può essere analizzata da qualsiasi URL del file Figma.</p>
            <p>Per i campi, consulta <a href="#Get2" class="MCXref xref" >[!UICONTROL Ottieni un file o un'immagine: File]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL File nodes]</b>
            </p>
            <p>Restituisce i nodi a cui fanno riferimento gli ID come oggetto JSON. I nodi vengono recuperati dal [!DNL Figma] file a cui fa riferimento [!UICONTROL Key].</p>
            <p>Per i campi, consulta <a href="#Get3" class="MCXref xref" >[!UICONTROL Ottieni un file o un'immagine: Nodi file]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Immagine]</b>
            </p>
            <p>Il modulo esegue il rendering delle immagini da un file.</p>
            <p>Per i campi, consulta <a href="#Get4" class="MCXref xref" >[!UICONTROL Ottieni un file o un'immagine: Immagine]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Riempimenti immagine]</b>
            </p>
            <p>Il modulo restituisce i collegamenti di download per tutte le immagini presenti nei riempimenti di immagini in un documento. I riempimenti delle immagini sono il modo in cui [!DNL Figma] rappresenta tutte le immagini fornite dall'utente. Quando si trascina un’immagine in [!DNL Figma], [!DNL Figma] crea un rettangolo con un singolo riempimento che rappresenta l'immagine e l'utente è in grado di trasformare il rettangolo (e le proprietà sul riempimento).</p>
            <p>Per i campi, consulta <a href="#Get5" class="MCXref xref" >[!UICONTROL Ottieni un file o un'immagine: Riempimenti immagine]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Ottieni un file o un&#39;immagine: File]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleziona il file da cui vuoi restituire JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versione ID]</td>
      <td>Immetti o mappa la versione del file che desideri che venga restituita dal modulo. Per il modulo corrente, lasciare vuoto questo campo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Per restituire solo un sottoinsieme del documento, immettere i nodi che si desidera restituire al modulo. Il modulo restituisce i nodi elencati, i relativi elementi secondari e qualsiasi cosa tra il nodo principale e i nodi elencati.</p>
        <p>Per ogni nodo che si desidera restituire, fare clic su <b>[!UICONTROL Aggiungi]</b> e immetti il testo del nodo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Immettere o mappare un numero intero che rappresenta la profondità della struttura del documento per la quale si desidera restituire i risultati. </p>
        <div class="example"><span class="autonumber"><span><b>Esempio: </b></span></span>
          <ul>
            <li>
              <p>Per restituire solo le pagine, immetti <code>1</code>.</p>
            </li>
            <li>
              <p>Per restituire pagine e oggetti di primo livello, immetti <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Per restituire tutti i nodi, lasciare vuoto questo campo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Geometria [!UICONTROL]</td>
      <td>Per restituire i dati vettoriali, immetti <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dati plug-in]</td>
      <td>Un elenco separato da virgole di ID plug-in e/o la stringa "[!UICONTROL shared]". Eventuali dati presenti nel documento scritto da tali plugin saranno inclusi nel risultato nella <code>pluginData</code> e <code>sharedPluginData</code> proprietà.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dati branch]</td>
      <td>Abilita questa opzione per restituire i metadati del ramo per il file richiesto. Se il file è un ramo, la chiave del file principale viene inclusa nella risposta restituita. Se il file ha rami, i relativi metadati vengono inclusi nella risposta restituita. Impostazione predefinita: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Ottieni un file o un&#39;immagine: Nodi file]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleziona il file da cui vuoi restituire JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Immettere i nodi che si desidera che il modulo restituisca e converta</p>
        <p>Per ogni nodo che si desidera restituire, fare clic su <b>[!UICONTROL Aggiungi]</b> e immetti il testo del nodo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versione ID]</td>
      <td>Immetti o mappa la versione del file che desideri che venga restituita dal modulo. Per il modulo corrente, lasciare vuoto questo campo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Immettere o mappare un numero intero che rappresenta la profondità della struttura del documento per la quale si desidera restituire i risultati. </p>
        <div class="example"><span class="autonumber"><span><b>Esempio: </b></span></span>
          <ul>
            <li>
              <p>Per restituire solo le pagine, immetti <code>1</code>.</p>
            </li>
            <li>
              <p>Per restituire pagine e oggetti di primo livello, immetti <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Per restituire tutti i nodi, lasciare vuoto questo campo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Geometria [!UICONTROL]</td>
      <td>Per restituire i dati vettoriali, immetti <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dati plug-in]</td>
      <td>Elenco separato da virgole degli ID dei plug-in e/o della stringa "shared". Eventuali dati presenti nel documento scritto da tali plug-in verranno inclusi nel risultato nelle proprietà pluginData e sharedPluginData .</td>
    </tr>
  </tbody>
</table>


##### Ottieni un file o un&#39;immagine: Immagine

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleziona il file da cui vuoi restituire JSON.</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>ID nodo]</td>
      <td>
        <p>Immetti i nodi di cui desideri eseguire il rendering nel modulo.</p>
        <p>Per ogni nodo di cui si desidera eseguire il rendering, fare clic su <b>[!UICONTROL Aggiungi]</b> e immetti il testo del nodo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Per ridimensionare l’immagine, immettete o mappate il fattore di scala. Questo numero deve essere compreso tra 0,01 e 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Formato]</td>
      <td>
        <p>Selezionare il formato per l'output dell'immagine.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - ID inclusione]</td>
      <td>Abilita questa opzione per includere gli attributi ID per tutti gli elementi di SVG. Predefinito: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Semplificare la traccia]</td>
      <td>Abilita questa opzione per semplificare i tratti interni/esterni e utilizza l’attributo di tratto, se possibile, invece di &lt;mask&gt;. Predefinito: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Utilizzare limiti assoluti]</td>
      <td>Abilita questa opzione per utilizzare le dimensioni complete del nodo indipendentemente dal fatto che sia ritagliato o che lo spazio intorno sia vuoto. Utilizzalo per esportare i nodi di testo senza ritaglio. Predefinito: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versione ID]</td>
      <td>Immetti o mappa la versione del file che desideri che venga restituita dal modulo. Per il modulo corrente, lasciare vuoto questo campo.</td>
    </tr>
  </tbody>
</table>

##### Ottieni un file o un&#39;immagine: Riempimenti immagine

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleziona il file da cui vuoi restituire JSON.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Cronologia delle versioni del file di elenco]

Questo modulo di ricerca restituisce la cronologia delle versioni di un singolo file in [!UICONTROL Figa].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Immettere o mappare l'ID file del file per il quale si desidera recuperare la cronologia delle versioni. </p>
        <ul>
          <li>
            <p>Se non conosci l’ID del file, fai clic su <b>[!UICONTROL Trova file]</b> e immetti o mappa l’ID del progetto a cui è associato il file, quindi seleziona il file .</p>
          </li>
          <li>
            <p>Se cerchi di trovare l’ID del file e non conosci l’ID del progetto, fai clic su <b>[!UICONTROL Trova progetti]</b> e immetti o mappa l’ID del team a cui appartiene il progetto a cui è associato il file. Seleziona il progetto, quindi seleziona il file .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare file di progetto]

Questo modulo di ricerca restituisce un elenco di tutti i file nel progetto specificato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Immetti o mappa l’ID progetto per il quale desideri recuperare i file. </p>
        <ul>
          <li>
            <p>Se non conosci l’ID del progetto, fai clic su <b>[!UICONTROL Trova progetti]</b> e immetti o mappa l’ID del team a cui è associato il progetto, quindi seleziona il progetto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elencare progetti]

Questo modulo di ricerca restituisce un elenco di tutti i progetti all&#39;interno del team specificato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Immetti o mappa l’ID progetto del progetto per il quale desideri recuperare i file. L'ID del team si trova nell'URL della pagina del team in Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>


### Componenti e stili

#### [!UICONTROL Ottenere uno stile o un componente]

Questo modulo di azione recupera un singolo stile o componente o un set di stili o componenti.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">Chiave &lt;[!UICONTROL Object&gt;]</td>
      <td>Immettere la chiave (identificatore univoco) dell'oggetto che si desidera recuperare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Immettere o mappare l'ID del team a cui sono associati i record o i record.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dimensione pagina]</td>
      <td>Immetti o mappa il numero o i risultati da restituire per pagina. Predefinito: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dopo]</td>
      <td>
        <p>Immettere o mappare il numero del risultato dopo il quale iniziare a recuperare i risultati. Questo può essere combinato con il campo [!UICONTROL Page Size] per impaginare i risultati.</p>
        <p>Questo valore non corrisponde agli ID oggetto.</p>
        <p>Questo campo non può essere utilizzato in combinazione con il campo [!UICONTROL Before].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Prima]</td>
      <td>
        <p>Immettere o mappare il numero del risultato prima del quale iniziare a recuperare i risultati. Questo può essere combinato con il campo [!UICONTROL Page Size] per impaginare i risultati.</p>
        <p>Questo valore non corrisponde agli ID oggetto.</p>
        <p>Questo campo non può essere utilizzato in combinazione con il campo [!UICONTROL After].</p>
      </td>
    </tr>
  </tbody>
</table>


### Altro

* [Effettuare una chiamata API](#make-an-api-call)

* [Eventi di controllo](#watch-events)


#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata all’API Figma senza dover pensare attraverso l’autenticazione. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dagli altri moduli Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare le [!DNL Figma] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Immettere un percorso relativo a <code>https://api.figma.com/v1/</code>.</p>
        <p>Ad esempio: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL, Metodo]</td>
      <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Eventi di controllo]

Questo modulo di attivazione avvia uno scenario in cui si verifica uno degli eventi seguenti per un team specifico nel tuo [!DNL Figma] spazio di squadra

* Aggiornamento file

* Aggiornamento della versione del file

* Eliminazione file

* Pubblicazione libreria

* Commento file

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Selezionare il webhook che il modulo controlla.</p>
        <p>Per aggiungere un nuovo webhook:</p>
        <ol>
          <li value="1">
            <p>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Selezionare la connessione che si desidera utilizzare per questo webhook. Per istruzioni su come collegare le [!DNL Figma] account a [!UICONTROL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crea una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base.</a></p>
          </li>
          <li value="3">
            <p>Selezionare il tipo di evento che si desidera controllare nel modulo.</p>
          </li>
          <li value="4">
            <p>Immettere l'ID del team di cui si desidera che il webhook guardi gli eventi.</p>
          </li>
          <li value="5">
            <p>Inserisci [!UICONTROL Status] o [!UICONTROL Description] degli eventi che desideri che il webhook guardi.</p>
          </li>
          <li value="6">
            <p>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
