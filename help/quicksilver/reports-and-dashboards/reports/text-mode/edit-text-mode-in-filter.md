---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare un filtro utilizzando la modalità testo
description: 'NOTA: aggiungi una sezione in questo articolo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Inoltre, crea una bozza di quest''area nell''articolo della panoramica Modalità testo)'''
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Modificare un filtro utilizzando la modalità testo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

È possibile modificare un filtro in un elenco o in un rapporto utilizzando la modalità testo per accedere ai campi non disponibili nell’interfaccia standard e creare filtri più complessi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare gli elementi di reporting in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare i filtri in un rapporto</p> <p>Gestire le autorizzazioni per un filtro per modificarlo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un rapporto o in un elenco, assicurati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica della sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modificare la modalità testo in un filtro

La modifica di un filtro in modalità testo è identica per i rapporti e gli elenchi. L’accesso alla visualizzazione da un rapporto o da un elenco è diverso.

>[!TIP]
>
>È consigliabile creare la maggior parte del filtro possibile in modalità standard, quindi convertire il filtro in modalità testo per modificarlo.

Per ulteriori informazioni sulla creazione dei filtri, vedi [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere al filtro da un rapporto, passa al rapporto, quindi fai clic su **Azioni dei rapporti** > **Modifica** > **Filtri** scheda .
   1. Per accedere al filtro da un elenco, passa all’elenco e dalla **Filtro** menu a discesa, passate il puntatore del mouse sul filtro da modificare e fate clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

      Viene aperto il generatore di filtri.

1. Fai clic su **Aggiungere una regola filtro** per iniziare ad aggiungere le condizioni del filtro, fai clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore.
1. Aggiungi istruzioni di filtro utilizzando la modalità testo. Ciascuna istruzione filtro può contenere le seguenti righe e informazioni aggiuntive:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Filtra riga/informazioni</td> 
      <td>Esempio</td> 
     </tr> 
     <tr> 
      <td> <p>Nome del campo e valore a cui è uguale nel modo in cui vengono visualizzati nel database Workfront.</p> <p>Questa riga è obbligatoria.</p> <p> Per ulteriori informazioni sulla modalità di visualizzazione degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Per filtrare le attività in stato In corso, utilizzare la riga seguente:</p> <p><code>status=INP</code> </p> <p>Suggerimento: Quando si filtrano gli stati, è necessario utilizzare il codice a tre lettere dello stato e non il nome.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Modificatore di nome campo e a cosa corrisponde il modificatore. Indica le condizioni che il campo a cui si sta filtrando deve soddisfare.</p> <p>Questa riga è obbligatoria.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Per indicare che lo stato delle attività filtrate deve essere uguale a In corso, utilizzare la riga seguente oltre a quella precedente:</p> <p><code>status_Mod=in</code> </p> <p>Se il modificatore è un intervallo, ci sono due righe per indicare il modificatore.</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Esempio: </b></span></span> 
        <p>Questo è un filtro in modalità testo che cerca le attività in corso, che hanno una data di completamento pianificata entro il mese corrente e vengono assegnate a un utente con un GUID specifico:</p> 
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
      <td> <p>Operatore di istruzione. Per impostazione predefinita, ogni istruzione filtro è connessa dall’operatore "AND". Questo non viene visualizzato nell’interfaccia della modalità testo. È inoltre possibile aggiungere un operatore "OR" tra due istruzioni per indicare che si desidera filtrare gli oggetti che soddisfano una o le altre due condizioni.</p> <p>Gli operatori di filtro sono necessari solo per i filtri con più di un’istruzione.</p> <p>Suggerimento:   
        <ul> 
         <li> <p>"OR" è sensibile all’uso di maiuscole e minuscole e deve essere sempre maiuscola.</p> </li> 
         <li> <p>Quando si cambia l’operatore da AND a OR, il numero di voci dell’elenco potrebbe aumentare.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Esempio: </b></span></span> 
        <p>Per filtrare le attività in uno stato In corso o con una data di completamento pianificata di oggi, utilizzare quanto segue: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Un carattere jolly che consente di generalizzare le informazioni in un filtro e fa riferimento all’ora corrente o all’utente che ha effettuato l’accesso.</p> <p>I caratteri jolly sono facoltativi.</p> <p>Suggerimento:   <p>È consigliabile utilizzare i caratteri jolly ogni volta che è possibile per rendere i filtri più dinamici e non duplicare gli stessi filtri per ogni utente o intervalli di tempo simili.</p> <p>Per informazioni sui caratteri jolly del filtro, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variabili filtro caratteri jolly</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Esempio: </b></span></span> 
        <p>Per filtrare le attività assegnate all'utente attualmente connesso, utilizza quanto segue:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Per aggiungere un’istruzione filtro connessa dall’operatore &quot;OR&quot;, procedi come segue:

   1. Aggiungi una nuova riga di codice e digita OR:1: seguita dall’oggetto o dall’attributo con cui desideri filtrare e dal valore con cui desideri confrontarlo. Per fare riferimento a attività che si trovano in uno stato diverso da Nuovo, utilizzare la riga seguente:

      ```
      OR:1:status=NEW
      ```

   1. Aggiungi una seconda riga e digita OR:1: seguita dall’oggetto , dal modificatore e dal codice del modificatore . Per definire il modificatore della riga di codice che fa riferimento a tutti gli stati dell&#39;attività, ad eccezione di Nuovo, utilizzare la seguente riga del modificatore:

      ```
      OR:1:status_Mod=notin
      ```

      Ciascuna riga della nuova istruzione deve essere preceduta da &quot;OR:`<number>`:&quot;

      Per informazioni sulla creazione di istruzioni &quot;OR&quot; in un filtro, vedi [Creare istruzioni &quot;OR&quot; nei filtri in modalità testo](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Puoi avere più istruzioni &quot;OR&quot; nello stesso filtro. Ogni volta che si dispone di una nuova istruzione &quot;OR&quot; il numero dopo &quot;OR:&quot; aumenta.
Per filtrare le attività che si trovano in uno stato In corso o che sono assegnate all&#39;utente connesso o che dispongono della data di completamento pianificata oggi, utilizzare quanto segue:
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. Fai clic su **Fine** per salvare le modifiche e continuare a modificare il rapporto o il filtro.
1. Fai clic su **Salva e chiudi** per salvare il rapporto o **Salva filtro** per salvare il filtro nell’elenco.
