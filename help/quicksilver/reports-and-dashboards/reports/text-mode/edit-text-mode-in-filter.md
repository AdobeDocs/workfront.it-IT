---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare un filtro utilizzando la modalità testo
description: È possibile modificare un filtro in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell’interfaccia standard e creare filtri più complessi.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 1%

---

# Modificare un filtro utilizzando la modalità testo

<!-- Audited: 1/2025 -->

È possibile modificare un filtro in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell’interfaccia standard e creare filtri più complessi.

Per ulteriori esempi in modalità testo durante la creazione di un filtro, vedere anche la sezione [Esempi di filtri personalizzati](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) nell&#39;articolo [Visualizzazione personalizzata, filtro e raggruppamento di esempi: indice articolo](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Filtri, Viste e Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard e Calendari per modificare gli elementi di reporting in un rapporto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare i filtri in un report</p> <p>Gestire le autorizzazioni per un filtro per modificarlo</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un report o in un elenco, accertati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati: indice articolo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modificare la modalità testo in un filtro

La modifica di un filtro tramite la modalità testo è identica per i report e gli elenchi. L’accesso al filtro da un rapporto o da un elenco è diverso.

>[!TIP]
>
>È consigliabile creare il maggior numero possibile di filtri in modalità standard, quindi convertire il filtro in modalità testo per modificarlo.

Per ulteriori informazioni sulla creazione di filtri, vedere [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   Per accedere al filtro da un elenco, vai all&#39;elenco e fai clic sull&#39;icona **Filtro**, quindi passa il puntatore del mouse sul filtro nel pannello laterale **Filtri** che desideri modificare e fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png). Nel pannello laterale **Filtri** viene visualizzato il filtro selezionato oppure viene aperto il generatore di filtri legacy.

   OPPURE

   Per accedere al filtro da un report, passa al report, quindi fai clic sulla scheda **Azioni report** > **Modifica** > **Filtri**.

1. Esegui una delle operazioni seguenti:

   Se si utilizza il pannello laterale **Filtri** in un elenco, fare clic su **Modalità testo**.

   OPPURE

   Se utilizzi il generatore di filtri legacy o in un report, fai clic su **Aggiungi una regola di filtro** per iniziare ad aggiungere le condizioni del filtro. Quindi fare clic su **Passa alla modalità testo** e quindi su **Modifica modalità testo** sul lato destro del generatore.

1. Aggiungere istruzioni di filtro utilizzando la modalità testo. Ogni istruzione di filtro può contenere le seguenti righe e informazioni aggiuntive:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filtra riga/informazioni</b></td> 
      <td><b>Esempio</b></td> 
     </tr> 
     <tr> 
      <td> <p>Nome del campo e valore che è uguale a quello visualizzato nel database di Workfront.</p> <p>Questa riga è obbligatoria.</p> <p> Per ulteriori informazioni sull'aspetto degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Per filtrare le attività con lo stato In corso, utilizzare la riga seguente:</p> <p><code>status=INP</code> </p> <p><b>SUGGERIMENTO</b>

   Quando si filtrano gli stati, è necessario utilizzare il codice di tre lettere dello stato e non il nome.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificatore del nome del campo e elemento corrispondente. Indica le condizioni che il campo in base al quale si sta filtrando deve soddisfare.</p> <p>Questa riga è obbligatoria.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Per indicare che lo stato delle attività per le quali si applica il filtro deve essere uguale a In corso, utilizzare la riga seguente oltre a quella precedente:</p> <p><code>status_Mod=in</code> </p> <p>Se il modificatore è un intervallo, sono disponibili due linee per indicare il modificatore.</p> 
       <div> <span class="autonumber"><span><b>ESEMPIO </b></span></span> 
        <p>Questo è un filtro in modalità testo che cerca le attività in corso, con una Data di completamento pianificata entro il mese corrente e che sono assegnate a un utente con un GUID specifico:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Per un elenco completo dei modificatori di filtro in modalità testo, vedere l'articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificatori di filtro e condizione</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Operatore di istruzioni. Per impostazione predefinita, ogni istruzione di filtro è connessa dall’operatore "AND". Questo non viene visualizzato nell’interfaccia in modalità testo. È inoltre possibile aggiungere un operatore "OR" tra due istruzioni per indicare che si desidera filtrare gli oggetti che possono soddisfare una o l’altra delle due condizioni.</p> <p>Gli operatori di filtro sono necessari solo per i filtri con più di un’istruzione.</p> <p>Suggerimento   
        <ul> 
         <li> <p>"OR" fa distinzione tra maiuscole e minuscole e deve essere sempre maiuscolo.</p> </li> 
         <li> <p>Quando si modifica l'operatore da AND a OR, il numero di voci di elenco potrebbe aumentare.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>ESEMPIO </b></span></span> 
        <p>Per filtrare le attività con lo stato In corso o con la data di completamento pianificata in data odierna, utilizzare quanto segue: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Un carattere jolly, che consente di generalizzare le informazioni in un filtro e fare riferimento all’ora corrente per l’utente che ha effettuato l’accesso.</p> <p>I caratteri jolly sono facoltativi.</p> <p>Suggerimento   <p>È consigliabile utilizzare i caratteri jolly quando possibile per rendere i filtri più dinamici e non duplicare gli stessi filtri per ogni utente o intervalli di tempo simili.</p> <p>Per informazioni sui caratteri jolly dei filtri, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Panoramica delle variabili dei filtri con caratteri jolly</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>ESEMPIO</b></span></span> 
        <p>Per filtrare le attività assegnate all'utente attualmente connesso, utilizzare quanto segue:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Per aggiungere un’istruzione di filtro connessa dall’operatore &quot;OR&quot;, effettua le seguenti operazioni:

   1. Aggiungere una nuova riga di codice e digitare OR:1: seguito dall&#39;oggetto o dall&#39;attributo in base al quale si desidera filtrare e dal valore con cui si desidera confrontarlo. Per fare riferimento alle attività in qualsiasi stato tranne Nuovo, utilizzare la riga seguente:

      `OR:1:status=NEW`

   1. Aggiungere una seconda riga e digitare OR:1: seguito dall&#39;oggetto, dal modificatore e dal codice del modificatore. Per definire il modificatore per la riga di codice che fa riferimento a tutti gli stati dei task ad eccezione di Nuovo, utilizzare la linea di modificatore seguente:

      `OR:1:status_Mod=notin`

      Ogni riga della nuova istruzione deve essere preceduta da &quot;OR:`<number>`:&quot;.

      Per informazioni sulla creazione di istruzioni &quot;OR&quot; in un filtro, vedere [Creare istruzioni &quot;OR&quot; nei filtri in modalità testo](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >È possibile avere più istruzioni &quot;OR&quot; nello stesso filtro. Ogni volta che si dispone di una nuova istruzione &quot;OR&quot;, il numero dopo &quot;OR:&quot; aumenta.
      >
      >Per filtrare le attività che si trovano nello stato In corso o che sono assegnate all&#39;utente connesso o che hanno la Data di completamento pianificata oggi, utilizza quanto segue:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Fai clic su **Applica** o **Fine** per salvare le modifiche apportate alla modalità testo e continuare a modificare il report o il filtro.
1. Fai clic su **Salva + Chiudi** per salvare il rapporto oppure su **Salva filtro** per salvare il filtro nell&#39;elenco.


