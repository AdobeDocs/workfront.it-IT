---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Anaplan
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1915'
ht-degree: 0%

---

# [!DNL Anaplan] moduli

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli Anaplan](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/anaplan-modules.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Anaplan] e collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Prerequisiti

Prima di poter utilizzare il connettore [!DNL Anaplan], è necessario verificare che siano soddisfatti i seguenti prerequisiti:

* Devi avere un account [!UICONTROL Anaplan] attivo.
* È necessario configurare le aree di lavoro, i modelli e altri oggetti [!DNL Anaplan] nell&#39;account [!UICONTROL Anaplan] prima che [!DNL Workfront Fusion] possa interagire con essi.

## Informazioni API di Anaplan

Il connettore Anaplan utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL di base</td> 
   <td>https://api.anaplan.com/2/0/
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versione API</td> 
   <td> v2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v1.11.5/td&gt; 
 </tbody> 
</table>

## Connetti [!DNL Anaplan] a [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

Per creare una connessione per i moduli [!DNL Anaplan]:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto alla casella [!UICONTROL Connessione].
1. Selezionare il tipo di connessione.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>Una connessione [!DNL Anaplan] [!UICONTROL Basic] richiede solo un indirizzo e-mail e una password per creare la connessione. </p> <p>Immettere un nome per la connessione, quindi immettere l'indirizzo di posta elettronica e la password dell'account [!DNL Anaplan].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA Certificate]</td> 
      <td> <p>Una connessione [!DNL Anaplan] [!UICONTROL CA Certificate] richiede una [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] e [!UICONTROL Encoded Signed Data]. Puoi generarli nel tuo account [!DNL Anaplan]. Per istruzioni, vedere la documentazione di [!DNL Anaplan].</p> <p>Immettere un nome per la connessione, quindi immettere la [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] e [!UICONTROL Encoded Signed Data] generati nell'account [!DNL Anaplan].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## [!DNL Anaplan] moduli e relativi campi

Quando configuri [!DNL Anaplan] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Anaplan], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!DNL Watch records]

Questo modulo di attivazione avvia uno scenario quando viene creato o aggiornato un record del tipo scelto.

>[!NOTE]
>
>Questo modulo restituisce i dati dei nuovi record. Non restituisce i dati dei record esistenti modificati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di oggetto da controllare</td> 
   <td>Selezionare il tipo di elemento che si desidera controllare. Lo scenario inizia quando questo tipo di record viene creato o aggiornato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID &lt;Oggetto&gt;</td> 
   <td>Immettere l'ID dell'oggetto in Anaplan, ad esempio un modello o un modulo, associato agli oggetti che si desidera controllare</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera vengano inseriti nel modulo in [action] durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Crea una voce di elenco]](#create-a-list-item)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Esegui un&#39;azione]](#run-an-action)
* [[!UICONTROL Aggiorna un record]](#update-a-record)
* [[!UICONTROL Carica un file]](#upload-a-file)

#### [!UICONTROL Crea una voce di elenco]

Questo modulo di azione aggiunge un nuovo elemento a un elenco in Anaplan.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>Seleziona o mappa l’ID del Workspace Anaplan contenente l’elenco in cui desideri aggiungere un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL ID modello]</td>
        <td>Seleziona o mappa l’ID del modello che contiene l’elenco in cui desideri aggiungere un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL ID elenco]</td>
        <td>Seleziona o mappa l’ID dell’elenco in cui desideri creare un elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Immettere un nome per il nuovo elemento.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>Immettere il codice per il nuovo elemento. I codici sono codici generati dall'utente che consentono di distinguere tra righe con lo stesso nome.</td>
    </tr>
    <tr>
        <td>[!UICONTROL padre]</td>
        <td>Immettere il nome dell'elemento padre in cui si desidera creare il nuovo elemento.</td>
    </tr>
    <tr>
        <td>Proprietà [!UICONTROL]</td>
        <td>Se nell'elenco a cui si desidera aggiungere un elemento sono presenti proprietà personalizzate, selezionare le proprietà per le quali si desidera aggiungere i valori, quindi aggiungere i valori.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Subsets]</td>
        <td>Se nell'elenco a cui si desidera aggiungere elementi sono presenti sottoinsiemi personalizzati, selezionare i sottoinsiemi a cui si desidera aggiungere l'elemento, quindi selezionare <b>[!UICONTROL Sì]</b> per aggiungere il nuovo elemento a tale sottoinsieme.</td>
    </tr>
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo consente di eseguire una chiamata API personalizzata all&#39;API [!DNL Anaplan].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Inserisci un percorso relativo a <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query] </td> 
   <td> <p>Immettere la stringa di query richiesta.</p> </td> 
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

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record esistente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’ID del Workspace Anaplan contenente l’oggetto da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID modello]</td> 
   <td>Immettete o mappate l'ID del modello che contiene l'oggetto da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Elimina</td> 
   <td> <p>Selezionare il tipo di oggetto da eliminare.</p> 
    <ul> 
     <li> <p><b>Azione</b> </p> <p>Seleziona o mappa l’azione da eliminare.</p> </li> 
     <li> <p><b>Voce elenco</b> </p> <p>Seleziona l’elenco da cui vuoi eliminare un elemento, quindi immetti o mappa l’ID o il codice dell’elemento da eliminare</p>  </li> 
     <li> <p><b>[!UICONTROL File]</b> </p> <p>Selezionare o mappare il file da eliminare.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un singolo record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da leggere.</p> 
    <ul> 
     <li> <p><b>Modello</b> </p> <p>Selezionate o mappate l'ID del modello da leggere</p> </li> 
     <li> <p><b>Elenco modelli</b> </p> <p>Seleziona o mappa gli ID del Workspace e del modello che contengono l’elenco da leggere, quindi seleziona l’elenco. Nel campo [!UICONTROL Tipo di dati] selezionare se si desidera leggere dati o metadati.</p> </li> 
     <li> <p><b>Versione modello</b> </p> <p>Seleziona o mappa l’ID del modello da leggere.</p> </li> 
     <li> <p><b>Utente</b> </p> <p>Seleziona se desideri restituire dati sul proprietario dell'account utilizzato o su un altro utente. Se si seleziona un altro utente, selezionare il nome dell'utente.</p> </li> 
     <li> <p><b>Workspace</b> </p> <p>Seleziona o mappa l’ID del Workspace che desideri leggere.</p> </li> 
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
        <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect Anaplan to Workfront Fusion]</a> in questo articolo.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Selezionare o mappare l'ID del Workspace [!DNL Anaplan] in cui si desidera eseguire l'azione</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL ID modello]</td>
        <td>Seleziona o mappa l’ID del modello in cui desideri eseguire l’azione.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo di azione]</td>
        <td>
          <p>Seleziona l’azione da eseguire</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Elimina]</b>
                </p>
                <p>Inserisci o mappa l’ID dell’azione da eliminare.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>Immetti o mappa l’ID della definizione di esportazione che desideri utilizzare. Puoi esportare i seguenti formati di file:</p>
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
                  <p><b>[!UICONTROL Importazione] </b>
                  </p>
                  <p style="font-weight: normal;">Immetti o mappa l’ID della definizione di importazione che desideri utilizzare.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>Immettere o mappare l'ID del processo che si desidera utilizzare. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Aggiorna un record]

