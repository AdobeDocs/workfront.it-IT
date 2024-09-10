---
title: Impostare una condizione personalizzata come predefinita per attività e problemi
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Quando un utente fa clic su Lavoraci o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Impostare una condizione personalizzata come predefinita per le attività e i problemi

Quando un utente fa clic su Lavoraci o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.

Workfront utilizza la condizione incorporata Going Smoothly come condizione predefinita per le attività e, separatamente, per i problemi. In qualità di amministratore di Workfront, puoi impostare la condizione predefinita per entrambi questi tipi di oggetto su una condizione personalizzata creata.

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

## Imposta una condizione personalizzata come condizione predefinita per le attività o per i problemi:

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Condizioni**.

1. Fai clic sulla scheda **Attività** o **Problemi**.

1. Fare clic su **Imposta condizioni predefinite**.
1. Nel menu a discesa, fai clic sulla condizione personalizzata che desideri come condizione predefinita per le attività (o i problemi).
1. Fai clic su **Salva**.

>[!NOTE]
>
>* Un utente che è assegnato a un’attività o a un problema, o che dispone delle autorizzazioni di gestione su di esso, può modificare manualmente la propria condizione. Per ulteriori informazioni, vedere [Aggiorna condizione per attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Le tre condizioni predefinite per le attività e i problemi forniti con Workfront procedono senza intoppi, con alcuni problemi e importanti ostacoli. Non è possibile nascondere o eliminare queste condizioni, ma è possibile modificarne nomi e colori. Oppure puoi crearne di nuovi da utilizzare, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

Per informazioni sulla configurazione di una condizione personalizzata come condizione predefinita per i progetti, vedere [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Per informazioni sulle condizioni personalizzate, vedere [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
