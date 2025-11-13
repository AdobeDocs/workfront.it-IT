---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creare un modello di progetto
description: È possibile creare ed eliminare modelli dall'area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni di progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 6%

---

# Creare un modello di progetto

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

È possibile creare ed eliminare modelli dall&#39;area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni di progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.

>[!NOTE]
>
>Un modello e le relative attività non dispongono di date effettive, ma di un&#39;indicazione del giorno (a partire dal quale potrebbe iniziare il progetto futuro) in cui un&#39;attività potrebbe iniziare e del giorno in cui l&#39;attività potrebbe dover essere completata. Quando si utilizzano i modelli per creare i progetti futuri, i progetti riceveranno le date effettive. Per informazioni, vedere [Creare un progetto](../create-projects/create-project.md).


È possibile creare un nuovo modello nei modi seguenti:

* Da zero, come descritto in questo articolo.
* Da progetti esistenti, salvando un progetto come modello.

  Per ulteriori informazioni sulla creazione di modelli da progetti esistenti, vedere [Salvare un progetto come modello](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiandolo da un altro modello.

  Per ulteriori informazioni sulla copia di un modello esistente, vedere [Copiare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Importando i blueprint. Per importare i blueprint è necessario essere un amministratore Workfront. Per informazioni, vedere [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

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
   <td> <p>Standard </p><p>Piano</p> <p>Per importare modelli da Blueprint è necessario essere un amministratore di sistema</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Per impostazione predefinita, disponi delle autorizzazioni di gestione per i modelli creati</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Creare un modello

{{step1-to-templates}}

1. Fare clic su **Nuovo modello**.

   Il modello è senza titolo.

   ![Nuovo modello](assets/create-template-nwe-2022-350x102.png)

1. Specificare un nome per il nuovo modello nell&#39;intestazione del modello, quindi premere **Invio.**
1. Fai clic sulla sezione **Attività modello** nel pannello a sinistra.
1. Fai clic su **Inizia ad aggiungere attività modello** per aggiungere attività in linea

   Oppure

   Fai clic su **Nuova attività modello** per iniziare ad aggiungere attività al modello nella casella **Nuova attività modello**.

   Nella nuova esperienza verrà visualizzata la casella **Crea attività modello**.

   ![Nuova esperienza per la nuova attività modello](assets/new-template-task-box-unshimmed.png)

1. (Condizionale) Utilizzando la nuova esperienza, aggiorna le informazioni nelle seguenti aree nella casella **Crea attività modello**:

   * Nome Attività Modello
   * Panoramica
   * Assegnazioni
   * Finanz
   * Moduli personalizzati
   * Documenti
   * Impostazioni

1. Fai clic su **Crea attività modello**

   Oppure

   Fai clic su **Torna alla vecchia esperienza** nella parte inferiore della casella **Crea attività modello**.

   La **nuova attività modello** si apre nella vecchia esperienza.

   ![Casella Attività nuovo modello](assets/new-template-task-box.png)

   >[!TIP]
   >
   >In Produzione, per impostazione predefinita viene aperta la vecchia esperienza.

1. Aggiorna le informazioni nelle seguenti aree nella casella **Nuova attività modello**:

   * Panoramica
   * Finanz
   * Impostazioni
   * Assegnazioni
   * Moduli personalizzati
   * Allega documento

     L&#39;aggiornamento delle informazioni per un&#39;attività modello è simile alla modifica delle attività in un progetto. Per ulteriori informazioni, vedere [Modifica attività](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). <!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >Impossibile aggiungere attività ricorrenti a un modello.

1. Fare clic su una delle seguenti opzioni:

   * **Salva attività modello** per salvare l&#39;attività modello corrente e chiude la casella Nuova attività modello.
   * **Salva attività modello e avviane un&#39;altra** per salvare l&#39;attività modello corrente e aprire un&#39;altra **nuova attività modello** per aggiungere un&#39;altra attività.
   * **Annulla** per chiudere la casella senza salvare l&#39;attività modello.
1. (Facoltativo) Dopo aver aggiunto le attività modello, nella sezione Attività modello, fai clic sull&#39;icona **Grafico di Gantt** nell&#39;angolo superiore destro dell&#39;Elenco attività per visualizzare una rappresentazione visiva dell&#39;elenco delle attività del modello.

   >[!TIP]
   >
   >Non è possibile modificare le attività direttamente da questo diagramma di Gantt.

1. Per aggiungere informazioni al nuovo modello, fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a sinistra del nome del modello nell&#39;intestazione, quindi fai clic su **Modifica**.

   Per informazioni sulla modifica di un modello, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >   L&#39;associazione di un modello di progetto a un gruppo (o la mancanza di un gruppo) influisce sul modo in cui le preferenze di progetto, attività e problema determinano determinate impostazioni nel modello.
   >
   >Per ulteriori informazioni, vedere la sezione &quot;Applicazione delle preferenze ai modelli e alle attività dei modelli&quot; nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Fai clic su **Salva**.
1. (Facoltativo) Aggiungi i seguenti elementi al modello

   * Documenti
   * Rischi
   * Processi di approvazione
   * Tariffe di fatturazione
   * Spese
   * Dettagli coda
   * Gruppi di argomenti e argomenti coda

1. (Facoltativo) Aggiungi i seguenti elementi alle attività nel modello:

   * Documenti
   * Spese
   * Approvazioni

   Per informazioni, vedere la sezione &quot;Aggiungere altri elementi a un modello&quot; nell&#39;articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




