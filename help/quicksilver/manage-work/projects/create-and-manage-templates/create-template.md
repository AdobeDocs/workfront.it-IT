---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creare un modello di progetto
description: È possibile creare ed eliminare modelli dall'area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e tutte le informazioni per le impostazioni future del progetto. Queste informazioni verranno quindi trasferite al progetto quando lo crei dal modello.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Creare un modello di progetto

È possibile creare ed eliminare modelli dall&#39;area Modelli. Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e tutte le informazioni per le impostazioni future del progetto. Queste informazioni verranno quindi trasferite al progetto quando lo crei dal modello.

>[!NOTE]
>
>Un modello e le relative attività non dispongono di date effettive, ma di un&#39;indicazione del giorno (a partire dal quale potrebbe iniziare il progetto futuro) in cui un&#39;attività potrebbe iniziare e del giorno in cui l&#39;attività potrebbe dover essere completata. Quando si utilizzano i modelli per creare i progetti futuri, i progetti riceveranno le date effettive. Per informazioni, consulta [Creare un progetto](../create-projects/create-project.md).


È possibile creare un nuovo modello nei modi seguenti:

* Da zero, come descritto in questo articolo.
* Da progetti esistenti, salvando un progetto come modello.

  Per ulteriori informazioni sulla creazione di modelli da progetti esistenti, consulta [Salvare un progetto come modello](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiandolo da un altro modello.

  Per ulteriori informazioni sulla copia di un modello esistente, vedere [Copiare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Se sei un amministratore di Workfront, puoi creare modelli importando Blueprint. Per informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Amministratore di sistema per l’importazione di modelli da Blueprint</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Per impostazione predefinita, disponi delle autorizzazioni di gestione per i modelli creati</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare un modello

1. Dalla sezione **Menu principale** ![](assets/main-menu-icon.png) click **Modelli**.

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
1. (Facoltativo) Se desideri aggiungere altri elementi al modello, consulta la sezione [Aggiungere elementi aggiuntivi a un modello](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) nell’articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Impostazioni modello determinate dall&#39;associazione di gruppi

L&#39;associazione di un modello di progetto a un gruppo (o la sua assenza) influisce sul modo in cui le preferenze di progetto, attività e problema determinano determinate impostazioni nel modello. Per ulteriori informazioni, consulta la sezione [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) nell’articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