Questo modulo di azione aggiorna un singolo record in [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da aggiornare.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Voce di elenco]</b> </p> <p>Per i campi, vedere <a href="#create-a-list-item" class="MCXref xref">Creare una voce di elenco</a> in questo articolo.</p> </li> 
     <li> <p><b>[!UICONTROL Dati cella modulo]</b> </p> <p>Quando si aggiornano i dati delle celle, vengono aggiornati anche tutti i calcoli a valle che utilizzano tali dati.</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID modello]</b> </p> <p>Selezionate o mappate il modello contenente la cella da aggiornare.</p> </li> 
       <li> <p><b>[!UICONTROL ID modulo]</b> </p> <p>Selezionare o mappare il modulo contenente la cella da aggiornare</p> </li> 
       <li> <p><b>[!UICONTROL Nome elemento riga]</b> </p> <p>Selezionare o mappare l'elemento riga della cella da aggiornare</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL ID Dimension]</p> <p>Seleziona o mappa la dimensione che si trova sull’elemento riga.</p> 
       <p><b>Nota: </b> 
       <ul>
       <li> La chiave di Dimension (valore) deve essere <code>dimensionName</code> (avanti) o <code>dimensionId</code> (ID).</li>
       <li>La chiave dell'elemento (valore) deve essere <code>itemName</code> (testo), <code>itemCode</code> (testo) o <code>itemId</code> (ID).</li>
       <li>Le chiavi di Dimension e di elemento devono essere dello stesso tipo (testo o ID).
       </ul>
        </p> 
        <p>Per informazioni sulle dimensioni, cercare i Dimension in [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Valore]</b> </p> <p>Immettere o mappare il nuovo valore per la cella.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Modello anno fiscale corrente]</b> </p> <p>Immettere l'ID Workspace e l'ID modello per il quale si desidera aggiornare l'anno fiscale, quindi immettere o mappare il nuovo anno per il modello.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica un file]

Questo modulo di azione carica un file in Anaplan. Il file deve essere già stato caricato su Anaplan. Puoi utilizzare questo modulo per caricarlo in posizioni aggiuntive all’interno di Anaplan.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Selezionare o mappare l'ID del Workspace [!DNL Anaplan] in cui si desidera caricare un file.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ID modello]</td>
<td>Seleziona o mappa l’ID del modello in cui desideri caricare un file.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ID file]</td>
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Anaplan], vedere <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Anaplan] a [!DNL Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipi di record]</td> 
   <td> <p>Selezionare il tipo di record da recuperare.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Aree Di Lavoro]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Models]</b> </p> </li> 
       <li> <p><b>[!UICONTROL elementi riga]</b> </p> <p>Selezionare o mappare l'ID del modello contenente gli elementi [!DNL line] che si desidera recuperare.</p> </li> 
       <li> <p><b>[!UICONTROL Elenchi modelli]</b> </p> <p>Selezionate o mappate l'ID di Workspace e l'ID modello che contengono gli elenchi di modelli che desiderate recuperare.</p> </li> 
       <li> <p><b>[!UICONTROL Calendario modello]</b> </p> <p>Seleziona o mappa l’ID del Workspace che contiene il calendario del modello da recuperare.</p> </li> 
       <li> <p><b>Versioni modello</b> </p> </li> 
       <li> <p>Selezionare o mappare [!UICONTROL ]l'ID del modello che contiene le versioni del modello che si desidera recuperare.</p> </li> 
       <li> <p><b>[!UICONTROL Utenti]</b> </p> </li> 
       <li> <p><b>[!Viste UICONTROL]</b> </p> <p>Seleziona se desideri scegliere la vista per modulo o per modello, quindi seleziona o mappa l’ID del modulo o del modello che contiene la vista da recuperare.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Restituisce la dimensione dell'area di lavoro]</td> 
   <td>Abilita questa opzione per restituire una stima delle dimensioni correnti dell’area di lavoro. Questa stima si basa sulle dimensioni di tutti i moduli contenuti nell’area di lavoro.</td> 
  </tr> 
 </tbody> 
</table>
