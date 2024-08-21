---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Spostare un gruppo
description: È possibile spostare un gruppo in un altro gruppo gestito dall'utente.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 1%

---

# Spostare un gruppo

È possibile spostare un gruppo in un altro gruppo gestito dall&#39;utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Spostare un gruppo in un altro gruppo

>[!NOTE]
>
>Se gli stati del gruppo spostato sono bloccati, eredita gli stati del nuovo gruppo padre.
>
>Se gli stati del gruppo spostato sono sbloccati, non ereditano gli stati del nuovo gruppo padre e non assumono gli stati del nuovo gruppo padre.
>
>Per ulteriori informazioni sugli stati del gruppo, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) e [Creare o modificare uno stato del gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Selezionare il gruppo di destinazione in cui si desidera spostare il gruppo, quindi fare clic sull&#39;icona Modifica ![](assets/edit-icon.png).
1. Nella casella **Modifica gruppo** visualizzata, in **Membri gruppo e amministratori gruppo**, iniziare a digitare il nome del gruppo che si desidera spostare, quindi fare clic su di esso quando viene visualizzato.
1. Fai clic su **Salva**.

>[!TIP]
>
>È inoltre possibile impostare un sottogruppo come gruppo di primo livello. Per istruzioni, vedere la sezione [Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di primo livello](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
