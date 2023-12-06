---
title: Aggiunta o eliminazione di tipi di oggetto da un modulo personalizzato esistente con il progettista del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile aggiungere o rimuovere tipi di oggetto dai moduli personalizzati con il progettista del modulo.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '532'
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
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
   <p>Nuovo piano: Standard</p>
   <p>oppure</p>
   <p>Piano corrente: piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td><p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Aggiungere tipi di oggetto a un modulo personalizzato esistente

È possibile aggiungere ulteriori tipi di oggetto al modulo in modo che possa essere associato a più oggetti.

>[!NOTE]
>
>Le autorizzazioni di interruzione di sezione possono essere influenzate dal tipo di oggetto. L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.
>
>Per ulteriori informazioni, consulta [Come più tipi di oggetto possono influire sulle autorizzazioni dell’interruzione di sezione](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato** nel pannello a sinistra.

   Nella visualizzazione visualizzata è possibile esaminare tutti i moduli personalizzati creati per l&#39;organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, con quale tipo di oggetto funziona e se è attivo.

1. Seleziona il modulo personalizzato a cui desideri aggiungere altri tipi di oggetto, quindi fai clic su **Modifica**.

1. Nella parte superiore del modulo fare clic sul segno più + dopo **Tipi di oggetto**, quindi seleziona il tipo desiderato nel menu visualizzato. È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   ![](assets/add-new-object.png)

1. Clic **Salva e chiudi**.

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

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato** nel pannello a sinistra.
1. Seleziona il modulo personalizzato da modificare, quindi fai clic su **Modifica**.
1. Fai clic sulla X su uno qualsiasi dei **Tipi di oggetto** da eliminare dal modulo, quindi fare clic su **Elimina** sul messaggio di avviso visualizzato.

   ![](assets/delete-object-types.png)

1. (Facoltativo) Ripetere il passaggio precedente per qualsiasi altro tipo di oggetto che si desidera rimuovere dal modulo.
1. Clic **Fine**, quindi fai clic su **Chiudi e salva**.
