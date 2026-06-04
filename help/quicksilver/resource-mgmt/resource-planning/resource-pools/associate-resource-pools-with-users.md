---
product-area: resource-management
navigation-topic: resource-pools
title: Associa gruppi di risorse agli utenti
description: È necessario creare un pool di risorse prima di associarlo agli utenti. È possibile associare gli utenti ai pool di risorse quando si creano i pool di risorse.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
TQID: https://experienceleague.adobe.com/OQBqFxBx-VGQsWF-2yGgcZk1EO-ZQ0MAlMsSH3fiMZo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 435
ht-degree: 10%

---

# Associare pool di risorse agli utenti

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Gestisci gruppi di risorse</p> <p>Modificare l’accesso a progetti, modelli e utenti</p></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per i progetti, i modelli e gli utenti a cui vuoi associare i Pool di Risorse</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associa i pool di risorse a un utente

{{step-1-to-users}}

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

{{step-1-to-users}}

1. Selezionare più utenti nell&#39;elenco e fare clic su **Modifica**.
1. Fare clic su **Pianificazione risorse**.
1. Inizia a digitare il nome di un pool di risorse che desideri associare agli utenti nel campo **Pool di risorse**, quindi selezionalo dall&#39;elenco, quando viene visualizzato.\
   È possibile associare più pool di risorse a più utenti.

   >[!NOTE]
   >
   >In questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivisi, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.

1. Fai clic su **Salva modifiche**.

Per ulteriori informazioni su come modificare gli utenti in blocco, vedere [Modificare i profili utente in blocco](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
