---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Aggiornare le informazioni nel diagramma di Gantt elenco attività
description: Il Diagramma di Gantt di un elenco di attività di Adobe Workfront mostra i dettagli relativi alle attività presenti in un progetto o in un modello.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Aggiorna le informazioni nell&#39;elenco attività [!UICONTROL Grafico di Gantt]

<!--Audited: 08/2025-->

Il [!UICONTROL Grafico di Gantt] di un elenco di attività di Adobe Workfront mostra i dettagli relativi alle attività presenti in un progetto o in un modello.

In un modello, l&#39;elenco delle attività [!UICONTROL Grafico di Gantt] riflette gli aggiornamenti effettuati nell&#39;elenco delle attività del modello a livello di attività del modello. Impossibile modificare il [!UICONTROL diagramma di Gantt] associato a un modello.

In un progetto è possibile aggiornare le informazioni sull&#39;attività direttamente nell&#39;elenco delle attività [!UICONTROL Diagramma di Gantt].

In questo articolo vengono descritte le azioni seguenti che è possibile eseguire direttamente nell&#39;Elenco attività [!UICONTROL Grafico di Gantt]:

* Modifica durata attività
* Crea o rimuovi relazioni predecessore
* Modifica delle date di inizio e fine dell&#39;attività
* Percentuale di completamento aggiornamento
* Livella risorse progetto

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso a progetti e attività tramite [!UICONTROL Edit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al progetto e alle attività</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project and tasks </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Modifica durata attività

1. Vai al progetto che desideri modificare.
1. Fai clic su **[!UICONTROL Attività]** nel pannello a sinistra.

   ![Area attività](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Fai clic sull&#39;icona **[!UICONTROL Grafico di Gantt]**.

   ![Fare clic sull&#39;icona Diagramma di Gantt](assets/click-gantt-chart-icon.png)

   Tutte le modifiche vengono salvate automaticamente quando l&#39;opzione **[!UICONTROL Salvataggio automatico]** è abilitata. Questa opzione è abilitata per impostazione predefinita.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![Impostazione manuale abilitata](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Passa il puntatore del mouse sulla sequenza temporale di un&#39;attività e trascina l&#39;indicatore della sequenza temporale su una data diversa.
1. Rilasciare l&#39;indicatore quando è stata raggiunta la nuova data di completamento corretta per l&#39;attività.
1. (Facoltativo e condizionale) Se hai selezionato di salvare manualmente le modifiche, fai clic sulle icone **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripristina]** se desideri annullare o duplicare le modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel diagramma di Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: utilizzare [!UICONTROL Comando + Z] per annullare e [!UICONTROL Comando + Maiusc + Z] per ripetere.
   >   * [!DNL Windows]: utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] per ripetere.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Crea o rimuovi relazioni predecessori

1. Vai al progetto che desideri modificare.
1. Nell&#39;area **[!UICONTROL Attività]** fare clic sull&#39;icona **[!UICONTROL Grafico di Gantt]**.

   L&#39;opzione **[!UICONTROL Salvataggio automatico]** è selezionata per impostazione predefinita, nel qual caso tutte le modifiche vengono salvate automaticamente.

   ![Fare clic sull&#39;icona Diagramma di Gantt](assets/click-gantt-chart-icon.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![Impostazione manuale abilitata](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Per creare una relazione predecessore, fare clic sul punto iniziale di un&#39;attività e trascinarla fino al punto finale dell&#39;attività.
1. Per eliminare una relazione predecessore, fare clic su una riga predecessore che connette due attività per selezionarla, quindi premere **[!UICONTROL Elimina]** sulla tastiera.\
   ![Elimina_predecessore.png](assets/delete-predecessor-350x152.png)

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sulle icone **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripristina]** se desideri annullare o duplicare le modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel diagramma di Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: utilizzare [!UICONTROL Comando + Z] per annullare e [!UICONTROL Comando + Maiusc + Z] per ripetere.
   >   * [!DNL Windows]: [!UICONTROL Utilizzare Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] per ripetere.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]**.

