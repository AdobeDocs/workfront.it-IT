---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operatori di condizione nelle espressioni personalizzate calcolate
description: È possibile utilizzare gli operatori di condizioni o i modificatori quando si creano dati personalizzati calcolati in Adobe Workfront quando si utilizza la modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# Operatori di condizione nei campi personalizzati calcolati

È possibile utilizzare gli operatori di condizioni o i modificatori quando si creano dati personalizzati calcolati in Adobe Workfront quando si utilizza la modalità testo.

Per informazioni sull&#39;utilizzo della modalità testo in Workfront, vedi [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Gli operatori di condizioni o i modificatori consentono di creare un’istruzione di condizione collegando i campi Workfront esistenti nelle istruzioni e generando un nuovo campo. L’utilizzo più comune degli operatori di condizioni consiste nel creare la condizione di un’istruzione &quot;IF&quot;.

È possibile utilizzare le istruzioni &quot;IF&quot; in Workfront per confrontare, formattare e stringa insieme i campi di dati a scopo di reporting e di dati personalizzati.

Puoi generare istruzioni &quot;IF&quot; per i seguenti elementi Workfront:

* Viste
* Raggruppamenti
* Campi personalizzati calcolati

Per ulteriori informazioni sulla creazione di istruzioni &quot;IF&quot;, vedi [Panoramica delle istruzioni &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Gli esempi contenuti in questa guida illustrano l’uso degli operatori di condizioni nei campi personalizzati calcolati. Puoi anche utilizzarli in colonne o raggruppamenti personalizzati calcolati, quando segui la sintassi corretta per i campi personalizzati calcolati nei rapporti.

Per informazioni sulla differenza di sintassi tra i campi personalizzati calcolati e i dati personalizzati calcolati nei rapporti, consulta [Campi personalizzati calcolati e colonne calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Per trovare i campi a cui si desidera fare riferimento nelle espressioni personalizzate calcolate, consulta l’ API Explorer . Per informazioni su API Explorer, consulta [Esplora API](../../../wf-api/general/api-explorer.md).

In Workfront è possibile utilizzare i seguenti modificatori di condizioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operatore condizione</th> 
   <th>Sintassi dell’operatore condizione</th> 
   <th>Definizione dell’operatore condizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Equal (Case Insensitive)</td> 
   <td>= </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è uguale al secondo campo.</p> <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per creare un'istruzione "IF" che confronta la data di completamento pianificata con la data di completamento prevista di un'attività: </p><pre>IF({projectsCompletionDate}={scheduledCompletionDate},"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr> 
   <td>Maggiore di </td> 
   <td>&gt; </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è maggiore del secondo campo. <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per creare un'istruzione "IF" che confronta la data di completamento pianificata con la data di completamento prevista di un'attività: </p><pre>IF({projectsCompletionDate}&gt;{scheduledCompletionDate},"In ritardo","")</pre></td> 
  </tr> 
  <tr> 
   <td>Maggiore o uguale a </td> 
   <td>&gt;= </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è maggiore o uguale al secondo campo. <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per creare un'istruzione "IF" che confronta la data di completamento pianificata con la data di completamento prevista di un'attività: </p><pre>IF({projectsCompletionDate}&gt;={scheduledCompletionDate},"In ritardo","In anticipo")</pre></td> 
  </tr> 
  <tr> 
   <td>Minore di </td> 
   <td>&lt; </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è minore del secondo campo. <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per creare un'istruzione "IF" che confronta la data di completamento pianificata con la data di completamento prevista di un'attività: </p><pre>IF({projectsCompletionDate}&lt;{scheduledCompletionDate},"Early","")</pre></td> 
  </tr> 
  <tr> 
   <td>Minore o uguale a </td> 
   <td>&lt;= </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è minore o uguale al secondo campo. <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per creare un'istruzione "IF" che confronta la data di completamento pianificata con la data di completamento prevista di un'attività: </p><pre>IF({projectsCompletionDate}&lt;={scheduledCompletionDate},"early","late")</pre></td> 
  </tr> 
  <tr> 
   <td>Non </td> 
   <td>! </td> 
   <td> <p>Aggiungi questo operatore davanti a uno qualsiasi degli operatori di cui sopra per negare l’operatore. </p> <p>Ad esempio: </p> 
    <ul> 
     <li>Uguale a: = </li> 
     <li>Non è uguale: != </li> 
    </ul> <p>L'aggiunta di questo operatore davanti alle seguenti espressioni dati aggiunge un'istruzione negativa alle espressioni: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>TRA </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Per informazioni su queste espressioni dati e per un elenco completo, consulta <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Espressioni dati calcolate</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Oppure </td> 
   <td>|| </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando l'espressione trova il primo o il secondo valore dell'istruzione. </p> <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per generare un'istruzione "IF" che contrassegna i progetti nello stato Corrente o Pianificazione come "Attivo": </p><pre>IF({status}="PLN"||{status}="CUR","Active","Not Active")</pre> </td> 
  </tr> 
  <tr> 
   <td> E </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando l'espressione trova un elemento che soddisfa due condizioni contemporaneamente. </p> <p>Ad esempio, utilizzare la seguente istruzione in un campo personalizzato calcolato per generare un'istruzione "IF" che individua i progetti in stato corrente e con condizione di rischio e li contrassegna come "Mediazione necessaria". </p><pre>IF({status}="CUR"&amp;&amp;{condizione}="AR","Mediazione necessaria",""))</pre> </td> 
  </tr> 
 </tbody> 
</table>
