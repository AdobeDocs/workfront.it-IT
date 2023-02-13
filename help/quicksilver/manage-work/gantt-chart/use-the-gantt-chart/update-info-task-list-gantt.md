---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Aggiornare le informazioni nell'elenco delle attività Diagramma di Gantt
description: Elenco attività Diagramma di Gantt mostra i dettagli relativi alle attività presenti in un progetto o in un modello.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 1%

---

# Aggiornare le informazioni nell’elenco delle attività [!UICONTROL Diagramma di Gantt]

Elenco attività [!UICONTROL Diagramma di Gantt] mostra i dettagli sulle attività presenti in un progetto o modello.

In un modello, l&#39;elenco delle attività [!UICONTROL Diagramma di Gantt] riflette gli aggiornamenti effettuati nell&#39;elenco delle attività del modello a livello di attività. Non è possibile modificare il [!UICONTROL Diagramma di Gantt] associato a un modello.

In un progetto, è possibile aggiornare le informazioni sulle attività direttamente nell&#39;elenco delle attività [!UICONTROL Diagramma di Gantt].

In questo articolo vengono descritte le seguenti azioni che è possibile eseguire direttamente nell’Elenco attività [!UICONTROL Diagramma di Gantt]:

* Modifica durata attività
* Creare o rimuovere relazioni predecessori
* Modifica date di inizio e fine attività
* Aggiornamento percentuale completato
* Risorse del progetto a livello di livello

## Requisiti di accesso

Devi disporre dei seguenti elementi per seguire i passaggi descritti in questo articolo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti e attività tramite modifica</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso al progetto e alle attività di gestione </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Modifica durata attività

1. Passa al progetto da modificare.
1. Fai clic su **[!UICONTROL Attività]** nel pannello a sinistra.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Fai clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   Tutte le modifiche vengono salvate automaticamente quando la **[!UICONTROL Salvataggio automatico]** è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Modalità di pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale Standard]** o **[!UICONTROL Pianificazione temporale]** per salvare manualmente le modifiche.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Passa il cursore del mouse sulla timeline di un’attività e trascina l’indicatore della linea temporale in una data diversa.
1. Rilasciare l&#39;indicatore quando è stata raggiunta la nuova data di completamento corretta per l&#39;attività.
1. (Facoltativo e condizionale) Se hai selezionato per salvare manualmente le modifiche, fai clic sul pulsante **[!UICONTROL Annulla]** o &#x200B;**[!UICONTROL Ripeti]** per annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Per annullare o ripristinare le modifiche nel diagramma di Gantt è possibile utilizzare le seguenti scelte rapide da tastiera:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzo [!UICONTROL Comando + Z] annullare [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzo [!UICONTROL Ctrl+Z] annullare [!UICONTROL Ctrl+Y] da ripristinare.


1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Creare o rimuovere relazioni predecessori

1. Passa al progetto da modificare.
1. In **[!UICONTROL Attività]** fai clic sull’area **[!UICONTROL Diagramma di Gantt]** icona.

   La **[!UICONTROL Salvataggio automatico]** è selezionata per impostazione predefinita, in tal caso tutte le modifiche vengono salvate automaticamente.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Modalità di pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale Standard]** o **[!UICONTROL Pianificazione temporale]** per salvare manualmente le modifiche.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Per creare una relazione predecessore, fare clic sul punto iniziale di un&#39;attività e trascinarla nel punto finale dell&#39;attività.
1. Per eliminare una relazione predecessore, fare clic su una riga predecessore che connette due attività per selezionarla, quindi premere **[!UICONTROL Elimina]** sulla tastiera.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Facoltativo e condizionale) Se hai selezionato per salvare manualmente le modifiche, fai clic sul pulsante **[!UICONTROL Annulla]** o &#x200B;**[!UICONTROL Ripeti]** per annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Per annullare o ripristinare le modifiche nel diagramma di Gantt è possibile utilizzare le seguenti scelte rapide da tastiera:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzo [!UICONTROL Comando + Z] annullare [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: [!UICONTROL Usa Ctrl+Z] annullare [!UICONTROL Ctrl+Y] da ripristinare.


