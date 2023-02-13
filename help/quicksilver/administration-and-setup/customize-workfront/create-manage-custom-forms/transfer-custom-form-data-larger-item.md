---
title: Trasferimento di dati modulo personalizzati durante la conversione di un oggetto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando il lavoro definito in un elemento di lavoro diventa troppo grande, è possibile convertirlo in un elemento di lavoro più grande.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Trasferimento di dati modulo personalizzati durante la conversione di un oggetto

A seconda delle esigenze aziendali dell’organizzazione, il lavoro definito in un’attività o in un problema potrebbe diventare troppo grande per gestirlo all’interno dell’attività o del problema. In questo caso, è possibile convertirli in un elemento di lavoro più grande:

* È possibile convertire i problemi in attività o progetti
* È possibile convertire le attività in progetti

Per trasferire i dati del modulo personalizzato da un problema a un&#39;attività o a un progetto, è necessario completare le due attività di questo articolo, nell&#39;ordine indicato di seguito.

Per ulteriori informazioni, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) o [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Primo: Copia il modulo personalizzato {#first-copy-the-custom-form}

Prima di tutto è necessario assicurarsi di conservare i dati del modulo personalizzato relativi a un&#39;attività o a un problema che si desidera convertire. Poiché i dati del modulo personalizzato devono corrispondere esattamente all’elemento convertito, è consigliabile duplicare il modulo in modo da poterlo allegare al nuovo oggetto.

>[!TIP]
>
>Un altro modo per conservare i dati del modulo personalizzato in questa situazione consiste nell’aggiungere al modulo personalizzato il tipo di oggetto più grande. Per istruzioni, consulta la sezione . [Iniziare a modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) nell&#39;articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato**.
1. Selezionare il modulo personalizzato di tipo task o problema, quindi fare clic su **Copia**.
1. In **Modulo personalizzato** specificare un nome per il nuovo modulo.

1. Da **Tipo di modulo** dal menu a discesa, selezionare il tipo di oggetto per il quale si desidera creare il nuovo modulo personalizzato

   **Esempio:** Se si desidera trasferire i dati del modulo personalizzato a un progetto, selezionare Progetto.

1. Fai clic su **Copia modulo**.

   Questo modulo personalizzato copiato può ora essere associato a un&#39;attività o a un progetto.

1. Continua su [Secondo: Convertire il problema o l’attività e trasferire i dati del modulo personalizzato](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Secondo: Convertire il problema o l’attività e trasferire i dati del modulo personalizzato {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Copiare il modulo personalizzato sul problema o sull&#39;attività da convertire, come spiegato nella sezione [Primo: Copia il modulo personalizzato](#first-copy-the-custom-form) in questo articolo.
1. Converti il problema o l&#39;attività utilizzando **Forms personalizzato** nella casella visualizzata per selezionare il modulo personalizzato copiato. Per istruzioni, vedi i seguenti articoli:

   * [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Convertire un problema in un’attività in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convertire un&#39;attività in un progetto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. In **Converti in (tipo di oggetto)** finestra di dialogo visualizzata, fai clic sul pulsante **Aggiungi Forms** menu a discesa e selezionare il modulo copiato nella sezione precedente.

   Le informazioni acquisite nei campi personalizzati del problema vengono ora trasferite al modulo personalizzato sull&#39;attività.

