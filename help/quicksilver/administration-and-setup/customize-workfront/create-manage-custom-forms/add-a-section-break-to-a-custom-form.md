---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Aggiungere un’interruzione di sezione a un modulo personalizzato con il generatore di moduli legacy
description: È possibile raggruppare i campi personalizzati e i widget in un modulo personalizzato in sezioni con intestazioni. Ciò è utile per presentare un’esperienza organizzata agli utenti che compileranno il modulo. Inoltre, se devi limitare l’accesso a determinati campi personalizzati e widget a determinati utenti, puoi inserirli in una sezione e quindi concedere l’accesso alla sezione solo a tali utenti.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 28961cda48ce4eec84ed272e660be6ba938be370
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Aggiungere un’interruzione di sezione a un modulo personalizzato con il generatore di moduli legacy

È possibile raggruppare i campi personalizzati e i widget in un modulo personalizzato in sezioni con intestazioni. Ciò è utile per presentare un’esperienza organizzata agli utenti che compileranno il modulo. Inoltre, se devi limitare l’accesso a determinati campi personalizzati e widget a determinati utenti, puoi inserirli in una sezione e quindi concedere l’accesso alla sezione solo a tali utenti.

Ad esempio, se devi tenere traccia delle informazioni riservate che solo gli amministratori di sistema possono visualizzare o modificare, puoi creare un’interruzione di sezione con le autorizzazioni Solo amministratore e inserire i campi sensibili in tale sezione.

Le impostazioni di accesso selezionate per una sezione sono direttamente correlate alle autorizzazioni di cui dispongono gli utenti sull’oggetto Workfront a cui è allegato il modulo personalizzato. È possibile nascondere o visualizzare una sezione a seconda che l&#39;utente disponga dell&#39;accesso per visualizzare, contribuire o gestire l&#39;oggetto. In alternativa, è possibile impostare una sezione su Solo amministratore in modo che solo gli utenti con un livello di accesso amministratore di sistema possano accedervi.

