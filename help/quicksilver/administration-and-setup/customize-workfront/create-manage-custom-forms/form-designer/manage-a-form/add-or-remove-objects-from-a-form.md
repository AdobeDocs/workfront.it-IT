---
title: Aggiunta o eliminazione di tipi di oggetto da un modulo personalizzato esistente con la struttura del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile aggiungere o rimuovere tipi di oggetti dai moduli personalizzati con la struttura del modulo.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# Aggiunta o eliminazione di tipi di oggetto da un modulo personalizzato esistente con la struttura del modulo

È possibile aggiungere o eliminare tipi di oggetto da un modulo personalizzato esistente con la struttura del modulo.

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
   <td>
   <p>Piano attuale: Standard</p>
   <p>oppure</p>
   <p>Piano legacy: Pianificare</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td><p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Aggiungere tipi di oggetto a un modulo personalizzato esistente

È possibile aggiungere ulteriori tipi di oggetti al modulo in modo che possa essere collegato a più oggetti.

>[!NOTE]
>
>Le autorizzazioni di interruzione di sezione possono essere influenzate dal tipo di oggetto. L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.
>
>Per ulteriori informazioni, consulta [Effetti di più tipi di oggetti sulle autorizzazioni delle interruzioni di sezione](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   Nella visualizzazione visualizzata, è possibile esaminare tutti i moduli personalizzati creati per la propria organizzazione. È inoltre possibile vedere chi ha creato ciascun modulo, con quale tipo di oggetto funziona e se è attivo.

1. Selezionare il modulo personalizzato a cui si desidera aggiungere altri tipi di oggetto, quindi fare clic su **Modifica**.

1. Nella parte superiore del modulo, fare clic sul segno più + dopo **Tipi di oggetti**, quindi seleziona il tipo desiderato nel menu visualizzato. È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   ![](assets/add-new-object.png)

1. Fai clic su **Salva e chiudi**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere il modulo aperto.

## Eliminare i tipi di oggetto in un modulo personalizzato

È possibile eliminare i tipi di oggetto da un modulo personalizzato esistente. Un modulo personalizzato deve avere almeno un tipo di oggetto.

>[!CAUTION]
>
>Se il modulo personalizzato è già stato associato a oggetti del tipo che si desidera eliminare e a cui si desidera aggiungere dati, tali dati vengono eliminati definitivamente quando si elimina tale tipo di oggetto sul modulo. Potrebbe includere informazioni storiche di cui gli utenti avranno bisogno in un secondo momento.
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche apportate.

Per eliminare un tipo di oggetto:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
1. Selezionare il modulo personalizzato da modificare, quindi fare clic su **Modifica**.
1. Fai clic sulla X su uno dei **Tipi di oggetti** che si desidera eliminare dal modulo, quindi fare clic su **Elimina** nel messaggio di avviso visualizzato.

   ![](assets/delete-object-types.png)

1. (Facoltativo) Ripetere il passaggio precedente per qualsiasi altro tipo di oggetto che si desidera rimuovere dal modulo.
1. Fai clic su **Fine**, quindi fai clic su **Chiudi e salva**.
