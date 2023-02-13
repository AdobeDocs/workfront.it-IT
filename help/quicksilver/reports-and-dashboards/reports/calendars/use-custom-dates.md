---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilizzare campi data personalizzati in un rapporto calendario
description: Un rapporto calendario è un rapporto dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un rapporto calendario per attività, problemi e progetti.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# Utilizzare campi data personalizzati in un rapporto calendario

A [!UICONTROL calendario] rapporto è un rapporto dinamico che fornisce una rappresentazione visiva del lavoro. È possibile utilizzare campi data personalizzati in un rapporto calendario per i seguenti oggetti:

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
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Accesso a [!UICONTROL Edit] e ai [!UICONTROL Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendars]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso a [!UICONTROL Gestisci] al report del calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

1. È necessario disporre di campi data personalizzati e di un valore all’interno del campo disponibile nel [!DNL Workfront] istanza. Se non si dispone di un modulo personalizzato impostato con date personalizzate, attenersi alle istruzioni contenute nelle prime due sezioni di [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Allegare il modulo personalizzato a un progetto, a un&#39;attività o a un problema che si prevede di aggiungere al calendario e specificare una data. Per ulteriori informazioni, consulta [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Imposta il gruppo di elementi

È possibile scegliere la modalità di visualizzazione del gruppo di elementi nel calendario.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Calendari]**.

1. Selezionare il calendario a cui si desidera aggiungere un nuovo gruppo di elementi.\
   Oppure\
   Fai clic su **[!UICONTROL + Nuovo calendario]** e immetti il nome del calendario.

   >[!NOTE]
   >
   >Devi avere [!UICONTROL Modifica] accesso [!UICONTROL Rapporti], [!UICONTROL Dashboard]e [!UICONTROL Calendari] nel livello di accesso per creare un rapporto sul calendario.

1. A sinistra, fai clic su **[!UICONTROL Aggiungi al calendario]**, quindi fai clic su **[!UICONTROL Aggiungi elementi avanzati]**.

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Denomina questo gruppo di elementi]</strong></td>
      <td>Digita un nome per il gruppo di elementi.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Selezionare un colore per il gruppo di elementi. Tutti gli elementi vengono visualizzati nel colore selezionato nel report del calendario.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campo data]</strong></td>
      <td>Scegli <strong>[!UICONTROL Date personalizzate]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Sul calendario, mostra]</strong></td>
      <td><p>Scegli come visualizzare le date:</p>
       <ul>
        <li><strong>[!UICONTROL Data singola]</strong>: Il calendario visualizza l'oggetto in una sola data.</li>
        <li><strong>[!UICONTROL Duration] (da inizio a fine)</strong>: Nel calendario l'oggetto viene visualizzato in un intervallo di giorni.<br><p>Nota: Se scegli <strong>[!UICONTROL Duration]</strong>, la data di fine specificata deve essere successiva alla data di inizio, altrimenti l'elemento non verrà visualizzato nel calendario.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Date personalizzate]</strong></td>
      <td><p>Immettere il nome della data personalizzato associato all'oggetto da tracciare.</p></td>
     </tr>
    </tbody>
   </table>

1. Procedi alla sezione seguente.

## Aggiungere oggetti al gruppo di elementi

Dopo aver impostato la modalità di visualizzazione degli elementi, è necessario aggiungere al raggruppamento gli oggetti che si desidera visualizzare nel calendario.

1. In **[!UICONTROL Cosa desideri aggiungere al calendario?]** sezione , seleziona

   * **[!UICONTROL Attività]**
   * **[!UICONTROL Progetti]**
   * **[!UICONTROL Problemi]**

1. Fai clic su **[!UICONTROL Aggiungi attività]**, **[!UICONTROL Aggiungi progetti]** oppure **[!UICONTROL Aggiungi problemi]**, a seconda del tipo di oggetto che si sta aggiungendo al calendario.\
   ![Selezionare l&#39;oggetto per il calendario](assets/field-name.png)

1. Nel menu a discesa, inizia a digitare il nome del campo, quindi seleziona l’origine del campo dell’oggetto da visualizzare nel calendario (ad esempio, **[!UICONTROL Attività in ritardo]**).
1. Imposta un&#39;istruzione condizione per il raggruppamento del calendario.

   ![Istruzione condizione](assets/condition-statement-calendar.png)

   Per informazioni sull’impostazione delle condizioni, consulta [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facoltativo) Specificare oggetti aggiuntivi per il raggruppamento del calendario ripetendo i passaggi 1-4.
1. In **[!UICONTROL Imposta le etichette Attività/Progetti/Problemi su...]** selezionare la modalità di etichettatura degli oggetti del raggruppamento di calendario nel calendario.

   >[!NOTE]
   >
   >Se le opzioni di etichetta predefinite non sono disponibili per un determinato oggetto, viene visualizzato il nome dell’oggetto. Ad esempio, quando [!UICONTROL Attività principale] l’etichetta è selezionata e non è presente alcuna attività principale associata all’oggetto, [!DNL Adobe Workfront] visualizza il nome dell&#39;oggetto visualizzato nel calendario.

1. Fai clic su **[!UICONTROL Salva]**.
