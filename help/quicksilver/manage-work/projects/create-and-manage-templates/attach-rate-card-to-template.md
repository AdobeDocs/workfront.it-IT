---
content-type: overview
product-area: templates
navigation-topic: financials
title: Allegare una scheda tariffa a un modello
description: Quando si assegna una scheda tariffaria a un modello, questa viene quindi allegata a tutti i progetti creati dal modello.
author: Lisa
feature: Work Management
source-git-commit: ace9a01e852e6d99ddc6f150c0ac34bd4ef44817
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 8%

---

# Allegare una scheda tariffa a un modello

Quando si assegna una scheda tariffaria a un modello, questa viene quindi allegata a tutti i progetti creati dal modello. La scheda tariffe diventa l’impostazione predefinita nel progetto, ma può essere sostituita se necessario.

Per informazioni sulle schede di tariffa, consulta [Gestire le schede di tariffa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Per informazioni sui modelli di progetto, vedere [Panoramica dei modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modificare l’accesso ai modelli</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per la scheda tariffe con le autorizzazioni per Modifica tariffe di fatturazione</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

La scheda tariffa che desideri assegnare al modello deve essere creata in Workfront. Per ulteriori informazioni, consulta [Gestione schede tariffarie](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Il campo **Scheda tariffa** deve essere abilitato per i modelli nel modello di layout.

1. Nel modello di layout fare clic sulla freccia rivolta verso il basso in **Personalizza gli elementi visualizzati dagli utenti**, quindi fare clic su **Modello**.
1. Nella sezione **Dettagli**, seleziona il campo **Scheda tariffa** nell&#39;area **Panoramica**.

   Per ulteriori informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Allegare una scheda tariffa a un modello

{{step1-to-templates}}

1. Crea un nuovo modello o modificane uno esistente.
1. Nella sezione Dettagli modello > Panoramica > Associazione modello, seleziona una scheda tariffa nel campo **Scheda tariffa**.

   Puoi scegliere solo le schede di valutazione per le quali disponi delle autorizzazioni.
Per limitare l’elenco dei risultati, puoi iniziare a digitare il nome di una scheda delle tariffe.

   ![Selezionare una scheda tariffaria nel modello](assets/select-rate-card-on-template.png)

1. Salva il modello dopo averlo modificato.

   Per ulteriori informazioni sulla creazione di un modello, vedere [Creare un modello di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md).

   Per ulteriori informazioni sulla modifica di un modello, vedere [Modifica modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

## Applicare il modello a un progetto

1. Crea un progetto utilizzando il modello.

   Esistono diversi modi per creare un progetto da un modello. Per informazioni, consulta questi articoli:

   * [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [Convertire un’attività in un progetto](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [Convertire un problema in un progetto](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   La scheda tariffe viene salvata automaticamente nel progetto. Nella sezione Panoramica > Associazione progetto della casella Nuovo progetto, è possibile rimuovere la scheda tariffa o selezionare una scheda tariffa diversa nel campo **Scheda tariffa**.

   ![Scheda di valutazione da modello visualizzata nei dettagli del progetto](assets/create-project-from-template-rate-card.png)

   La scheda tariffe e le tariffe associate vengono visualizzate nell&#39;area Tariffe progetto.

   Puoi anche rimuovere la scheda delle tariffe dal progetto o allegare una scheda diversa nell’area Tariffe. Per ulteriori informazioni, vedere [Allegare una scheda tariffe a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

   ![Scheda di valutazione da modello sul progetto](assets/template-rates-on-project.png)

   >[!NOTE]
   >
   >Se nel modello è presente un tasso individuale e al modello è associata anche una scheda tasso, quando si crea un progetto dal modello, sia il tasso individuale che la scheda tasso verranno visualizzati nell&#39;elenco dei tassi.

1. (Facoltativo) Per applicare la scheda tariffa a un progetto esistente, allega il modello al progetto.

   Quando utilizzi l&#39;opzione **Personalizza e allega** nell&#39;anteprima del modello, puoi selezionare l&#39;elemento **Scheda tariffa** nella sezione Allega modello > Opzioni per aggiungere la scheda tariffa al progetto. Deseleziona la casella di controllo per escludere la scheda della tariffa dal trasferimento al progetto.

   Per ulteriori informazioni, vedere [Allegare un modello a un progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. (Facoltativo) Per salvare la scheda della tariffa da un progetto specifico in un modello, salva il progetto come modello.

   Nella sezione Opzioni della casella Salva come modello, è possibile selezionare l&#39;elemento **Scheda tariffa** per aggiungere la scheda tariffa al modello. Deselezionare la casella di controllo per escludere la scheda del tasso dal trasferimento al modello.

   Per ulteriori informazioni, vedere [Salvare un progetto come modello](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md).


