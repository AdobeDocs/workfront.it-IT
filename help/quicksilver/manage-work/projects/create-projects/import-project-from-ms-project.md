---
product-area: projects
navigation-topic: create-projects
title: Importare un progetto da Microsoft Project
description: Puoi importare progetti da Microsoft Project ad Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importate un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# Importare un progetto da Microsoft Project

<!-- Audited: 4/2025 -->

Puoi importare progetti da Microsoft Project ad Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importate un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.

>[!IMPORTANT]
>
>Non tutti i campi del progetto Microsoft vengono trasferiti a Workfront.
>
>Per ulteriori informazioni sulla compatibilità dei campi tra Workfront e Microsoft Project, vedere [Mappatura dei campi di Microsoft Project ai progetti Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Nuovo: Standard </p> 
   Oppure
   <p>Corrente: Piano </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto, ricevi automaticamente le autorizzazioni di gestione per il progetto </p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
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

## Creare un progetto da un progetto MS

Puoi creare un progetto dall&#39;area **Progetti** nel **Menu principale** o dall&#39;area **Progetti** di un portfolio o di un programma.

1. Accedi a Microsoft Project e apri un progetto da cui desideri importare in Workfront.
1. Fare clic su **File**, quindi su **Salva con nome** per salvare il progetto come file XML.

1. Accedi a Workfront.
1. Esegui una delle operazioni seguenti:

   * Fai clic sull&#39;icona **Main Menu** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Workfront oppure fai clic su **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, fai clic su **Projects**, quindi espandi **New Project**.
   * Vai a un portfolio, quindi espandi **Nuovo progetto**.
   * Vai a un programma, quindi espandi **Nuovo progetto**.
   * Se sei un amministratore gruppo, puoi creare un progetto nella sezione **Progetti** di un gruppo che gestisci. Per ulteriori informazioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Fare clic su **Importa MS Project**. Viene visualizzata la finestra di dialogo **Importa file MS**.

   ![Menu a discesa Nuovo progetto](assets/import-ms-project-option.png)

1. Fai clic su **Seleziona file**, quindi cerca il file .xml sul computer che hai esportato da Microsoft Project.
1. Importa il file selezionato. Workfront avvia il processo di importazione e crea un nuovo progetto basato sul file esportato da Microsoft Project.

   Al termine del processo di importazione, viene visualizzata la pagina Nuovo progetto in cui viene confermato il completamento dell&#39;importazione.

   >[!NOTE]
   >
   >Workfront ha un limite di tempo di 15 minuti per il caricamento dei file. Se il caricamento del file richiede più tempo, ti consigliamo di suddividere il progetto in progetti più piccoli e importarli separatamente. Dopo l&#39;importazione in Workfront, spostare le attività da un progetto all&#39;altro per combinarle in un progetto. Per informazioni sullo spostamento delle attività, vedere [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Facoltativo) Continua a modificare il progetto in Workfront. Per informazioni sulla modifica dei progetti, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >Lo stato di un nuovo progetto creato da un modello corrisponde a quello definito dall&#39;amministratore di Workfront nell&#39;area **Preferenze progetto** o da un amministratore di gruppo nell&#39;area **Preferenze progetto gruppo**. Per informazioni sulla configurazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
