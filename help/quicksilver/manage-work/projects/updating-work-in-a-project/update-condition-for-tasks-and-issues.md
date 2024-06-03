---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna condizione per attività e problemi
description: La condizione di un’attività o di un problema è un flag applicato a tale attività o problema per indicarne la direzione. Diverso dallo stato dell'elemento di lavoro, che indica la fase corrente di sviluppo dell'elemento.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 1%

---

# Aggiorna condizione per attività e problemi

{{highlighted-preview}}

La condizione di un’attività o di un problema è un flag applicato a tale attività o problema per indicarne la direzione. Diverso dallo stato dell&#39;elemento di lavoro, che indica la fase corrente di sviluppo dell&#39;elemento.

È possibile impostare la condizione di un&#39;attività o di un problema in modo automatico o manuale.

I valori di Condizione a cui si fa riferimento in questo articolo sono disponibili in Workfront per impostazione predefinita. L’amministratore di Adobe Workfront può creare condizioni personalizzate per l’ambiente, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisiti di accesso {#access-requirements}

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>

Per le nuove licenze:
<ul><li><p>Standard per le attività</p></li>
   <li><p>Collaboratore o versione successiva per i problemi</p></li></ul>


Per le licenze correnti:
<ul><li><p>Lavoro o superiore per le attività</p></li>
   <li><p>Richiedi o superiore per problemi</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizzare o accedere ai progetti in modo più avanzato</p> <p>Modificare l’accesso ad attività e problemi </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi per visualizzarne la condizione</p>
   <p>Gestire le autorizzazioni su attività e problemi per aggiornare la condizione</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Per poter aggiornare manualmente la condizione di un’attività o un problema, devi esserti assegnato.

## Individuare la condizione delle attività e dei problemi

Le condizioni vengono visualizzate come flag associato ad attività o problemi. Possono anche essere associate a un numero che può essere visualizzato nei rapporti invece che nell’etichetta. Per ulteriori informazioni sull&#39;associazione delle condizioni ai numeri, vedere [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Puoi individuare la Condizione delle attività e dei problemi nelle seguenti aree di Workfront:

* <span class="preview">La pagina Dettagli, dopo che è stata aggiunta da un amministratore di Workfront o di gruppo al modello di layout. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md). </span>

* <span class="preview">L’intestazione di un’attività o di un problema, dopo che un amministratore di Workfront o di un gruppo l’ha aggiunta al modello di layout. Per informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). </span>

* Il pannello Riepilogo, dopo che un amministratore di Workfront o di gruppo lo ha aggiunto al modello di layout. Per informazioni, consulta [Personalizzare Home e Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Report ed elenchi quando si visualizza il campo Condizione in una visualizzazione o in un raggruppamento.

  >[!NOTE]
  >
  >Quando la parola &quot;condizione&quot; viene visualizzata nel campo Nome campo di un rapporto Voce diario, indica che la condizione di un elemento è stata aggiornata. Quando il campo Condizione viene tracciato nei rapporti Scritture contabili, i valori Nuovo e Vecchio numero visualizzano il numero associato alla condizione anziché il nome. Se per un&#39;attività o un problema non è stata originariamente definita una condizione e successivamente la si aggiorna, la voce del giornale di registrazione che acquisisce l&#39;aggiornamento visualizzerà il valore Numero precedente del campo Condizione come -2.147.483.648.

## Aggiorna automaticamente la condizione aggiornando lo stato

Quando ti viene assegnata un’attività o un problema e fai clic su **Lavoraci** , Avvia attività o Avvia problema, o aggiornarne lo stato, la Condizione dell’attività o del problema cambia automaticamente con la Condizione predefinita associata a **Senza problemi**.

Per informazioni sull&#39;utilizzo di una condizione personalizzata come condizione predefinita, vedere gli articoli  [Impostare una condizione personalizzata come predefinita per le attività e i problemi](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) e [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Per informazioni sulla modifica dello stato dell&#39;attività, vedere [Aggiorna stato attività](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Per informazioni sulla modifica dello stato del problema, vedere [Aggiorna stato problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Per informazioni sull&#39;impostazione del pulsante Lavoraci su un pulsante Avvia attività o Avvia problema, vedere [Sostituire il pulsante Lavoraci con un pulsante Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Aggiorna manualmente la condizione

È necessario essere assegnati a un&#39;attività o al problema o disporre delle autorizzazioni di gestione per potervi impostare la condizione.

È possibile aggiornare manualmente la condizione di un&#39;attività o di un problema in un report o elenco di attività o problemi quando si visualizza il campo Condizione nella visualizzazione.

>[!NOTE]
>
>È possibile chiedere all&#39;amministratore del sistema o del gruppo di aggiungere il campo Condizione al pannello Riepilogo per semplificarne l&#39;aggiornamento in varie aree di Workfront.
>
>Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizzare Home e Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Per aggiornare manualmente la condizione di un’attività o di un problema, effettua una delle seguenti operazioni:

<div class="preview">

1. Per aggiornare la Condizione di un’attività o di un problema nell’intestazione dell’attività o del problema:

   1. (Condizionale) Se l’amministratore del Workfront o del gruppo ha aggiunto il campo Condizione all’intestazione dell’attività o del problema del modello di layout, fai clic su **Condizione** nell’intestazione e seleziona una delle seguenti opzioni:
      * Senza problemi
      * Qualche dubbio
      * Problemi notevoli

      ![](assets/condition-in-task-header.png)
   1. Fai clic su Invio per salvare la condizione.

1. Per aggiornare la Condizione di un’attività o di un problema nella sezione Dettagli dell’attività o del problema:

   1. (Condizionale) Se l’amministratore del Workfront o del gruppo ha aggiunto il campo Condizione alla sezione Dettagli di un’attività o di un problema nel modello di layout, fai clic su **Dettagli** nel pannello a sinistra, fai clic su **Condizione** e selezionare una delle opzioni seguenti:
      * Senza problemi
      * Qualche dubbio
      * Problemi notevoli
1. Clic **Salva modifiche**. La condizione dell’attività o del problema è aggiornata.

</div>

Per aggiornare la condizione di un&#39;attività o di un problema in un report o in un elenco:

1. Vai a un elenco di attività o problemi per i quali disponi delle autorizzazioni di gestione. Assicurati che **Condizione** nella visualizzazione dell&#39;elenco.

1. Aggiornare il **Condizione** del problema o dell’attività in linea, facendo doppio clic sulla condizione esistente e selezionando un nuovo valore dal menu a discesa.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >Le condizioni possono essere personalizzate per il tuo ambiente, per cui potresti trovare più di tre opzioni per Condizione nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli elencati sopra. Per informazioni sulla personalizzazione delle Condizioni in Workfront, consulta [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Premi **Invio** sulla tastiera o fare clic all&#39;esterno del campo Condizione per salvare la nuova attività o il problema Condizione.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


