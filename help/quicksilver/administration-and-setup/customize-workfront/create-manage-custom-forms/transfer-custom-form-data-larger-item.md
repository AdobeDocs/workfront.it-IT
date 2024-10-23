---
title: Trasferisci dati modulo personalizzato durante la conversione di un oggetto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando il lavoro definito in un elemento di lavoro diventa troppo grande, è possibile convertirlo in un elemento di lavoro più grande.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Trasferimento dei dati del modulo personalizzato durante la conversione di un oggetto

A seconda delle esigenze aziendali dell’organizzazione, il lavoro definito in un’attività o in un problema potrebbe diventare troppo grande da gestire all’interno dell’attività o del problema. In questo caso, è possibile convertirli in un elemento di lavoro più grande:

* È possibile convertire i problemi in attività o in progetti
* È possibile convertire le attività in progetti

Per trasferire i dati del modulo personalizzato da un problema a un’attività o a un progetto, è necessario completare le due attività di questo articolo, nell’ordine seguente.

Per ulteriori informazioni, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) o [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Primo: aggiungere altri oggetti al modulo personalizzato

{{step-1-to-setup}}

1. Fare clic su **Forms personalizzato**.
1. Trova il modulo necessario, quindi fai clic sull&#39;icona ![Modifica](assets/edit-icon.png).
1. Nella parte superiore del modulo, aggiungi l’oggetto in cui intendi convertire l’attività o il problema.

   >[!INFO]
   >
   >**Esempio**: se si desidera trasferire i dati del modulo personalizzato in un progetto, selezionare Progetto.

1. Fai clic su **Applica** nella parte inferiore del modulo.

1. Continua su [Secondo: converti il problema o l&#39;attività e trasferisci i dati del modulo personalizzato](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Secondo: convertire il problema o l’attività e trasferire i dati del modulo personalizzato {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Aggiungere altri oggetti al modulo personalizzato per il problema o l&#39;attività da convertire, come illustrato nella sezione [Primo: aggiungere altri oggetti al modulo personalizzato](#first-add-additonal-objects-to-the-custom-form) in questo articolo.
1. Convertire il problema o l&#39;attività utilizzando l&#39;opzione **Forms** personalizzato nella casella visualizzata per selezionare il modulo personalizzato necessario. Per istruzioni, vedere i seguenti articoli:

   * [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Convertire un problema in un’attività in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convertire un’attività in un progetto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Nella finestra di dialogo **Converti in (tipo di oggetto)** visualizzata, fare clic sul menu a discesa **Aggiungi Forms** e selezionare il modulo copiato nella sezione precedente.

   Le informazioni acquisite nei campi personalizzati del problema ora vengono trasferite al modulo personalizzato per l’attività.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->