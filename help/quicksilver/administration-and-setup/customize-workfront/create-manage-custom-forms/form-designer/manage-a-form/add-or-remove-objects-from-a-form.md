---
title: Aggiunta o eliminazione di tipi di oggetto da un modulo personalizzato esistente con il progettista del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile aggiungere o rimuovere tipi di oggetto dai moduli personalizzati con il progettista del modulo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Aggiunta o eliminazione di tipi di oggetto da un modulo personalizzato esistente con il progettista del modulo

È possibile aggiungere o eliminare tipi di oggetto da un modulo personalizzato esistente mediante lo strumento di progettazione del modulo.

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td><p>Accesso amministrativo ai moduli personalizzati</p></td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aggiungere tipi di oggetto a un modulo personalizzato esistente

È possibile aggiungere ulteriori tipi di oggetto al modulo in modo che possa essere associato a più oggetti.

>[!NOTE]
>
>Le autorizzazioni di interruzione di sezione possono essere influenzate dal tipo di oggetto. L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.
>
>Per ulteriori informazioni, vedere [Come più tipi di oggetto possono influire sulle autorizzazioni di interruzione di sezione](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   Nella visualizzazione visualizzata è possibile esaminare tutti i moduli personalizzati creati per l&#39;organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, con quale tipo di oggetto funziona e se è attivo.

1. Selezionare il modulo personalizzato a cui si desidera aggiungere altri tipi di oggetto, quindi fare clic su ![Icona Modifica](assets/edit-icon2.png).

1. Nella parte superiore del modulo fare clic sul segno più + dopo **Tipi di oggetto**, quindi selezionare il tipo desiderato nel menu visualizzato. È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   ![](assets/add-new-object.png)

1. Fare clic su **Salva e chiudi**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

## Eliminare tipi di oggetto in un modulo personalizzato

È possibile eliminare tipi di oggetto da un modulo personalizzato esistente. Un modulo personalizzato deve avere almeno un tipo di oggetto.

>[!CAUTION]
>
>Se il modulo personalizzato è già stato allegato a oggetti del tipo che si desidera eliminare e vi sono stati aggiunti dati, questi verranno eliminati definitivamente quando si elimina tale tipo di oggetto nel modulo. Potrebbe includere informazioni storiche di cui gli utenti avranno bisogno in un secondo momento.
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche.

Per eliminare un tipo di oggetto:

{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
1. Seleziona il modulo personalizzato da modificare, quindi fai clic sull&#39;![icona Modifica](assets/edit-icon2.png).
1. Fare clic sulla X su uno qualsiasi dei **Tipi di oggetto** che si desidera eliminare dal modulo.

   ![](assets/delete-object-types.png)

1. (Facoltativo) Ripetere il passaggio precedente per qualsiasi altro tipo di oggetto che si desidera rimuovere dal modulo.
1. Fai clic su **Applica**, quindi su **Salva e chiudi**.
