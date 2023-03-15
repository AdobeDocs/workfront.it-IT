---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configurare la condivisione di campi e widget personalizzati con il generatore di moduli legacy
description: Per impostazione predefinita, quando si aggiunge un nuovo campo o widget personalizzato a un modulo personalizzato, chiunque nel sistema abbia accesso a moduli personalizzati può modificare le proprietà dell’elemento, ad esempio l’etichetta e il nome. Puoi modificare questa impostazione controllando con chi può essere condivisa.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---

# Configurare la condivisione di campi e widget personalizzati con il generatore di moduli legacy

Per impostazione predefinita, quando si aggiunge un nuovo campo o widget personalizzato a un modulo personalizzato, chiunque nel sistema abbia accesso a moduli personalizzati può modificare le proprietà dell’elemento, ad esempio l’etichetta e il nome. Puoi modificare questa impostazione controllando con chi può essere condivisa.

Per informazioni sui campi e i widget personalizzati nei moduli personalizzati, consultare [Aggiunta di un campo personalizzato a un modulo personalizzato con il modulo precedente](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiunta o modifica di un widget di risorse in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configurare la condivisione per un campo o un widget personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Se configuri la condivisione per un campo o widget personalizzato nell’istanza Workfront della tua organizzazione, procedi come segue:

   1. Fai clic sul pulsante **Campi** scheda .
   1. Seleziona l&#39;elemento per il quale vuoi configurare la condivisione, quindi fai clic su **Condividi**.

   Oppure, se stai configurando la condivisione per un campo o widget personalizzato esistente in un modulo personalizzato, procedi come segue:

   1. Seleziona il modulo personalizzato, quindi fai clic su **Modifica**.
   1. Nell’area di modifica del modulo a destra, selezionare l’elemento per il quale si desidera configurare la condivisione.
   1. Nel pannello a sinistra, fai clic su **Campo di condivisione**.


1. In **Accesso a campi personalizzati** casella visualizzata, specifica con chi condividere l’elemento e come desideri condividerlo:

   1. Vicino all&#39;angolo inferiore sinistro del **Accesso a campi personalizzati** box, sotto **Consenti accesso al campo personalizzato a**, inizia a digitare il nome di un utente, team, ruolo di lavoro, gruppo o società con cui desideri condividere l’elemento, quindi fai clic sul nome quando viene visualizzato.

      ![](assets/share-field-give-access-to.jpg)

   1. Per informazioni più specifiche sulla modalità di condivisione dell’elemento, fai clic sull’elenco a discesa a destra del nome, quindi utilizza una delle opzioni seguenti:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Visualizzare</td> 
         <td> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire all’utente o agli utenti di utilizzare il proprio accesso per aggiungere l’elemento a un modulo personalizzato o condividerlo con altri utenti.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Gestire</td> 
         <td> <p>Consente di accedere al campo personalizzato e di visualizzarlo nella Libreria campi e nella pagina in cui si creano moduli personalizzati.</p> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera che l'utente o gli utenti possano utilizzare il proprio accesso per eliminare l'elemento dal sistema o condividerlo con altri utenti.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri nomi all’elenco e configurare le relative opzioni.
1. (Facoltativo) Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) nell’angolo in alto a destra se desideri scegliere un’opzione di condivisione a livello di sistema per il campo.

   In questo menu a discesa non vengono visualizzate contemporaneamente tutte le opzioni seguenti. Ad esempio, il secondo viene visualizzato solo quando sono selezionati gli altri due.

   * **Rendi questo sistema modificabile a livello di sistema in modo che tutti possano modificarlo in Workfront** (opzione predefinita)

      Quando si aggiunge un campo o un widget personalizzato senza limitare la condivisione, tutti gli utenti del sistema che hanno accesso ai moduli personalizzati possono visualizzarlo e modificarne le proprietà.

   * **Rimuovi l&#39;accesso alle modifiche a livello di sistema**

      Limita l’accesso solo a coloro che hai aggiunto all’elenco.

   * **Rendi visibile a livello di sistema, per tutti gli utenti di Workfront**

1. Fai clic su **Salva** o **Salva e chiudi**.

## Accesso ereditato a campi e widget personalizzati quando viene condiviso un modulo personalizzato

Quando un utente condivide un modulo personalizzato con un gruppo, un ruolo, un team o un’azienda, i destinatari ereditano l’accesso Visualizza a tutti i campi e widget personalizzati presenti nel modulo. Questo livello di accesso agli elementi del modulo viene sempre mantenuto in modo che il modulo possa funzionare per i destinatari come previsto dalla persona che lo ha creato. Questo vale anche per i destinatari che hanno accesso a Modifica al modulo.

È possibile individuare gli utenti che hanno ereditato l’accesso a un campo o a un widget personalizzato e rimuovere l’accesso a tale campo.

>[!NOTE]
>
>Se un destinatario dispone dell&#39;accesso Gestione a un campo o widget personalizzato nel modulo personalizzato condiviso, tale accesso viene mantenuto per il destinatario.

* [Informazioni su chi ha ereditato l’accesso a un campo o a un widget personalizzato](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Rimuovere l’accesso a un campo o a un widget personalizzato in un modulo personalizzato condiviso](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Informazioni su chi ha ereditato l’accesso a un campo o a un widget personalizzato {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Fai clic sul pulsante **Campi** , quindi seleziona il campo, l’immagine o il widget di accesso.
1. Nella casella visualizzata, fai clic su **Autorizzazioni ereditate** e visualizzare i nomi visualizzati.
1. Fai clic su **Annulla**.

### Rimuovere l’accesso a un campo o a un widget personalizzato in un modulo personalizzato condiviso {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se è necessario rimuovere l’accesso a un campo o a un widget personalizzato in un modulo personalizzato condiviso, è necessario annullare la condivisione del modulo. Per istruzioni, consulta la sezione . [Rimuovere l’accesso a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) nell&#39;articolo [Condivisione di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
