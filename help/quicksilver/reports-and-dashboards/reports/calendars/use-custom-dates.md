---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare campi data personalizzati in un rapporto di calendario
description: Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per attività, problemi e progetti.
author: Jenny
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# Utilizzare campi data personalizzati in un report calendario

Un report [!UICONTROL calendar] è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per i seguenti oggetti:

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

## Prerequisiti

1. È necessario disporre di campi data personalizzati e di un valore all&#39;interno del campo disponibile nell&#39;istanza [!DNL Workfront]. Se non hai configurato un modulo personalizzato con date personalizzate, segui le istruzioni in [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Allegare il modulo personalizzato a un progetto, un&#39;attività o un problema che si intende aggiungere al calendario e specificare una data. Per ulteriori informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

{{step1-to-calendars}}

1. Selezionare il calendario a cui si desidera aggiungere un nuovo gruppo di elementi, scegliere il menu Altro, quindi **Modifica**.
Oppure
Fai clic su **[!UICONTROL + Nuovo calendario]**, immetti il nome del progetto, quindi fai clic su **[!UICONTROL Aggiungi elementi avanzati]**.

   >[!NOTE]
   >
   >Per creare un report del calendario è necessario disporre dell&#39;accesso [!UICONTROL Modifica] a [!UICONTROL Report], [!UICONTROL Dashboard] e [!UICONTROL Calendari] nel proprio livello di accesso.

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
      <td>Scegliere <strong>[!UICONTROL Date personalizzate]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nel calendario, mostra]</strong></td>
      <td><p>Scegliere la modalità di visualizzazione delle date:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: il calendario visualizza l'oggetto in un'unica data.</li>
        <li><strong>[!UICONTROL Duration] (dall'inizio alla fine)</strong>: il calendario visualizza l'oggetto in un intervallo di giorni.<br><p>Nota: se si sceglie <strong>[!UICONTROL Durata]</strong>, la data di fine specificata deve essere successiva alla data di inizio, altrimenti l'elemento non verrà visualizzato nel calendario.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Date personalizzate]</strong></td>
      <td><p>Immettere il nome di data personalizzato associato all'oggetto che si desidera monitorare.</p><p><strong>NOTA:</strong> la ricerca del nome di data personalizzato è limitata a 50 risultati per evitare problemi di prestazioni.</td>
     </tr>
    </tbody>
   </table>

1. Passare alla sezione seguente.

### Aggiungere oggetti al gruppo di elementi

Dopo aver impostato la modalità di visualizzazione degli elementi, è necessario aggiungere al raggruppamento gli oggetti che si desidera visualizzare nel calendario.

1. In **[!UICONTROL Cosa aggiungere al calendario?]** sezione, seleziona

   * **[!UICONTROL Attività]**
   * **[!UICONTROL Progetti]**
   * **[!UICONTROL Problemi]**

1. Fai clic su **[!UICONTROL Aggiungi attività]**, **[!UICONTROL Aggiungi progetti]**, **[!UICONTROL Aggiungi problemi]** o **Indisponibilità** a seconda del tipo di oggetto che stai aggiungendo al calendario.

1. Nel menu a discesa, iniziare a digitare il nome del campo, quindi selezionare l&#39;origine del campo dell&#39;oggetto che si desidera visualizzare nel calendario, ad esempio **[!UICONTROL Attività in ritardo]**.
1. Imposta un&#39;istruzione di condizione per il raggruppamento del calendario.


   Per informazioni sull&#39;impostazione delle condizioni, vedere [Filtri e modificatori di condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   ![Seleziona l&#39;oggetto per il calendario](assets/calendar-field-name.png)

1. (Facoltativo) Specificare oggetti aggiuntivi per il raggruppamento del calendario ripetendo i passaggi da 1 a 4.
1. Nel campo **[!UICONTROL Imposta le etichette Attività/Progetti/Problemi come campo...]**, seleziona l&#39;etichetta degli oggetti in questo raggruppamento di calendari nel calendario.

   >[!NOTE]
   >
   >Se le opzioni predefinite dell&#39;etichetta non sono disponibili per un determinato oggetto, viene visualizzato il nome dell&#39;oggetto. Ad esempio, quando l&#39;etichetta [!UICONTROL Attività padre] è selezionata e non è associata alcuna attività padre all&#39;oggetto, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto visualizzato nel calendario.

   ![imposta etichette attività](assets/set-task-labels.png)
1. Fai clic su **[!UICONTROL Salva]**.

