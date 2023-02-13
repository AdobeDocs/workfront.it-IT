---
title: Imposta una condizione personalizzata come predefinita per le attività e i problemi
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Quando un utente fa clic su Lavora su o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Imposta una condizione personalizzata come predefinita per le attività e i problemi

Quando un utente fa clic su Lavora su o aggiunge un commento di aggiornamento a una nuova attività a cui è stato assegnato (senza impostare manualmente una condizione per l’attività), Adobe Workfront visualizza la condizione predefinita per le attività, configurata in Configurazione. Lo stesso vale per i problemi.

Workfront utilizza la condizione integrata Andare liscio come condizione predefinita per le attività e, separatamente, per i problemi. In qualità di amministratore di Workfront, è possibile modificare la condizione predefinita per entrambi questi tipi di oggetti in una condizione personalizzata creata dall’utente.

## Requisiti di accesso

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Imposta una condizione personalizzata come condizione predefinita per le attività o per i problemi:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Condizioni**.

1. Fai clic sul pulsante **Attività** o **Problemi** scheda .

1. Fai clic su **Imposta condizioni predefinite**.
1. Nel menu a discesa, fare clic sulla condizione personalizzata che si desidera utilizzare come condizione predefinita per le attività (o problemi).
1. Fai clic su **Salva**.

>[!NOTE]
>
>* Un utente assegnato a un&#39;attività o a un problema, o che dispone di autorizzazioni di gestione, può modificare manualmente la sua condizione. Per ulteriori informazioni, consulta [Aggiorna condizione per attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Le tre condizioni predefinite per le attività e i problemi che vengono forniti con Workfront sono Andare liscio, alcune preoccupazioni e i principali blocchi di marcia. Non è possibile nascondere o eliminare queste condizioni, ma è possibile modificarne nomi e colori. Oppure puoi crearne di nuovi da utilizzare, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>


Per informazioni sulla configurazione di una condizione personalizzata come condizione predefinita per i progetti, consulta [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Per informazioni sulle condizioni personalizzate, consulta [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
