---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: I moduli CSV di Adobe Workfront Fusion consentono di creare file CSV e di analizzare il testo CSV da un valore di testo ricevuto o da un file.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

La [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] I moduli ti consentono di creare file CSV e di analizzare il testo CSV da un valore di testo ricevuto o da un file.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Crea CSV]

La [!UICONTROL Crea CSV] Aggregator consente di creare un testo CSV dai valori di testo ricevuti.

Per ulteriori informazioni sugli aggregatori, vedi [Modulo Aggregator in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleziona il modulo utilizzato per aggregare i campi necessari.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregated Fields]</td>
        <td>Seleziona i campi da aggregare dall’elenco dei campi disponibili.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Includi intestazioni nella prima riga]</td>
        <td>Selezionare questa opzione per includere le intestazioni nel risultato.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>Inserisci il filtro per raggruppare i risultati. Ad esempio, immetti una data.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td>
        <td>Selezionare questa opzione per interrompere lo scenario in assenza di risultati.</td>
    </tr>
</table>

## [!UICONTROL Crea CSV (avanzato)]

La [!UICONTROL Crea CSV (avanzato)] Aggregator consente di creare un testo CSV dai valori di testo ricevuti. Utilizza una struttura di dati che definisce le colonne CSV nel file CSV risultante. Una volta definite, le colonne vengono visualizzate come campi nella configurazione del modulo CSV e possono essere mappate al modulo successivo nello scenario.

Per ulteriori informazioni sugli aggregatori, vedi [Modulo Aggregator in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

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
   <td> <p>Seleziona la struttura dati per aggregare i campi nel modo desiderato. Dopo aver definito la struttura dati, puoi mappare gli elementi ai campi corrispondenti.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Strutture dei dati in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Includi intestazioni nella prima riga] </td> 
   <td>Selezionare questa opzione per includere le intestazioni nel risultato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>Inserisci il filtro per raggruppare i risultati. Ad esempio, immetti una data. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota] </td> 
   <td>Selezionare questa opzione per interrompere lo scenario in assenza di risultati. </td> 
  </tr> 
 </tbody> 
</table>


<p>Supponiamo che tu voglia esportare i tuoi contatti Google in un file CSV con due colonne "Nome completo" e "E-mail". Il bundle di output dal modulo [!UICONTROL Google Contatti] &gt;[!UICONTROL Ottieni contatti da un gruppo] ha la seguente struttura. Gli indirizzi e-mail vengono memorizzati all’interno della <code>[!UICONTROL Emails[]]</code> elemento, che è una matrice di raccolte, ciascuna raccolta contenente due elementi: <code>Label</code> e <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Se si utilizza il semplice [!DNL Create CSV] modulo, ti viene offerto un elenco di caselle di controllo corrispondenti agli elementi di primo livello di un bundle. Se si tenta di selezionare <code>Full name</code> e <code>Emails</code> elementi, il modulo [!UICONTROL Crea CSV] produce il seguente output, che probabilmente non è quello che desideri:</p>
<p>"email","fullName"</p>
<p>"[oggetto Object]","Shon Winer"</p>
<p>"[oggetto Object]","Lizeth Fulmore"</p>
<p>"[oggetto Object]","Hilario Gullatt"</p>
<p>"[oggetto Object]","Abby Eisenbarth"</p>
<p>Dall'elemento <code>Full Name</code> è di tipo semplice Testo, viene esportato correttamente. Ma l'oggetto <code>Emails</code>, di tipo complesso Array di raccolte, viene esportato come [oggetto Object], ovvero in che modo le raccolte e gli array vengono trasformati in testo per impostazione predefinita. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati per elementi in Adobe Workfront Fusion</a>.</p>
<p>Per esportare il contenuto del <code>Email </code>della prima raccolta <code>Emails[]</code> è necessario invece utilizzare il modulo [!UICONTROL Crea CSV (avanzato)]. Il modulo ti consente di definire singole colonne del file CSV e di mappare gli elementi, compresi quelli nidificati.</p>
<ol>
<li value="1">Inserisci il modulo [!UICONTROL Crea CSV (avanzato)] in uno scenario e apri la relativa configurazione.</li>
<li value="2">Fai clic sul pulsante <strong>[!UICONTROL Aggiungi]</strong> pulsante accanto al campo [!UICONTROL Data structure] per creare una nuova struttura dati.</li>
<li value="3"> <p>Scrivi un nome per la struttura dati e fai clic sul pulsante <strong>[!UICONTROL Aggiungi elemento]</strong> per aggiungere le singole colonne. Per esportare due colonne: "Full Name" (Nome completo) e "Email" (E-mail), la struttura dati risultante sarà simile alla seguente:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Una volta definita correttamente la struttura Dati, i campi corrispondenti a ogni singola colonna devono essere visualizzati nella configurazione del modulo [!UICONTROL Crea CSV (avanzato)] in modo da poter mappare gli elementi. Prendi il primo oggetto dal <code>[!UICONTROL Emails[]]</code> matrice e mappa il relativo elemento <code>Email </code>al campo/colonna Email:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Esegui lo scenario. Dall'elemento <code>Emails[1]: Email</code> mappato alla colonna "E-mail" è di tipo semplice Testo, viene esportato correttamente ora:</p> <p>"Nome completo","Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analizza CSV]

La [!UICONTROL Analizza CSV] trasformatore consente di analizzare il testo CSV da un valore di testo ricevuto o da un file.

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
   <td> <p>Seleziona questa opzione se la prima riga del testo CSV contiene intestazioni.</p> <p>Nota: Il modulo non utilizza queste intestazioni per etichettare le colonne nell'output. Al contrario, questo campo assicura che le intestazioni non siano incluse nei dati di output.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Seleziona il delimitatore per il file CSV. Il carattere di delimitazione è il carattere di testo che indica il limite tra valori o campi separati.</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>Scheda [!UICONTROL]</li> 
     <li> <p>[!UICONTROL Altro]</p> <p>Se selezioni [!UICONTROL Altro], immetti il carattere di delimitazione utilizzato dal file CSV per separare i valori. È necessario immettere esattamente un carattere.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mantieni virgolette all’interno di un campo non quotato]</td> 
   <td>Abilita questa opzione per mantenere le virgolette.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">CSV</td> 
   <td>Immetti o mappa il file CSV da analizzare.<p>Nota: <p>Se i dati sono in formato binario (in genere da un file), devi utilizzare la funzione `toString()` per convertire i dati binari in [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
