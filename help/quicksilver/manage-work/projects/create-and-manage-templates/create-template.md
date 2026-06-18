---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creare un modello di progetto
description: È possibile creare ed eliminare modelli dall'area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni di progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/JqR-bwIq1AVMOMz3aTWIKoiPep1VQ6IaONbbuDJ1AiA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 790
ht-degree: 9%

---

# Creare un modello di progetto

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard </p><p>Piano</p> <p>Per importare modelli da Blueprint è necessario essere un amministratore di sistema</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Per impostazione predefinita, disponi delle autorizzazioni di gestione per i modelli creati</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
</table>
-->

## Creare un modello

{{step1-to-templates}}

1. Fare clic su **Nuovo modello**.

1. (Condizionale) A seconda dell&#39;archiviazione documenti utilizzata dall&#39;organizzazione, fare clic su una delle opzioni seguenti:

   * **Nuovo modello**, quando l&#39;amministratore di Workfront sceglie **Adobe Cloud Storage** o **Legacy Workfront** e ha selezionato o meno l&#39;impostazione **Consenti all&#39;utente di selezionare il provider di archiviazione**.
   * **Nuovo modello (archiviazione legacy)**, quando l&#39;amministratore di Workfront sceglie **Archiviazione cloud Adobe** o **Workfront legacy** e seleziona anche l&#39;impostazione **Consenti all&#39;utente di selezionare il provider di archiviazione**.

     Questa opzione viene visualizzata solo quando nell&#39;area Consenti impostazione **Consenti all&#39;utente di selezionare il provider di archiviazione** è selezionato.

     Per ulteriori informazioni, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

     Un modello viene creato e il suo nome predefinito segue i seguenti modelli, a seconda del Workfront di archiviazione utilizzato per i documenti:

      * **Modello senza titolo** per modello di archiviazione Workfront.

        Un modello di archiviazione legacy di Workfront visualizza un&#39;icona **Archiviazione legacy di Workfront** ![Icona progetto di archiviazione legacy](assets/legacy-storage-project-icon.png) accanto al nome.

      * **Modello senza titolo - &lt; Mese giorno, anno ora.minuto.secondo >** per un modello di archiviazione cloud Adobe

        >[!IMPORTANT]
        >
        >I modelli che utilizzano l’archiviazione Adobe devono avere nomi univoci.

   ![Nuovo modello](assets/create-template-nwe-2022-350x102.png)

1. Specificare un nome per il nuovo modello nell&#39;intestazione del modello, quindi premere **Invio.**
1. Fai clic sulla sezione **Attività modello** nel pannello a sinistra.
1. Fai clic su **Inizia ad aggiungere attività modello** per aggiungere attività in linea

   Oppure

   Fai clic su **Nuova attività modello** per iniziare ad aggiungere attività al modello nella casella **Nuova attività modello**.

   La casella **Crea attività modello** si apre quando si fa clic su **Nuova attività modello**.

   ![Nuova esperienza per la nuova attività modello](assets/new-template-task-box-unshimmed.png)

1. (Facoltativo) Aggiorna le informazioni nelle seguenti aree nella casella **Crea attività modello**:

   * Nome Attività Modello
   * Panoramica
   * Assegnazioni
   * Finanz
   * Moduli personalizzati
   * Documenti
   * Impostazioni

   L&#39;aggiornamento delle informazioni per un&#39;attività modello è simile alla modifica delle attività modello.

   Per ulteriori informazioni, vedere [Modifica attività modello](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-template-task.md).

   >[!NOTE]
   >
   >Impossibile aggiungere attività ricorrenti a un modello.

1. Fai clic su **Crea attività modello**.

1. (Facoltativo) Dopo aver aggiunto le attività modello, nella sezione **Attività modello** fai clic sull&#39;icona **Grafico di Gantt** ![Icona di Gantt](assets/gantt-icon.png) nell&#39;angolo superiore destro dell&#39;elenco attività per visualizzare una rappresentazione visiva dell&#39;elenco attività del modello.

   >[!TIP]
   >
   >Non è possibile modificare le attività direttamente da un diagramma di Gantt delle attività modello.

1. Per aggiungere informazioni al nuovo modello, fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome del modello nell&#39;intestazione, quindi fai clic su **Modifica**.

   Per informazioni sulla modifica di un modello, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >L&#39;associazione di un modello di progetto a un gruppo (o la mancanza di un gruppo) influisce sul modo in cui le preferenze di progetto, attività e problema determinano determinate impostazioni nel modello.
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




