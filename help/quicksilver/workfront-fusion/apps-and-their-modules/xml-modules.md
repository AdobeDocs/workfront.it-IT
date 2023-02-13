---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: L'app XML consente di analizzare un testo in formato XML tramite XML &gt; Analizzare il modulo XML e convertirlo in un bundle per rendere i dati disponibili ad altri moduli. È inoltre possibile convertire un bundle in un testo in formato XML tramite XML &gt; Crea modulo XML
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 1%

---

# XML

La [!UICONTROL XML] l&#39;app consente di analizzare un testo in formato XML tramite [!UICONTROL XML] > [!UICONTROL Analizza XML] e convertirlo in un bundle per rendere i dati disponibili ad altri moduli. È inoltre possibile convertire un bundle in un testo in formato XML tramite il [!UICONTROL XML] > [!UICONTROL Crea XML] modulo

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

## [!UICONTROL Analizza XML]

La [!UICONTROL XML] > [!UICONTROL Analizza XML] Il modulo analizza un testo in formato XML ed emette un singolo bundle contenente tutte le informazioni estratte dal file XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La struttura dati descrive la struttura dell’XML per rendere disponibile l’output del modulo nel pannello di mappatura per i moduli seguenti.</p> <p>Se si dispone di un esempio del codice XML da analizzare, è possibile utilizzarlo per generare la struttura dati:</p> 
    <ol> 
     <li value="1">Fai clic sul pulsante <strong>[!UICONTROL Aggiungi]</strong> pulsante .</li> 
     <li value="2">Fai clic sul pulsante <strong>[!UICONTROL Generator]</strong> pulsante .</li> 
     <li value="3">Copia e incolla l’esempio XML nel <strong>[!UICONTROL Dati di esempio]</strong> campo .</li> 
     <li value="4">Fai clic su <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Verifica che la struttura dati sia stata generata correttamente.</li> 
     <li value="6"> <p>Fai clic sul pulsante <strong>[!UICONTROL Save]</strong> per salvare la struttura dati.</p> <p>Puoi saltare i passaggi 2-5 per fornire una struttura dati vuota. Se la struttura dati è vuota, l’output del modulo non è disponibile nel pannello di mappatura fino a quando il modulo non è stato eseguito almeno una volta.</p> </li> 
    </ol> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Strutture dei dati in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conserva i numeri come testo]</td> 
   <td>Abilitare questa opzione per garantire che i numeri rimangano come valori di testo (stringa). In caso contrario, i numeri vengono inviati ai valori numerici.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Immettere o mappare il testo in formato XML che si desidera analizzare.</p> <p>Se utilizzi una formula, accertati che il tipo di valore del risultato sia (o possa essere forzata automaticamente) il tipo di dati [!UICONTROL Text]. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Se il tipo di valore del risultato è [!UICONTROL Buffer] (dati binari), utilizza il <code>toString()</code> per convertirlo nel tipo di dati Testo . Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a> e <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati di elementi in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Per scaricare un file XML da un URL e analizzarne il contenuto:
>
>1. Crea un nuovo scenario.
>1. Inserisci [!UICONTROL HTTP] > [!UICONTROL Ottieni un file] modulo
>1. Apri la configurazione del modulo e configurala come segue:

