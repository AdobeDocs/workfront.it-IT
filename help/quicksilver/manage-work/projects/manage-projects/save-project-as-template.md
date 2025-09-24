---
product-area: projects;templates
navigation-topic: manage-projects
title: Salvare un progetto come modello
description: Puoi salvare un progetto come modello a livello di progetto, in modo che gli utenti possano visualizzarlo nell’interfaccia utente; esiste un altro articolo a cui è possibile fare collegamento più approfondito (passo dopo passo). Questa funzionalità deve essere disponibile sia nell'area Progetti che in quella Modelli.)
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# Salvare un progetto come modello

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<!--
<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

Se decidi che un progetto si ripeterà in un secondo momento, puoi creare un modello da quel progetto esistente. Sarà quindi possibile utilizzare nuovamente il modello per creare progetti futuri che potrebbero contenere informazioni simili o condividere la stessa sequenza temporale o le stesse assegnazioni con il progetto esistente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard </p>
   Oppure 
   <p>Corrente: Piano </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un progetto </p> <p>Ottieni le autorizzazioni di gestione per il modello dopo aver salvato il progetto come modello</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Salvare un progetto come modello

<!--
Saving a project as a template differs in the Production and the Preview environments. 

### Save a project as a template in the Production environment


1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/qs-more-icon-on-an-object.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td>Use the drop-down list to select any custom forms to attach to the template. If any custom forms have already been associated with the project, all of the data fields from those custom forms are displayed.<br>You can include up to 10 custom forms on a single template.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Manage Forms** to remove or reorder the forms. For information about how to remove and reorder custom forms on the template, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Click **Next Step.**
1. In the **Options** section, select the checkbox beside any information you want to clear from the template.

   ![](assets/save-as-template-options-step-350x109.png)

1. Click **Next Step.**
1. In the **Exclude** section, select any tasks that you want to exclude from the project.

   ![](assets/save-as-template-exclude-350x205.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates and can either be attached to an existing project or used to create a new one.


<div class="preview">

### Save a project as a template in the Preview environment

-->

1. Vai al progetto che desideri salvare come modello.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/qs-more-icon-on-an-object.png), quindi **Salva come modello**.
1. Nella sezione **Salva come modello** specificare le informazioni seguenti per il modello:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome Modello</td> 
      <td>Specificare un nome per il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Fornisci una descrizione per il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p><strong>Sì</strong>: altri utenti possono trovare il modello e allegarlo ai progetti.</p> </li> 
        <li><strong>No</strong>: altri utenti non possono trovare il modello e non possono allegarlo ai progetti.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Utilizza l’elenco a discesa per selezionare i moduli personalizzati da allegare al modello. Se al progetto sono già stati associati moduli personalizzati, vengono visualizzati tutti i campi di dati di tali moduli personalizzati.<br>È possibile includere fino a 10 moduli personalizzati in un singolo modello.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Forms personalizzato** nel pannello a sinistra per rimuovere o riordinare i moduli.

   Per riordinare i moduli, trascinarli nell&#39;ordine corretto.
Per rimuovere un modulo, selezionarlo, quindi fare clic su **Rimuovi**. Fare clic su **Annulla** per rimuovere i moduli selezionati.

   ![Area moduli personalizzati nella casella Salva come modello](assets/custom-forms-ara-in-save-as-template-box.png)

1. Se necessario, aggiorna le informazioni nei moduli personalizzati allegati. Le informazioni verranno trasferite al modello.

1. Fai clic su **Opzioni** nel pannello a sinistra, quindi seleziona la casella di controllo accanto alle informazioni da trasferire al modello. Gli elementi deselezionati non vengono trasferiti al modello. Per impostazione predefinita, tutte le opzioni sono deselezionate.

   ![Area Opzioni nella casella Salva come modello](assets/options-area-in-save-as-template-box.png)

1. Fai clic su **Escludi** nel pannello a sinistra, quindi seleziona le attività da escludere dal progetto. Per impostazione predefinita, tutte le attività sono deselezionate.

   ![Escludi area nella casella Salva come modello](assets/exclude-area-save-as-template-box.png)

1. Fai clic su **Fine e salva modello** nell&#39;angolo superiore destro della schermata.

   Il modello viene ora visualizzato nell’elenco dei modelli disponibili e può essere allegato a un progetto esistente o utilizzato per crearne uno nuovo.

