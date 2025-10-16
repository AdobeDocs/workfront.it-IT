---
title: Crea tipi di record
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell'organizzazione.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# Crea tipi di record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi relativi al lavoro necessari per il ciclo di vita dell&#39;organizzazione.

Per ulteriori informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p>Qualsiasi pacchetto di Workflow e Planning</p>
<p><b>NOTA</b></p>
<p>Per configurare i tipi di record collegabili: </p>
<ul> 
<li><p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></li></ul>

<div class="preview">
<p>Per configurare i tipi di record globali:</p>

<ul> 
<li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> -->

## Considerazioni sulla creazione di tipi di record

* È possibile creare tipi di record in un&#39;area di lavoro nei modi seguenti:

   * Automaticamente:
      * Quando crei un’area di lavoro utilizzando un modello.

        Per informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Quando li importi utilizzando un file CSV o Excel.

        Per ulteriori informazioni, vedere [Creare tipi di record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

     >[!TIP]
     >
     >Quando si importa un tipo di record da un file CSV o Excel, è anche possibile importare record e campi.

   * Manualmente:

      * Da zero.

        Questo articolo descrive come creare tipi di record da zero.

     <!--
        * <span class="preview">By adding them from another workspace</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


* È possibile spostare tipi di record all&#39;interno di una sezione e da una sezione di un&#39;area di lavoro a un&#39;altra. Non è possibile spostare tipi di record da un&#39;area di lavoro a un&#39;altra.

## Creare tipi di record utilizzando un modello di area di lavoro

È possibile creare automaticamente i tipi di record quando si crea un&#39;area di lavoro utilizzando un modello di Workfront Planning. Ogni modello contiene tipi di record di esempio.

Per informazioni sulla creazione di aree di lavoro, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

Per informazioni sui tipi di record inclusi in ogni modello, vedere [Elenco dei modelli di area di lavoro](/help/quicksilver/planning/architecture/workspace-templates.md).

Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono raggruppati nelle sezioni seguenti:

* Tipi di record operativi
* Tassonomie

È possibile aggiungere manualmente tipi di record nelle sezioni Tipi di record operativi e Tassonomie. Per informazioni, vedere la sezione [Creare un record da zero](#create-a-record-type-from-scratch) in questo articolo.

## Creare un tipo di record da zero

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera creare un tipo di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. (Facoltativo) Fai clic su **Aggiungi sezione** per aggiungere una nuova sezione all&#39;area di lavoro.
1. Fai clic su **Aggiungi tipo di record**, quindi su **Aggiungi manualmente**.

   Viene visualizzata la casella Aggiungi tipo di record. <!--update screen shot for preview-->

   ![Aggiungi la casella del tipo di record con le opzioni di aspetto](assets/add-record-type-box-with-appearance-options.png)

1. Aggiorna le seguenti informazioni nella scheda **Aspetto**:

   * Sostituire &quot;Tipo di record senza titolo&quot; con il nome del tipo di record futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descrizione**: aggiungere ulteriori informazioni sul tipo di record.
   * Selezionare un colore e una forma per l&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il nuovo tipo di record. Colore dell&#39;icona del tipo di record. Il grigio è selezionato per impostazione predefinita.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. (Facoltativo e condizionale) Se sei un amministratore di sistema, fai clic sulla scheda **Impostazioni avanzate** <span class="preview">o **Impostazioni per più aree di lavoro**</span> e aggiorna le informazioni sulle funzionalità per più aree di lavoro del tipo di record.

   Per ulteriori informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production - Jan 2026-->

   ![Casella Modifica tipo di record con scheda Impostazioni avanzate](assets/edit-record-type-box-advanced-settings-tab.png)

   Per ulteriori informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Fai clic su **Salva**.

   La scheda del tipo di record viene aggiunta alla sezione e all&#39;area di lavoro selezionate.
Sulla scheda viene visualizzata la descrizione del tipo di record.

   ![Scheda tipo record con descrizione](assets/record-type-card-with-description.png)

   Se hai selezionato di connettere questo record da altre aree di lavoro, l&#39;icona **Record collegabile** ![Icona Connetti da altri spazi](assets/connect-from-other-workspaces-icon.png) viene visualizzata sulla scheda record.

   <span class="preview">Se hai scelto di consentire l&#39;aggiunta di questo record ad altre aree di lavoro, l&#39;icona del **record globale** ![icona del tipo di record globale](assets/global-icon.png) viene visualizzata sulla scheda record. </span>

1. (Facoltativo) Passa il puntatore del mouse sulla scheda del tipo di record, fai clic sull&#39;icona **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica** o <span class="preview">**Impostazioni**</span> per modificare le informazioni sul tipo di record.

   Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facoltativo) Fare clic sulla scheda tipo di record per aprire la pagina tipo di record.

   ![Tipo di record operativo vuoto](assets/operational-record-type-blank.png)

   Per impostazione predefinita, la pagina del tipo di record viene visualizzata nella vista tabella. Le colonne della tabella sono campi associati al nuovo tipo di record. Ogni riga è un record univoco da aggiungere.

   Per impostazione predefinita, i campi seguenti vengono visualizzati nelle colonne della vista tabella di un tipo di record operativo:

   * Nome
   * Descrizione
   * Data di inizio
   * Data di fine
   * Stato

1. (Facoltativo) Aggiorna il nome del tipo di record nell’intestazione della pagina

   Oppure

   Fai clic sull&#39;icona **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record e fai clic su **Modifica** per rinominarlo o modificare le informazioni su di esso. Per ulteriori informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facoltativo) Fare clic su **+ Nuovo record** per aggiungere record del tipo di record selezionato. Per ulteriori informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
1. (Facoltativo) Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della tabella per aggiungere altri campi al tipo di record.

   Per ulteriori informazioni sulla creazione dei campi, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

1. (Facoltativo) Fare clic sulla freccia rivolta a sinistra a sinistra del nome del tipo di record nell&#39;intestazione per tornare all&#39;area di lavoro selezionata.

1. (Facoltativo) Dall’area di lavoro, fai clic su una scheda del tipo di record e tieni premuto per trascinarla in un punto desiderato o per spostarla in un’altra sezione.

   Le modifiche vengono salvate automaticamente.

   Per ulteriori informazioni sull&#39;aggiunta di record, l&#39;eliminazione o la modifica di tipi di record o l&#39;aggiornamento della visualizzazione nella pagina del tipo di record, vedere gli articoli seguenti:

   * [Crea record](/help/quicksilver/planning/records/create-records.md)
   * [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Gestisci visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md)

## Creare tipi di record importando informazioni da un file CSV o Excel

Quando si importano informazioni da un file CSV o Excel, è possibile importare quanto segue:

* Tipi di record
* Record
* Campi record

Per ulteriori informazioni, vedere [Creare tipi di record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

<!--

<div class="preview">

## Create record types by adding existing ones from another workspace 

You can add record types to a workspace by adding existing ones from another workspace. You can only add record types that have been configured as global record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->