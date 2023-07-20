---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Aggiorna informazioni nell'elenco delle attività Diagramma di Gantt
description: Nell'elenco delle attività Diagramma di Gantt vengono visualizzati i dettagli relativi alle attività presenti in un progetto o modello.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 1%

---

# Aggiorna informazioni nell&#39;elenco delle attività [!UICONTROL Diagramma di Gantt]

Elenco delle attività [!UICONTROL Diagramma di Gantt] mostra i dettagli sulle attività presenti in un progetto o modello.

In un modello, l&#39;elenco delle attività [!UICONTROL Diagramma di Gantt] riflette gli aggiornamenti effettuati nell&#39;elenco delle attività del modello a livello di attività. Impossibile modificare il [!UICONTROL Diagramma di Gantt] associato a un modello.

In un progetto è possibile aggiornare le informazioni sull&#39;attività direttamente nell&#39;elenco delle attività [!UICONTROL Diagramma di Gantt].

In questo articolo vengono descritte le azioni seguenti che è possibile eseguire direttamente nell&#39;Elenco attività [!UICONTROL Diagramma di Gantt]:

* Modifica durata attività
* Crea o rimuovi relazioni predecessore
* Modifica delle date di inizio e fine dell&#39;attività
* Percentuale di completamento aggiornamento
* Livella risorse progetto

## Requisiti di accesso

Per seguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso a progetti e attività tramite [!UICONTROL Edit]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al progetto e alle attività </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Modifica durata attività

1. Vai al progetto che desideri modificare.
1. Clic **[!UICONTROL Attività]** nel pannello a sinistra.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Fai clic su **[!UICONTROL Diagramma di Gantt]** icona.

   ![Fai clic sull’icona Diagramma di Gantt](assets/click-gantt-chart-icon.png)

   Tutte le modifiche vengono salvate automaticamente quando **[!UICONTROL Salvataggio automatico]** l&#39;opzione è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic su **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Passa il puntatore del mouse sulla sequenza temporale di un&#39;attività e trascina l&#39;indicatore della sequenza temporale su una data diversa.
1. Rilasciare l&#39;indicatore quando è stata raggiunta la nuova data di completamento corretta per l&#39;attività.
1. (Facoltativo e condizionale) Se hai selezionato di salvare manualmente le modifiche, fai clic sul pulsante **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripeti]** se si desidera annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel diagramma di Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzare [!UICONTROL Comando+Z] per annullare e [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] da ripristinare.
   >   
   >

1. Clic **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Crea o rimuovi relazioni predecessori

1. Vai al progetto che desideri modificare.
1. In **[!UICONTROL Attività]** , fare clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona.

   Il **[!UICONTROL Salvataggio automatico]** è selezionata per impostazione predefinita, nel qual caso tutte le modifiche vengono salvate automaticamente.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Facoltativo) Fai clic su **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Per creare una relazione predecessore, fare clic sul punto iniziale di un&#39;attività e trascinarla fino al punto finale dell&#39;attività.
1. Per eliminare una relazione predecessore, fare clic su una linea predecessore che collega due attività per selezionarla, quindi premere **[!UICONTROL Elimina]** sulla tastiera.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sul pulsante **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripeti]** se si desidera annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel diagramma di Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzare [!UICONTROL Comando+Z] per annullare e [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: [!UICONTROL Usa Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] da ripristinare.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]** .

## Modifica delle date di inizio e fine dell&#39;attività

1. Vai al progetto che desideri modificare.
1. In **[!UICONTROL Attività]** , fare clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona.

   Tutte le modifiche vengono salvate automaticamente quando **[!UICONTROL Salvataggio automatico]** l&#39;opzione è abilitata. È attivata per impostazione predefinita.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Facoltativo) Fai clic su **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Posizionare il puntatore del mouse sul centro dell&#39;operazione e individuare la freccia multidirezionale.
1. Fare clic e trascinare l&#39;attività fino alla data desiderata.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Se si modifica la data dell&#39;attività in modo da influire sul vincolo dell&#39;attività, fare clic su **[!UICONTROL Accetta]** per confermare la modifica del vincolo attività.

   >[!NOTE]
   >
   >Se l&#39;attività presenta uno dei seguenti vincoli, il sistema aggiorna [!UICONTROL Vincolo attività] a [!UICONTROL Iniziare non prima] Se il progetto è pianificato dalla [!UICONTROL Data di inizio] o [!UICONTROL Finire non Dopo di] se il progetto è programmato da [!UICONTROL Data di completamento]:
   >
   >   
   >   
   >   * [!UICONTROL Più Presto Possibile]
   >   * [!UICONTROL Più Tardi Possibile]
   >   * [!UICONTROL Primo Orario Disponibile]
   >   * [!UICONTROL Ultimo Orario Disponibile]
   >   
   >   
   >In alcuni casi, le relazioni dei predecessori potrebbero impedire che le attività vengano avviate prima e lo spostamento non è consentito.

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sul pulsante **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripeti]** se si desidera annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Per annullare o ripristinare le modifiche apportate al [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzare [!UICONTROL Comando+Z] per annullare e [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] da ripristinare.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]**.

## Percentuale di completamento aggiornamento

1. Vai al progetto che desideri modificare.
1. In **[!UICONTROL Attività]** , fare clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   Tutte le modifiche vengono salvate automaticamente quando **[!UICONTROL Salvataggio automatico]** l&#39;opzione è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic su **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.
1. Fare doppio clic sul numero percentuale all&#39;interno dell&#39;attività e immettere il numero.

   >[!IMPORTANT]
   >
   >Devi avere [!UICONTROL % completamento] selezionato in [!UICONTROL Opzioni] per aggiornare la percentuale di completamento. A questo scopo, fai clic su **[!UICONTROL Opzioni]** e seleziona **[!UICONTROL % completamento]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sul pulsante **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripeti]** se si desidera annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Per annullare o ripristinare le modifiche apportate al [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilizzare [!UICONTROL Comando+Z] per annullare e [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >   * [!DNL Windows]: Utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] da ripristinare.
   >   
   >

1. Clic **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Livellare le risorse del progetto

È possibile utilizzare l&#39;Elenco attività [!UICONTROL Diagramma di Gantt] per livellare le risorse.

Per informazioni sul livellamento delle risorse in [!UICONTROL Diagramma di Gantt], vedi [Livellare le risorse in [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

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
