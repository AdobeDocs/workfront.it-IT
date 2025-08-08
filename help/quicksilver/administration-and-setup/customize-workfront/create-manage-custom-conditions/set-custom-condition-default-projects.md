---
title: Imposta una condizione personalizzata come predefinita per i progetti
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Se il Tipo di condizione di un progetto è impostato su Stato avanzamento invece che Manuale, Adobe Workfront visualizza automaticamente una delle tre condizioni predefinite incorporate nel progetto (Su destinazione, A rischio o In difficoltà) durante l’avanzamento, come spiegato in Panoramica sulla condizione e sul tipo di condizione del progetto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 183bdced08da75cfb15fe2cc0f0804dec7f07f23
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Impostare una condizione personalizzata come predefinita per i progetti

Se il tipo di condizione di un progetto è impostato su Stato di avanzamento invece di Manuale, Adobe Workfront visualizza automaticamente una delle tre condizioni predefinite incorporate nel progetto (Su destinazione, A rischio o In difficoltà) durante l&#39;avanzamento, come spiegato in [Panoramica sulla condizione e sul tipo di condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Condizione nell&#39;intestazione del progetto](assets/condition-in-project-header-nwe.png)

È possibile impostare le condizioni personalizzate come condizioni predefinite anziché utilizzare queste tre condizioni predefinite incorporate. Ad esempio, puoi modificare la condizione predefinita In Target in modo che venga visualizzata come Finestra di tracciamento in tutti i progetti.

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
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Imposta una condizione personalizzata come condizione predefinita per tutti i progetti:

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Condizioni**.

1. Fare clic sulla scheda **Progetti**.
1. Fare clic su **Imposta condizioni predefinite**.
1. Nel menu a discesa della condizione predefinita che si desidera modificare, fare clic sulla condizione personalizzata che si desidera utilizzare.
1. Ripetere il passaggio precedente per qualsiasi altra condizione predefinita che si desidera modificare.
1. Fai clic su **Salva**.

Per informazioni sull&#39;impostazione di una condizione personalizzata come condizione predefinita per attività e problemi, vedere [Impostare una condizione personalizzata come predefinita per attività e problemi](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Per informazioni sulla configurazione di un progetto in modo che gli utenti possano aggiornarne manualmente le condizioni, vedere [Aggiorna condizione per attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
