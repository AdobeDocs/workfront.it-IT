---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminare un campo personalizzato o un widget dal sistema
description: Per migliorare le prestazioni del sistema e semplificare l'utilizzo dei moduli da parte degli utenti, è possibile rimuovere campi e widget personalizzati dal sistema quando non sono più utilizzati.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Eliminare un campo personalizzato o un widget dal sistema

Per migliorare le prestazioni del sistema e semplificare l&#39;utilizzo dei moduli da parte degli utenti, è possibile rimuovere campi e widget personalizzati dal sistema quando non sono più utilizzati.

>[!CAUTION]
>
>L’eliminazione di un campo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati immessi dagli utenti nel campo durante la compilazione dei moduli personalizzati allegati agli oggetti. I dati eliminati non possono essere recuperati.
>
>È possibile visualizzare tutte le maschere e i report personalizzati che utilizzano un campo personalizzato che si desidera eliminare per valutare le possibili ripercussioni. Per ulteriori informazioni, consulta [Visualizzare tutti i moduli personalizzati che utilizzano un campo personalizzato o un widget particolare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) e [Visualizzare tutti i rapporti che utilizzano un particolare campo personalizzato o widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>In alternativa, per una soluzione alternativa che puoi utilizzare per evitare la perdita di dati in campi non più utilizzati, consulta [Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti](#remove-a-custom-field-without-losing-data-that-users-have-entered) in questo articolo.

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

## Eliminare un campo personalizzato o un widget dal sistema

{{step-1-to-setup}}

1. Clic **Forms personalizzato.**
1. Clic **Campi** per aprire l&#39;area Campi.
1. Seleziona il campo o il widget personalizzato, quindi fai clic su **Elimina**.
1. Se si è certi di voler eliminare definitivamente l&#39;elemento e (nel caso di un campo personalizzato) tutti i dati associati sugli oggetti a cui è stato associato, fare clic su **Sì, elimina**.

## Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Non è possibile annullare la rimozione di un campo personalizzato da un modulo personalizzato contenente più di 500 campi e widget. Se si rimuove il campo, non sarà possibile aggiungerlo nuovamente finché il modulo non avrà meno di 500 campi e widget.

1. Determinare quali campi personalizzati si desidera rimuovere dal modulo personalizzato originale, ma non rimuoverli a questo punto.
1. Crea un nuovo modulo personalizzato:

   1. Aggiungere i campi personalizzati al nuovo modulo che si desidera rimuovere dal modulo personalizzato originale.

      * Se utilizzi il generatore di moduli personalizzati, consulta [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Se si utilizza il progettista del modulo, vedere [Aggiungere campi nuovi o esistenti al modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. Salva il nuovo modulo personalizzato.

1. Limitare l&#39;accesso al modulo personalizzato solo agli utenti con accesso amministrativo, come descritto in [Condividere un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Applicare il nuovo modulo personalizzato agli oggetti in cui è già applicato il modulo personalizzato originale, come descritto in [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   L’applicazione del nuovo modulo personalizzato a questi oggetti garantisce che i dati storici di reporting non siano interessati.

1. Modificare il modulo personalizzato originale e rimuovere i campi personalizzati aggiunti al nuovo modulo (nel passaggio 2).

   I campi rimossi dal modulo personalizzato originale ora sono disponibili solo nel nuovo modulo personalizzato creato. Gli utenti possono visualizzare il modulo personalizzato sull’oggetto, ma gli utenti senza accesso amministrativo non possono modificarlo.
