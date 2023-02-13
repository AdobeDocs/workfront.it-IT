---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Eliminare un campo o un widget personalizzato dal sistema
description: Per migliorare le prestazioni del sistema e semplificare l’utilizzo dei moduli da parte degli utenti, è possibile rimuovere campi e widget personalizzati dal sistema quando non vengono più utilizzati.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Eliminare un campo o un widget personalizzato dal sistema

Per migliorare le prestazioni del sistema e semplificare l’utilizzo dei moduli da parte degli utenti, è possibile rimuovere campi e widget personalizzati dal sistema quando non vengono più utilizzati.

>[!CAUTION]
>
>L’eliminazione di un campo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati immessi dagli utenti nel campo durante la compilazione di moduli personalizzati associati agli oggetti. Impossibile recuperare i dati eliminati.
>
>È possibile visualizzare tutti i moduli e i rapporti personalizzati che utilizzano un campo personalizzato da eliminare per valutare le eventuali ripercussioni. Per ulteriori informazioni, consulta [Visualizza tutti i moduli personalizzati che utilizzano un campo o un widget personalizzato specifico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) e [Visualizzare tutti i rapporti che utilizzano un campo personalizzato o un widget particolare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Oppure, per una soluzione alternativa che puoi utilizzare per evitare di perdere dati nei campi non più utilizzati, vedi [Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti](#remove-a-custom-field-without-losing-data-that-users-have-entered) in questo articolo.

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

## Eliminare un campo o un widget personalizzato dal sistema

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato.**
1. Fai clic sul pulsante **Campi** scheda .
1. Seleziona il campo o il widget personalizzato, quindi fai clic su **Elimina**.
1. Se si desidera eliminare definitivamente l&#39;elemento e, nel caso di un campo personalizzato, tutti i dati associati agli oggetti in cui è stato allegato, fare clic su **Sì, Elimina**.

## Rimuovere un campo personalizzato senza perdere i dati immessi dagli utenti {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>La rimozione di un campo personalizzato da un modulo personalizzato contenente più di 500 campi e widget non può essere annullata. Se si rimuove il campo, non è possibile aggiungerlo nuovamente finché il modulo non dispone di meno di 500 campi e widget.

1. Determinare i campi personalizzati che si desidera rimuovere dal modulo personalizzato originale, ma non rimuoverli a questo punto.
1. Crea un nuovo modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. Aggiungere i campi personalizzati al nuovo modulo che si desidera rimuovere dal modulo personalizzato originale, come descritto in [Riutilizzare un campo o un widget personalizzato in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. Salvare il nuovo modulo personalizzato.

1. Limita l’accesso al modulo personalizzato solo agli utenti con accesso amministrativo, come descritto in [Condivisione di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Applicare il nuovo modulo personalizzato agli oggetti in cui è già applicato il modulo personalizzato originale, come descritto in [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   L’applicazione del nuovo modulo personalizzato a questi oggetti assicura che i dati storici dei rapporti non vengano interessati.

1. Modificare il modulo personalizzato originale e rimuovere i campi personalizzati aggiunti al nuovo modulo (nel passaggio 2).

   I campi rimossi dal modulo personalizzato originale sono ora disponibili solo nel nuovo modulo personalizzato creato. Gli utenti possono visualizzare il modulo personalizzato sull’oggetto, ma gli utenti senza accesso amministrativo non possono modificare il modulo personalizzato.
