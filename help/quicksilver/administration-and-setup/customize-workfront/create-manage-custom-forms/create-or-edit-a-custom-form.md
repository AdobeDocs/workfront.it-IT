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
source-git-commit: 8af1890b2e2ae613279b5191cf8f2190364fb524
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Creare o modificare un modulo personalizzato con il generatore di moduli legacy

<!--Audited: 01/2024-->

Puoi creare o modificare un nuovo modulo personalizzato. Entrambe le attività sono illustrate in questo articolo.

Per informazioni sulla creazione di un nuovo modulo personalizzato da un modulo esistente, vedi [Copiare un modulo personalizzato per crearne uno nuovo con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

Questo articolo descrive come creare un modulo personalizzato utilizzando il Generatore di moduli legacy. Per informazioni sulla creazione di un modulo personalizzato tramite Progettazione moduli, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>Nuovo: Standard</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni sui requisiti di accesso, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Inizia a creare un modulo personalizzato

{{step-1-to-setup}}

1. Clic **Forms personalizzato** nel pannello a sinistra.

   I moduli personalizzati vengono visualizzati in un elenco. Puoi rivedere tutti i moduli personalizzati e i campi personalizzati creati per la tua organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, gli oggetti associati e se è attivo.

1. Clic **Nuovo modulo personalizzato.**
1. Seleziona almeno un tipo di oggetto da associare al modulo personalizzato, quindi fai clic su **Continua**.

   ![](assets/choose-object-type.jpg)

1. Il giorno **Impostazioni modulo** scheda visualizzata, digita un **Titolo modulo** e un&#39;opzione **Descrizione** per il modulo personalizzato.

1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sul pulsante **più** firma dopo **Tipi di oggetto**, quindi selezionare il tipo di oggetto desiderato nel menu visualizzato.

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

1. (Facoltativo) Fai clic su **X** su un tipo di oggetto per eliminarlo dal modulo.

   Per informazioni sull&#39;eliminazione dei tipi di oggetto da un modulo personalizzato già salvato, vedere [Eliminare tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Clic **Fine** nell&#39;angolo inferiore sinistro dello schermo.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

1. Se si desidera aggiungere un nuovo campo personalizzato al modulo, continuare con l&#39;operazione [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Inizia a modificare un modulo personalizzato

È possibile modificare un modulo personalizzato in qualsiasi momento dopo la sua creazione.

>[!CAUTION]
>
>Per informazioni sulla rimozione di campi da un modulo personalizzato senza perdere i dati immessi dagli utenti in tali campi, vedere la sezione [Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) nell’articolo [Eliminare un campo personalizzato o un widget dal sistema](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>In generale, si consiglia di ridurre al minimo il numero di volte in cui si modifica un modulo personalizzato già in uso. Non esiste un sistema di notifica per avvisare gli utenti che utilizzano il modulo personalizzato delle modifiche.

{{step-1-to-setup}}

1. Clic **Forms personalizzato** nel pannello a sinistra.

   I moduli personalizzati vengono visualizzati in un elenco. Puoi rivedere tutti i moduli personalizzati e i campi personalizzati creati per la tua organizzazione. È inoltre possibile vedere chi ha creato ogni modulo, gli oggetti associati e se è attivo.

1. Seleziona il modulo personalizzato da modificare, quindi fai clic su **Modifica**.
1. (Facoltativo) Per modificare il titolo e la descrizione del modulo personalizzato, fai clic sul pulsante **Impostazioni modulo** , quindi digita un **Titolo modulo** e **Descrizione**.

1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sul segno più + dopo **Tipi di oggetto**, quindi seleziona il tipo desiderato nel menu visualizzato.

   ![](assets/add-object-type-existing-form.png)

   È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   È inoltre possibile fare clic sulla X su un tipo di oggetto per eliminarlo dal modulo. Questa operazione deve essere eseguita con cautela quando si desidera eliminare un tipo di oggetto da un modulo personalizzato già salvato. Per ulteriori informazioni, consulta [Eliminare tipi di oggetto in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Clic **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

1. Se si desidera aggiungere un nuovo campo personalizzato al modulo, continuare con l&#39;operazione [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) o [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oppure

   Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