>
>   **URL**: URL del file XML (ad esempio `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Fai clic su **[!UICONTROL OK]**&#x200B; salvare e chiudere la configurazione del modulo.
1. Aggiungi [!UICONTROL XML] > [!UICONTROL Analizza XML] modulo, collegalo dopo [!UICONTROL HTTP] > [!UICONTROL Ottieni un file] e configuralo come segue:
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Data structure]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Fai clic sul pulsante <strong>[!UICONTROL Aggiungi]</strong> pulsante .</li> 
&gt;        <li value="2">Fai clic sul pulsante <strong>[!UICONTROL Generator]</strong> pulsante .</li> 
&gt;        <li value="3">Nel browser Web, apri una nuova scheda o finestra.</li> 
&gt;        <li value="4">Inserisci l’URL utilizzato nel terzo passaggio nella barra degli indirizzi e recupera il file XML.</li> 
&gt;        <li value="5">Seleziona tutto il testo XML e copialo negli Appunti.</li> 
&gt;        <li value="6">Chiudi la scheda o la finestra e torna allo scenario.</li> 
&gt;        <li value="7">Incolla il testo XML copiato nel campo Dati di esempio.</li> 
&gt;        <li value="8">Fai clic su <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">Verifica che la struttura dati sia stata generata correttamente.</li> 
&gt;        <li value="10">Fai clic su <strong>[!UICONTROL Save]</strong> per salvare la struttura dati.</li> 
&gt;       </ol> <p>È possibile saltare i passaggi da 2 a 9 per fornire una struttura dati vuota. Se la struttura dati è vuota, l’output del modulo non è disponibile nel pannello di mappatura fino a quando il modulo non è stato eseguito almeno una volta.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Mappa la <code>Data </code>elemento dall’output del modulo [!UICONTROL HTTP] &gt; [!UICONTROL Ottieni un file] nel campo . Utilizza la <code>toString()</code> per convertire il suo valore dal tipo [!UICONTROL Buffer] (dati binari) al tipo di dati [!UICONTROL Text].</p> <p>Puoi copiare e incollare il codice della formula nel campo : <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Per ulteriori informazioni sui tipi di dati Buffer e Testo , consulta <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati per elementi in Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>


## [!UICONTROL Analisi degli attributi XML]

Per impostazione predefinita, la [!UICONTROL XML] > [!UICONTROL Analizza XML] il modulo mette gli attributi in una raccolta speciale `_attributes` come figlio del nodo che ha questi attributi. Se il nodo è un nodo di testo e ha attributi, vengono aggiunte due proprietà speciali: `_attributes` per gli attributi e `_value` per il contenuto di testo del nodo.

>[!INFO]
**Esempio:** XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

è convertito in questo bundle:

![](assets/xml-converted-to-bundle.png)

## Crea XML

La [!UICONTROL XML] > [!UICONTROL Crea XML] Il modulo converte un bundle in un testo in formato XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>La struttura dati descrive la struttura dell'XML risultante. Se si dispone di un esempio del codice XML che si desidera creare, è possibile utilizzarlo per generare la struttura dati:</p> 
    <ol> 
     <li value="1">Fai clic sul pulsante <strong>[!UICONTROL Aggiungi]</strong> pulsante .</li> 
     <li value="2">Fai clic sul pulsante <strong>[!UICONTROL Generator]</strong> pulsante .</li> 
     <li value="3">Copia e incolla l’esempio XML nel campo Dati di esempio.</li> 
     <li value="4">Fai clic sul pulsante <strong>[!UICONTROL Save]</strong> pulsante .</li> 
     <li value="5">Verifica che la struttura dati sia stata generata correttamente.</li> 
     <li value="6">Fai clic su <strong>[!UICONTROL Save]</strong> per salvare la struttura dati.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome elemento radice]</td> 
   <td>Immettere il nome dell'elemento principale dell'XML. Il valore predefinito è <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Immetti il nome file da utilizzare nel<code> !DOCTYPE SYSTEM</code> dichiarazione</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID PUBBLICO DI [!UICONTROL Doctype]</td> 
   <td>Immetti il nome file da utilizzare nel<code> !DOCTYPE PUBLIC</code> dichiarazione</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dichiarazione Xml Striscia di [!UICONTROL]</td> 
   <td>Attiva questa opzione per rimuovere la dichiarazione XML <code>&lt;?xml ... ?&gt;</code> e <code>&lt;!DOCTYPE ... &gt;</code>e lascia solo l'elemento principale XML e il relativo contenuto.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
**Esempio:**
Un caso d’uso tipico è quello di trasformare i dati da un [!DNL Google] > foglio di calcolo in XML.
1. Posiziona il [!DNL Google Sheets] > [!UICONTROL Seleziona righe] nel tuo scenario per recuperare i dati. Imposta il modulo per recuperare le righe dal [!DNL Google] foglio di calcolo. Imposta il &#x200B;**[!UICONTROL Numero massimo di righe restituite]** a un numero ridotto, ma maggiore di uno a scopo di test (esempio, tre). Esegui il [!DNL Google Sheets] modulo facendo clic con il pulsante destro del mouse e scegliendo &quot;**[!UICONTROL Esegui solo questo modulo]**.&quot; Verifica l’output del modulo.
1. Collega [!UICONTROL Aggregatore array] modulo dopo [!DNL Google Sheets] modulo . Nella configurazione del modulo, scegli la [!DNL Google Sheets] nel modulo **[!UICONTROL Nodo di origine]** campo . Lascia gli altri campi così come sono per il momento.
1. Collega [!UICONTROL XML] > [!UICONTROL Crea XML] modulo dopo [!UICONTROL Aggregatore array] modulo .
   La configurazione del modulo richiede una struttura dati che descrive la struttura dell&#39;output XML. Fai clic sul pulsante **[!UICONTROL Aggiungi]** per aprire la configurazione della struttura dati. Il modo più semplice per creare questa struttura dati è generarla automaticamente da un esempio XML.
1. Fai clic sul pulsante **[!UICONTROL Generatore]** e incolla l&#39;esempio XML nel [!UICONTROL Dati di esempio] campo:

![](assets/sample-data-field-350x146.png)
1. Fai clic su **[!UICONTROL Salva]**. Il campo Specifica nella struttura dati contiene ora la struttura generata.
1. Modifica il nome della struttura dati in modo che sia più specifico e fai clic su **[!UICONTROL Salva]**. Un campo corrispondente all’attributo dell’array principale viene visualizzato come campo mappabile nella configurazione del modulo JSON.
1. Fai clic sul pulsante **[!UICONTROL Mappa]** accanto al campo e mappa il `Array[]` dell&#39;articolo [!UICONTROL Aggregatore array] output:
1. Fai clic su **[!UICONTROL OK]** per chiudere la configurazione del modulo XML.
1. Apri la configurazione del [!UICONTROL Aggregatore array] modulo . Modificare la **[!UICONTROL Struttura di Target]** da Personalizzato a un campo del modulo XML corrispondente all&#39;elemento XML padre.Mappa elementi dal [!DNL Google Sheets] ai campi appropriati.
1. Fai clic su **[!UICONTROL OK]** per chiudere la configurazione del modulo Aggregator Array.
1. Esegui lo scenario.

   Il modulo XML genera il file XML corretto.
1. Apri la configurazione del [!DNL Google Sheets] e aumentare il [!UICONTROL Numero massimo di righe restituite] deve essere maggiore del numero di righe nel foglio di calcolo per elaborare tutti i dati.
   Il file XML risultante può essere salvato in [!DNL Dropbox], inviato come allegato tramite e-mail, caricato tramite FTP su un server e così via.


## Aggiunta di attributi XML

Se desideri aggiungere attributi a un nodo complesso (un nodo che conterrà altri nodi), devi aggiungere una raccolta con il nome `_attributes` per la nota complessa nella struttura dati personalizzata. Questa raccolta verrà mappata sugli attributi del nodo. Se desideri aggiungere attributi a un nodo di testo (ad esempio: `<node attr="1">abc</node>`), devi aggiungere una raccolta `_attributes` per gli attributi e una proprietà text `_value` per il valore del nodo per questo nodo nella struttura dati personalizzata.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Risoluzione dei problemi: Impossibile mappare dati da [!UICONTROL Analizza XML] modulo

Assicurati che la struttura dati sia definita correttamente. In alternativa, è possibile utilizzare una struttura dati vuota ed eseguire il modulo almeno una volta per elaborare un input XML.
