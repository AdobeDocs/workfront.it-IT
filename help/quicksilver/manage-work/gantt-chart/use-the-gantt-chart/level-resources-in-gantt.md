---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Livellare le risorse in  [!UICONTROL Diagramma di Gantt]
description: Informazioni su come livellare le risorse nel Diagramma di Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Livellare le risorse in [!UICONTROL Diagramma di Gantt]

Il livellamento delle risorse su un progetto ha due scopi:

* Per regolare automaticamente la sovrassegnazione di tempo per gli assegnatari.
* Per creare automaticamente una programmazione realistica delle attività per un progetto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso [!UICONTROL Edit] ai progetti</p> <p><b>NOTA</b>

Se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Panoramica sul livellamento delle risorse

Se la stessa risorsa viene assegnata a due attività diverse, è possibile utilizzare il livellamento delle risorse per modificare la cronologia delle attività in modo che non vengano eseguite contemporaneamente.

Quando si livellano le risorse in un progetto, considera quanto segue:

* Il livellamento delle risorse si applica solo a un progetto, quindi [!DNL Adobe Workfront] non livella le risorse in più progetti alla volta.
* Se **[!UICONTROL Impegno]** è selezionato come **[!UICONTROL Tipo di durata]**, [!DNL Workfront] non livella le risorse.
* Quando più utenti vengono assegnati alla stessa attività, il livellamento verrà annullato.
* Condizioni per il tipo di **[!UICONTROL Vincolo attività]** avrà la precedenza sul livellamento delle risorse. Ad esempio, se **[!UICONTROL Date Fisse]** è selezionato come [!UICONTROL Vincolo attività], il livellamento delle risorse non modificherà le date delle attività.
* Le relazioni con i predecessori avranno la precedenza sul livellamento delle risorse.
* **[!UICONTROL Livellamento risorse]** deve essere impostato su **[!UICONTROL Manuale]** per il progetto al fine di regolare il livellamento nel [!UICONTROL Diagramma di Gantt]. Se disponi delle autorizzazioni di gestione per il progetto, puoi far sì che il sistema livelli automaticamente le risorse regolando questa impostazione sul progetto e selezionando **[!UICONTROL Automatico]** invece di **[!UICONTROL Manuale]** nel **[!UICONTROL Modifica Progetto]** casella.

  ![](assets/resource-leveling-mode-350x177.png)

* In qualità di proprietario del progetto o di assegnatario dell&#39;attività, è possibile introdurre un ritardo di livellamento per un&#39;attività per indicare che è molto probabile che l&#39;attività richieda più tempo. Per informazioni sull&#39;aggiunta di un ritardo di livellamento a un&#39;attività, vedere [Ritardo livellamento attività di aggiornamento](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Applicare il livellamento delle risorse in [!UICONTROL Diagramma di Gantt]

È possibile utilizzare l&#39;Elenco attività [!UICONTROL Diagramma di Gantt] per livellare le risorse.

1. Vai al progetto che desideri livellare.
1. In **[!UICONTROL Attività]** , fare clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona.

   Tutte le modifiche vengono salvate automaticamente quando **[!UICONTROL Salvataggio automatico]** l&#39;opzione è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic su **[!UICONTROL Piano] modalità** e seleziona **[!UICONTROL Salvataggio manuale standard]** o **[!UICONTROL Pianificazione sequenza temporale]** per salvare le modifiche manualmente.

   >[!TIP]
   >
   >Non è possibile livellare le risorse in  [!UICONTROL Diagramma di Gantt] quando [!UICONTROL Salvataggio automatico] l&#39;opzione è abilitata.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Fai clic su **[!UICONTROL Livella Risorse]** menu a discesa.

   ![Level_resources.png](assets/level-resouces.png)

1. Selezionare una delle opzioni seguenti:

   * **[!UICONTROL Livella ora]**: applica il livellamento delle risorse all&#39;attività selezionata.
   * **[!UICONTROL Cancella livellamento]**: rimuove tutti i livelli di risorse dall’attività selezionata.

   >[!NOTE]
   >
   >Le risorse potrebbero essere sovrassegnate se assegnate a più attività che si verificano nello stesso intervallo di tempo.

1. (Facoltativo e condizionale) Se hai disabilitato l’opzione Salvataggio automatico, fai clic sul pulsante **[!UICONTROL Annulla]** o&#x200B;**[!UICONTROL Ripeti]** se si desidera annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Per annullare o ripristinare le modifiche apportate al [!UICONTROL Diagramma di Gantt]:
   >
   >* [!DNL Mac]: Utilizzare [!UICONTROL Comando+Z] per annullare e [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >* Windows: utilizzare [!UICONTROL Ctrl + Z] per annullare e [!UICONTROL Ctrl + Y] da ripristinare.


1. Clic **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
