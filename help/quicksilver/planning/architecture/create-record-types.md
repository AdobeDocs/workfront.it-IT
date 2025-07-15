---
title: Crea tipi di record
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell'organizzazione.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 459e3883101b644a91d5e2a32288cf5b02a02bd9
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# Crea tipi di record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi relativi al lavoro necessari per il ciclo di vita dell&#39;organizzazione.

Per ulteriori informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>Nell'ambiente di produzione, tutti gli utenti, inclusi gli amministratori di sistema, devono essere assegnati a un modello di layout che includa Planning.</p>
<p><span class="preview">Nell'ambiente di anteprima, per impostazione predefinita, Planning è abilitato per utenti standard e amministratori di sistema.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
        * <span class="preview">By importing then from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add cross-workspace record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md). </span>-->


* È possibile spostare tipi di record all&#39;interno di una sezione e da una sezione di un&#39;area di lavoro a un&#39;altra. Non è possibile spostare tipi di record da un&#39;area di lavoro a un&#39;altra.

## Creare tipi di record utilizzando un modello di area di lavoro

È possibile creare automaticamente i tipi di record quando si crea un&#39;area di lavoro utilizzando un modello di Workfront Planning. Ogni modello contiene tipi di record di esempio.

Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono raggruppati nelle sezioni seguenti:

* Tipi di record operativi
* Tassonomie

È possibile aggiungere manualmente tipi di record nelle sezioni Tipi di record operativi e Tassonomie.

Per informazioni sulla creazione di aree di lavoro, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

Per informazioni sui tipi di record inclusi in ogni modello, vedere [Elenco dei modelli di area di lavoro](/help/quicksilver/planning/architecture/workspace-templates.md).

## Creare un tipo di record da zero

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera creare un tipo di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. (Facoltativo) Fai clic su **Aggiungi sezione** per aggiungere una nuova sezione all&#39;area di lavoro.
1. Fai clic su **Aggiungi tipo di record**, quindi su **Aggiungi manualmente**.

   Viene visualizzata la casella Aggiungi tipo di record.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![Aggiungi la casella del tipo di record con le opzioni di aspetto](assets/add-record-type-box-with-appearance-options.png)

1. Aggiorna le seguenti informazioni nella scheda **Aspetto**:

   * Sostituire &quot;Tipo di record senza titolo&quot; con il nome del tipo di record futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descrizione**: aggiungere ulteriori informazioni sul tipo di record.
   * Selezionare un colore e una forma per l&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il nuovo tipo di record. Colore dell&#39;icona del tipo di record. Il grigio è selezionato per impostazione predefinita.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. (Facoltativo e condizionale) Se sei un amministratore di sistema, fai clic su **Impostazioni avanzate** e aggiorna le seguenti informazioni nella sezione **Ambito di connettività**: <!--the info here is duplicated in the Edit record types article-->

   * Abilita l&#39;impostazione **Connetti da altra area di lavoro**. Se attivato, il tipo di record è accessibile e può essere connesso da altre aree di lavoro.
   * Scegliere le aree di lavoro da cui è possibile accedere al tipo di record. Scegli una delle seguenti opzioni:

      * **A livello di sistema**: gli utenti possono connettersi a questo tipo di record da tutte le aree di lavoro in cui dispongono di autorizzazioni di gestione.
      * **Aree di lavoro specifiche**: aggiungere i nomi delle aree di lavoro a cui i responsabili area di lavoro possono connettersi a questo tipo di record.

   ![Casella Crea tipo di record nella scheda Impostazioni avanzate](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
    <div class="preview">
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
        * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
            You can designate specific users who can add this record type to other workspaces. 
        * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
            You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
        For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
        ******** replace screen shot below **********
        ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
    -->

1. Fai clic su **Crea**.

   La scheda del tipo di record viene aggiunta alla sezione e all&#39;area di lavoro selezionate.
Sulla scheda viene visualizzata la descrizione del tipo di record.

   ![Scheda tipo record con descrizione](assets/record-type-card-with-description.png)

1. (Facoltativo) Passa il puntatore del mouse sulla scheda del tipo di record, fai clic sull&#39;icona **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica** per modificare le informazioni sul tipo di record.
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

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as cross-workspace record types. 

For information, see [Add cross-workspace record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

</div>

-->