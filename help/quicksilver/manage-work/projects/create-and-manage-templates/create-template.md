---
product-area: templates
navigation-topic: templates-navigation-topic
title: Creare un modello di progetto
description: È possibile creare ed eliminare modelli dall’area Modelli. Quando si crea un nuovo modello, è possibile immettere le informazioni per tutte le attività e tutte le informazioni per le impostazioni di progetto future. Queste informazioni vengono quindi trasferite al progetto quando lo si crea dal modello.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Creare un modello di progetto

È possibile creare ed eliminare modelli dall’area Modelli. Quando si crea un nuovo modello, è possibile immettere le informazioni per tutte le attività e tutte le informazioni per le impostazioni di progetto future. Queste informazioni vengono quindi trasferite al progetto quando lo si crea dal modello.

Puoi creare un nuovo modello nei seguenti modi:

* Da zero, come descritto in questo articolo.
* Da progetti esistenti, salvando un progetto come modello.

   Per ulteriori informazioni sulla creazione di modelli da progetti esistenti, consulta [Salvare un progetto come modello](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiandolo da un altro modello.

   Per ulteriori informazioni sulla copia di un modello esistente, consulta [Copiare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Gli amministratori di Workfront possono creare modelli importando Blueprint. Per informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td> <p>Piano </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Amministratore di sistema per l’importazione di modelli da Blueprint</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Per impostazione predefinita, disponi delle autorizzazioni di gestione per i modelli creati</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un modello

1. Da **Menu principale** ![](assets/main-menu-icon.png) click **Modelli**.

1. Fai clic su **Nuovo modello**.

   Il modello è senza titolo.

   ![Nuovo modello](assets/create-template-nwe-2022-350x102.png)

1. Specificare un nome per il nuovo modello nell&#39;intestazione del modello, quindi premere **Entra.**
1. Fai clic sul pulsante **Attività dei modelli** nel pannello a sinistra.
1. Fai clic su **Inizio dell&#39;aggiunta di attività modello**.

   Oppure

   Fai clic su **Nuova attività modello** per iniziare ad aggiungere attività al modello.

   L&#39;aggiunta di attività modello a un modello è identica all&#39;aggiunta di attività a un progetto.

   Per ulteriori informazioni sull’aggiunta di attività a un progetto, consulta [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Non è possibile aggiungere attività ricorrenti a un modello.

1. (Facoltativo) Fai clic sul pulsante **Diagramma di Gantt** nell&#39;angolo in alto a destra dell&#39;Elenco attività per visualizzare una rappresentazione visiva dell&#39;elenco delle attività del modello.

   >[!TIP]
   >
   >Non è possibile modificare le attività direttamente da questo diagramma di Gantt.

1. Per aggiungere informazioni al nuovo modello, fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica**.

   Per informazioni sulla modifica di un modello, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Fai clic su **Salva modifiche**.
1. (Facoltativo) Per aggiungere altri elementi al modello, consulta la sezione . [Aggiungere altri elementi a un modello](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) nell&#39;articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Impostazioni del modello determinate dall’associazione del gruppo

L’associazione di un modello di progetto a un gruppo (o la sua assenza) influisce sul modo in cui il progetto, l’attività e le preferenze relative ai problemi determinano determinate impostazioni nel modello. Per ulteriori informazioni, consulta la sezione . [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
