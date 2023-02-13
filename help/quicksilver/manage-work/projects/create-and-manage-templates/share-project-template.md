---
product-area: templates
navigation-topic: templates-navigation-topic
title: Condividere i modelli di progetto
description: Puoi condividere un modello con gli utenti oppure puoi definire in che modo i progetti creati da un modello verranno condivisi con gli utenti utilizzando le seguenti opzioni di condivisione a livello di modello.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Condividere i modelli di progetto

Puoi condividere un modello con gli utenti oppure puoi definire in che modo i progetti creati da un modello verranno condivisi con gli utenti utilizzando le seguenti opzioni di condivisione a livello di modello.

Quando si condivide un oggetto in Adobe Workfront, è possibile consentire ad altri utenti di visualizzare, contribuire o modificare tale oggetto.

Per informazioni sulle autorizzazioni di Workfront, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per informazioni sulle autorizzazioni che puoi concedere agli utenti quando condividi un modello, vedi [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Condividere un modello {#share-a-template}

Puoi condividere i tuoi modelli con altri utenti utilizzando Condivisione modelli. Questa azione definisce gli utenti autorizzati per il modello.

>[!NOTE]
>
>Quando si designa un utente attivo come proprietario del modello, tale utente riceve automaticamente le autorizzazioni di gestione sul modello. Per informazioni sulla designazione di un utente come proprietario del modello, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Per condividere un modello:

1. Da **Menu principale** icona ![](assets/main-menu-icon.png), fai clic su **Modelli**.

1. Esegui una delle operazioni seguenti:\
   Fai clic sul nome di un modello per aprirlo, quindi fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png), quindi **Condivisione dei modelli**.

   Oppure

   Seleziona un modello dall’elenco, fai clic sull’icona Condividi . ![](assets/share-icon.png), quindi fai clic su **Modello.**

   >[!TIP]
   >
   >È possibile condividere un oggetto solo con utenti attivi, team, ruoli o aziende.

1. In **Accesso a modelli** selezionare le persone, i team, i ruoli, i gruppi o le aziende con cui si desidera condividere il modello.

   Puoi anche fare clic sul pulsante **Opzioni** per rendere il modello disponibile a livello di sistema:

1. Dal menu a discesa per ogni entità con cui stai condividendo, seleziona una delle seguenti opzioni:

   * **Visualizza**: Gli utenti con queste autorizzazioni possono visualizzare il modello e creare un progetto utilizzando esso o allegarlo a un progetto esistente.

      >[!TIP]
      >
      >Per poter creare progetti, l’amministratore di Workfront deve concedere all’utente l’accesso a Modifica progetti.

   * **Gestisci**: Gli utenti con queste autorizzazioni possono modificare o eliminare il modello.

      Per informazioni sulle impostazioni avanzate ![](assets/gear-icon-in-access-levels.png) disponibile qui, vedi la sezione [Impostazioni avanzate per la condivisione dei modelli](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) nell&#39;articolo [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Fai clic su **Salva**.

## Condivisione di un progetto da un modello {#share-a-project-from-a-template}

Con la condivisione dei progetti modello, puoi definire chi dispone delle autorizzazioni sui progetti creati dal modello a livello di modello.

Per condividere con gli utenti progetti futuri creati da un modello:

1. Esegui una delle operazioni seguenti:\
   Fai clic sul nome di un modello per aprirlo, quindi fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png), quindi **Condivisione dei modelli**.

   ![Condividi progetto da modello](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Oppure

   Seleziona un modello dall’elenco, fai clic su **Condividi**, quindi fai clic su **Progetto.**

1. In **Accesso al progetto** seleziona le persone, i team, i ruoli, i gruppi o le aziende con cui è condiviso il modello.

   >[!TIP]
   >
   >È possibile condividere un oggetto solo con utenti attivi, team, ruoli o aziende.

1. Dal menu a discesa per ogni entità, seleziona una delle seguenti opzioni:

   * **Nessun accesso**: Puoi specificare quali utenti non avranno accesso al modello.\
      Questa opzione è disponibile solo quando si condividono in blocco progetti da modelli. 
   * **Visualizza**: Gli utenti con queste autorizzazioni possono visualizzare i progetti creati dal modello.
   * **Collaborare**: Gli utenti con queste autorizzazioni possono contribuire ai progetti creati dal modello 
   * **Gestisci**: Gli utenti con queste autorizzazioni possono gestire o eliminare i progetti creati da questo modello.

1. (Facoltativo) Fai clic sul pulsante **Opzioni** per rendere i progetti disponibili a livello di sistema.
1. Fai clic su **Salva**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Condividere in massa modelli e progetti da modelli

È possibile condividere più modelli e progetti contemporaneamente da più modelli.

>[!NOTE]
>
>Quando selezioni più modelli, non puoi visualizzare chi dispone già delle autorizzazioni per i singoli modelli.

1. Passa a un elenco di modelli.
1. Seleziona più modelli, quindi fai clic su ![Condividi](assets/share-icon.png).

   ![Condividere in massa modelli o progetti](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >È possibile condividere un oggetto solo con utenti attivi, team, ruoli o aziende.

1. Fai clic su **Modello** per condividere i modelli selezionati.

   Oppure

   Fai clic su **Progetto** per condividere i progetti che verranno creati dai modelli selezionati.

1. Continua a condividere i modelli o i progetti, come descritto nelle sezioni seguenti di questo articolo:

   * [Condividere un modello](#share-a-template)
   * [Condivisione di un progetto da un modello](#share-a-project-from-a-template)
