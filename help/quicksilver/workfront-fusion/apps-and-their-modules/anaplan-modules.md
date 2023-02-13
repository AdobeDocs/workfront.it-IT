---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Anaplan
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Anaplan e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 1%

---

# [!DNL Anaplan] Moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Anaplan], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
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

Prima di poter utilizzare il [!DNL Anaplan] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* Devi avere un attivo [!UICONTROL Anaplan] conto.
* Devi configurare Aree di lavoro, Modelli e altri [!DNL Anaplan] oggetti [!UICONTROL Anaplan] prima del [!DNL Workfront Fusion] può interagire con loro.

## Connetti [!DNL Anaplan] a [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

Per creare una connessione per [!DNL Anaplan] moduli:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] scatola.
1. Selezionare il tipo di connessione.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>Un [!DNL Anaplan] La connessione [!UICONTROL Basic] richiede solo un indirizzo e-mail e una password per creare la connessione. </p> <p>Immetti un nome per la connessione, quindi inserisci il tuo indirizzo e-mail e la password del tuo [!DNL Anaplan] conto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA Certificate]</td> 
      <td> <p>Un [!DNL Anaplan] La connessione al certificato CA richiede una [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] e [!UICONTROL Encoded Signed Data]. Puoi generarli nel tuo [!DNL Anaplan] conto. Per istruzioni, consulta la sezione [!DNL Anaplan] documentazione.</p> <p>Immetti un nome per la connessione, quindi immetti la [!UICONTROL Certificate Key], i [!UICONTROL Encoded Data] e i [!UICONTROL Encoded Signed Data] generati nel tuo [!DNL Anaplan] conto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo .

## [!DNL Anaplan] moduli e relativi campi

Quando si configura [!DNL Anaplan] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Anaplan] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!DNL Watch records]

Questo modulo di attivazione avvia uno scenario in cui viene creato o aggiornato un record del tipo scelto.

>[!NOTE]
>
>Questo modulo restituisce i dati dei nuovi record. Non restituisce i dati dei record esistenti modificati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di oggetto da controllare</td> 
   <td>Selezionare il tipo di elemento da visualizzare. Lo scenario inizia quando questo tipo di record viene creato o aggiornato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>Immettere l'ID dell'oggetto in Anaplan, ad esempio un modello o un modulo, associato agli oggetti che si desidera visualizzare</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo [action] venga utilizzato durante ogni ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Creare una voce di elenco]](#create-a-list-item)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Esegui un&#39;azione]](#run-an-action)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Caricare un file]](#upload-a-file)

#### [!UICONTROL Creare una voce di elenco]

Questo modulo di azione aggiunge un nuovo elemento a un elenco in Anaplan.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>Seleziona o mappa l’ID di Analysis Workspace contenente l’elenco in cui desideri aggiungere un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Model ID]</td>
        <td>Selezionare o mappare l'ID del modello che contiene l'elenco in cui si desidera aggiungere un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL List ID]</td>
        <td>Seleziona o mappa l’ID dell’elenco in cui desideri creare un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Immettere un nome per il nuovo elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>Inserire il codice per il nuovo elemento. I codici sono codici generati dall’utente che consentono di distinguere tra elementi con lo stesso nome.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Elemento padre]</td>
        <td>Immettere il nome dell'elemento padre in cui si desidera creare il nuovo elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Properties]</td>
        <td>Se l’elenco a cui si desidera aggiungere un elemento dispone di proprietà personalizzate, selezionare le proprietà per le quali si desidera aggiungere i valori, quindi aggiungere i valori.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Sottoinsiemi]</td>
        <td>Se l’elenco a cui si desidera aggiungere elementi dispone di sottoinsiemi personalizzati, selezionare i sottoinsiemi a cui si desidera aggiungere l’elemento, quindi selezionare <b>[!UICONTROL Sì]</b> per aggiungere il nuovo elemento al sottoinsieme.</td>
    </tr>
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo ti consente di eseguire una chiamata API personalizzata al [!DNL Anaplan] API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record esistente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’ID di Analysis Workspace contenente l’oggetto da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model ID]</td> 
   <td>Immettere o mappare l'ID del modello contenente l'oggetto che si desidera eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Elimina</td> 
   <td> <p>Selezionare il tipo di oggetto da eliminare.</p> 
    <ul> 
     <li> <p><b>Azione</b> </p> <p>Seleziona o mappa l’azione da eliminare.</p> </li> 
     <li> <p><b>Voce di elenco</b> </p> <p>Seleziona l’elenco da cui vuoi eliminare un elemento, quindi immetti o mappa l’ID o il codice dell’elemento da eliminare</p>  </li> 
     <li> <p><b>[!UICONTROL File]</b> </p> <p>Selezionare o mappare il file da eliminare.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un record singolo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da leggere.</p> 
    <ul> 
     <li> <p><b>Modello</b> </p> <p>Selezionare o mappare l'ID del modello da leggere</p> </li> 
     <li> <p><b>Elenco modelli</b> </p> <p>Selezionare o mappare gli ID dell'area di lavoro e del modello che contengono l'elenco da leggere, quindi selezionare l'Elenco. Nel campo [!UICONTROL Data type], seleziona se desideri leggere i dati o i metadati.</p> </li> 
     <li> <p><b>Versione modello</b> </p> <p>Selezionare o mappare l'ID del modello da leggere.</p> </li> 
     <li> <p><b>Utente</b> </p> <p>Selezionare se si desidera restituire i dati relativi al proprietario dell'account utilizzato o a un altro utente. Se selezioni un altro utente, seleziona il nome dell’utente.</p> </li> 
     <li> <p><b>Area di lavoro</b> </p> <p>Seleziona o mappa l’ID dell’area di lavoro da leggere.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Esegui un&#39;azione]

