---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminare i tipi di oggetto in un modulo personalizzato
description: In un modulo personalizzato esistente è possibile eliminare i tipi di oggetto associati al modulo. In seguito a questa operazione, gli utenti non possono più collegare il modulo a oggetti di quel tipo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Eliminare i tipi di oggetto in un modulo personalizzato

In un modulo personalizzato esistente è possibile eliminare i tipi di oggetto associati al modulo. In seguito a questa operazione, gli utenti non possono più collegare il modulo a oggetti di quel tipo.

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

## Eliminare i tipi di oggetto in un modulo personalizzato

È possibile eliminare i tipi di oggetto da un modulo personalizzato esistente.

Un modulo personalizzato deve avere almeno un tipo di oggetto.

>[!CAUTION]
>
>Se il modulo personalizzato è già stato associato a oggetti del tipo che si desidera eliminare e a cui si desidera aggiungere dati, tali dati vengono eliminati definitivamente quando si elimina tale tipo di oggetto sul modulo. Potrebbe includere informazioni storiche di cui gli utenti avranno bisogno in un secondo momento.
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche apportate.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
1. Selezionare il modulo personalizzato da modificare, quindi fare clic su **Modifica**.
1. Fai clic sulla X su uno dei **Tipi di oggetti** che si desidera eliminare dal modulo, quindi fare clic su **Elimina** nel messaggio di avviso visualizzato.

   ![](assets/click-x-object-types.jpg)

1. (Facoltativo) Ripetere il passaggio precedente per qualsiasi altro tipo di oggetto che si desidera rimuovere dal modulo.
1. Fai clic su **Fine**, quindi fai clic su **Chiudi e salva**.