## Modifica delle date di inizio e fine dell&#39;attività

1. Vai al progetto che desideri modificare.
1. Nell&#39;area **[!UICONTROL Attività]** fare clic sull&#39;icona **[!UICONTROL Grafico di Gantt]**.

   Tutte le modifiche vengono salvate automaticamente quando l&#39;opzione **[!UICONTROL Salvataggio automatico]** è abilitata. Questa opzione è abilitata per impostazione predefinita.

   ![Fare clic sull&#39;icona Diagramma di Gantt](assets/click-gantt-chart-icon.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   ![Impostazione manuale abilitata](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Posizionare il puntatore del mouse sul centro dell&#39;operazione e individuare la freccia multidirezionale.
1. Fare clic e trascinare l&#39;attività fino alla data desiderata.

   ![Modifica_data_finale.png](assets/change-start-end-date.png)

1. Se si modifica la data dell&#39;attività in modo da influire sul vincolo dell&#39;attività, fare clic su **[!UICONTROL Accetta]** per confermare la modifica del vincolo dell&#39;attività.

   >[!NOTE]
   >
   >Se l&#39;attività presenta uno dei seguenti vincoli, il sistema aggiorna il [!UICONTROL Vincolo attività] in [!UICONTROL Iniziare non prima] rispetto a se il progetto è pianificato dalla [!UICONTROL Data inizio] o [!UICONTROL Finire non oltre il] se il progetto è pianificato dalla [!UICONTROL Data completamento]:
   >
   >   
   >   
   >   * [!UICONTROL Il Prima Possibile]
   >   * [!UICONTROL Più Tardi Possibile]
   >   * [!UICONTROL Primo Orario Disponibile]
   >   * [!UICONTROL Ultimo Orario Disponibile]
   >   
   >   
   >In alcuni casi, le relazioni dei predecessori potrebbero impedire che le attività vengano avviate prima e lo spostamento non è consentito.

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sulle icone **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripristina]** se desideri annullare o duplicare le modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: utilizzare [!UICONTROL Comando + Z] per annullare e [!UICONTROL Comando + Maiusc + Z] per ripetere.
   >   * [!DNL Windows]: utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] per ripetere.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]**.

## Percentuale di completamento aggiornamento

1. Vai al progetto che desideri modificare.
1. Nell&#39;area **[!UICONTROL Attività]** fare clic sull&#39;icona **[!UICONTROL Grafico di Gantt]**.

   ![Fare clic sull&#39;icona Diagramma di Gantt](assets/click-gantt-chart-icon.png)

   Tutte le modifiche vengono salvate automaticamente quando l&#39;opzione **[!UICONTROL Salvataggio automatico]** è abilitata. Questa opzione è abilitata per impostazione predefinita.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Modalità pianificazione]** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.
1. Fare doppio clic sul numero percentuale all&#39;interno dell&#39;attività e immettere il numero.

   >[!IMPORTANT]
   >
   >Per aggiornare la percentuale di completamento, nella finestra di dialogo [!UICONTROL Opzioni] deve essere selezionato [!UICONTROL % Completato]. A tale scopo, fare clic sull&#39;icona **[!UICONTROL Opzioni]** e selezionare **[!UICONTROL % Completato]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Facoltativo e condizionale) Se hai selezionato di salvare le modifiche manualmente, fai clic sulle icone **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripristina]** se desideri annullare o duplicare le modifiche.

   >[!TIP]
   >
   >È possibile utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche nel [!UICONTROL Diagramma di Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: utilizzare [!UICONTROL Comando + Z] per annullare e [!UICONTROL Comando + Maiusc + Z] per ripetere.
   >   * [!DNL Windows]: utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] per ripetere.
   >   
   >

1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

## Livellare le risorse del progetto

È possibile utilizzare l&#39;Elenco attività [!UICONTROL Grafico di Gantt] per livellare le risorse.

Per informazioni sul livellamento delle risorse nel [!UICONTROL Diagramma di Gantt], vedere [Livellare le risorse nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

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
