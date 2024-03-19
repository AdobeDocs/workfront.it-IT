---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configurare la condivisione per campi personalizzati e widget con il generatore di moduli legacy
description: Per impostazione predefinita, quando si aggiunge un nuovo campo personalizzato o widget a un modulo personalizzato, chiunque nel sistema con accesso ai moduli personalizzati può modificare le proprietà di tale elemento, ad esempio l’etichetta e il nome. Puoi cambiare questa impostazione controllando con chi può essere condiviso.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Configurare la condivisione per campi personalizzati e widget con il generatore di moduli legacy

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti oppure nell’ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Per impostazione predefinita, quando si aggiunge un nuovo campo personalizzato o widget a un modulo personalizzato, chiunque nel sistema con accesso ai moduli personalizzati può modificare le proprietà di tale elemento, ad esempio l’etichetta e il nome. Puoi cambiare questa impostazione controllando con chi può essere condiviso.

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedi [Aggiungere un campo personalizzato a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configurare la condivisione per un campo personalizzato o un widget

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Se stai configurando la condivisione per un campo personalizzato o un widget nell’istanza Workfront della tua organizzazione, effettua le seguenti operazioni:

   1. Clic **Campi** per aprire l&#39;area Campi.
   1. Selezionare l&#39;elemento per il quale si desidera configurare la condivisione, quindi fare clic su **Condividi** <span class="preview">o ![Icona Condividi](assets/share-icon.png).</span>

   Oppure, se stai configurando la condivisione per un campo personalizzato o un widget in un modulo personalizzato esistente, effettua le seguenti operazioni:

   1. Seleziona il modulo personalizzato, quindi fai clic su **Modifica** <span class="preview">o ![Icona Modifica](assets/edit-icon.png).</span>
   1. Nell&#39;area di modifica dei moduli a destra, selezionare l&#39;elemento per il quale si desidera configurare la condivisione.
   1. Nel pannello a sinistra, fai clic su **Condividi campo**.

1. In **Accesso al campo personalizzato** nella casella visualizzata, specificare l&#39;utente con cui si desidera condividere l&#39;elemento e la modalità di condivisione:

   1. Vicino all&#39;angolo inferiore sinistro del **Accesso al campo personalizzato** casella, sotto **Assegna accesso al campo personalizzato a**, iniziare a digitare il nome di un utente, team, mansione, gruppo o società con cui si desidera condividere l&#39;elemento, quindi fare clic sul nome quando viene visualizzato.

      ![](assets/share-field-give-access-to.jpg)

   1. Per informazioni più specifiche sulla modalità di condivisione dell&#39;elemento, fare clic sull&#39;elenco a discesa a destra del nome, quindi utilizzare una delle opzioni seguenti:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Visualizzare</td> 
         <td> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> specificare se si desidera che l'utente o gli utenti possano utilizzare il proprio accesso per aggiungere l'elemento a un modulo personalizzato o condividerlo con altri utenti.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Gestire</td> 
         <td> <p>Consente di modificare il campo personalizzato e di visualizzarlo nella Libreria campi e nella pagina in cui si creano i moduli personalizzati.</p> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> specificare se si desidera che l'utente o gli utenti possano utilizzare il proprio accesso per eliminare l'elemento dal sistema o condividerlo con altri utenti.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) nell’angolo in alto a destra per scegliere un’opzione di condivisione a livello di sistema per il campo.

   Non tutte le seguenti opzioni vengono visualizzate contemporaneamente in questo menu a discesa. Ad esempio, il secondo viene visualizzato solo quando si seleziona uno degli altri due.

   * **Rendi modificabile a livello di sistema in modo che tutti in Workfront possano modificarlo** (opzione predefinita)

     Quando si aggiunge un campo personalizzato o un widget e non si limita la condivisione, tutti gli utenti del sistema che hanno accesso ai moduli personalizzati possono visualizzarlo e modificarne le proprietà.

   * **Rimuovi l&#39;accesso alle modifiche a livello di sistema**

     Limita l’accesso solo a coloro che hai aggiunto all’elenco.

   * **Rendi visibile a livello di sistema in modo che tutti in Workfront possano visualizzarlo**

1. Clic **Salva** o **Salva e chiudi**.

## Accesso ereditato a campi e widget personalizzati quando viene condiviso un modulo personalizzato

Quando qualcuno condivide un modulo personalizzato con un gruppo, una mansione, un team o una società, i destinatari ereditano l’accesso in visualizzazione a tutti i campi personalizzati e i widget presenti nel modulo. Questo livello di accesso agli elementi nel modulo viene sempre mantenuto, in modo che il modulo possa funzionare per i destinatari come previsto dalla persona che lo ha creato. Ciò vale anche per i destinatari che dispongono dell’accesso di modifica al modulo.

Puoi scoprire chi ha ereditato l’accesso a un campo personalizzato o a un widget e rimuoverne l’accesso.

>[!NOTE]
>
>Se un destinatario dispone dell’accesso in gestione a un campo personalizzato o a un widget nel modulo personalizzato condiviso, tale accesso viene mantenuto per il destinatario.

* [Scopri chi ha ereditato l’accesso a un campo o a un widget personalizzato](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Rimuovere l&#39;accesso a un campo personalizzato o a un widget in un modulo personalizzato condiviso](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Scopri chi ha ereditato l’accesso a un campo o a un widget personalizzato {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Fai clic su **Campi** , quindi selezionare il campo, l&#39;immagine o il widget di accesso.
1. Nella casella visualizzata, fai clic su **Autorizzazioni ereditate** e visualizzare i nomi visualizzati.
1. Clic **Annulla**.

### Rimuovere l&#39;accesso a un campo personalizzato o a un widget in un modulo personalizzato condiviso {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se devi rimuovere l’accesso a un campo personalizzato o a un widget in un modulo personalizzato condiviso, devi annullare la condivisione del modulo. Per le istruzioni del caso, vedere nella sezione [Rimuovere l’accesso a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) nell’articolo [Condividere un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
