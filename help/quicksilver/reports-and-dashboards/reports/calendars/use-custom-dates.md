---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare campi data personalizzati in un report calendario
description: Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per attività, problemi e progetti.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 1%

---

# Utilizzare campi data personalizzati in un report calendario

Un report [!UICONTROL calendar] è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per i seguenti oggetti:

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
   <td> <p>Accesso di [!UICONTROL Edit] a [!UICONTROL Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendars]</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al report calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

1. È necessario disporre di campi data personalizzati e di un valore all&#39;interno del campo disponibile nell&#39;istanza [!DNL Workfront]. Se non si dispone di un modulo personalizzato con date personalizzate, seguire le istruzioni in [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Allegare il modulo personalizzato a un progetto, un&#39;attività o un problema che si intende aggiungere al calendario e specificare una data. Per ulteriori informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Calendari]**.

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
   >Se le opzioni predefinite dell&#39;etichetta non sono disponibili per un determinato oggetto, viene visualizzato il nome dell&#39;oggetto. Ad esempio, quando l&#39;etichetta [!UICONTROL Attività padre] è selezionata e non è associata alcuna attività padre all&#39;oggetto, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto visualizzato nel calendario.

1. Fai clic su **[!UICONTROL Salva]**.
