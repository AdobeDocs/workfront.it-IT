---
title: Record duplicati
description: È possibile duplicare un record esistente nella vista tabella. Alla pagina del tipo di record viene aggiunta una copia identica del record esistente.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---


# Record duplicati

<!--update the metadata after GA-->

{{planning-important-intro}}

In Adobe Workfront Planning, un record è un&#39;istanza di un tipo di record.

È possibile duplicare un record esistente nella vista tabella. Alla pagina del tipo di record viene aggiunta una copia identica del record esistente.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

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
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Autorizzazioni Contribute o superiori per un'area di lavoro</a> </p>  
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

*Per ulteriori informazioni, vedere [Requisiti di accesso per la documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Duplica un record <!--in a record type table (I don't think you can create them elsewhere right now)-->

È possibile creare record nella vista tabella di una pagina del tipo di record duplicandone uno esistente. Un record identico a quello esistente viene creato e aggiunto al record originale.


{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.
Tutti i record del tipo selezionato vengono visualizzati nella vista.

1. (Condizionale) Seleziona una vista tabella.

1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sul nome di un record, quindi fai clic sul menu **Altro** in linea con il nome del record, quindi fai clic sull&#39;icona **Duplica** ![](assets/duplicate-icon-gray.png).

     ![](assets/more-menu-from-record-in-table-view.png)

   * Seleziona un record, quindi fai clic sull&#39;icona ![](assets/duplicate-icon-white-and-blue.png) **Duplica** nella barra degli strumenti nella parte inferiore della pagina.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Sotto il record originale viene creato un record identico con lo stesso nome. Tutti i campi del nuovo record vengono compilati con le stesse informazioni del record originale.

1. (Facoltativo) Iniziare ad aggiornare le informazioni sul nuovo record nei campi disponibili nella visualizzazione tabella oppure fare clic sul record e aggiornare le informazioni nell&#39;anteprima o nella pagina del record.

   >[!NOTE]
   >
   >  * Non esistono campi obbligatori per i record. È tuttavia consigliabile aggiungere informazioni per il campo principale di un record, in quanto è utile identificare i record quando si collegano tra loro record. Per ulteriori informazioni sui campi primari, vedere [Gestire la visualizzazione tabella](/help/quicksilver/planning/views/manage-the-table-view.md) e [Panoramica campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * I campi che fanno riferimento ad altri tipi di record o campi calcolati sono campi di sola lettura.

   Per ulteriori informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere l&#39;aggiunta di nuovi record o delle relative informazioni quando questi vengono aggiunti nella vista tabella:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripristinare una modifica.