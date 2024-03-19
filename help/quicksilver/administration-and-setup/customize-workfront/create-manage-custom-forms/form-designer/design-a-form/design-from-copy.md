---
title: Progettare un modulo da una copia con il progettista del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato da una copia con il progettista del modulo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Progettare un modulo da una copia con il progettista del modulo

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti oppure nell’ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

È possibile progettare un nuovo modulo personalizzato basato su un modulo esistente. È possibile allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.

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

## Copiare un modulo personalizzato per crearne uno nuovo

{{step-1-to-setup}}

1. Clic **Forms personalizzato.**
1. Seleziona il modulo personalizzato da utilizzare come base per un nuovo modulo personalizzato, quindi fai clic su **Copia** <span class="preview">o ![Icona Copia](assets/copy-icon.png).</span>
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

1. Seleziona il modulo appena copiato, quindi fai clic su **Modifica** <span class="preview">o ![Icona Modifica](assets/edit-icon.png).</span>
1. Apportare le modifiche desiderate al modulo, come descritto nelle sezioni seguenti della [Progettare un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) articolo:

   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Aggiungi campi di testo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Aggiungere campi calcolati](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Aggiungi pulsanti di scelta, gruppo di caselle di controllo e elenchi a discesa](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Aggiungere campi di tipo typeahead e date](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Aggiungere immagini, PDF e video](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Aggiungere file Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Facoltativo) Dopo aver fatto clic su **Salva+Chiudi**, allegare il modulo all&#39;oggetto in cui si desidera utilizzarlo, come descritto in [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
