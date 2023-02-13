---
product-area: resource-management
navigation-topic: resource-pools
title: Creare pool di risorse
description: I pool di risorse sono raccolte di utenti che consentono di gestire più facilmente le risorse in Adobe Workfront. Per ulteriori informazioni sui pool di risorse, consulta Panoramica sui pool di risorse .
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---

# Creare pool di risorse

I pool di risorse sono raccolte di utenti che consentono di gestire più facilmente le risorse in Adobe Workfront. Per ulteriori informazioni sui pool di risorse, consulta [Panoramica dei pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Gestione pool di risorse</p> <p>Modificare l’accesso a utenti, progetti e modelli</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti e i modelli a cui si desidera associare i pool di risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un pool di risorse {#create-a-resource-pool}

1. Accedi come utente che ha accesso alla modifica dei pool di risorse.\
   Per ulteriori informazioni, consulta [Creare un pool di risorse](#create-a-resource-pool).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.
1. Fai clic su **Pool di risorse** nel pannello a sinistra.\
   ![resource_pool_tab.png](assets/resource-pools-tab-350x198.png)

1. Fai clic su **Nuovo pool di risorse**.
1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td>Nome del pool di risorse.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione</strong></td>
      <td>Breve descrizione di questo pool di risorse. Ad esempio, puoi specificare lo scopo da utilizzare.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Membri del gruppo</strong></td>
      <td><p> Aggiungi gli utenti al pool di risorse singolarmente.<br>Oppure <br>Per aggiungere una grande quantità di utenti al pool di risorse alla volta. Puoi aggiungere una delle seguenti entità associate agli utenti o alla raccolta di utenti:
        <ul>
         <li><strong>Team</strong>: tutti i membri del team vengono aggiunti al pool di risorse.</li>
         <li><strong>Gruppi</strong>: tutti i membri del gruppo vengono aggiunti al pool di risorse.</li>
         <li><strong>Ruoli</strong>: tutti gli utenti associati a tale ruolo vengono aggiunti al pool di risorse.</li>
         <li><strong>Aziende</strong>: tutti gli utenti della società vengono aggiunti al pool di risorse.</li>
        </ul><p>Suggerimento: Puoi aggiungere solo utenti attivi, team, <span>ruoli,</span> o le aziende.</p><p>Nota: Se un utente diventa membro di un gruppo, team, società o è associato a un ruolo di lavoro dopo l'aggiunta del gruppo, del team, della società o del ruolo di lavoro al pool di risorse, il nuovo membro non viene aggiunto automaticamente al pool di risorse. <br>Se un utente appartiene al team, al gruppo, alla società e al ruolo di lavoro che si sta aggiungendo, allo stesso tempo l'utente viene aggiunto una sola volta al pool di risorse.<br>Gli utenti disattivati dopo l’aggiunta al pool di risorse vengono visualizzati in grigio nell’elenco degli utenti e contrassegnati come disattivati.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facoltativo) Utilizza il **Annulla** collegamento per rimuovere gli utenti aggiunti tramite un gruppo, un team, una società o un ruolo di lavoro.

   >[!NOTE]
   >
   >Non vi è alcun limite al numero di utenti che è possibile avere in un pool di risorse. Tuttavia, consigliamo di non aggiungere troppi utenti a un pool di risorse, in quanto altrimenti la gestione delle risorse potrebbe diventare una sfida. L’elenco degli utenti mostra solo i primi 2.000 utenti nel pool di risorse, elencati in ordine alfabetico.

   ![Pool_risorse_NUOVO__UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Facoltativo) Fai clic sull’icona X a destra del nome di un utente per rimuovere un utente. Per ulteriori informazioni sulla rimozione degli utenti da un pool di risorse, consulta [Rimuovere utenti dai pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Facoltativo) Utilizza il **Ricerca** per trovare un utente nel pool di risorse.
1. Fai clic su **Crea**.
