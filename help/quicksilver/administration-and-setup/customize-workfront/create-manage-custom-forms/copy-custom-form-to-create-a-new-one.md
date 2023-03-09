---
user-type: administrator
product-area: system-administration
keywords: crea,personalizzato,modulo,copia,base,altro
navigation-topic: create-and-manage-custom-forms
title: Copiare un modulo personalizzato per crearne uno nuovo con il generatore legacy
description: È possibile creare un nuovo modulo personalizzato basato su un modulo esistente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Copiare un modulo personalizzato per crearne uno nuovo con il generatore legacy

È possibile creare un nuovo modulo personalizzato basato su un modulo esistente.

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
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Copiare un modulo personalizzato per crearne uno nuovo

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato.**
1. Seleziona il modulo personalizzato da utilizzare come base per un nuovo modulo personalizzato, quindi fai clic su **Copia**.
1. In **Copia modulo personalizzato** nella casella visualizzata, digitare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome modulo</td> 
      <td>Digitare un nome per il modulo copiato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Tipi di moduli </p> </td> 
      <td> <p>In <b>Tipo di modulo</b> selezionare i tipi di oggetto che si desidera utilizzare nel modulo personalizzato e fare clic sulla X accanto ai tipi che si desidera rimuovere. I tipi già associati al modulo sono disabilitati nell'elenco.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>Il modulo deve essere associato ad almeno un tipo di oggetto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Copia modulo**.

   Nel modulo originale, se i campi calcolati fanno riferimento a campi incompatibili con un tipo di oggetto aggiunto al nuovo modulo, verrà visualizzato un messaggio in cui viene richiesto di modificare i calcoli in tali campi.

   Analogamente, se un&#39;opzione di accesso per un&#39;interruzione di sezione nel modulo originale non è compatibile con un tipo di oggetto aggiunto al nuovo, verrà visualizzato un messaggio in cui viene richiesto di modificare l&#39;opzione.

1. Seleziona il modulo appena copiato, quindi fai clic su **Modifica**.
1. Apportare le modifiche desiderate al modulo, come illustrato nei seguenti articoli:

   * [Copiare un modulo personalizzato per crearne uno nuovo con il generatore di moduli legacy](#Add2)
   * [Aggiungere dati calcolati a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Facoltativo) Dopo aver fatto clic su **Salva+Chiudi**, allegare il modulo all&#39;oggetto in cui si desidera utilizzarlo, come descritto in [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
