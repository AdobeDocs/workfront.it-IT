---
title: Creare un modulo da una copia
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile creare un modulo personalizzato da una copia con il progettista del modulo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
TQID: https://experienceleague.adobe.com/WaLGsLpGDMXGvNd7W-8JzmgJYiCaxSd-gaMoGy6j-Zc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 3e77f50ee2297a9c552e27bfcdf7f08a6a4c89b5
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 24%

---

# Creare un modulo da una copia

È possibile progettare un nuovo modulo personalizzato basato su un modulo esistente. Puoi allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr>  
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Apportare le modifiche al modulo, come descritto nelle sezioni seguenti dell&#39;articolo [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md):

   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Aggiungere campi di testo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Aggiungere campi calcolati](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Aggiungi pulsanti di scelta, gruppi di caselle di controllo e elenchi a discesa](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Aggiungi campi data](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-date-fields)
   * [Aggiungere immagini, PDF e video](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Aggiungere file Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [Aggiungere campi per pianificare una connessione](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. (Facoltativo) Dopo aver fatto clic su **Salva e chiudi**, allegare il modulo all&#39;oggetto in cui si desidera utilizzarlo, come descritto in [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
