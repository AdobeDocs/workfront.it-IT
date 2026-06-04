---
product-area: projects
navigation-topic: create-projects
title: Importare un progetto da progetto di Microsoft
description: Puoi importare progetti da Microsoft Project ad Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importate un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/drxvgi-xQLjEt5JOL6-MxLdkmVcXxkcXMN14nwmNZvs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 9%

---

# Importare un progetto da progetto di Microsoft

<!-- Audited: 10/2025 -->

Puoi importare progetti da Microsoft Project ad Adobe Workfront e gestire tutti i tuoi progetti in un’unica applicazione. Ogni volta che importate un progetto da Microsoft Project, viene creato un nuovo progetto in Workfront.

>[!IMPORTANT]
>
>Non tutti i campi del progetto Microsoft vengono trasferiti a Workfront.
>
>Per ulteriori informazioni sulla compatibilità dei campi tra Workfront e Microsoft Project, vedere [Mappatura dei campi di Microsoft Project ai progetti Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

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
   <td> <p>Standard</p> 
    <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> 
   <p>Se si aggiunge un progetto a un portfolio o a un programma, è necessario disporre dell'accesso di modifica a portafogli e programmi.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Quando crei un progetto, ricevi automaticamente le autorizzazioni di gestione per il progetto</p>
   <p>Se aggiungi un progetto a un portfolio o a un programma, devi disporre delle autorizzazioni di gestione per il portfolio e il programma.</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
old permissions model: 

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
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
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

   * Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Projects** ed espandi **New Project**.
   * Vai a un portfolio, quindi espandi **Nuovo progetto**.
   * Vai a un programma, quindi espandi **Nuovo progetto**.
   * Se sei un amministratore gruppo, puoi creare un progetto nella sezione **Progetti** di un gruppo che gestisci. Per ulteriori informazioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Fare clic su **Importa MS Project**.

   ![Menu a discesa Nuovo progetto](assets/import-ms-project-option.png)

   Viene visualizzata la casella **Importa file MS**.

1. Fai clic su **Seleziona file**, quindi cerca il file .xml sul computer che hai esportato da Microsoft Project.
1. Importa il file selezionato. Workfront avvia il processo di importazione e crea un nuovo progetto basato sul file esportato da Microsoft Project.

   >[!NOTE]
   >
   >Workfront ha un limite di tempo di 15 minuti per il caricamento dei file. Se il caricamento del file richiede più tempo, ti consigliamo di suddividere il progetto in progetti più piccoli e importarli separatamente. Dopo l&#39;importazione in Workfront, spostare le attività da un progetto all&#39;altro per combinarle in un progetto. Per informazioni sullo spostamento delle attività, vedere [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Al termine del processo di importazione, viene visualizzata la pagina Nuovo progetto in cui viene confermato il completamento dell&#39;importazione.

   >[!CAUTION]
   >
   >Se l’istanza di Workfront ha accesso sia all’archiviazione cloud Workfront che Adobe per i documenti, l’importazione di un progetto da MS Project crea un progetto di archiviazione Workfront legacy, anche quando l’amministratore di Workfront ha impostato l’archiviazione cloud Adobe come predefinita per il sistema.
   >
   >Per ulteriori informazioni, vedere [Panoramica sulla gestione dei documenti per progetti e oggetti correlati](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).


1. (Facoltativo) Continua a modificare il progetto in Workfront. Per informazioni sulla modifica dei progetti, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >Lo stato di un nuovo progetto creato da un modello corrisponde a quello definito dall&#39;amministratore di Workfront nell&#39;area **Preferenze progetto** o da un amministratore di gruppo nell&#39;area **Preferenze progetto gruppo**. Per informazioni sulla configurazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