Questo modulo di azione importa, esporta, elimina o elabora un’azione.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#Connect" class="MCXref xref" >[!UICONTROL Connetti Anaplan a Workfront Fusion]</a> in questo articolo.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Seleziona o mappa l’ID del [!DNL Anaplan] Area di lavoro in cui si desidera eseguire l'azione</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL Model ID]</td>
        <td>Selezionare o mappare l'ID del modello in cui si desidera eseguire l'azione.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo di azione]</td>
        <td>
          <p>Seleziona l’azione da eseguire</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Elimina]</b>
                </p>
                <p>Immetti o mappa l’ID dell’azione da eliminare.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>Immetti o mappa l’ID della definizione di esportazione che desideri utilizzare. È possibile esportare nei seguenti formati di file:</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL Import] </b>
                  </p>
                  <p style="font-weight: normal;">Immetti o mappa l’ID della definizione di importazione che desideri utilizzare.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>Immetti o mappa l’ID del processo da utilizzare. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un singolo record in [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da aggiornare.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Voce di elenco]</b> </p> <p>Per i campi, consulta <a href="#create-a-list-item" class="MCXref xref">Creare una voce di elenco</a> in questo articolo.</p> </li> 
     <li> <p><b>[!UICONTROL Dati cella modulo]</b> </p> <p>Quando si aggiornano i dati delle celle, vengono aggiornati anche tutti i calcoli downstream che utilizzano tali dati.</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Model ID]</b> </p> <p>Selezionare o mappare il modello contenente la cella che si desidera aggiornare.</p> </li> 
       <li> <p><b>[!UICONTROL Module ID]</b> </p> <p>Seleziona o mappa il modulo che contiene la cella che desideri aggiornare</p> </li> 
       <li> <p><b>[!UICONTROL Nome elemento riga]</b> </p> <p>Selezionare o mappare l'elemento riga della cella che si desidera aggiornare</p> </li> 
       <li> <p style="font-weight: bold;">ID Dimension</p> <p>Seleziona o mappa la dimensione presente sull’elemento di riga.</p> 
       <p><b>Nota: </b> 
       <ul>
       <li> La chiave di Dimension (valore) deve essere <code>dimensionName</code> (successivo) o <code>dimensionId</code> (ID).</li>
       <li>La chiave dell'elemento (valore) deve essere <code>itemName</code> (testo), <code>itemCode</code> (testo), oppure <code>itemId</code> (ID).</li>
       <li>Le chiavi di Dimension ed elemento devono essere dello stesso tipo (testo o ID).
       </ul>
        </p> 
        <p>Per informazioni sulle dimensioni, cerca i Dimension nel [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Value]</b> </p> <p>Immettere o mappare il nuovo valore per la cella.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Modello anno fiscale corrente]</b> </p> <p>Immettere l'ID area di lavoro e l'ID modello del modello per il quale si desidera aggiornare l'anno fiscale, quindi immettere o mappare il nuovo anno per il modello.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file in Anaplan. Il file deve essere già stato caricato su Anaplan. Puoi utilizzare questo modulo per caricarlo in posizioni aggiuntive all’interno di Anaplan.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Seleziona o mappa l’ID del [!DNL Anaplan] Area di lavoro in cui desideri caricare un file.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Model ID]</td>
<td>Seleziona o mappa l'ID del modello in cui desideri caricare un file.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL File ID]</td>
<td>Seleziona o mappa l’ID del file da caricare.</td>
</tr>
</tbody>
</table>
</div>

### Ricerche

#### [!UICONTROL Ottieni record]

Questo modulo di ricerca restituisce tutti i record accessibili del tipo selezionato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Anaplan], vedi <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipi di record]</td> 
   <td> <p>Selezionare il tipo di record da recuperare.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Models]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Line items]</b> </p> <p>Seleziona o mappa l'ID del modello che contiene il [!DNL line] elementi da recuperare.</p> </li> 
       <li> <p><b>Elenchi di modelli [!UICONTROL]</b> </p> <p>Selezionare o mappare l'ID dell'area di lavoro e dell'ID modello contenente gli elenchi di modelli che si desidera recuperare.</p> </li> 
       <li> <p><b>Calendario modelli [!UICONTROL]</b> </p> <p>Selezionare o mappare l'ID dell'area di lavoro contenente il calendario del modello che si desidera recuperare.</p> </li> 
       <li> <p><b>Versioni modello</b> </p> </li> 
       <li> <p>Selezionare o mappare [!UICONTROL ]l'ID del modello che contiene le versioni del modello che si desidera recuperare.</p> </li> 
       <li> <p><b>[!UICONTROL Users]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Visualizzazioni]</b> </p> <p>Selezionare se si desidera scegliere la visualizzazione per modulo o per modello, quindi selezionare o mappare l'ID del modulo o del modello che contiene la vista che si desidera recuperare.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Restituisci dimensione area di lavoro]</td> 
   <td>Abilita questa opzione per restituire una stima della dimensione corrente dell'area di lavoro. Questa stima si basa sulle dimensioni di tutti i moduli contenuti nell’area di lavoro.</td> 
  </tr> 
 </tbody> 
</table>
