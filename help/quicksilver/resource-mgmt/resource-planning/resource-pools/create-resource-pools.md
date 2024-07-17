---
product-area: resource-management
navigation-topic: resource-pools
title: Creare i pool di risorse
description: I pool di risorse sono insiemi di utenti che consentono di gestire più facilmente le risorse in Adobe Workfront. Per ulteriori informazioni sui pool di risorse, vedere Panoramica sui pool di risorse.
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# Creare i pool di risorse

I pool di risorse sono insiemi di utenti che consentono di gestire più facilmente le risorse in Adobe Workfront. Per ulteriori informazioni sui pool di risorse, vedere [Panoramica sui pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Gestisci gruppi di risorse</p> <p>Modifica l'accesso a Utenti, Progetti e Modelli</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per i progetti e i modelli a cui si desidera associare i gruppi di risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Creare un gruppo di risorse {#create-a-resource-pool}

1. Accedi come utente con accesso in modifica ai gruppi di risorse.\
   Per ulteriori informazioni, vedere [Creare un pool di risorse](#create-a-resource-pool).

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fare clic su **Risorse**.
1. Fai clic su **Pool di Risorse** nel pannello a sinistra.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Fare clic su **Nuovo pool di risorse**.
1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td>Questo è il nome del Pool di Risorse.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione</strong></td>
      <td>Breve descrizione del gruppo di risorse. Ad esempio, puoi specificare a quale scopo deve essere utilizzato.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Membri del gruppo</strong></td>
      <td><p> Aggiungere singolarmente gli utenti al Pool di Risorse.<br>Oppure <br>Per aggiungere contemporaneamente molti utenti al gruppo di risorse. Puoi aggiungere una delle seguenti entità associate a utenti o a una raccolta di utenti:
        <ul>
         <li><strong>Team</strong>: tutti i membri del team vengono aggiunti al Pool di Risorse.</li>
         <li><strong>Gruppi</strong>: tutti i membri del gruppo vengono aggiunti al Pool di Risorse.</li>
         <li><strong>Ruoli</strong>: tutti gli utenti associati a tale ruolo vengono aggiunti al Pool di Risorse.</li>
         <li><strong>Società</strong>: tutti gli utenti della società vengono aggiunti al Pool di Risorse.</li>
        </ul><p>Suggerimento: puoi aggiungere solo utenti attivi, team, <span>ruoli,</span> o aziende.</p><p>Nota: se un utente diventa membro di un gruppo, team, società o è associato a una mansione dopo che il gruppo, il team, la società o la mansione sono stati aggiunti al Pool di risorse, il nuovo membro non viene aggiunto automaticamente al Pool di risorse. <br>Se un utente appartiene al team, al gruppo, alla società e alla mansione che si sta aggiungendo, l'utente verrà aggiunto una sola volta al Pool di Risorse.<br>Gli utenti disattivati dopo essere stati aggiunti al Pool di Risorse vengono visualizzati in grigio nell'elenco degli utenti e contrassegnati come disattivati.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facoltativo) Usa il collegamento **Annulla** per rimuovere gli utenti aggiunti tramite un gruppo, un team, una società o una mansione.

   >[!NOTE]
   >
   >Non esiste alcun limite al numero di utenti che è possibile avere in un Pool di Risorse. Tuttavia, si consiglia di non aggiungere troppi utenti a un Pool di Risorse, altrimenti la gestione delle risorse potrebbe diventare una sfida. L&#39;elenco degli utenti mostra solo i primi 2.000 utenti nel Pool di Risorse e sono elencati in ordine alfabetico.

   ![Pool di Risorse_NUOVO___UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Facoltativo) Fai clic sull’icona X a destra del nome di un utente per rimuoverlo. Per ulteriori informazioni sulla rimozione degli utenti da un pool di risorse, vedere [Rimuovere gli utenti dai pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Facoltativo) Utilizza l&#39;opzione **Cerca** per trovare un utente nel Pool di Risorse.
1. Fai clic su **Crea**.
