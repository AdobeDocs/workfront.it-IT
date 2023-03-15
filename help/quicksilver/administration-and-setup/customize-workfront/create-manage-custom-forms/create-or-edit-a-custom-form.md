---
title: Creare o modificare un modulo personalizzato con il modulo precedente
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile creare o modificare un nuovo modulo personalizzato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: bf0d9201d50f16795676928e55b82d854b16211c
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# Creare o modificare un modulo personalizzato con il modulo precedente

È possibile creare o modificare un nuovo modulo personalizzato. Entrambe le attività sono spiegate in questo articolo.

Per informazioni sulla creazione di un nuovo modulo personalizzato da uno esistente, vedere [Copiare un modulo personalizzato per crearne uno nuovo con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

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

## Iniziare a creare un modulo personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   Nella visualizzazione visualizzata, puoi esaminare tutti i moduli personalizzati e i campi personalizzati creati per la tua organizzazione. È inoltre possibile vedere chi ha creato ciascun modulo e i campi ad esso associati.

1. Fai clic su **Nuovo modulo personalizzato.**
1. Selezionare almeno un tipo di oggetto da associare al modulo personalizzato, quindi fare clic su **Continua**.

   ![](assets/choose-object-type.jpg)

1. Sulla **Impostazioni modulo** scheda visualizzata, digitare un **Titolo modulo** e un **Descrizione** per il modulo personalizzato.

1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere associato a più oggetti, fare clic sul segno più dopo Tipi di oggetto, quindi selezionare il tipo di oggetto desiderato nel menu visualizzato.

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati. È inoltre possibile fare clic sulla X di un tipo di oggetto per eliminarlo dal modulo.

   Per informazioni sull’eliminazione dei tipi di oggetto da un modulo personalizzato già salvato, vedere [Eliminare i tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Fai clic su **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere il modulo aperto.

1. Se si desidera aggiungere un nuovo campo personalizzato al modulo, continuare su [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo o un widget personalizzato in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Per continuare a creare il modulo personalizzato in altri modi, procedere con uno dei seguenti articoli:

   * [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Iniziare a modificare un modulo personalizzato

È possibile modificare un modulo personalizzato in qualsiasi momento dopo averlo creato.

>[!CAUTION]
>
>Per informazioni sulla rimozione dei campi da un modulo personalizzato senza perdere i dati immessi dagli utenti in tali campi, vedere la sezione [Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) nell&#39;articolo [Eliminare un campo o un widget personalizzato dal sistema](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche apportate.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   Nella visualizzazione visualizzata, è possibile esaminare tutti i moduli personalizzati creati per la propria organizzazione. È inoltre possibile vedere chi ha creato ciascun modulo, con quale tipo di oggetto funziona e se è attivo.

1. Selezionare il modulo personalizzato da modificare, quindi fare clic su **Modifica**.
1. (Facoltativo) Per modificare il titolo e la descrizione del modulo personalizzato, fare clic sul pulsante **Impostazioni modulo** , quindi digita un **Titolo modulo** e **Descrizione**.

1. (Facoltativo) Per aggiungere altri tipi di oggetto al modulo in modo che possa essere collegato a più oggetti, fare clic sul segno più + dopo **Tipi di oggetti**, quindi seleziona il tipo desiderato nel menu visualizzato.

   ![](assets/add-object-type-existing-form.png)

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   È inoltre possibile fare clic sulla X di un tipo di oggetto per eliminarla dal modulo. Questa operazione deve essere eseguita con cautela quando si desidera eliminare un tipo di oggetto da un modulo personalizzato già salvato. Per ulteriori informazioni, consulta [Eliminare i tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Fai clic su **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere il modulo aperto.

1. Se si desidera aggiungere un nuovo campo personalizzato al modulo, continuare su [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo o un widget personalizzato in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Per continuare a creare il modulo personalizzato in altri modi, procedere con uno dei seguenti articoli:

   * [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
