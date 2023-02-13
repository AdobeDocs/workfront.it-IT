---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Livello di risorse nel  [!UICONTROL Diagramma di Gantt]
description: Informazioni su come livellare le risorse nel Diagramma di Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Livello di risorse nel [!UICONTROL Diagramma di Gantt]

Il livellamento delle risorse su un progetto ha due scopi:

* Per regolare automaticamente l&#39;allocazione eccessiva del tempo per gli assegnatari.
* Creazione automatica di una pianificazione delle attività realistica per un progetto

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti con [!UICONTROL Edit]</p> <p><b>NOTA</b>

Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso a [!UICONTROL Gestire] al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Panoramica del livellamento delle risorse

Se la stessa risorsa viene assegnata a due attività diverse, è possibile utilizzare il livellamento delle risorse per regolare la timeline delle attività in modo che non si verifichino contemporaneamente.

Quando livelli le risorse su un progetto, considera quanto segue:

* Il livellamento delle risorse si applica solo a un progetto, quindi [!DNL Adobe Workfront] non livella le risorse per più di un progetto alla volta.
* Se **[!UICONTROL Guida allo sforzo]** è selezionato come **[!UICONTROL Tipo di durata]**, [!DNL Workfront] non livella le risorse.
* Quando più utenti vengono assegnati alla stessa attività, il livellamento verrà annullato.
* Condizioni per il tipo di **[!UICONTROL Vincolo attività]** ha la precedenza sul livellamento delle risorse. Ad esempio, se **[!UICONTROL Date fisse]** è selezionato come [!UICONTROL Vincolo attività], il livellamento delle risorse non modificherà le date delle attività.
* Le relazioni predecessori avranno la precedenza sul livellamento delle risorse.
* **[!UICONTROL Livello risorse]** deve essere impostato su **[!UICONTROL Manuale]** per il progetto al fine di regolare il livellamento nel [!UICONTROL Diagramma di Gantt]. Se disponi delle autorizzazioni di gestione per il progetto, puoi fare in modo che il sistema livelli automaticamente le risorse regolando questa impostazione sul progetto e selezionando **[!UICONTROL Automatico]** anziché **[!UICONTROL Manuale]** in **[!UICONTROL Modifica progetto]** scatola.

   ![](assets/resource-leveling-mode-350x177.png)

* In qualità di proprietario del progetto o di assegnatario dell&#39;attività, è possibile introdurre un ritardo di livellamento per un&#39;attività per indicare che è molto probabile che l&#39;attività abbia bisogno di tempo aggiuntivo. Per informazioni sull&#39;aggiunta di un ritardo di livellamento a un&#39;attività, vedere [Aggiorna ritardo livellamento attività](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Applica il livellamento delle risorse nel [!UICONTROL Diagramma di Gantt]

È possibile utilizzare l’elenco delle attività [!UICONTROL Diagramma di Gantt] per livellare le risorse.

1. Passa al progetto da livellare.
1. In **[!UICONTROL Attività]** fai clic sull’area **[!UICONTROL Diagramma di Gantt]** icona.

   Tutte le modifiche vengono salvate automaticamente quando la **[!UICONTROL Salvataggio automatico]** è abilitata. È attivata per impostazione predefinita.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Pianificare] modalità** e seleziona **[!UICONTROL Salvataggio manuale Standard]** o **[!UICONTROL Pianificazione temporale]** per salvare manualmente le modifiche.

   >[!TIP]
   >
   >Non è possibile livellare le risorse nel  [!UICONTROL Diagramma di Gantt] quando [!UICONTROL Salvataggio automatico] è abilitata.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Fai clic sul pulsante **[!UICONTROL Risorse di livello]** menu a discesa.

   ![Level_resources.png](assets/level-resouces.png)

1. Selezionare una delle seguenti opzioni:

   * **[!UICONTROL Livello]**: Applica il livellamento delle risorse all&#39;attività selezionata.
   * **[!UICONTROL Cancella livellamento]**: Rimuove tutto il livellamento delle risorse dall’attività selezionata.

   >[!NOTE]
   >
   >Le risorse potrebbero essere sovrassegnate se assegnate a più attività che si verificano nello stesso intervallo di tempo.

1. (Facoltativo e condizionale) Se hai disattivato l’opzione Salvataggio automatico , fai clic sul pulsante **[!UICONTROL Annulla]** o &#x200B;**[!UICONTROL Ripeti]** per annullare o duplicare una delle modifiche.

   >[!TIP]
   >
   >Puoi utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare le modifiche in [!UICONTROL Diagramma di Gantt]:
   >
   >* [!DNL Mac]: Utilizzo [!UICONTROL Comando + Z] annullare [!UICONTROL Comando + Maiusc + Z] da ripristinare.
   >* Windows: Utilizzo [!UICONTROL Ctrl+Z] annullare [!UICONTROL Ctrl+Y] da ripristinare.



1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo superiore destro del [!UICONTROL Diagramma di Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p> <p> <img src="assets/qs-task-edit-icon-highlighted-350x154.png" style="width: 350;height: 154;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
