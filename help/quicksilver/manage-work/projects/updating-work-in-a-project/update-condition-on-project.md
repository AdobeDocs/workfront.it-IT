---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna condizione per un progetto
description: La Condizione di un progetto è un flag posizionato su di esso per indicare se il lavoro associato a esso sta andando senza problemi o se hai incontrato blocchi stradali. Questo è diverso dallo Stato del progetto, che indica se ci stai lavorando attivamente o meno.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: b7f59552e5b66a3b2db765a49abdb2f49b1a51ec
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Aggiorna condizione per un progetto

La Condizione di un progetto è un flag posizionato su di esso per indicare se il lavoro associato a esso sta andando senza problemi o se hai incontrato blocchi stradali. Questo è diverso dallo Stato del progetto, che indica se ci stai lavorando attivamente o meno.

È possibile impostare la condizione di un progetto in modo automatico o manuale. Per cambiare manualmente la condizione di un progetto, devi essere il proprietario del progetto o disporre dei diritti di gestione per esso.

L&#39;amministratore di Adobe Workfront può creare condizioni personalizzate per l&#39;ambiente, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>

Per le nuove licenze:
<p>Standard</p>

Per le licenze correnti:
<ul><li><p>Piano</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Visualizzare o accedere ai progetti in modo più avanzato</p> <p>Modificare l’accesso ad attività e problemi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi per visualizzarne la condizione</p>
   <p>Gestire le autorizzazioni su attività e problemi per aggiornare la condizione</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   ![](assets/project-details-overview-select-condition.png)

1. Nel campo **Condizione**, seleziona tra le seguenti opzioni quella che corrisponde alla tua comprensione del corretto svolgimento del lavoro associato o dell&#39;eventuale ritardo:

   * **Su Target**
   * **A Rischio**
   * **Problemi**

   Per ulteriori informazioni sulle condizioni del progetto, vedere [Panoramica sulla condizione e sul tipo di condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Le condizioni possono essere personalizzate per il tuo ambiente, per cui potresti trovare più di tre opzioni per Condizione nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli elencati sopra. Per informazioni sulla personalizzazione delle Condizioni in Workfront, vedere [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Fai clic su **Salva modifiche**.
