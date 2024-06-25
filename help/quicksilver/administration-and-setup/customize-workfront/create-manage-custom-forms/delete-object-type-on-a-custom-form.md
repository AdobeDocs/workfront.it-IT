---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminare tipi di oggetto in un modulo personalizzato
description: In un modulo personalizzato esistente è possibile eliminare i tipi di oggetto associati al modulo. Dopo questa operazione, gli utenti non potranno più allegare il modulo a oggetti di quel tipo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Eliminare tipi di oggetto in un modulo personalizzato

{{form-designer-default}}

In un modulo personalizzato esistente è possibile eliminare i tipi di oggetto associati al modulo. Dopo questa operazione, gli utenti non potranno più allegare il modulo a oggetti di quel tipo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Eliminare tipi di oggetto in un modulo personalizzato

È possibile eliminare tipi di oggetto da un modulo personalizzato esistente.

Un modulo personalizzato deve avere almeno un tipo di oggetto.

>[!CAUTION]
>
>Se il modulo personalizzato è già stato allegato a oggetti del tipo che si desidera eliminare e vi sono stati aggiunti dati, questi verranno eliminati definitivamente quando si elimina tale tipo di oggetto nel modulo. Potrebbe includere informazioni storiche di cui gli utenti avranno bisogno in un secondo momento.
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche.

{{step-1-to-setup}}

1. Clic **Forms personalizzato** nel pannello a sinistra.
1. Seleziona il modulo personalizzato da modificare, quindi fai clic su ![Icona Modifica](assets/edit-icon.png).
1. Fai clic sulla X su uno qualsiasi dei **Tipi di oggetto** da eliminare dal modulo, quindi fare clic su **Elimina** sul messaggio di avviso visualizzato.

   ![](assets/click-x-object-types.jpg)

1. (Facoltativo) Ripetere il passaggio precedente per qualsiasi altro tipo di oggetto che si desidera rimuovere dal modulo.
1. Clic **Fine**, quindi fai clic su **Salva e chiudi**.
