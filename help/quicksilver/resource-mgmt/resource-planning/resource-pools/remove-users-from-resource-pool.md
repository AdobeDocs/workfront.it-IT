---
product-area: resource-management
navigation-topic: resource-pools
title: Rimuovere utenti dai pool di risorse
description: Sebbene non vi sia alcun limite al numero di utenti che è possibile avere in un pool di risorse, l'elenco degli utenti visualizza solo i primi 2.000 utenti, elencati in ordine alfabetico.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f18bf59202ba524173774a0215f4071bd6e77432
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Rimuovere utenti dai pool di risorse

{{preview-and-fast-release-Q424}}

Sebbene non vi sia alcun limite al numero di utenti che è possibile avere in un pool di risorse, l&#39;elenco degli utenti visualizza solo i primi 2.000 utenti, elencati in ordine alfabetico.

È consigliabile rimuovere gli utenti che sono stati disattivati o che hanno spostato ruoli o reparti, per assicurarsi di disporre sempre di un elenco accurato di utenti in tutti i pool di risorse.

Per ulteriori informazioni sui pool di risorse, vedere [Panoramica sui pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Gestisci gruppi di risorse</p> <p>Accesso di visualizzazione o superiore agli utenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Rimuovere utenti da un gruppo di risorse

È possibile rimuovere utenti da un Pool di Risorse quando tali utenti non sono più necessari in tale Pool.

Per rimuovere un utente da un gruppo di risorse:

{{step1-to-resourcing}}

1. Fai clic su **Pool di Risorse** nel pannello a sinistra.
1. Seleziona un Pool di Risorse e fai clic su **Modifica**.
Oppure\
   Fare clic sul nome di un gruppo di risorse.

1. Inizia a digitare il nome di un utente da rimuovere nel campo **Cerca in questo Pool di Risorse**.\
   Oppure\
   Per rimuovere tutti gli utenti associati a tali entità, inizia a digitare il nome di un&#39;azienda, una mansione, un team o un gruppo.

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:<span>

   ![Rimuovi utenti dal Pool di Risorse](assets/remove-users-from-resource-pool.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Ricerca nel pool di risorse](assets/search-inside-new-resource-pool-350x314.png)

1. Fai clic sull&#39;icona &quot;x&quot; a livello di utente per rimuovere un utente dal Pool di Risorse. Vengono rimossi da tutti gli elenchi in cui compaiono.\
   Oppure\
   Per rimuovere tutti gli utenti associati a una mansione, un gruppo, un team o una società, fare clic su **Rimuovi** a livello di mansione, gruppo, team o società. In questo modo tutti gli utenti associati a tale mansione, gruppo, team o società verranno rimossi dal Pool di Risorse.

1. Fai clic su **Salva**.
