---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna condizione per un progetto
description: La condizione di un progetto è un flag apposto su di esso per indicare se il lavoro associato sta procedendo senza intoppi o se sono stati rilevati blocchi stradali. Questo è diverso dallo stato del progetto, che indica se ci stai lavorando attivamente o meno.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# Aggiorna condizione per un progetto

La condizione di un progetto è un flag apposto su di esso per indicare se il lavoro associato sta procedendo senza intoppi o se sono stati rilevati blocchi stradali. Questo è diverso dallo stato del progetto, che indica se ci stai lavorando attivamente o meno.

Puoi impostare automaticamente o manualmente la condizione di un progetto. Per modificare manualmente la condizione di un progetto, devi essere il proprietario del progetto o disporre dei diritti di gestione.

L’amministratore di Adobe Workfront può creare condizioni personalizzate per l’ambiente, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Imposta automaticamente la condizione

L’impostazione automatica della condizione di un progetto dipende dal tipo di condizione del progetto. Per impostare automaticamente la condizione del progetto, è necessario impostare il tipo di condizione su Stato di avanzamento per Workfront.

Quando si impostano le preferenze di progetto nell’area Configurazione, l’amministratore di Workfront o di gruppo determina l’impostazione predefinita del campo Tipo di condizione per i nuovi progetti nel sistema. Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Quando crei un progetto, la condizione del progetto viene impostata automaticamente in modo che corrisponda allo stato di avanzamento del progetto in quel momento. Lo stato di avanzamento del progetto si basa sullo stato di avanzamento delle attività del progetto.

Per informazioni sulle condizioni del progetto e sul modo in cui vengono calcolate in base allo stato di avanzamento, consulta [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Aggiornare manualmente la condizione di un progetto

Se si imposta il tipo di condizione del progetto su Manuale invece che Stato avanzamento, è possibile aggiornare manualmente la condizione di un progetto.

1. Passa al progetto per il quale desideri aggiornare la condizione.
1. Fai clic sul pulsante **Dettagli progetto** sezione .

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Assicurati che **Tipo di condizione** campo impostato su **Manuale**.

1. In **Condizione** selezionare tra le opzioni seguenti quella che corrisponde alla comprensione dell&#39;andamento del lavoro associato o dell&#39;eventuale ritardo:

   * **Puntuale**
   * **A Rischio**
   * **In difficoltà**

   Per ulteriori informazioni sulle condizioni del progetto, consulta [Panoramica del tipo di condizione e condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Le condizioni possono essere personalizzate per il tuo ambiente, quindi potresti trovare più di tre opzioni per Condition nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli sopra elencati. Per informazioni sulla personalizzazione delle condizioni in Workfront, consulta [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Fai clic su **Salva**.Click **Salva modifiche**.
