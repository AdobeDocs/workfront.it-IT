---
product-area: projects
navigation-topic: create-projects
title: Crea un Progetto
description: Un progetto è una grande unità di lavoro in Adobe Workfront. Puoi creare progetti da zero, utilizzare un modello o convertire problemi o attività in progetti.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 1%

---

# Crea un Progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

<!-- Audited: 12/2023 -->

I progetti rappresentano una grande quantità di lavoro che deve essere fatto in Adobe Workfront.

## Requisiti di accesso

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Nuovo: Standard</p>
        <p>oppure</p>
        <p>Corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto, ricevi automaticamente le autorizzazioni di gestione per il progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Modi per creare progetti

Puoi creare un progetto in Workfront utilizzando uno dei seguenti metodi:

* Crea un progetto da zero senza utilizzare un modello. Questo articolo descrive come creare un progetto da zero.

* Copia un progetto esistente.\
  Per ulteriori informazioni sulla copia di un progetto, consulta [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

* Utilizza un modello.\
  Per ulteriori informazioni sull’utilizzo di un modello per creare un nuovo progetto, consulta [Creare un progetto utilizzando un modello](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importa un progetto da Microsoft Project.\
  Per ulteriori informazioni sull’importazione di un progetto da MS Project, consulta [Importare un progetto da Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importa un progetto utilizzando i kick-start.

  In qualità di amministratore di Workfront, puoi importare progetti utilizzando una funzione di avvio.

  Per informazioni sull’importazione di dati tramite l’avvio automatico in Workfront, consulta [Importare dati in Adobe Workfront utilizzando un modello di avvio](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Per informazioni sull&#39;importazione di progetti mediante l&#39;avvio, vedere [Scenario di avvio: preparazione semplice per l’importazione di un progetto e un’attività](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Pubblicare un’iniziativa da uno scenario in Adobe Workfront Scenario Planner. Scenario Planner richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta [Panoramica sulla pianificazione degli scenari](../../../scenario-planner/scenario-planner-overview.md). Per informazioni sulla creazione di progetti a partire da iniziative di pubblicazione, consulta  [Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

## Prerequisiti

Prima di iniziare, è necessario assicurarsi che:

* L’amministratore di sistema o di gruppo ha abilitato la preferenza &quot;Consenti agli utenti di creare progetti senza utilizzare un modello&quot; nell’area Configura.

  Per ulteriori informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Impostazioni predefinite nuovo progetto

Quando crei un progetto, Workfront applica a esso una serie di impostazioni predefinite. Ad esempio, le modalità Stato, Gruppo e Pianificazione sono predefinite al momento della creazione di un progetto.

Considera quanto segue:

* In qualità di amministratore di Workfront o di un gruppo, puoi configurare le impostazioni predefinite per un nuovo progetto durante la configurazione delle Preferenze di progetto per l’intera istanza di Workfront o per un gruppo.
* Workfront applica le impostazioni del gruppo, se presenti, prima di applicare quelle impostate dall&#39;amministratore Workfront.
* Lo stato predefinito di un nuovo progetto corrisponde a quello definito dall&#39;amministratore di Workfront nell&#39;area Preferenze progetto principale o da un amministratore di gruppo (o da un amministratore di Workfront) nell&#39;area Preferenze progetto per un gruppo.

  >[!NOTE]
  >
  >Lo stato predefinito di un nuovo progetto è Pianificazione. Quando si apportano modifiche al nuovo progetto, questo assicura che le notifiche non vengano inviate agli utenti assegnati al progetto.
  >
  >Per ulteriori informazioni sulla configurazione dello stato predefinito e di altre impostazioni predefinite per un nuovo progetto, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Esistono i seguenti scenari per la definizione del gruppo e dello stato di un nuovo progetto da parte di Workfront:

   * Se crei un progetto da zero, il Gruppo del progetto sarà il Gruppo Predefinito.

     Lo stato del progetto è lo stato predefinito nelle Preferenze progetto del Gruppo predefinito, se presente, o dell’istanza Workfront. È possibile modificare lo stato predefinito durante la creazione del progetto impostando qualsiasi stato disponibile per il gruppo del progetto.

   * Se crei un progetto utilizzando un modello, le impostazioni del modello hanno la precedenza su quelle stabilite dall’amministratore di Workfront o di gruppo.

     Il Gruppo del nuovo progetto è il Gruppo del modello. Se il modello non è associato a un gruppo, il gruppo del progetto è il gruppo predefinito dell’utente che crea il progetto.

     Lo stato predefinito di un nuovo progetto creato da un modello corrisponde a quello definito dall&#39;amministratore di Workfront nell&#39;area Preferenze progetto principale o da un amministratore di gruppo (o amministratore Workfront) nell&#39;area Preferenze progetto per il gruppo. È possibile modificare lo stato predefinito durante la creazione di un progetto da un modello a uno qualsiasi degli stati del gruppo del progetto, che è il gruppo del modello o il gruppo predefinito dell&#39;utente che crea il progetto.

   * Se si crea un progetto convertendo un problema, il gruppo di un nuovo progetto è il gruppo del progetto esistente del problema. Se l’utente che converte il problema non ha accesso al progetto del problema o se il progetto del problema non ha un gruppo, il gruppo del nuovo progetto è il gruppo predefinito dell’utente che converte il problema.

     Gli stati del nuovo progetto corrispondono agli stati del gruppo associato al progetto, che è il Gruppo del progetto originale o il Gruppo Predefinito dell’utente che converte il problema.

     Se utilizzi un modello durante la creazione del progetto convertendo il problema, consulta il secondo scenario qui sopra per capire quale gruppo e quale Stato di Workfront si applica al nuovo progetto.

## Creare un progetto da zero

>[!NOTE]
>
>Se stai creando un progetto utilizzando un modello, ti consigliamo di visualizzare anche l’articolo [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Esegui una delle operazioni seguenti:

   * Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro. Clic **Progetti**, quindi espandi **Nuovo progetto**.
   * Vai a un portfolio, quindi espandi **Nuovo progetto**.
   * Vai a un programma, quindi espandi **Nuovo progetto**.
   * Se sei un amministratore gruppo, puoi anche creare un progetto nella sezione Progetti di un gruppo che gestisci. Per ulteriori informazioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menu Nuovo progetto](assets/new-project-dropdown-nwe-350x358.png)

1. Clic **Nuovo progetto** per creare un progetto da zero.
1. Digita un nome per il progetto. Premi Invio per salvare il nome.

   ![Inserisci un nome per il progetto](assets/rename-untitled-project.png)

   L’intestazione della pagina del progetto presenta una breve panoramica dello stato e dell’avanzamento correnti di un progetto. Le informazioni nell&#39;intestazione del progetto cambiano con l&#39;aggiornamento delle informazioni sul progetto.

1. Clic **Inizia ad aggiungere attività**.

   Oppure

   Clic **Crea Attività** per aggiungere attività al progetto e assegnare loro risorse.

   Per ulteriori informazioni sull’aggiunta di attività a un progetto, consulta [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Modifica i dettagli del progetto facendo clic su **Altro** menu e quindi **Modifica** ![](assets/qs-edit-icon.png) accanto al nome del progetto.

   Il **Modifica Progetto** viene visualizzata.

   Per ulteriori informazioni sulla modifica di un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Facoltativo) Dopo aver configurato le impostazioni del progetto e aggiunto le attività, puoi modificare lo stato del progetto in **Corrente**.

   Questo indica che il progetto è pronto per essere avviato e che gli utenti assegnati alle attività ora possono iniziare a lavorarci.

   Per ulteriori informazioni sugli stati dei progetti, vedi [Accedere all’elenco degli stati del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
