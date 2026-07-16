---
title: Condivisione di un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile configurare l'accesso per un modulo personalizzato per controllare gli utenti che possono visualizzarlo, condividerlo e modificarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
TQID: https://experienceleague.adobe.com/gpJQedqcdtjaxvhVuWKgJVpfAPAT2ICSgO6nRFLvimM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b0dd2c2c448c829b2ce1559ddc87880c9a47a68f
workflow-type: tm+mt
source-wordcount: 967
ht-degree: 5%

---

# Condividere un modulo personalizzato

È possibile configurare l&#39;accesso per un modulo personalizzato in modo da controllare chi può visualizzarlo, condividerlo e modificarlo, ovvero la persona, il ruolo, il gruppo, il team, la società e il profilo aziendale.

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

## Accesso ai moduli personalizzati {#access-to-custom-forms}

Per impostazione predefinita, quando si crea un nuovo modulo personalizzato e qualcuno lo allega a un oggetto, qualsiasi utente assegnato all’oggetto può visualizzare e compilare il modulo. Sono inclusi gli utenti con licenze Collaboratore o Richiesta e gli utenti esterni.

Tuttavia, in un oggetto in cui il modulo personalizzato non è già allegato, un utente (anche se dispone di un livello di accesso Standard o Planner) non può allegarlo dal menu a discesa Forms personalizzato a meno che non si verifichi una delle seguenti condizioni:

* Qualcuno ha condiviso il modulo personalizzato come &quot;Tutti nel sistema possono visualizzare e allegare&quot;
* Qualcuno ha condiviso il modulo personalizzato con l’utente o con il suo team, mansione, gruppo, azienda o profilo aziendale concedendo almeno l’autorizzazione Visualizzazione con l’opzione Allega a dati personalizzati selezionata
* L’utente dispone di una licenza Standard o Plan e il loro livello di accesso consente l’accesso amministrativo ai moduli personalizzati

<!--

## Share a custom form from the list of forms

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access-to-custom-forms) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Select the custom form, then click ![Share icon](assets/share-icon.png).
1. In the box that displays, under **Give custom form access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the custom form with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, company, or business profile you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>This option provides the ability to view and fill out the custom form on objects. At the object level, users must also have at least Contribute access with the <strong>Edit custom form</strong> advanced setting enabled. For example, if the form is attached to a project, users must have Contribute access to that project, or they will not be able to fill out the form.</p>
      
      <p><b>NOTE</b>: For users with Light and Contributor licenses (or Work, Review, and Request licenses), this is the highest available option.</p>
      
      <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><strong>Share</strong>: Ability to share the custom form with others in the system</p> <p>Users with a Light or Contributor license (or Work, Review, or Request license) can share a custom form only through the API or a custom forms report.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>This option available only for users with a Standard or Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow following:</p> 
       <ul> 
        <li> <p><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
        <li><strong>Delete</strong>: Delete the custom form from the system</li> 
        <li><strong>Share</strong>: Share the custom form with others in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Remove system-wide access**.

   If you change your mind, you can click **Make this visible system-wide** (the default option).

   >[!NOTE]
   >
   >* When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >* Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use **Make this visible system-wide**. When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.

1. Click **Save**.

-->

## Condividere un modulo personalizzato

