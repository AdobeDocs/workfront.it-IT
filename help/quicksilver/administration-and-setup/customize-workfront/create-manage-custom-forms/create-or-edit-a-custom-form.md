---
title: Creare o modificare un modulo personalizzato con il generatore di moduli legacy
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puoi creare o modificare un nuovo modulo personalizzato.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Creare o modificare un modulo personalizzato con il generatore di moduli legacy

<!--Audited: 01/2024-->

{{form-designer-default}}

È possibile creare un nuovo modulo personalizzato o modificare un modulo esistente. Entrambe le attività sono illustrate in questo articolo.

Per informazioni sulla creazione di un nuovo modulo personalizzato da uno esistente, vedere [Copiare un modulo personalizzato per crearne uno nuovo con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

Questo articolo descrive come creare un modulo personalizzato utilizzando il Generatore di moduli legacy. Per informazioni sulla creazione di un modulo personalizzato tramite Progettazione moduli, vedere [Progettare un modulo con Progettazione moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td><p>Nuovo: Standard</p>
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

+++

## Inizia a creare un modulo personalizzato

{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   I moduli personalizzati vengono visualizzati in un elenco. Puoi rivedere tutti i moduli personalizzati e i campi personalizzati creati per la tua organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, gli oggetti associati e se è attivo.

1. Fare clic su **Nuovo modulo personalizzato.**
1. Selezionare almeno un tipo di oggetto da associare al modulo personalizzato, quindi fare clic su **Continua**.

   ![](assets/choose-object-type.jpg)

1. Nella scheda **Impostazioni modulo** visualizzata, digitare un **Titolo modulo** e una **Descrizione** facoltativa per il modulo personalizzato.

1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sul segno **più** dopo **Tipi di oggetto**, quindi selezionare il tipo di oggetto desiderato nel menu visualizzato.

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

1. (Facoltativo) Fai clic su **X** in un tipo di oggetto per eliminarlo dal modulo.

   Per informazioni sull&#39;eliminazione di tipi di oggetto da un modulo personalizzato già salvato, vedere [Eliminare tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Fai clic su **Fine** nell&#39;angolo inferiore sinistro della schermata.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

1. Se desideri aggiungere un nuovo campo personalizzato al modulo, continua con [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un&#39;interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Inizia a modificare un modulo personalizzato

È possibile modificare un modulo personalizzato in qualsiasi momento dopo la sua creazione.

>[!CAUTION]
>
>Per informazioni sulla rimozione di campi da un modulo personalizzato senza perdere i dati immessi dagli utenti in tali campi, vedere la sezione [Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) nell&#39;articolo [Eliminare un campo personalizzato o un widget dal sistema](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche.

{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   I moduli personalizzati vengono visualizzati in un elenco. Puoi rivedere tutti i moduli personalizzati e i campi personalizzati creati per la tua organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, gli oggetti associati e se è attivo.

1. Seleziona il modulo personalizzato da modificare, quindi fai clic sull&#39;![icona Modifica](assets/edit-icon.png).
1. (Facoltativo) Per modificare il titolo e la descrizione del modulo personalizzato, fare clic sulla scheda **Impostazioni modulo**, quindi digitare **Titolo modulo** e **Descrizione**.

1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sul segno più + dopo **Tipi di oggetto**, quindi selezionare il tipo desiderato nel menu visualizzato.

   ![](assets/add-object-type-existing-form.png)

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   È inoltre possibile fare clic sulla X su un tipo di oggetto per eliminarlo dal modulo. Questa operazione deve essere eseguita con cautela quando si desidera eliminare un tipo di oggetto da un modulo personalizzato già salvato. Per ulteriori informazioni, vedere [Eliminare i tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Fai clic su **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

1. Se desideri aggiungere un nuovo campo personalizzato al modulo, continua con [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un&#39;interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
