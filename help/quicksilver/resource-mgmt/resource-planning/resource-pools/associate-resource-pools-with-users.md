---
product-area: resource-management
navigation-topic: resource-pools
title: Associa i pool di risorse agli utenti
description: È necessario creare un pool di risorse prima di associarlo agli utenti. È possibile associare gli utenti ai pool di risorse quando si creano i pool di risorse.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Associa i pool di risorse agli utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

I pool di risorse sono insiemi di utenti che consentono di gestire le risorse in Adobe Workfront.

È necessario creare un pool di risorse prima di associarlo agli utenti.

È possibile associare gli utenti ai pool di risorse quando si creano i pool di risorse.

Se si creano pool di risorse senza popolarli con gli utenti, è possibile associarli in seguito durante la modifica o la creazione di nuovi utenti.

Per informazioni sui pool di risorse, vedere [Panoramica sui pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Per informazioni sulla creazione di pool di risorse, vedere [Creare pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Gestisci gruppi di risorse</p> <p>Modificare l’accesso a progetti, modelli e utenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per i progetti, i modelli e gli utenti a cui si associano i pool di risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Associa i pool di risorse a un utente

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fare clic su **Utenti**.
1. Seleziona la casella accanto al nome di un utente dall&#39;elenco, quindi fai clic su **Modifica**.
1. Fare clic su **Pianificazione risorse**.
1. Inizia a digitare il nome di un pool di risorse che desideri associare all&#39;utente nel campo **Pool di risorse**, quindi selezionalo dall&#39;elenco, quando viene visualizzato.\
   È possibile associare più pool di risorse a un utente.\
   ![aggiungi_pool_risorse_a_utente.png](assets/add-resource-pool-to-user-350x307.png)

1. Fai clic su **Salva modifiche**.

Per ulteriori informazioni sulla modifica degli utenti, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Per ulteriori informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associa gruppi di risorse a utenti in blocco

È possibile modificare più utenti in blocco e associare gli stessi pool di risorse a tutti gli utenti contemporaneamente.

Per associare in blocco i pool di risorse a più utenti:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fare clic su **Utenti**.
1. Selezionare più utenti nell&#39;elenco e fare clic su **Modifica**.
1. Fare clic su **Pianificazione risorse**.
1. Inizia a digitare il nome di un pool di risorse che desideri associare agli utenti nel campo **Pool di risorse**, quindi selezionalo dall&#39;elenco, quando viene visualizzato.\
   È possibile associare più pool di risorse a più utenti.

   >[!NOTE]
   >
   >In questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivisi, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.

1. Fai clic su **Salva modifiche**.

Per ulteriori informazioni su come modificare gli utenti in blocco, vedere [Modificare i profili utente in blocco](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
