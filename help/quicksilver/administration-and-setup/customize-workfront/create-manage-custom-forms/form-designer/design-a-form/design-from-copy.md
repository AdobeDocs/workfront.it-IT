---
title: Progettare un modulo da una copia
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato da una copia con il progettista del modulo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Progettare un modulo da una copia

È possibile progettare un nuovo modulo personalizzato basato su un modulo esistente. È possibile allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.

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

+++

## Copiare un modulo personalizzato per crearne uno nuovo

{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato.**
1. Seleziona il modulo personalizzato da utilizzare come base per un nuovo modulo personalizzato, quindi fai clic sull&#39;![icona Copia](assets/copy-icon.png).
1. Nella casella **Copia modulo personalizzata** visualizzata digitare le informazioni seguenti:

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
      <td> <p>Nella casella <b>Tipo modulo</b> selezionare i tipi di oggetto con cui si desidera utilizzare il modulo personalizzato e fare clic sulla X accanto ai tipi che si desidera rimuovere. I tipi già associati al modulo sono disabilitati nell'elenco.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Il modulo deve essere associato ad almeno un tipo di oggetto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Copia**.

   Nel modulo originale, se i campi calcolati fanno riferimento a campi incompatibili con un tipo di oggetto aggiunto al nuovo modulo, verrà visualizzato un messaggio in cui viene richiesto di modificare i calcoli in tali campi.

   Analogamente, se un&#39;opzione di accesso per un&#39;interruzione di sezione nel modulo originale non è compatibile con un tipo di oggetto aggiunto al nuovo, verrà visualizzato un messaggio in cui viene richiesto di modificare l&#39;opzione.

1. Seleziona il modulo appena copiato, quindi fai clic sull&#39;![icona Modifica](assets/edit-icon.png).
1. Apportare le modifiche al modulo, come descritto nelle sezioni seguenti dell&#39;articolo [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md):

   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Aggiungi campi di testo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Aggiungere campi calcolati](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Aggiungi pulsanti di scelta, gruppo di caselle di controllo e elenchi a discesa](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Aggiungere campi di tipo typeahead e date](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Aggiungere immagini, PDF e video](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Aggiungere file Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Facoltativo) Dopo aver fatto clic su **Salva+Chiudi**, allegare il modulo all&#39;oggetto in cui si desidera utilizzarlo, come descritto in [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
