---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminare o disattivare un modulo personalizzato
description: È possibile eliminare o disattivare un modulo personalizzato dal sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Eliminare o disattivare un modulo personalizzato

È possibile eliminare o disattivare un modulo personalizzato dal sistema.

>[!CAUTION]
>
>L’eliminazione di un modulo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati presenti negli oggetti associati al modulo. Impossibile recuperare i dati eliminati. È consigliabile disattivare un modulo personalizzato, se si disattiva un modulo personalizzato non più utilizzato, conservare tutti i dati storici associati.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Eliminare un modulo personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato.**
1. Seleziona il modulo personalizzato, quindi fai clic su **Elimina**.
1. Se si desidera eliminare definitivamente il modulo personalizzato e tutti i dati associati agli oggetti in cui è stato allegato, fare clic su **Sì, Elimina**.

## Disattivare un modulo personalizzato

È possibile disattivare i moduli personalizzati non più utilizzati senza perdere i dati storici associati. Gli utenti non possono aggiungere un modulo personalizzato inattivo agli oggetti, ma possono comunque visualizzare e aggiungere dati ai campi degli oggetti in cui era già allegato.

Anche i campi di un modulo personalizzato inattivo possono essere modificati in linea in una visualizzazione. Se durante una modifica in linea un utente aggiunge un campo da un modulo personalizzato inattivo, il modulo si allega automaticamente all’oggetto, anche se il modulo personalizzato è disattivato.

Se si riattiva un modulo personalizzato, vengono mantenute le impostazioni precedenti e gli utenti possono interagire con esso come se non fosse mai stato disattivato.

Per disattivare un modulo personalizzato:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fare clic sul nome del modulo personalizzato che si desidera disattivare.
1. Fai clic sul pulsante **Impostazioni modulo** scheda .
1. Disattiva la **È attivo** opzione .
1. Fai clic su **Salva e chiudi**.
