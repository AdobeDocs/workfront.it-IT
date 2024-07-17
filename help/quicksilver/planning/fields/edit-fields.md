---
title: Modifica impostazioni campo
description: In Adobe Workfront Planning è possibile modificare le impostazioni dei campi già creati. In questo articolo viene descritto come modificare le impostazioni per i campi di Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: dc8e6f730ec88fc66c3486987e064b5f0760fb80
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Modifica impostazioni campo

{{planning-important-intro}}

È possibile modificare le impostazioni dei campi già creati in Adobe Workfront Planning.

Per informazioni sulla creazione dei campi di Adobe Workfront Planning, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

In questo articolo viene descritto come modificare le impostazioni per i campi di Workfront Planning. Per informazioni sulla modifica dei valori dei campi per i record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

## Requisiti di accesso

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
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerazioni sulla modifica delle impostazioni dei campi

Prima di apportare modifiche alla configurazione di un campo, è necessario considerare quanto segue:

* Se disponi delle autorizzazioni di gestione per l’area di lavoro a cui appartengono i campi, puoi modificare i campi creati o quelli creati da altri utenti.
* È possibile modificare un campo nella tabella del tipo di record.
* Non è possibile modificare un campo nella pagina record o in un&#39;altra visualizzazione, all&#39;esterno della visualizzazione tabella.
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

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aggiorna le informazioni sul campo e fai clic su **Salva**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Non è possibile aggiornare il tipo di campo dopo il salvataggio del campo.
   >
   >* Quando si modificano le configurazioni dei campi (opzioni di campo o espressioni di formula), i record che contengono già informazioni nei campi modificati aggiorneranno i propri valori in tempo reale. Non viene visualizzato alcun avviso né registro di controllo per le modifiche al valore attivate dalle modifiche alla configurazione del campo. Tutti gli utenti che visualizzano i campi visualizzeranno immediatamente i nuovi valori con le modifiche.

   Le informazioni sul campo vengono aggiornate per tutti gli utenti con accesso alla visualizzazione dell&#39;area di lavoro.

1. (Condizionale) Per i campi record collegati, fare clic su **Modifica campi di ricerca** e aggiungere o rimuovere i campi dal tipo di record collegato.

   Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

