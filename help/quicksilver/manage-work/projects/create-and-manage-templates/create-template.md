---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creare un modello di progetto
description: È possibile creare ed eliminare modelli dall'area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni di progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 094a54d2d1f6445aa9611152cb632d85be74bbeb
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Creare un modello di progetto

<!-- Audited: 1/2024 -->

È possibile creare ed eliminare modelli dall&#39;area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni di progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.

>[!NOTE]
>
>Un modello e le relative attività non dispongono di date effettive, ma di un&#39;indicazione del giorno (a partire dal quale potrebbe iniziare il progetto futuro) in cui un&#39;attività potrebbe iniziare e del giorno in cui l&#39;attività potrebbe dover essere completata. Quando si utilizzano i modelli per creare i progetti futuri, i progetti riceveranno le date effettive. Per informazioni, consulta [Creare un progetto](../create-projects/create-project.md).


È possibile creare un nuovo modello nei modi seguenti:

* Da zero, come descritto in questo articolo.
* Da progetti esistenti, salvando un progetto come modello.

  Per ulteriori informazioni sulla creazione di modelli da progetti esistenti, consulta [Salvare un progetto come modello](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiandolo da un altro modello.

  Per ulteriori informazioni sulla copia di un modello esistente, vedere [Copiare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Importando i blueprint. Per importare i blueprint è necessario essere un amministratore Workfront. Per informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisiti di accesso

Devi avere i seguenti:

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
   <td> <p>Nuovo: Standard </p><p>Oppure </p><p>Corrente: Piano </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Per importare modelli da Blueprint è necessario essere un amministratore di sistema</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Per impostazione predefinita, disponi delle autorizzazioni di gestione per i modelli creati</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare un modello

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Modelli**.

1. Clic **Nuovo modello**.

   Il modello è senza titolo.

   ![Nuovo modello](assets/create-template-nwe-2022-350x102.png)

1. Specifica un nome per il nuovo modello nell’intestazione del modello, quindi premi **Immettete.**
1. Fai clic su **Attività modello** nel pannello a sinistra.
1. Clic **Inizia ad aggiungere le attività modello**.

   Oppure

   Clic **Crea Attività Modello** per iniziare ad aggiungere attività al modello.

   L&#39;aggiunta di attività modello a un modello è identica all&#39;aggiunta di attività a un progetto.

   Per ulteriori informazioni sull’aggiunta di attività a un progetto, consulta [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Impossibile aggiungere attività ricorrenti a un modello.

1. (Facoltativo) Fai clic su **Diagramma di Gantt** nell&#39;angolo superiore destro dell&#39;Elenco task per visualizzare una rappresentazione visiva dell&#39;elenco dei task del modello.

   >[!TIP]
   >
   >Non è possibile modificare le attività direttamente da questo diagramma di Gantt.

1. Per aggiungere informazioni al nuovo modello, fare clic su **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica**.

   Per informazioni sulla modifica di un modello, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Clic **Salva modifiche**.
1. (Facoltativo) Se desideri aggiungere altri elementi al modello, consulta la sezione [Aggiungere elementi aggiuntivi a un modello](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) nell’articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Impostazioni modello determinate dall&#39;associazione di gruppi

L&#39;associazione di un modello di progetto a un gruppo (o la mancanza di un gruppo) influisce sul modo in cui le preferenze di progetto, attività e problema determinano determinate impostazioni nel modello. Per ulteriori informazioni, consulta la sezione [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) nell’articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
