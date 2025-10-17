---
title: Creare tipi di record importando informazioni da un file CSV o Excel
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell'organizzazione importando informazioni da un file CSV o Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Creare tipi di record importando informazioni da un file CSV o Excel

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell&#39;organizzazione importando informazioni da un file CSV o Excel.

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
<p>Oppure</p>
<p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
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
</table>-->


## Considerazioni sull&#39;importazione di tipi di record utilizzando un file Excel o CSV

* Ogni foglio del file Excel diventa un tipo di record. Il nome del foglio diventa il nome del tipo di record.
* Se è presente un solo foglio o se si importa un file CSV, il nome del file diventa il nome del tipo di record.
* Le intestazioni delle colonne di ciascun foglio diventano i campi associati a ciascun tipo di record.
* I campi sono univoci per i rispettivi tipi di record.
* Ogni riga di ogni foglio diventa un record univoco associato al rispettivo tipo di record.
* Ogni foglio del file Excel non deve superare i seguenti:
   * 25.000 righe
   * 500 colonne
* Il file non deve superare i 5 MB.
* I fogli vuoti non sono supportati.
* I campi dei tipi seguenti non sono supportati e non possono essere mappati ai campi del foglio di importazione:

   * Campi di connessione ai tipi di oggetto Workfront e AEM Assets.
   * Campi di ricerca da record di Planning o oggetti Workfront e AEM Assets connessi
   * Campi formula
   * Data di creazione, Creato da
   * Data ultima modifica, Autore ultima modifica
   * Data di approvazione, Approvato da
   * People

Per importare tipi di record utilizzando un file Excel o CSV:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera creare i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. Fare clic su **Aggiungi tipo di record**.
1. Fare clic su **Carica dal file**.
1. Trascina e rilascia un file Excel o CSV salvato in precedenza sul computer, oppure fai clic su **Seleziona un file CSV o Excel** per cercarne uno, quindi selezionalo.
1. Fare clic su **Anteprima e modifica**.

   La casella **Anteprima e modifica** viene visualizzata con le seguenti informazioni:

   * I nomi dei fogli o dei tipi di record futuri vengono visualizzati nel pannello sinistro. Per impostazione predefinita, Workfront Planning seleziona un&#39;icona e un colore per ogni nuovo tipo di record.
   * Il primo foglio o il tipo di record viene selezionato e i nomi dei campi associati vengono visualizzati come intestazioni di colonna. Il tipo di ogni campo è selezionato per impostazione predefinita.
   * Ogni riga rappresenta un nuovo record. Nella casella Anteprima e modifica vengono visualizzati solo i primi 10 record.

   ![Casella di anteprima e modifica](assets/preview-and-edit-box.png)

1. (Facoltativo) Fate clic sul nome di ciascun foglio nel pannello a sinistra per esaminare le informazioni in esso contenute.

   >[!NOTE]
   >
   >I fogli vuoti non sono supportati e sono oscurati.

1. (Facoltativo) Deseleziona i fogli che non desideri importare dal pannello a sinistra.

   ![Seleziona i fogli da importare con non selezionato](assets/select-sheets-to-import-drop-down-with-unselected.png)

   I fogli deselezionati vengono visualizzati con uno sfondo grigio.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra di un&#39;intestazione di colonna per eseguire una delle operazioni seguenti nella scheda **Campo**:

   ![Scheda campo nella casella di importazione mapping tipo di record](assets/field-tab-on-record-type-import-mapping-box.png)

   * Rinomina uno dei campi
   * Cambia il tipo di campo **&#x200B;**
   * Aggiorna il campo **Descrizione**

1. (Facoltativo) Fare clic sulla scheda **Connessione** per associare le informazioni della colonna a un campo connesso di altri tipi di record.

   ![Scheda Connessione nella casella di mappatura importazione tipo di record](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >È possibile eseguire il mapping solo ai campi dei record connessi a Workfront Planning. Non è possibile eseguire il mapping a campi da connessioni Workfront o AEM Assets. Per ulteriori informazioni, vedere la sezione [Considerazioni sull&#39;importazione di tipi di record tramite un file Excel o CSV](#considerations-about-importing-record-types-using-an-excel-or-csv-file) in questo articolo.

1. (Condizionale) Dopo aver aggiornato le informazioni sul campo, fai clic su **Salva**.

1. Fare clic su **Importa** quando si è pronti per importare il file.

   Le informazioni seguenti vengono importate in Workfront Planning:

   * Nuovi tipi di record
   * Nuovi campi associati a ciascun tipo di record
   * Nuovi record associati a ciascun tipo di record

   È possibile iniziare a gestire campi e record nelle pagine dei tipi di record.

   Tutti coloro che hanno accesso a Workfront Planning e all&#39;area di lavoro possono ora visualizzare e modificare i tipi di record importati e le relative informazioni.
