---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare le date previste in un report calendario
description: Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare i campi Data prevista in un report calendario per attività, problemi e progetti.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# Usa [!UICONTROL Date previste] in un report calendario

Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare i campi Data prevista in un report calendario per i seguenti oggetti:

* Attività
* Problemi
* Progetti

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL ]Modifica accesso a [!UICONTROL Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendars]</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al report calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Calendari]**.

1. Selezionare il calendario a cui si desidera aggiungere un nuovo gruppo di elementi.\
   Oppure\
   Fare clic su **[!UICONTROL + Nuovo calendario]** e immettere il nome del calendario.

   >[!NOTE]
   >
   >Per creare un report del calendario è necessario disporre dell&#39;accesso [!UICONTROL Modifica] a [!UICONTROL Report], [!UICONTROL Dashboard] e [!UICONTROL Calendari] nel proprio livello di accesso.

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
      <td><p>Scegliere <strong>[!UICONTROL Date previste]</strong>. Per ulteriori informazioni sulle date previste, consulta </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Panoramica della data di inizio prevista del progetto</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica della data di completamento prevista per progetti, attività e problemi</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nel calendario, mostra]</strong></td>
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

## Aggiungere oggetti al gruppo di elementi

Dopo aver impostato la modalità di visualizzazione degli elementi, è necessario aggiungere al raggruppamento gli oggetti che si desidera visualizzare nel calendario.

1. In **[!UICONTROL Cosa aggiungere al calendario?]** sezione, seleziona

   * **[!UICONTROL Attività]**
   * **[!UICONTROL Progetti]**
   * **[!UICONTROL Problemi]**

1. Fai clic su **[!UICONTROL Aggiungi attività]**, **[!UICONTROL Aggiungi progetti]** o **[!UICONTROL Aggiungi problemi]**, a seconda del tipo di oggetto che stai aggiungendo al calendario.\
   ![Seleziona l&#39;oggetto per il calendario](assets/field-name.png)

1. Nel menu a discesa, iniziare a digitare il nome del campo, quindi selezionare l&#39;origine del campo dell&#39;oggetto che si desidera visualizzare nel calendario, ad esempio **[!UICONTROL Attività in ritardo]**.
1. Imposta un&#39;istruzione di condizione per il raggruppamento del calendario.

   ![Istruzione condizione](assets/condition-statement-calendar.png)

   Per informazioni sull&#39;impostazione delle condizioni, vedere [Filtri e modificatori di condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facoltativo) Specificare oggetti aggiuntivi per il raggruppamento del calendario ripetendo i passaggi da 1 a 4.
1. Nel campo **[!UICONTROL Imposta le etichette Attività/Progetti/Problemi come campo...]**, seleziona l&#39;etichetta degli oggetti in questo raggruppamento di calendari nel calendario.

   >[!NOTE]
   >
   >Se le opzioni predefinite dell&#39;etichetta non sono disponibili per un determinato oggetto, viene visualizzato il nome dell&#39;oggetto. Ad esempio, quando l&#39;etichetta dell&#39;attività padre è selezionata e all&#39;oggetto non è associata alcuna attività padre, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto visualizzato nel calendario.

1. Fai clic su **[!UICONTROL Salva]**.
