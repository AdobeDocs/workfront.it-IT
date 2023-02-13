---
product-area: resource-management
navigation-topic: resource-pools
title: Associare pool di risorse con gli utenti
description: Associare pool di risorse con gli utenti
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Associare pool di risorse con gli utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

I pool di risorse sono raccolte di utenti che consentono di gestire le risorse in Adobe Workfront.

È necessario creare un pool di risorse prima di associarlo agli utenti.

È possibile associare gli utenti ai pool di risorse durante la creazione dei pool di risorse.

Se si creano pool di risorse senza popolarli con gli utenti, in seguito è possibile associarli agli utenti durante la modifica o la creazione di nuovi utenti.

Per informazioni sui pool di risorse, consulta [Panoramica dei pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Per informazioni sulla creazione di pool di risorse, consulta [Creare pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Gestione pool di risorse</p> <p>Accesso a progetti, modelli e utenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti, i modelli e gli utenti a cui si associano i pool di risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Associa pool di risorse a un utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Utenti**.
1. Seleziona dall’elenco la casella accanto al nome di un utente, quindi fai clic su **Modifica**.
1. Fai clic su **Pianificazione delle risorse**.
1. Inizia a digitare il nome di un pool di risorse che desideri associare all&#39;utente nel **Pool di risorse** quindi selezionarlo dall&#39;elenco quando viene visualizzato.\
   È possibile associare più pool di risorse a un utente.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Fai clic su **Salva modifiche**.

Per ulteriori informazioni sulla modifica degli utenti, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Per ulteriori informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associare pool di risorse con utenti in blocco

È possibile modificare più utenti in blocco e associare contemporaneamente gli stessi pool di risorse a tutti gli utenti.

Per associare pool di risorse a più utenti in blocco:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Utenti**.
1. Seleziona diversi utenti nell’elenco e fai clic su **Modifica**.
1. Fai clic su **Pianificazione delle risorse**.
1. Inizia a digitare il nome di un pool di risorse che desideri associare agli utenti nel **Pool di risorse** quindi selezionarlo dall&#39;elenco quando viene visualizzato.\
   È possibile associare più pool di risorse a più utenti.

   >[!NOTE]
   >
   >In questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivise, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.

1. Fai clic su **Salva modifiche**.

Per ulteriori informazioni su come modificare gli utenti in blocco, consulta [Modificare in blocco i profili utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
