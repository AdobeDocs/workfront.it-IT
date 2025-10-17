---
title: Impostare una condizione personalizzata come predefinita per attività e problemi
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Quando un utente fa clic su Lavoraci o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Impostare una condizione personalizzata come predefinita per le attività e i problemi

Quando un utente fa clic su Lavoraci o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.

Workfront utilizza la condizione incorporata Going Smoothly come condizione predefinita per le attività e, separatamente, per i problemi. In qualità di amministratore di Workfront, puoi impostare la condizione predefinita per entrambi questi tipi di oggetto su una condizione personalizzata creata.

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
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Per informazioni sulla configurazione di una condizione personalizzata come condizione predefinita per i progetti, vedere [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).
