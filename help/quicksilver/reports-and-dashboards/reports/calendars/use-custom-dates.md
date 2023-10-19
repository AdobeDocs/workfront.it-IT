---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare campi data personalizzati in un report calendario
description: Un report calendario è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per attività, problemi e progetti.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# Utilizzare campi data personalizzati in un report calendario

A [!UICONTROL calendario] report è un report dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un report calendario per i seguenti oggetti:

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
   <td> <p>Accesso di [!UICONTROL Edit] a [!UICONTROL Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendars]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al report calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

1. Devi avere campi data personalizzati e un valore all’interno del campo disponibile nel tuo [!DNL Workfront] dell&#39;istanza. Se non hai impostato un modulo personalizzato con date personalizzate, segui le istruzioni riportate nelle prime due sezioni di [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Allegare il modulo personalizzato a un progetto, un&#39;attività o un problema che si intende aggiungere al calendario e specificare una data. Per ulteriori informazioni, consulta [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Calendari]**.

1. Selezionare il calendario a cui si desidera aggiungere un nuovo gruppo di elementi.\
   Oppure\
   Clic **[!UICONTROL + Nuovo calendario]** e inserisci il nome del calendario.

   >[!NOTE]
   >
   >Devi avere [!UICONTROL Modifica] accesso a [!UICONTROL Rapporti], [!UICONTROL Dashboard], e [!UICONTROL Calendari] nel tuo livello di accesso per creare un rapporto sul calendario.

1. A sinistra, fai clic su **[!UICONTROL Aggiungi al calendario]**, quindi fai clic su **[!UICONTROL Aggiungi elementi avanzati]**.

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
      <td>Scegli <strong>[!UICONTROL Date personalizzate]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nel calendario, mostra]</strong></td>
      <td><p>Scegliere la modalità di visualizzazione delle date:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: il calendario visualizza l’oggetto in un’unica data.</li>
        <li><strong>[!UICONTROL Duration] (dall'inizio alla fine)</strong>: il calendario visualizza l’oggetto in un arco di giorni.<br><p>Nota: se si sceglie <strong>[!UICONTROL Duration]</strong>, la data di fine specificata deve essere successiva alla data di inizio, altrimenti l'elemento non verrà visualizzato nel calendario.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Date personalizzate]</strong></td>
      <td><p>Immettere il nome di data personalizzato associato all'oggetto che si desidera monitorare.</p><p><strong>NOTA:</strong> La ricerca del nome della data personalizzata è limitata a 50 risultati per evitare problemi di prestazioni.</td>
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

1. Clic **[!UICONTROL Aggiungi attività]**, **[!UICONTROL Aggiungi progetti]**, o **[!UICONTROL Aggiungi problemi]**, a seconda del tipo di oggetto che si sta aggiungendo al calendario.\
   ![Seleziona oggetto per calendario](assets/field-name.png)

1. Nel menu a discesa, iniziare a digitare il nome del campo, quindi selezionare l&#39;origine del campo dell&#39;oggetto che si desidera visualizzare nel calendario (ad esempio, **[!UICONTROL Attività in ritardo]**).
1. Imposta un&#39;istruzione di condizione per il raggruppamento del calendario.

   ![Istruzione condizione](assets/condition-statement-calendar.png)

   Per informazioni sull&#39;impostazione delle condizioni, vedere [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facoltativo) Specificare oggetti aggiuntivi per il raggruppamento del calendario ripetendo i passaggi da 1 a 4.
1. In **[!UICONTROL Imposta le etichette Attività/Progetti/Problemi su...]** , selezionare il modo in cui gli oggetti del raggruppamento del calendario vengono etichettati nel calendario.

   >[!NOTE]
   >
   >Se le opzioni predefinite dell&#39;etichetta non sono disponibili per un determinato oggetto, viene visualizzato il nome dell&#39;oggetto. Ad esempio, quando [!UICONTROL Attività padre] l&#39;etichetta è selezionata e all&#39;oggetto non è associata alcuna attività padre, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto che si sta visualizzando nel calendario.

1. Fai clic su **[!UICONTROL Salva]**.
