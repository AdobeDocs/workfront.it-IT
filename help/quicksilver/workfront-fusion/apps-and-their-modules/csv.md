---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: I moduli CSV di Adobe Workfront Fusion consentono di creare file CSV e analizzare il testo CSV da un valore di testo ricevuto o da un file.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 1%

---

# CSV

Il [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] I moduli consentono di creare file CSV e analizzare il testo CSV da un valore di testo ricevuto o da un file.

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

## [!UICONTROL Crea CSV]

Il [!UICONTROL Crea CSV] Aggregator consente di creare un testo CSV dai valori di testo ricevuti.

Per ulteriori informazioni sugli aggregatori, consulta [Modulo aggregatore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleziona il modulo utilizzato per aggregare i campi necessari.</td>
    </tr>
    <tr>
        <td>Campi Aggregati [!UICONTROL]</td>
        <td>Selezionare i campi da aggregare dall'elenco dei campi disponibili.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Includi intestazioni nella prima riga]</td>
        <td>Seleziona questa opzione per includere le intestazioni nel risultato.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Raggruppa per]</td>
        <td>Immettere il filtro per raggruppare i risultati. Ad esempio, inserisci una data.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td>
        <td>Selezionare questa opzione per interrompere lo scenario quando non sono presenti risultati.</td>
    </tr>
</table>

## [!UICONTROL Crea CSV (avanzato)]

Il [!UICONTROL Crea CSV (avanzato)] Aggregator consente di creare un testo CSV dai valori di testo ricevuti. Utilizza una struttura di dati che definisce le colonne CSV nel file CSV risultante. Una volta definite, le colonne vengono visualizzate come campi nella configurazione del modulo CSV e possono essere mappate a un modulo successivo nello scenario.

Per ulteriori informazioni sugli aggregatori, consulta [Modulo aggregatore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Seleziona il modulo app che utilizzi per aggregare i campi necessari.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Seleziona la struttura dati per aggregare i campi nel modo desiderato. Dopo aver definito la struttura dati, puoi mappare gli elementi ai campi corrispondenti.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Strutture di dati in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Includi intestazioni nella prima riga] </td> 
   <td>Seleziona questa opzione per includere le intestazioni nel risultato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Raggruppa per] </td> 
   <td>Immettere il filtro per raggruppare i risultati. Ad esempio, inserisci una data. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota] </td> 
   <td>Selezionare questa opzione per interrompere lo scenario quando non sono presenti risultati. </td> 
  </tr> 
 </tbody> 
</table>


<p>Supponiamo che tu voglia esportare i tuoi contatti Google in un file CSV con due colonne "Nome completo" e "E-mail". Il bundle di output del modulo [!UICONTROL Contatti Google] &gt;[!UICONTROL Ottieni contatti da un gruppo] presenta la seguente struttura. Gli indirizzi e-mail vengono memorizzati all’interno del <code>[!UICONTROL Emails[]]</code> item, un array di raccolte, ciascuna delle quali contiene due elementi: <code>Label</code> e <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Se si utilizza il semplice [!DNL Create CSV] modulo, ti viene offerto un elenco di caselle di controllo corrispondenti agli elementi di livello superiore di un bundle. Se tenta di spuntare <code>Full name</code> e <code>Emails</code> elementi, il modulo [!UICONTROL Crea CSV] produce il seguente output, che probabilmente non è quello desiderato:</p>
<p>"emails","fullName"</p>
<p>"[oggetto oggetto]","Shon Winer"</p>
<p>"[oggetto]","Lizeth Fulmore"</p>
<p>"[oggetto]","Hilario Gullatt"</p>
<p>"[oggetto]","Abby Eisenbarth"</p>
<p>Dal momento dell'elemento <code>Full Name</code> è di tipo semplice Testo, viene esportato correttamente. Ma l'elemento <code>Emails</code>, che è di tipo complesso Array di raccolte, viene esportato come [oggetto Oggetto], che è il modo in cui le raccolte e gli array vengono trasformati in testo per impostazione predefinita. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati degli elementi in Adobe Workfront Fusion</a>.</p>
<p>Per esportare il contenuto del <code>Email </code>elemento della prima raccolta del <code>Emails[]</code> è necessario utilizzare il modulo [!UICONTROL Create CSV (advanced)]. Il modulo ti consente di definire singole colonne del file CSV e di mappare ad esse gli elementi, inclusi quelli nidificati.</p>
<ol>
<li value="1">Inserisci il modulo [!UICONTROL Create CSV (advanced)] in uno scenario e apri la relativa configurazione.</li>
<li value="2">Fai clic su <strong>[!UICONTROL Add]</strong> accanto al campo [!UICONTROL Data structure] per creare una nuova struttura dati.</li>
<li value="3"> <p>Scrivi un nome per la struttura Dati e fai clic su <strong>[!UICONTROL Add item]</strong> per aggiungere le singole colonne. Se desideri esportare due colonne: "Nome completo" e "E-mail", la struttura dati risultante sarà simile alla seguente:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Dopo aver definito correttamente la struttura dati, i campi corrispondenti a ogni singola colonna devono essere visualizzati nella configurazione del modulo [!UICONTROL Crea CSV (avanzato)] per consentire la mappatura degli elementi. Prendi il primo oggetto dal <code>[!UICONTROL Emails[]]</code> array e mappa il relativo elemento <code>Email </code>al campo/colonna E-mail:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Esegui lo scenario. Dal momento dell'elemento <code>Emails[1]: Email</code> mappato alla colonna "E-mail" è di tipo semplice Testo, viene esportato correttamente ora:</p> <p>"Nome completo","E-mail"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analizza CSV]

Il [!UICONTROL Analizza CSV] Il trasformatore consente di analizzare il testo CSV da un valore di testo ricevuto o da un file.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero di colonne]</td> 
   <td>Specifica il numero di colonne nel file CSV.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contiene intestazioni]</td> 
   <td> <p>Seleziona questa opzione se la prima riga del testo CSV contiene intestazioni.</p> <p>Nota: il modulo non utilizza queste intestazioni per etichettare le colonne nell’output. Questo campo assicura, invece, che le intestazioni non vengano incluse nei dati di output.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Seleziona il delimitatore per il file CSV. Il delimitatore è il carattere di testo che indica il limite tra valori o campi separati.</p> 
    <ul> 
     <li>[!UICONTROL Virgola]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Altro]</p> <p>Se si seleziona [!UICONTROL Altro], immettere il carattere di delimitazione utilizzato dal file CSV per separare i valori. È necessario immettere esattamente un carattere.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mantieni virgolette all'interno di un campo senza virgolette]</td> 
   <td>Abilita questa opzione per mantenere le virgolette.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Immetti o mappa il file CSV da analizzare.<p>Nota: <p>Se i dati sono in formato binario (in genere da un file), è necessario utilizzare la funzione "toString()" per convertire i dati binari in [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
