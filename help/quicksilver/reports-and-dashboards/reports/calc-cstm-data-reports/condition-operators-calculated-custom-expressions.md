---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Operatori condizione nelle espressioni personalizzate calcolate
description: È possibile utilizzare operatori di condizione o modificatori per la creazione di dati personalizzati calcolati in Adobe Workfront quando si utilizza la modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 639a696c19d79cf2415a45ccb9849ec183fb0bb8
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# Operatori condizione nei campi personalizzati calcolati

<!-- Audited: 2/2024 -->

È possibile utilizzare operatori di condizione o modificatori per la creazione di dati personalizzati calcolati in Adobe Workfront quando si utilizza la modalità testo. Per informazioni sull’utilizzo della modalità testo in Workfront, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Gli operatori o i modificatori di condizione consentono di creare un&#39;istruzione di condizione connettendo campi Workfront esistenti nelle istruzioni e generando un nuovo campo. Gli operatori di condizione vengono utilizzati in genere per creare la condizione di un&#39;istruzione &quot;IF&quot;.

È possibile utilizzare le istruzioni &quot;IF&quot; in Workfront per confrontare, formattare e stringere insieme campi di dati a scopo di reporting e di dati personalizzati.

Puoi creare istruzioni &quot;IF&quot; per i seguenti elementi di Workfront:

* Viste
* Raggruppamenti
* Campi personalizzati calcolati

Per ulteriori informazioni sulla creazione di istruzioni &quot;IF&quot;, vedere [Panoramica delle istruzioni &quot;IF&quot;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Gli esempi in questa guida illustrano l’utilizzo degli operatori condizione nei campi personalizzati calcolati. Puoi utilizzarli anche in colonne o raggruppamenti personalizzati calcolati, seguendo la sintassi corretta per i campi personalizzati calcolati nei rapporti.

Per informazioni sulla differenza di sintassi tra i campi personalizzati calcolati e i dati personalizzati calcolati nei rapporti, consulta [Campi personalizzati calcolati e colonne calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Per trovare i campi a cui desideri fare riferimento nelle espressioni personalizzate calcolate, fai riferimento a API Explorer. Per informazioni su API Explorer, consulta [API Explorer](../../../wf-api/general/api-explorer.md).

In Workfront puoi utilizzare i seguenti modificatori di condizioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operatore condizione</th> 
   <th>Sintassi dell’operatore di condizione</th> 
   <th>Definizione dell’operatore condizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Equal (Case Insensitive)</td> 
   <td>= </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è uguale al secondo campo.</p> <p>Ad esempio, utilizzare l'istruzione seguente in un campo personalizzato calcolato per generare un'istruzione "IF" che confronta la Data di completamento pianificata con la Data di completamento prevista di un'attività: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Maggiore di </td> 
   <td>&gt; </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è maggiore del secondo campo. <p>Ad esempio, utilizzare l'istruzione seguente in un campo personalizzato calcolato per generare un'istruzione "IF" che confronta la Data di completamento pianificata con la Data di completamento prevista di un'attività: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Maggiore o uguale a </td> 
   <td>&gt;= </td> 
   <td>Utilizzare questo operatore per indicare che la condizione è soddisfatta quando il primo campo dell'istruzione è maggiore o uguale al secondo campo. <p>Ad esempio, utilizzare l'istruzione seguente in un campo personalizzato calcolato per generare un'istruzione "IF" che confronta la Data di completamento pianificata con la Data di completamento prevista di un'attività: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Minore di </td> 
   <td>&lt; </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è minore del secondo campo. <p>Ad esempio, utilizzare l'istruzione seguente in un campo personalizzato calcolato per generare un'istruzione "IF" che confronta la Data di completamento pianificata con la Data di completamento prevista di un'attività: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Minore o uguale a </td> 
   <td>&lt;= </td> 
   <td>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando il primo campo dell'istruzione è minore o uguale al secondo campo. <p>Ad esempio, utilizzare l'istruzione seguente in un campo personalizzato calcolato per generare un'istruzione "IF" che confronta la Data di completamento pianificata con la Data di completamento prevista di un'attività: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Non </td> 
   <td>! </td> 
   <td> <p>Aggiungi questo operatore davanti a uno degli operatori precedenti per negarlo. </p> <p>Ad esempio: </p> 
    <ul> 
     <li>È uguale a: = </li> 
     <li>Non è uguale a: != </li> 
    </ul> <p>L’aggiunta di questo operatore davanti alle seguenti espressioni di dati aggiunge un’istruzione negativa alle espressioni: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>TRA </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Per informazioni su queste espressioni di dati e per un elenco completo, vedi <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Panoramica delle espressioni di dati calcolati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Oppure </td> 
   <td>|| </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione viene soddisfatta quando l'espressione trova il primo o il secondo valore dell'istruzione. </p> <p>Ad esempio, utilizza l’istruzione seguente in un campo personalizzato calcolato per creare un’istruzione "IF" che contrassegna i progetti con lo stato Corrente o Pianificazione come "Attivo": </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> E </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Utilizzare questo operatore per indicare che la condizione è soddisfatta quando l'espressione trova un elemento che soddisfa due condizioni contemporaneamente. </p> <p>Ad esempio, utilizza l’istruzione seguente in un campo personalizzato calcolato per generare un’istruzione "IF" che trova i progetti nello stato Corrente con una condizione A rischio e li contrassegna come "Mediazione necessaria". </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>