Invece di lasciare un modulo personalizzato nello stato di condivisione predefinito (descritto in [Accesso ai moduli personalizzati](#access-to-custom-forms) in questo articolo), puoi configurare livelli specifici di accesso al modulo per determinati utenti, ruoli, gruppi, team, aziende e profili aziendali.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato nell&#39;elenco, quindi fai clic sull&#39;icona ![Condividi](assets/share-icon.png).

   Oppure

   Aprire un modulo personalizzato o crearne uno nuovo. Quindi, fai clic su **Condividi** in alto a destra nella finestra di progettazione del modulo.

1. Nella casella Condivisione, in **Concedi l&#39;accesso al modulo personalizzato a**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo, della società o del profilo aziendale con cui vuoi condividere il modulo personalizzato, quindi premi **Invio** quando viene visualizzato il nome.
1. Per regolare l’accesso per l’utente, il team, la mansione, il gruppo, l’azienda o il profilo aziendale appena aggiunto, fai clic sul menu a discesa a destra del nome, quindi configura una delle seguenti opzioni disponibili e le relative impostazioni avanzate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzazione</td> 
      <td> <p>Questa opzione consente di visualizzare e compilare il modulo personalizzato sugli oggetti. A livello di oggetto, gli utenti devono inoltre disporre almeno dell'accesso Contribute con l'impostazione avanzata <strong>Modifica modulo personalizzato</strong> abilitata. Ad esempio, se il modulo è allegato a un progetto, gli utenti devono avere l'accesso Contribuisci a tale progetto, altrimenti non potranno compilare il modulo.</p>

   <p><b>NOTA</b>: per gli utenti con licenze Light e Contributor (o Licenze Work, Review e Request), questa è l'opzione più alta disponibile.</p> <p>Fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell'accesso di gestione</li> 
        <li> <p><strong>Condividi</strong>: possibilità di condividere il modulo personalizzato con altri utenti nel sistema</p> <p>Gli utenti con una licenza Light o Contributor (o Licenza Lavoro, Revisione o Richiesta) possono condividere un modulo personalizzato solo tramite l’API o un rapporto di moduli personalizzati.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestione</td> 
      <td> <p>Questa opzione è disponibile solo per gli utenti con una licenza Standard o Plan. </p> <p>Oltre a poter aggiungere il modulo agli oggetti a cui hanno accesso per la modifica, gli utenti possono anche modificare completamente il modulo personalizzato, incluse le operazioni di aggiunta, modifica ed eliminazione dei campi.</p> <p>Fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li> <p><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell'accesso di gestione</p> </li> 
        <li><strong>Elimina</strong>: elimina il modulo personalizzato dal sistema</li> 
        <li><strong>Condividi</strong>: condividi il modulo personalizzato con altri utenti nel sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi 5-6 per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Se desideri limitare l&#39;accesso al modulo personalizzato (sugli oggetti a cui è allegato) a quelli specificati nei passaggi precedenti, fai clic sulla freccia a discesa sotto **Chi ha accesso**, quindi seleziona **Solo gli invitati possono accedere**.

   Se cambi idea, puoi selezionare **Tutti nel sistema possono visualizzare**.

   >[!NOTE]
   >
   >* Quando si rende visibile un modulo personalizzato a livello di sistema, è possibile consentire agli utenti di visualizzarlo e compilarlo solo sugli oggetti a cui sono assegnati, non di allegarlo ad altri oggetti. È possibile concedere la possibilità di allegare il modulo personalizzato agli oggetti utilizzando l&#39;opzione &quot;Allega a dati personalizzati&quot; descritta nel passaggio 6.
   >* La maggior parte delle organizzazioni desidera assicurarsi che tutti gli utenti del sistema possano compilare un modulo personalizzato quando è allegato agli oggetti su cui lavorano e visualizzarne i dati nei rapporti. Se questo è vero per la tua organizzazione, ti consigliamo di utilizzare **Tutti nel sistema possono visualizzare**.
   >* Se si seleziona **Tutti nel sistema possono visualizzare e allegare**, tutti gli utenti possono allegare il modulo ad altri oggetti.
   >
   >![Condividi modulo personalizzato](assets/share-custom-forms-all-can-attach.png)
   >   
   >Se si teme un modulo personalizzato in cui gli utenti potrebbero immettere dati sensibili quando è allegato a determinati oggetti, limitare la condivisione per questi *oggetti* potrebbe essere più efficace rispetto a limitare l&#39;accesso al modulo stesso.

1. Fai clic su **Salva**.

## Rimuovere l’accesso a un modulo personalizzato

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato nell&#39;elenco, quindi fai clic sull&#39;icona ![Condividi](assets/share-icon.png).
1. Nella casella Condivisione fare clic sul menu a discesa a destra del nome dell&#39;utente, del team, della mansione, del gruppo, della società o del profilo aziendale che non si desidera più avere accesso speciale al modulo e selezionare **Rimuovi**.
1. (Facoltativo) Ripetere il passaggio precedente per gli altri nomi che si desidera rimuovere.
1. Fai clic su **Salva**.

