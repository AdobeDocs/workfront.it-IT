---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare le date pianificate in un rapporto calendario
description: Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare i campi Data pianificata in un report calendario per attività, problemi e progetti.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 2%

---

# Usa [!UICONTROL date pianificate] in un report calendario

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. Puoi utilizzare i campi [!UICONTROL Data pianificata] in un report calendario per i seguenti oggetti:

* Attività
* Problemi
* Progetti

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a rapporti, dashboard e calendari</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire l’accesso al report del calendario</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

{{step1-to-calendars}}

1. Selezionare il calendario a cui si desidera aggiungere un nuovo gruppo di elementi.
Oppure
Fare clic su **[!UICONTROL + Nuovo calendario]** e immettere il nome del calendario.

   >[!NOTE]
   >
   >Per creare un report calendario, è necessario disporre dell&#39;accesso Modifica a Report, Dashboard e Calendari nel proprio livello di accesso.

1. A sinistra, fai clic su **[!UICONTROL Aggiungi al calendario]**, quindi su **[!UICONTROL Aggiungi elementi avanzati]**.

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Denomina questo gruppo di elementi]</strong></td>
      <td>Digitare un nome per il gruppo di elementi.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Selezionare un colore per il gruppo di elementi. Tutti gli elementi vengono visualizzati nel colore selezionato nel report calendario.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Scegliere <strong>[!UICONTROL Date pianificate]</strong>. Per ulteriori informazioni sulle date pianificate, consulta </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Panoramica della data di inizio pianificata del progetto</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Panoramica della data di inizio pianificata dell'attività</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica della data di completamento pianificata dell'attività</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Impostare la data di completamento pianificata del progetto</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sul calendario, mostra</strong></td>
      <td><p>Scegliere la modalità di visualizzazione delle date:</p>
       <ul>
        <li><strong>[!UICONTROL Solo data di inizio]</strong>: il calendario visualizza l'oggetto in un'unica data.</li>
        <li><strong>[!UICONTROL Solo data di fine]</strong>: il calendario visualizza l'oggetto in un'unica data.</li>
        <li><strong>[!UICONTROL Duration] (dall'inizio alla fine)</strong>: il calendario visualizza l'oggetto in un intervallo di giorni.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Passa alle date effettive quando disponibili]</strong></td>
      <td><p>Il calendario passa automaticamente alle date effettive quando sono disponibili. <br>Scegliere <strong>[!UICONTROL Sì]</strong> o <strong>[!UICONTROL No]</strong> per passare alle date effettive quando disponibili. Per ulteriori informazioni sulle date effettive, consulta</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Panoramica della data di inizio effettiva del progetto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Panoramica della data di completamento effettiva del progetto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Passare alla sezione seguente.

## Aggiungere oggetti al gruppo di elementi in Anteprima

Dopo aver impostato la modalità di visualizzazione degli elementi, è necessario aggiungere al raggruppamento gli oggetti che si desidera visualizzare nel calendario.

1. In **[!UICONTROL Cosa aggiungere al calendario?]** sezione, seleziona

   * **[!UICONTROL Attività]**
   * **[!UICONTROL Progetti]**
   * **[!UICONTROL Problemi]**


1. Fai clic su **[!UICONTROL Aggiungi attività]**, **[!UICONTROL Aggiungi progetti]** o **[!UICONTROL Aggiungi problemi]**, a seconda del tipo di oggetto che stai aggiungendo al calendario.

1. Nel menu a discesa, iniziare a digitare il nome del campo, quindi selezionare l&#39;origine del campo dell&#39;oggetto che si desidera visualizzare nel calendario, ad esempio **[!UICONTROL Attività in ritardo]**.
1. Imposta un&#39;istruzione di condizione per il raggruppamento del calendario.


   ![Seleziona l&#39;oggetto per il calendario](assets/calendar-field-name.png)

   Per informazioni sull&#39;impostazione delle condizioni, vedere [Filtri e modificatori di condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facoltativo) Specificare oggetti aggiuntivi per il raggruppamento del calendario ripetendo i passaggi da 1 a 4.

1. Nel campo **[!UICONTROL Imposta le etichette Attività/Progetti/Problemi come campo...]**, seleziona l&#39;etichetta degli oggetti in questo raggruppamento di calendari nel calendario.

   >[!NOTE]
   >
   >Se le opzioni predefinite dell&#39;etichetta non sono disponibili per un determinato oggetto, viene visualizzato il nome dell&#39;oggetto. Ad esempio, quando l&#39;etichetta [!UICONTROL Attività padre] è selezionata e non è associata alcuna attività padre all&#39;oggetto, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto visualizzato nel calendario.

   ![imposta etichette attività](assets/set-task-labels.png)
1. Fai clic su **[!UICONTROL Salva]**.

1. Fai clic su **[!UICONTROL Salva]**.

