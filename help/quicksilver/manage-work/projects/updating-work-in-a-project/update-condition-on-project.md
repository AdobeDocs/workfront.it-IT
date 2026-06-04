---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna condizione per un progetto
description: La Condizione di un progetto è un flag posizionato su di esso per indicare se il lavoro associato a esso sta andando senza problemi o se hai incontrato blocchi stradali. Questo è diverso dallo Stato del progetto, che indica se ci stai lavorando attivamente o meno.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/rZhmS-9XbtoehUQOv2QIwTgdEk4eGB7JfZiLvQXhCZM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 532
ht-degree: 8%

---

# Aggiornare condizione per un progetto

La Condizione di un progetto è un flag posizionato su di esso per indicare se il lavoro associato a esso sta andando senza problemi o se hai incontrato blocchi stradali. Questo è diverso dallo Stato del progetto, che indica se ci stai lavorando attivamente o meno.

È possibile impostare la condizione di un progetto in modo automatico o manuale. Per cambiare manualmente la condizione di un progetto, devi essere il proprietario del progetto o disporre dei diritti di gestione per esso.

L&#39;amministratore di Adobe Workfront può creare condizioni personalizzate per l&#39;ambiente, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
  <p>Standard</p>
   <p>Piano</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizzare o accedere ai progetti in modo più avanzato</p> <p>Modificare l’accesso ad attività e problemi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi per visualizzarne la condizione</p>
   <p>Gestire le autorizzazioni su attività e problemi per aggiornare la condizione</p>
     </td> 
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
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>
-->

## Imposta automaticamente la condizione

L’impostazione automatica della condizione di un progetto è determinata dal tipo di condizione del progetto. Per impostare automaticamente la condizione del progetto, è necessario impostare il tipo di condizione sullo stato di avanzamento in Workfront.

L’amministratore del Workfront o del gruppo determina il valore predefinito del campo Tipo di condizione per i nuovi progetti nel sistema quando imposta le preferenze del progetto nell’area Configura. Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Quando si crea un progetto, la Condizione del progetto viene impostata automaticamente in modo che corrisponda allo Stato di avanzamento del progetto in quel momento. Lo stato di avanzamento del progetto si basa sull&#39;avanzamento delle attività del progetto.

Per informazioni sulle condizioni del progetto e su come vengono calcolate in base allo stato di avanzamento, vedere [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Aggiornare manualmente la condizione per un progetto

Se si imposta il tipo di condizione del progetto su Manuale invece che su Stato avanzamento, è possibile aggiornare manualmente la condizione di un progetto.

1. Vai al progetto per il quale desideri aggiornare la Condizione.
1. Fai clic sulla sezione **Dettagli progetto** nel pannello a sinistra.

1. Verificare che il campo **Tipo di condizione** sia impostato su **Manuale**.

   ![Condizione di selezione panoramica dettagli progetto](assets/project-details-overview-select-condition.png)

1. Nel campo **Condizione**, seleziona tra le seguenti opzioni quella che corrisponde alla tua comprensione del corretto svolgimento del lavoro associato o dell&#39;eventuale ritardo:

   * **Su Target**
   * **A Rischio**
   * **Problemi**

   Per ulteriori informazioni sulle condizioni del progetto, vedere [Panoramica sulla condizione e sul tipo di condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Le condizioni possono essere personalizzate per il tuo ambiente, per cui potresti trovare più di tre opzioni per Condizione nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli elencati sopra. Per informazioni sulla personalizzazione delle Condizioni in Workfront, vedere [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Fai clic su **Salva modifiche**.
