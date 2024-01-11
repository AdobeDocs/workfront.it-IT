---
title: Panoramica sui campi formula
description: In Adobe Maestro, puoi creare campi formula che utilizzano funzioni e campi esistenti per calcolare un nuovo valore personalizzato.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ae60512c337d778939ef6c48fd2eda8b279dcce
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# Panoramica sui campi formula

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Puoi creare campi personalizzati in Adobe Maestro facendo riferimento a campi esistenti e collegandoli tramite una formula. A tale scopo, è possibile creare un campo personalizzato di tipo Formula.

I campi formula generano un nuovo valore utilizzando i valori esistenti di altri campi di un tipo di record e una funzione che indica come devono essere calcolati i valori esistenti.

Per informazioni, consulta [Crea campi](../fields/create-fields.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Non ci sono controlli di accesso per Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Considerazioni sui campi formula

* I campi formula fanno riferimento a campi che appartengono allo stesso tipo di record. Non è possibile fare riferimento a campi di altri tipi di record durante la creazione di un campo formula. <!--is this still accurate??-->
* Non è possibile modificare il tipo di campo Campo di un campo Formula dopo averlo salvato.
* È possibile aggiornare il calcolo di un campo formula dopo averlo salvato e i risultati del calcolo vengono aggiornati automaticamente per tutti i record dello stesso tipo.
* È necessario aggiungere i campi a cui si fa riferimento nelle formule così come vengono visualizzati nell&#39;interfaccia Maestro.
* L’utilizzo di campi di ricerca da tipi di record collegati in una formula sarà disponibile in un secondo momento.

## Formule supportate

I campi formula Maestro supportano tutte le espressioni dei campi calcolati di Workfront. Per ulteriori informazioni, consulta [Panoramica delle espressioni di dati calcolati](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Inoltre, sono supportate le seguenti espressioni per i campi formula Maestro:

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
   <td> <p>Restituisce l'ID di un record.</p> <p>L’espressione viene formattata come segue:

<code>{ID}</code>
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
   <td> <p>Restituisce il numero della settimana in un anno. In alternativa, è possibile indicare il giorno in cui inizia la settimana (utilizzare 1 per la domenica o 2 per il lunedì). Se omesso, per impostazione predefinita le settimane iniziano di domenica.</p> <p>L’espressione viene formattata come segue:

<code>WEEKOFYEAR(date,2)</code>
o
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>





