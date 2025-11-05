---
product-area: projects
navigation-topic: create-tasks
title: Crea sottoattività
description: In Adobe Workfront, le attività possono avere relazioni padre-figlio. Le attività secondarie sono denominate attività secondarie. È possibile creare sottoattività nell'elenco delle attività trasformando un'attività principale in sottoattività. È inoltre possibile impostare un'attività secondaria come attività principale.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Crea sottoattività

<!-- Audited: 01/2025 -->

In Adobe Workfront, le attività possono avere relazioni padre-figlio. Le attività secondarie sono denominate attività secondarie. È possibile creare sottoattività nell&#39;elenco delle attività rendendo un&#39;attività principale una sottoattività di un&#39;altra attività. È inoltre possibile impostare un&#39;attività secondaria come attività principale.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto con la possibilità di aggiungere attività o versione successiva</p> 
   <p>Quando crei un’attività, ricevi automaticamente le autorizzazioni di gestione per l’attività</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Crea sottoattività

È possibile creare sottoattività dall&#39;elenco delle attività o dalla sezione delle sottoattività delle attività.

>[!TIP]
>
>La creazione di sottoattività per un progetto è simile alla creazione di sottoattività modello per le attività modello in un modello.


### Crea sottoattività dall&#39;elenco delle attività {#create-subtasks-from-the-task-list}

1. Passare al progetto in cui si desidera creare le sottoattività.
1. Fai clic sulla sezione **Attività** nel pannello a sinistra.
1. (Facoltativo) Se l&#39;attività che si desidera impostare come padre non si trova già direttamente sotto l&#39;attività che si desidera impostare come padre, trascinarla nella posizione appropriata nell&#39;elenco delle attività.
1. Selezionare l&#39;attività che si desidera impostare come sottoattività ed eseguire una delle operazioni seguenti:

   * Fai clic sull&#39;icona **Rientro** ![](assets/indent-icon-nwe-33x29.png) per rendere l&#39;attività selezionata una sottoattività dell&#39;attività direttamente sopra di essa.
   * Quando si utilizza una tastiera QWERTY inglese standard, premere Option + > (Mac) o Alt + > (Windows) sulla tastiera. Altre lingue possono utilizzare i comandi Option + , (Mac) o Alt + , (Windows) per applicare un rientro.

     >[!TIP]
     >
     >Le scelte rapide da tastiera non funzionano quando si modificano attività in modalità di modifica in linea. In questo caso, utilizzare l&#39;icona Rientro ![](assets/indent-icon-nwe-33x29.png) per creare sottoattività.

   * Trascinare e rilasciare l&#39;attività sull&#39;attività che si desidera designare come attività padre.

     >[!NOTE]
     >
     >È possibile applicare un rientro alle attività solo quando l&#39;elenco delle attività è ordinato in base al numero di attività e non sono stati applicati raggruppamenti all&#39;elenco.

### Crea sottoattività dalla sezione Attività secondarie {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>L’amministratore di Workfront o di gruppo potrebbe rimuovere la sezione Sottoattività nel tuo ambiente utilizzando un modello di layout.

1. Passare al progetto in cui si desidera creare le sottoattività.
1. Fai clic sulla sezione **Attività** nel pannello a sinistra.
1. Fare clic sul nome dell&#39;attività in cui si desidera creare un&#39;attività secondaria.
1. Se disponibile, fai clic sulla sezione **Sottoattività** nel pannello a sinistra.
1. Fai clic su **Nuova attività.**

   Per informazioni sulla creazione di attività, vedere [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Fai clic su **Crea attività.**

   La nuova attività viene creata come sottoattività dell&#39;attività selezionata al passaggio 3. <!--ensure this is accurate-->

## Rendere un&#39;attività secondaria un&#39;attività principale

1. Passare al progetto in cui si desidera impostare un&#39;attività secondaria come attività principale.
1. Fai clic sulla sezione **Attività** nel pannello a sinistra.
1. Selezionare l&#39;attività secondaria che si desidera rendere un&#39;attività principale.
1. Fai clic sull&#39;icona **Rientro negativo** ![](assets/outdent-icon-nwe-31x29.png) per rendere l&#39;attività secondaria un&#39;attività principale.

   Oppure

   Su una tastiera QWERTY inglese standard, premere Option + &lt; (Mac) o Alt + &lt; (Windows). Altri linguaggi possono usare i comandi Opzione + . (Mac) o Alt + . (Windows) per annullare il rientro.

   >[!NOTE]
   >
   >È possibile annullare il rientro delle attività solo quando l&#39;elenco delle attività è ordinato in base al numero di attività e non sono stati applicati raggruppamenti all&#39;elenco delle attività.