1. Fai clic su **[!UICONTROL Salva]** .

## Modifica date di inizio e fine attività

1. Passa al progetto da modificare.
1. In **[!UICONTROL Attività]** fai clic sull’area **[!UICONTROL Diagramma di Gantt]** icona.

   Tutte le modifiche vengono salvate automaticamente quando la **[!UICONTROL Salvataggio automatico]** è abilitata. È attivata per impostazione predefinita.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Modalità di pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale Standard]** o **[!UICONTROL Pianificazione temporale]** per salvare manualmente le modifiche.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Passa il puntatore del mouse sopra il centro dell’attività e individua la freccia multidirezionale.
1. Fai clic su e trascina l’attività fino alla data desiderata.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Se si modifica la data dell&#39;attività in modo da influenzare il vincolo dell&#39;attività, fare clic su **[!UICONTROL Accetta]** per confermare la modifica del vincolo dell&#39;attività.

   >[!NOTE]
   >
   >Se l&#39;attività presenta uno dei seguenti vincoli, il sistema aggiorna il [!UICONTROL Vincolo attività] a [!UICONTROL Inizia non prima] Than se il progetto è pianificato dal [!UICONTROL Data di inizio] o [!UICONTROL Fine entro] se il progetto è pianificato dalla [!UICONTROL Data completamento]:
   >
   >   
   >   
   >   * [!UICONTROL Più Presto Possibile]
   >   * [!UICONTROL Più Tardi Possibile]
   >   * [!UICONTROL Primo Orario Disponibile]
   >   * [!UICONTROL Ultimo Orario Disponibile]

   >   
   >   
   >In alcuni casi, le relazioni predecessori potrebbero impedire l&#39;avvio precedente delle attività e lo spostamento delle attività non è consentito.

1. (Facoltativo e condizionale) Se hai selezionato per salvare manualmente le modifiche, fai clic sul pulsante **[!UICONTROL Annulla]** o &#x200B;**[!UICONTROL Ripeti]** per annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Puoi utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche in [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzo [!UICONTROL Comando + Z] annullare [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzo [!UICONTROL Ctrl+Z] annullare [!UICONTROL Ctrl+Y] da ripristinare.


1. Fai clic su **[!UICONTROL Salva]**.

## Aggiornamento percentuale completato

1. Passa al progetto da modificare.
1. In **[!UICONTROL Attività]** fai clic sull’area **[!UICONTROL Diagramma di Gantt]** icona.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   Tutte le modifiche vengono salvate automaticamente quando la **[!UICONTROL Salvataggio automatico]** è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Modalità di pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale Standard]** o **[!UICONTROL Pianificazione temporale]** per salvare manualmente le modifiche.
1. Fare doppio clic sul numero di percentuale all&#39;interno dell&#39;attività e immettere il numero.

   >[!IMPORTANT]
   >
   >Devi avere [!UICONTROL % completato] selezionato in [!UICONTROL Opzioni] per aggiornare la percentuale di completamento. A questo scopo, fai clic sul pulsante **[!UICONTROL Opzioni]** e seleziona **[!UICONTROL % completato]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >

1. (Facoltativo e condizionale) Se hai selezionato per salvare manualmente le modifiche, fai clic sul pulsante **[!UICONTROL Annulla]** o &#x200B;**[!UICONTROL Ripeti]** per annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Puoi utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche in [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzo [!UICONTROL Comando + Z] annullare [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzo [!UICONTROL Ctrl+Z] annullare [!UICONTROL Ctrl+Y] da ripristinare.


1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Risorse di progetto a livello di livello

È possibile utilizzare l’elenco delle attività [!UICONTROL Diagramma di Gantt] per livellare le risorse.

Per informazioni sul livellamento delle risorse nel [!UICONTROL Diagramma di Gantt], vedi [Livello di risorse nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
