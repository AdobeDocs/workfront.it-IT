---
title: Panoramica sui campi formula
description: In Adobe Workfront Planning è possibile creare campi formula che utilizzano funzioni e campi esistenti per calcolare un nuovo valore personalizzato.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7288c6fb0f5d45758e0a82b8d1283e1f43ae94e6
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 7%

---

# Panoramica sui campi formula

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile creare campi personalizzati in Adobe Workfront Planning facendo riferimento a campi esistenti e collegandoli in un campo di tipo Formula.

I campi formula generano un nuovo valore utilizzando i valori esistenti di altri campi di un tipo di record e una funzione che indica come devono essere calcolati i valori esistenti.

Per informazioni, vedere la sezione &quot;Formula&quot; nell&#39;articolo [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un'area di lavoro e il tipo di record </a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr>

</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Considerazioni sui campi formula

* I campi formula fanno riferimento a campi che appartengono allo stesso tipo di record.
* È possibile fare riferimento a campi di altri tipi di record solo quando si collega un altro tipo di record a quello per il quale si sta creando un campo formula.
* Il riferimento ai tipi di record connessi o ai relativi campi di ricerca in una formula dipende dalle autorizzazioni di cui si dispone per i tipi di record connessi. Se non si dispone delle autorizzazioni necessarie per visualizzare il tipo di record, non è possibile fare riferimento ai relativi campi in una formula.
* Non è possibile modificare il tipo di campo Campo di un campo Formula dopo averlo salvato.
* È possibile aggiornare il calcolo di un campo formula dopo averlo salvato e i risultati del calcolo vengono aggiornati automaticamente per tutti i record dello stesso tipo.
* È necessario aggiungere i campi a cui si fa riferimento nelle formule così come vengono visualizzati nell&#39;interfaccia di Workfront Planning.
* È possibile fare riferimento solo ai campi visualizzati nella visualizzazione tabella di un tipo di record o nella pagina dei dettagli del record.
* È possibile definire il formato per il valore di un calcolo di formula scegliendo tra le opzioni di formato riportate di seguito.

   * Testo
   * Numero
   * Percentuale
   * Valuta
   * Tag
   * Data

  Per ulteriori informazioni, vedere la sezione &quot;Formula&quot; nell&#39;articolo [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).
* È possibile fare riferimento ai campi formula nelle nuove formule. Una volta aggiornato il valore in un campo a cui si fa riferimento in un campo formula, tutti i campi successivi che fanno riferimento a tale campo o ai campi formula che contengono tale campo verranno aggiornati automaticamente.


<!--

<div class="preview">

## Limitations of formula fields

* You can add a maximum of 20 formula fields for one record type. 

   Formula lookup fields added from connected record types do not count against this limit. 

* The formula expression cannot exceed 50,000 characters. 

* Formula fields might display as `#ERROR!` in the following cases:
   * When a field used in a formula is deleted.
   * When a field used in an aggregated lookup field displays as `#ERROR!`. 
   
      For example, if you display a lookup field that contains aggregated lookup formula fields and one of the referenced formula fields  displays as `#ERROR!`. 
   *  When a formula value cannot be displayed in the selected format. 
   
      For example, if I select Number for the Format of a formula field, and the fields used in the formula are text fields that display only non-numeric text values, the formula result will display as `#ERROR!`, because it cannot parse the text into a number.
 
 </div>
 
 -->

## Formule supportate

I campi formula di Adobe Workfront Planning supportano la maggior parte delle espressioni dei campi calcolati di Workfront.

>[!NOTE]
>
>Le seguenti espressioni di Workfront non sono supportate per i campi formula di Workfront Planning:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* CAMBIA
>* FORMATO

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Per un elenco completo delle espressioni di Workfront, vedere [Panoramica delle espressioni di dati calcolati](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Sono inoltre supportate le seguenti espressioni per i campi formula di Workfront Planning. Le espressioni seguenti non sono supportate per le espressioni Workfront:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Espressione</th> 
   <th>Spiegazione ed esempio</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Restituisce una stringa concatenata per delimitatore.</p> <p>L’espressione viene formattata come segue:

<code>ARRAYJOIN(delimitatore,matrice)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Restituisce una matrice con valori univoci.</p> <p>L’espressione viene formattata come segue:

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Restituisce l'ID di un record. Ogni record ha un ID univoco.</p> <p>L’espressione viene formattata come segue:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Restituisce i dati da JSON in base al valore JSONPath fornito. Se JSONPath non esiste nel JSON, verrà restituito un risultato vuoto. </p> <p>L’espressione viene formattata come segue:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Imposta il fuso orario di una data e un’ora su un fuso orario specifico.</p> <p>L’espressione viene formattata come segue:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Restituisce il numero di settimana in un anno. Facoltativamente, puoi indicare il giorno in cui inizia la settimana (usa 1 per domenica o 2 per lunedì). Se omesso, le settimane iniziano di domenica, per impostazione predefinita.</p> <p>L’espressione viene formattata come segue:

<code>WEEKOFYEAR(date,2)</code>
o
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>
