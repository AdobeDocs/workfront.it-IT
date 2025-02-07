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
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Spostare un gruppo

È possibile spostare un gruppo in un altro gruppo gestito dall&#39;utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Seleziona il gruppo di destinazione in cui desideri spostare il gruppo, quindi fai clic sull&#39;icona Modifica ![icona Modifica](assets/edit-icon.png).
1. Nella casella **Modifica gruppo** visualizzata, in **Membri gruppo e amministratori gruppo**, iniziare a digitare il nome del gruppo che si desidera spostare, quindi fare clic su di esso quando viene visualizzato.
1. Fai clic su **Salva**.

>[!TIP]
>
>È inoltre possibile impostare un sottogruppo come gruppo di primo livello. Per istruzioni, vedere la sezione [Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di primo livello](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
