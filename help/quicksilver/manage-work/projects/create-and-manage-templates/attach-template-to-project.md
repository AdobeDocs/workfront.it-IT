---
product-area: templates
navigation-topic: templates-navigation-topic
title: Allegare un modello a un progetto
description: È possibile allegare un modello a un progetto durante la fase iniziale di creazione del progetto o dopo la sua creazione.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Allegare un modello a un progetto

È possibile allegare un modello a un progetto durante la fase iniziale di creazione del progetto o dopo la sua creazione.

Per ulteriori informazioni sulla creazione di un progetto utilizzando un modello, vedere [Creare un progetto utilizzando un modello](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti </p> <p>Per informazioni sull'accesso al progetto, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l'accesso ai progetti</a>.</p> <p>Accesso ai modelli</p> <p>Per informazioni sulle autorizzazioni per i modelli, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Condividere un modello</a>. </p> <p>Per informazioni sull'accesso ai modelli, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l'accesso ai modelli</a>.</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto</p> <p>Per informazioni sulle autorizzazioni del progetto, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condividere un progetto in Adobe Workfront</a>. </p> <p>Visualizza autorizzazioni o versioni successive per il modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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

È possibile allegare un modello a un progetto in Workfront dalla pagina del progetto o da un elenco o report di progetti.

1. Vai al progetto in cui desideri allegare un modello e fai clic sull&#39;icona **Altro** ![Altro](assets/qs-more-icon-on-an-object.png) a destra del nome del progetto

   ![Altro menu a discesa](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Vai a un elenco o a un report di progetti e seleziona un progetto, quindi fai clic sull&#39;icona **Altro** ![Altro](assets/qs-more-icon-on-an-object.png) nella parte superiore dell&#39;elenco.

   ![Menu Altro espanso](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Fare clic su **Allega modello**.

   Viene visualizzata la casella Allega modello (Attach Template).

1. Inizia a digitare il nome del modello da allegare nel campo **Cerca modelli**, quindi fai clic su di esso quando viene visualizzato.nell&#39;elenco

   Oppure

   Fare clic sul nome di un modello nell&#39;area **Altri modelli**.

   A destra viene visualizzata un&#39;anteprima del modello che contiene le seguenti informazioni sul modello:

   * Durata
   * Proprietario
   * Numero di attività di primo livello (include un elenco delle prime tre attività di primo livello)
   * Numero totale di attività
   * Nomi dei moduli personalizzati allegati

   ![Allega casella modello](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Facoltativo) Fai clic sull&#39;icona **Preferiti** ![Preferiti](assets/favorites-icon-small.png) a sinistra del nome del modello per contrassegnarlo come preferito. In questo modo il modello viene spostato nell&#39;elenco Preferiti.

   ![Icona Preferiti nell&#39;elenco modelli](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Facoltativo) Fai di nuovo clic sull&#39;icona **Preferiti** ![Preferiti](assets/favorites-icon-selected.png) per rimuoverla dall&#39;elenco Preferiti.
1. Fare clic su **Personalizza e allega**.

   ![Allega modello](assets/attach-template-large-box-nwe-350x262.png)

1. Aggiorna le informazioni nelle sezioni seguenti prima di allegare il modello (oppure fai clic su **Allega modello** in qualsiasi momento):

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
      <td> <p>Fare clic sul campo per visualizzare un elenco delle attività del progetto. Selezionare l'attività di progetto che si desidera completare prima di poter avviare le attività modello. In alternativa, puoi saltare questo passaggio e impostare relazioni all’interno del progetto dopo aver allegato il modello. </p> <p> Seleziona le informazioni relative al <strong>Tipo di dipendenza</strong>, <strong>Lag</strong> e specifica se il predecessore deve essere <strong>Imposto</strong> o meno. </p> </td> 
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
      <td> <p>Deselezionate le caselle di controllo accanto alle informazioni che desiderate cancellare dal modello prima di allegarle al progetto. Queste informazioni non vengono trasferite dal modello al progetto. Per ulteriori informazioni su ciascun campo, vedere <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Panoramica sull'associazione di un modello a un progetto</a>. </p> <p>Importante: se si seleziona la casella <strong>Impostazione proprietà coda e problemi</strong>, i dettagli coda del modello sovrascriveranno quelli del progetto. In questo caso, le Regole di instradamento, gli Argomenti coda e i Gruppi di argomenti del modello vengono aggiunti a quelli del progetto. <br>Se il progetto è configurato come coda di richieste e il modello allegato al progetto non è configurato come coda di richieste, le informazioni sulla coda del progetto vengono rimosse se si lascia selezionata la casella <strong>Proprietà coda e configurazione problemi</strong>. <br>Se si deseleziona la casella <strong>Proprietà coda e Configurazione problema</strong>, tutte le impostazioni di Configurazione coda del progetto vengono mantenute e nessuna impostazione di Configurazione coda del modello viene allegata. </p> </td> 
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
   >* Se i campi dei moduli personalizzati del modello esistono già nel progetto e contengono informazioni, queste vengono mantenute nel progetto. Non è possibile modificarli durante l&#39;associazione del modello.

1. Fare clic su **Allega modello.**
1. Fare clic su **Annulla allegato** per interrompere l&#39;associazione del modello.

   Oppure

   Consenti all&#39;allegato di completare l&#39;aggiunta del modello al progetto.

   Dopo aver allegato il modello, è possibile modificare il progetto e modificare le attività, le informazioni o le impostazioni in base alle esigenze.

1. (Facoltativo) Fai clic su **Dettagli progetto**, quindi su **Panoramica** per visualizzare il nome del modello allegato nell&#39;area **Relazioni progetto**.

   >[!TIP]
   >
   >Se si allegano più modelli al progetto, in questo campo viene visualizzato solo il modello applicato per primo. Per informazioni, vedere la sezione [Allegare più modelli a un progetto esistente e visualizzare le informazioni sul modello](#attach-multiple-templates-to-an-existing-project-and-view-template-information) in questo articolo.

1. (Facoltativo) Rimuovi le informazioni sul modello dal progetto in cui è stato allegato il modello. Per informazioni, vedere [Rimuovere le informazioni sul modello da un progetto](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Allegare più modelli a un progetto esistente e visualizzare le informazioni sul modello {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

È possibile allegare più modelli (uno alla volta) allo stesso progetto, seguendo i passaggi descritti nella sezione [Allegare un modello a un progetto esistente](#attach-a-template-to-an-existing-project) in questo articolo. In questo modo le attività e altre informazioni di ogni modello vengono aggiunte al progetto.

>[!TIP]
>
>Quando si allegano diversi modelli a un progetto, nell&#39;area Dettagli progetto viene visualizzato solo il modello associato per primo.

Per capire quale modello viene applicato a un progetto:

1. Passa a un progetto a cui è associato un modello.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Trova il nome del modello allegato al progetto nel campo **Modello** nella parte inferiore della sezione **Panoramica** in **Relazioni progetto**.

   ![Informazioni modello sul progetto](assets/nwe-template-info-on-project-350x356.png)


