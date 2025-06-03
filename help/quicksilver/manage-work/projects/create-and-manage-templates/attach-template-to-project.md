---
product-area: templates
navigation-topic: templates-navigation-topic
title: Allegare un modello a un progetto
description: È possibile allegare un modello a un progetto durante la fase iniziale di creazione del progetto o dopo la sua creazione.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Allegare un modello a un progetto

<!-- Audited: 5/2025 -->

È possibile allegare un modello a un progetto durante la fase iniziale di creazione del progetto o dopo la sua creazione.

Per ulteriori informazioni sulla creazione di un progetto utilizzando un modello, vedere [Creare un progetto utilizzando un modello](../../../manage-work/projects/create-projects/create-project-from-template.md).

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p>
   <p>Oppure</p>
   <p>Corrente: Piano</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti </p> <p>Per informazioni sull'accesso al progetto, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l'accesso ai progetti</a>.</p> <p>Accesso ai modelli</p> <p>Per informazioni sulle autorizzazioni per i modelli, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Condividere un modello</a>. </p> <p>Per informazioni sull'accesso ai modelli, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l'accesso ai modelli</a>.</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare e modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto</p> <p>Per informazioni sulle autorizzazioni del progetto, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condividere un progetto in Adobe Workfront</a>. </p> <p>Visualizza autorizzazioni o versioni successive per il modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Allega un modello a un progetto esistente {#attach-a-template-to-an-existing-project}

È possibile allegare un modello a un progetto dalla pagina del progetto o da un elenco o report di progetti.

{{step1-to-projects}}

1. Nella pagina **Progetti** selezionare il progetto a cui si desidera allegare un modello.

1. Fai clic sull&#39;icona **Altro** ![Icona Altro](assets/qs-more-icon-on-an-object.png) a destra del nome del progetto.

   ![Altro menu a discesa](assets/more-dropdown.png)

   Oppure

   Vai a un elenco o a un report di progetti e seleziona un progetto, quindi fai clic sull&#39;icona **Altro** ![Altro](assets/qs-more-icon-on-an-object.png) nella parte superiore dell&#39;elenco.

   ![Menu Altro espanso](assets/more-menu-expanded.png)


1. Fare clic su **Allega modello**. Viene visualizzata la casella **Allega modello**.

1. Inizia a digitare il nome del modello da allegare nel campo **Cerca modelli**, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   Oppure

   Fare clic sul nome di un modello nell&#39;area **Altri modelli**.

   A destra viene visualizzata un&#39;anteprima del modello che contiene le seguenti informazioni sul modello:

   * Durata
   * Proprietario
   * Numero di attività di primo livello (include un elenco delle prime tre attività di primo livello)
   * Numero totale di attività
   * Nomi dei moduli personalizzati allegati

   ![Allega casella modello](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Facoltativo) Fai clic sull&#39;icona **Preferiti** ![Preferiti](assets/favorites-icon-small.png) a destra del nome del modello per contrassegnarlo come preferito e spostarlo nell&#39;elenco **Preferiti**.

1. (Facoltativo) Fai di nuovo clic sull&#39;icona **Preferiti** ![Preferiti](assets/favorites-icon-selected.png) per rimuoverla dall&#39;elenco **Preferiti**.
1. Fare clic su **Personalizza e allega**. Viene aperto il pannello laterale **Allega modello**.

1. (Facoltativo) Aggiorna le informazioni nelle sezioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sezione Attività</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le attività modello selezionate di seguito vengono importate nel progetto. Deseleziona quelli da escludere. </td> 
      <td>Deseleziona le attività da escludere dal modello prima di allegarle al progetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selezionare l'attività di progetto che si desidera come predecessore delle attività in questo modello.</td> 
      <td> <p>Fare clic sul campo per visualizzare un elenco delle attività del progetto, quindi selezionare l'attività che deve essere completata prima che le attività del modello possano iniziare. In alternativa, puoi saltare questo passaggio e impostare relazioni all’interno del progetto dopo aver allegato il modello. </p> <p> Selezionare le informazioni relative al <strong>Tipo di dipendenza</strong>, al <strong>Tempo di ritardo</strong> e se si desidera applicare il predecessore selezionando la casella di controllo <strong>Applica predecessore</strong>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selezionare l'attività di progetto che si desidera utilizzare come padre delle attività in questo modello.</td> 
      <td> Selezionare l'attività di progetto che si desidera designare come attività padre per tutte le attività modello. Se non si effettua una selezione, tutte le attività modello vengono visualizzate alla fine delle attività progetto correnti. Puoi saltare questo passaggio e spostare le attività all’interno del progetto dopo aver allegato il modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sezione Opzioni</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gli elementi selezionati di seguito vengono trasferiti al progetto. Deseleziona quelli da escludere.</td> 
      <td> <p>Deseleziona le caselle di controllo relative alle informazioni da escludere dal modello prima di allegarle al progetto. Per ulteriori informazioni su ciascun campo, vedere <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Panoramica sull'associazione di un modello a un progetto</a>. </p> <p>Importante: se si seleziona la casella <strong>Impostazione proprietà coda e problemi</strong>, i dettagli coda del modello sovrascriveranno quelli del progetto. In questo caso, le Regole di instradamento, gli Argomenti coda e i Gruppi di argomenti del modello vengono aggiunti a quelli del progetto. <br>Se il progetto è configurato come coda di richieste e il modello associato al progetto non è impostato come coda di richieste, le informazioni sulla coda del progetto vengono rimosse se si lascia selezionata la casella <strong>Proprietà coda e configurazione problemi</strong>. <br>Se si deseleziona la casella <strong>Proprietà coda e Configurazione problema</strong>, tutte le impostazioni di Configurazione coda del progetto vengono mantenute e nessuna impostazione di Configurazione coda del modello viene allegata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sezione Forms personalizzata</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Forms personalizzato</td> 
      <td> <p>Quando i moduli personalizzati vengono allegati al modello, i relativi nomi vengono visualizzati nel pannello a sinistra. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Aggiorna le informazioni nei moduli personalizzati. Queste informazioni vengono trasferite al progetto.

   >[!TIP]
   >
   >* Questo passaggio è obbligatorio quando i moduli personalizzati nel modello contengono campi obbligatori vuoti.
   >* Se i campi dei moduli personalizzati del modello esistono già nel progetto e contengono informazioni, queste vengono mantenute nel progetto. Non è possibile modificarli mentre si allega il modello.

1. Fare clic su **Allega modello.**
1. Fare clic su **Annulla allegato** per interrompere l&#39;associazione del modello.

   Oppure

   Consenti all&#39;allegato di completare l&#39;aggiunta del modello al progetto.

   Dopo aver allegato il modello, è possibile modificare il progetto e modificare le attività, le informazioni o le impostazioni in base alle esigenze.

1. (Facoltativo) Nel pannello a sinistra, fai clic su **Dettagli progetto**, quindi su **Panoramica** per visualizzare il nome del modello allegato nell&#39;area **Relazioni progetto**.

   >[!TIP]
   >
   >Se si allegano più modelli al progetto, in questo campo verrà visualizzato solo il modello applicato per primo. Per informazioni, vedere la sezione [Allegare più modelli a un progetto esistente e visualizzare le informazioni sul modello](#attach-multiple-templates-to-an-existing-project-and-view-template-information) in questo articolo.

1. (Facoltativo) Rimuovi le informazioni sul modello dal progetto in cui è stato allegato il modello. Per informazioni, vedere [Rimuovere le informazioni sul modello da un progetto](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Allegare più modelli a un progetto esistente e visualizzare le informazioni sul modello {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

È possibile allegare più modelli (uno alla volta) allo stesso progetto seguendo i passaggi descritti nella sezione [Allegare un modello a un progetto esistente](#attach-a-template-to-an-existing-project) in questo articolo. In questo modo le attività e altre informazioni di ogni modello vengono aggiunte al progetto.

>[!TIP]
>
>Quando alleghi più modelli a un progetto, nell’area Dettagli progetto viene visualizzato solo il modello allegato per primo.

Per visualizzare il modello applicato a un progetto:

{{step1-to-projects}}

1. Nella pagina **Progetti** selezionare il progetto a cui è associato un modello.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra.

1. Individua il nome del modello associato al progetto nel campo **Modello** nella parte inferiore della sezione **Panoramica** in **Relazioni progetto**.

   ![Informazioni sul modello in un progetto](assets/nwe-template-info-on-project-350x356.png)


