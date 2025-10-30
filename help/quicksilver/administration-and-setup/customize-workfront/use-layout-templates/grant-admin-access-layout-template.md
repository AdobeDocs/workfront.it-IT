---
title: Concedere l’accesso amministrativo per un modello di layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront, puoi concedere l’accesso amministrativo per un modello layout agli amministratori di gruppi di un particolare gruppo, affinché possano modificare il modello. Questo non assegna il modello agli utenti del gruppo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Concedere l’accesso amministrativo per un modello di layout

{{preview-fast-release-general}}

In qualità di amministratore di Adobe Workfront, puoi concedere l’accesso amministrativo per un modello layout agli amministratori di gruppi di un particolare gruppo, affinché possano modificare il modello. Questo non assegna il modello agli utenti del gruppo.

Per informazioni sull&#39;assegnazione di utenti a un modello di layout, vedere [Assegnare utenti a un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
        <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Concedere l’accesso amministrativo per un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic su **Concedi l&#39;accesso a** nella sezione superiore della pagina.
1. Nella casella visualizzata fare clic su **Aggiungi un gruppo**, iniziare a digitare il nome del gruppo, fare clic sul nome quando viene visualizzato, quindi fare clic su **Fine**.

   Tutti gli utenti designati come amministratori di gruppo per il gruppo specificato possono amministrare il modello layout. Tuttavia, il modello non viene assegnato al membro del gruppo per il loro utilizzo. Per informazioni sull&#39;assegnazione di un modello di layout a un gruppo, vedere [Assegnare un modello di layout agli utenti](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) in questo articolo.

   >[!NOTE]
   >
   >* Quando un amministratore gruppo crea un modello di layout, l’assegnazione dell’accesso amministrativo è obbligatoria. Il modello di layout è designato per e visibile solo al gruppo specificato. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Per informazioni sugli amministratori di gruppi, vedere [Amministratori di gruppi](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Se non si concede l&#39;accesso amministrativo agli amministratori del gruppo in un determinato gruppo, tutti gli utenti che possono modificare gli account utente avranno accesso amministrativo al modello di layout. Alcuni amministratori di Workfront scelgono di non concedere l&#39;accesso amministrativo per un modello di layout per renderlo un modello di layout a livello di sistema.

1. Puoi fare clic su <span class="preview">**Applica**</span> o **Salva** in qualsiasi momento per salvare i tuoi progressi, quindi continuare a modificare il modello in un secondo momento.
