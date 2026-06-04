---
product-area: projects
navigation-topic: plan-a-project
title: Aggiorna proprietari e sponsor progetto
description: Quando crei un progetto in Adobe Workfront, l’utente viene automaticamente impostato come Proprietario del progetto. Puoi aggiornare questo campo con un altro utente. Puoi anche aggiornare il campo Sponsor progetto di un progetto.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YqTw5b0p4p605v7O0wVx99A7gLvJYF8xEPtthwW0CWc
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
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 9%

---

# Aggiornare proprietari e sponsor del progetto

<!--Audited: 07/2024-->

Quando crei un progetto in Adobe Workfront, l’utente viene automaticamente impostato come Proprietario del progetto. Puoi aggiornare questo campo con un altro utente. Puoi anche aggiornare il campo Sponsor progetto di un progetto.

Per informazioni sui proprietari e gli sponsor dei progetti, vedere [Panoramica sui proprietari e sugli sponsor dei progetti](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Puoi identificare un proprietario e uno sponsor per un modello. Quando crei un progetto da tale modello, il proprietario del modello diventa il proprietario del progetto e lo sponsor del modello diventa lo sponsor del progetto.
>
>Se il modello non dispone di un Proprietario, l’utente che crea il progetto dal modello diventa il Proprietario del progetto.
>
>Per informazioni sulla modifica dei modelli, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Modificare le autorizzazioni per un progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Aggiornare il proprietario di un progetto

Quando aggiungi un utente come proprietario del progetto, Workfront assegna automaticamente le autorizzazioni necessarie per visualizzare il progetto.

1. Vai al progetto che desideri aggiornare.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/qs-edit-icon.png) nell&#39;angolo superiore destro dell&#39;area Dettagli progetto, quindi fai clic su **Panoramica**.

1. Specifica il nome di un utente per il campo **Proprietario progetto**.

   Solo gli utenti attivi possono essere specificati come Proprietari del progetto.

1. Fai clic su **Salva modifiche**.

   Il Proprietario del progetto viene aggiornato nell’intestazione del progetto e nell’area Dettagli progetto.

   ![Proprietario cointeressati progetto evidenziato](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Aggiornare lo sponsor di un progetto

Quando aggiungi un utente come sponsor del progetto di un progetto, Workfront assegna automaticamente a tale utente le autorizzazioni per visualizzare il progetto.

>[!TIP]
>
>Se l&#39;utente aggiunto come sponsor del progetto è un amministratore di sistema, non viene aggiunto all&#39;elenco Condivisione del progetto.

1. Vai al progetto che desideri aggiornare.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/qs-edit-icon.png) nell&#39;angolo superiore destro dell&#39;area Dettagli progetto, quindi fai clic su **Panoramica**.

1. Specificare il nome di un utente per il campo **Sponsor progetto**.

   Solo gli utenti attivi possono essere specificati come sponsor del progetto.

1. Fai clic su **Salva modifiche**.

   Lo sponsor del progetto viene aggiornato nella sezione Project Details (Dettagli progetto).

   ![Sponsor parti interessate progetto evidenziato](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
