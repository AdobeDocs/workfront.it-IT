---
product-area: projects
navigation-topic: create-tasks
title: Crea sottoattività
description: In Adobe Workfront, le attività possono avere relazioni padre-figlio. Le attività secondarie sono denominate attività secondarie. È possibile creare sottoattività nell'elenco delle attività trasformando un'attività principale in sottoattività. È inoltre possibile impostare un'attività secondaria come attività principale.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Crea sottoattività

<!-- Audited: 01/2025 -->

In Adobe Workfront, le attività possono avere relazioni padre-figlio. Le attività secondarie sono denominate attività secondarie. È possibile creare sottoattività nell&#39;elenco delle attività trasformando un&#39;attività principale in sottoattività. È inoltre possibile impostare un&#39;attività secondaria come attività principale.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Nuovo: Standard</p>
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto e l'attività padre con la possibilità di aggiungere attività o versione successiva</p> <p>Dopo aver creato l'attività, si ricevono automaticamente le autorizzazioni di gestione.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crea sottoattività

È possibile creare sottoattività dall&#39;elenco delle attività o dalla sezione delle sottoattività delle attività.

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
1. Se presente, fai clic sulla sezione **Sottoattività** nel pannello a sinistra.
1. Fai clic su **Nuova attività.**

   Segui i passaggi descritti nel seguente articolo per continuare a creare la sottoattività: [Crea attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Fai clic su **Crea attività.**

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