Per informazioni sulle autorizzazioni per gli oggetti, vedi [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per informazioni sui campi personalizzati e i widget nei moduli personalizzati, vedi [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

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
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p></td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare e configurare l’accesso per una sezione in un modulo personalizzato

1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Aggiungere al modulo campi e widget personalizzati, come descritto in [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Durante la creazione o la modifica del modulo personalizzato, sul **Aggiungi un campo** , fare clic su **Interruzione di sezione**.

   ![](assets/click-section-break.jpg)

1. Il giorno **Impostazioni campo** , configura le opzioni desiderate per la sezione:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra la sezione. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita del testo per spiegare agli utenti a cosa serve la sezione. Questo viene visualizzato sotto l’etichetta della sezione nel modulo personalizzato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Aggiungi logica</p></td> 
      <td><p>Utilizza la logica di visualizzazione per specificare se la sezione deve essere visualizzata nel modulo, in base alle selezioni effettuate dagli utenti nei campi personalizzati a scelta multipla durante la compilazione del modulo.</p><p><strong>NOTA:</strong> Se a tutti i singoli campi di un’interruzione di sezione è applicata una logica di visualizzazione e questi sono tutti nascosti come risultato della logica, l’intera sezione sarà nascosta nel modulo personalizzato. Ciò si verifica anche se la logica di visualizzazione non viene applicata all’interruzione di sezione.</p><p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Concedi l’accesso</p> </td> 
      <td> <p> Per visualizzare questa sezione e modificare i valori dei campi, seleziona le autorizzazioni necessarie per un oggetto a cui è allegato il modulo personalizzato.
       <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono visualizzare i valori dei campi</b>:</p> 
         <ul>
          <li><strong>Visualizza</strong>: visualizzare le autorizzazioni per l’oggetto</li>
          <li><p><b>Modifica limitata</b>: (disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
          <p>Consente agli utenti di contribuire all'oggetto se si tratta di un progetto, attività o problema.</p>
          <p>Consente agli utenti di modificare il profilo o di disporre dell'autorizzazione di profilo per l'oggetto, se si tratta di un utente.</p></li> 
          <li><b>Modifica</b>: gestione delle autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
        <p>Le seguenti autorizzazioni sono disponibili in <b>Gli utenti con questo accesso all’oggetto possono modificare i valori dei campi</b>: </p> 
         <ul> 
          <li> <p><b>Modifica limitata</b>: (disponibile solo se l’oggetto è un progetto, un’attività, un problema o un utente):</p> 
           <p>Se l'oggetto rappresenta un progetto, un'attività o un problema, questa autorizzazione consente agli utenti di contribuire all'oggetto</p>
          <p>Se l’oggetto è un utente, questa autorizzazione consente agli utenti di modificare il profilo o di essere proprietari dell’autorizzazione di profilo per l’oggetto.</p> 
          <li><b>Modifica</b>: gestione delle autorizzazioni per l’oggetto </li> 
          <li><b>Solo amministratore</b>: livello di accesso Amministratore di sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Per informazioni sulle autorizzazioni per gli oggetti, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Gli utenti senza le autorizzazioni specificate qui non possono visualizzare i campi personalizzati e i widget nella sezione. </p> <p>Questo vale anche se visualizzi i valori dei campi nei rapporti o li utilizzi nei campi calcolati nella generazione rapporti in modalità testo.</p> </li>
       <li><p>Per i moduli personalizzati per richieste/problemi: se è necessario l’accesso di visualizzazione per visualizzare i campi nell’interruzione di sezione, ma è necessario l’accesso di amministratore per modificare i campi, la sezione e tutti i relativi campi non saranno visibili agli utenti non amministratori durante la compilazione del modulo. Una volta creata la richiesta, gli utenti con accesso di visualizzazione possono visualizzare i campi nella sezione.</p></li>
       <li> <p>L'associazione di più tipi di oggetto al modulo può modificare le autorizzazioni di visualizzazione e modifica disponibili in questi passaggi. Per ulteriori informazioni, consulta <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Come più tipi di oggetto possono influenzare le autorizzazioni di interruzione di sezione in un modulo personalizzato</a> in questo articolo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Trascina o aggiungi almeno un campo personalizzato o un widget nella nuova sezione.

   Questa operazione è necessaria prima di salvare la sezione.

1. Clic **Fine**.

   >[!TIP]
   >
   >Puoi fare clic su **Applica** in qualsiasi momento durante la creazione di un modulo personalizzato per salvare le modifiche e mantenere aperto il modulo.

1. Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Come più tipi di oggetto possono influire sulle autorizzazioni dell’interruzione di sezione {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorizzazione Modifica limitata per le interruzioni di sezione del modulo personalizzato è disponibile solo per i tipi di oggetto Progetto, Attività, Problema e Utente.

In un modulo personalizzato con un&#39;interruzione di sezione configurata con l&#39;autorizzazione Modifica limitata, se si aggiunge uno degli altri tipi di oggetto al modulo (Portfolio, Programma, Documento, Società, Fatturazione, Iterazione, Spesa o Gruppo), verrà richiesto di passare all&#39;autorizzazione Modifica, che è compatibile sia con il tipo di oggetto sia con i tipi di oggetto esistenti nel modulo.

>[!INFO]
>
>**Esempio:** In un modulo personalizzato associato al tipo di oggetto Progetto, viene configurata un’interruzione di sezione con l’autorizzazione Modifica limitata.
>
>Aggiungendo al modulo il tipo di oggetto Portfolio, l&#39;opzione di autorizzazione Modifica limitata non sarà più disponibile per l&#39;interruzione di sezione nel modulo.
>
>Un messaggio sullo schermo richiede di passare all&#39;autorizzazione Modifica, che è l&#39;opzione più simile a Modifica limitata e compatibile sia con il tipo di oggetto Progetto che con il tipo di oggetto Portfolio.

