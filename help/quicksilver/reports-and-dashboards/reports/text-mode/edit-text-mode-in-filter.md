---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare un filtro utilizzando la modalità testo
description: "NOTA: aggiungi una sezione in questo articolo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Inoltre, crea un'area bozza nell'articolo di panoramica sulla modalità testo"
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: be47bc4da5e3921a7c36e19831acde91aad55db1
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Modificare un filtro utilizzando la modalità testo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

È possibile modificare un filtro in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell’interfaccia standard e creare filtri più complessi.

Per ulteriori esempi in modalità testo durante la creazione di un filtro, consulta anche la sezione &quot;Esempi di filtri personalizzati&quot; nell’articolo [Esempi di visualizzazione, filtro e raggruppamento personalizzati](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard e Calendari per modificare gli elementi di reporting in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare i filtri in un report</p> <p>Gestire le autorizzazioni per un filtro per modificarlo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un report o in un elenco, accertati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modificare la modalità testo in un filtro

La modifica di un filtro tramite la modalità testo è identica per i report e gli elenchi. L’accesso al filtro da un rapporto o da un elenco è diverso.

>[!TIP]
>
>È consigliabile creare il maggior numero possibile di filtri in modalità standard, quindi convertire il filtro in modalità testo per modificarlo.

Per ulteriori informazioni sulla creazione di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere al filtro da un rapporto, passa al rapporto, quindi fai clic su **Azioni report** > **Modifica** > **Filtri** scheda.
   1. Per accedere al filtro da un elenco, vai all’elenco e da **Filtro** , posizionare il mouse sul filtro che si desidera modificare e fare clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

      Viene aperto il generatore di filtri.

1. Clic **Aggiungere una regola di filtro** per aggiungere le condizioni del filtro, fai clic su **Passa alla modalità testo** nell’angolo superiore destro del generatore.
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
      <td> <p>Nome del campo e valore a cui è uguale come appaiono nel database di Workfront.</p> <p>Questa riga è obbligatoria.</p> <p> Per ulteriori informazioni sull'aspetto degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Per filtrare le attività con lo stato In corso, utilizzare la riga seguente:</p> <p><code>status=INP</code> </p> <p><b>SUGGERIMENTO</b>

   Quando si filtrano gli stati, è necessario utilizzare il codice di tre lettere dello stato e non il nome.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificatore del nome del campo e corrispondente funzione del modificatore. Indica le condizioni che il campo in base al quale si sta filtrando deve soddisfare.</p> <p>Questa riga è obbligatoria.</p> </td> 
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
        <p>Per un elenco completo dei modificatori di filtro in modalità testo, consulta l’articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificatori di filtri e condizioni</a>.</p> 
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
      <td> <p>Un carattere jolly che consente di generalizzare le informazioni in un filtro e fare riferimento all'ora corrente o all'utente che ha effettuato l'accesso.</p> <p>I caratteri jolly sono facoltativi.</p> <p>Suggerimento   <p>È consigliabile utilizzare i caratteri jolly quando possibile per rendere i filtri più dinamici e non duplicare gli stessi filtri per ogni utente o intervalli di tempo simili.</p> <p>Per informazioni sui caratteri jolly dei filtri, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variabili filtro con caratteri jolly</a>.</p> </p> </td> 
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

   1. Aggiungi una nuova riga di codice e digita OR:1: seguito dall&#39;oggetto o dall&#39;attributo in base al quale si desidera filtrare e dal valore con cui si desidera confrontarlo. Per fare riferimento alle attività in qualsiasi stato tranne Nuovo, utilizzare la riga seguente:

      ```
      OR:1:status=NEW
      ```

   1. Aggiungi una seconda riga e digita OR:1: seguito dall&#39;oggetto, dal modificatore e dal codice del modificatore. Per definire il modificatore per la riga di codice che fa riferimento a tutti gli stati dei task ad eccezione di Nuovo, utilizzare la linea di modificatore seguente:

      ```
      OR:1:status_Mod=notin
      ```

      Ogni riga della nuova istruzione deve essere preceduta da &quot;OR:`<number>`:&quot;.

      Per informazioni sulla creazione di istruzioni &quot;OR&quot; in un filtro, consulta [Creare istruzioni &quot;OR&quot; nei filtri in modalità testo](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>È possibile avere più istruzioni &quot;OR&quot; nello stesso filtro. Ogni volta che si dispone di una nuova istruzione &quot;OR&quot;, il numero dopo &quot;OR:&quot; aumenta.
Per filtrare le attività che si trovano nello stato In corso o che sono assegnate all&#39;utente connesso o che hanno la Data di completamento pianificata oggi, utilizza quanto segue:
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. Clic **Fine** se desideri salvare le modifiche e continuare a modificare il rapporto o il filtro.
1. Clic **Salva e chiudi** per salvare il report oppure **Salva filtro** per salvare il filtro nell&#39;elenco.


