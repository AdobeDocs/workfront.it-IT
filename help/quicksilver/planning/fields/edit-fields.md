---
title: Modifica impostazioni campo
description: In Adobe Workfront Planning è possibile modificare le impostazioni dei campi già creati. In questo articolo viene descritto come modificare le impostazioni per i campi di Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 0%

---


# Modifica impostazioni campo

<!--leave the choice value information in yellow till January 2026-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile modificare le impostazioni dei campi esistenti in Adobe Workfront Planning.

Per informazioni sulla creazione dei campi di Adobe Workfront Planning, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

In questo articolo viene descritto come modificare le impostazioni per i campi di Workfront Planning. Per informazioni sulla modifica dei valori dei campi per i record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

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
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Considerazioni sulla modifica delle impostazioni dei campi

Prima di apportare modifiche alla configurazione di un campo, è necessario considerare quanto segue:

* È possibile modificare le impostazioni dei campi solo dalla tabella del tipo di record.
* Non è possibile modificare le impostazioni di un campo nella pagina record o in un&#39;altra visualizzazione, all&#39;esterno della visualizzazione tabella.
* Non è possibile modificare il tipo di campo dopo il salvataggio del campo.
* Non è possibile deselezionare l&#39;impostazione Consenti numeri negativi precedentemente selezionata per un campo Numerico, Percentuale o Valuta se sono già presenti valori negativi memorizzati nei record a cui è associato.
* Dopo aver salvato il campo, puoi modificare la configurazione dei seguenti elementi di campo:

   * Nome o descrizione di un campo
   * Opzioni di un campo a selezione singola o multipla.
   * Espressione di un campo Formula.

  >[!WARNING]
  >
  >Quando si modificano le espressioni della formula o si aggiungono o si rimuovono opzioni da un campo di tipo selezionato, si verifica una perdita di dati per i record che contengono già informazioni memorizzate nei campi la cui configurazione viene modificata.
  >
  >Non viene visualizzato alcun avviso o indicazione che possa verificarsi questa perdita di dati quando si modifica la configurazione dei campi.
  >
  >Non viene inviata alcuna notifica agli altri utenti circa la modifica della configurazione del campo.

* È possibile modificare i campi di ricerca esistenti dai record connessi.
* Oltre a modificare il campo come descritto nella sezione [Modifica impostazioni campo](#edit-field-settings-1) di questo articolo, è possibile modificare le scelte di un campo a selezione singola o multipla quando si modifica un record nella vista tabella, mentre si aggiornano i valori dei campi. Per informazioni, vedere la sezione [Aggiungere nuove scelte a un campo di selezione esistente durante la modifica dei record nella vista tabella](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) in questo articolo.

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Modifica impostazioni campo

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i campi record.

   Viene aperto il workspace e tutti i tipi di record nel workspace vengono visualizzati su schede.

1. Fare clic sulla scheda di un tipo di record.

   Verrà aperta la pagina del tipo di record.

1. (Condizionale) Fare clic sulla scheda di una **visualizzazione Tabella**.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.
1. Passa il puntatore del mouse sull&#39;intestazione di colonna di un campo che desideri modificare, quindi fai clic sulla freccia rivolta verso il basso dopo il nome del campo, quindi fai clic su **Modifica campo**

   Oppure

   Fare doppio clic sull&#39;intestazione di colonna per il campo.

   ![Menu freccia dopo il nome del campo nell&#39;intestazione della tabella evidenziato](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aggiorna le informazioni sul campo e fai clic su **Salva**.

   Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Non è possibile aggiornare il tipo di campo dopo il salvataggio del campo.
   >
   >* Quando si modificano le configurazioni dei campi (opzioni di campo o espressioni di formula), i record che contengono già informazioni nei campi modificati aggiorneranno i propri valori in tempo reale. Non viene visualizzato alcun avviso né registro di controllo per le modifiche al valore attivate dalle modifiche alla configurazione del campo. Tutti gli utenti che visualizzano i campi visualizzeranno immediatamente i nuovi valori con le modifiche.

   Le informazioni sul campo vengono aggiornate per tutti gli utenti con accesso alla visualizzazione dell&#39;area di lavoro.

1. (Condizionale) Per i campi record connessi, fare clic su **Modifica campi di ricerca** e aggiungere o rimuovere i campi di ricerca dal tipo di record connesso.

   Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).


## Aggiungere nuove scelte a un campo di selezione esistente durante la modifica di record nella vista tabella

<!--some of this information is also available in Edit records article - update both when necessary-->

È possibile aggiungere nuove scelte a un campo a selezione singola o multipla esistente durante la modifica di record nella vista tabella.

>[!IMPORTANT]
>
>La funzionalità descritta in questa sezione è disponibile solo nella vista tabella. Non è disponibile in altre aree in cui vengono visualizzati campi a selezione singola o multipla.

**ESEMPIO**

È possibile che sia presente un campo a selezione singola denominato Stato con le opzioni Nuovo e Chiuso e che si desideri aggiungere una scelta per uno stato In corso. È possibile aggiungere la scelta eseguendo una delle operazioni seguenti:

* Modifica del campo. Per informazioni, vedere la sezione [Modifica impostazioni campo](#edit-field-settings-1) in questo articolo.
* Aggiunta di una nuova opzione durante la modifica del record nella vista tabella, come descritto di seguito.

Per aggiungere una nuova scelta a un campo di selezione esistente durante la modifica di un record:

1. Passare a una pagina del tipo di record e aprire la visualizzazione tabella.
1. Aggiungere come nuova colonna il campo a selezione singola o multipla a cui si desidera aggiungere una scelta nella vista a tabella. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).
1. Inizia a modificare il campo in linea facendo doppio clic sulla cella del campo.
1. Digitare il nome della scelta che si desidera aggiungere, quindi fare clic su **Aggiungi scelta**.

   ![Aggiungi la scelta nel campo a selezione singola nella vista tabella](assets/add-choice-in-table-view-for-single-select-field.png)

   La nuova scelta viene aggiunta immediatamente al campo a selezione singola.

   <span class="preview">A ogni scelta viene aggiunto un nuovo valore. Puoi utilizzare i valori di scelta nelle chiamate API o in altre integrazioni. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).</span>

