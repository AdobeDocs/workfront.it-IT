---
title: Gestire la pagina record
description: È possibile modificare il layout dell'anteprima record e della pagina in Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gestire la pagina record

{{planning-important-intro}}

È possibile modificare il layout dell&#39;anteprima record e della pagina in Adobe Workfront Planning.

L&#39;anteprima del record è una visualizzazione ridotta della pagina del record visualizzata nella visualizzazione di un tipo di record.

Quando si modifica il layout di un&#39;anteprima record e di una pagina, le modifiche hanno effetto sulle caselle di anteprima e sulle pagine dei dettagli di tutti i record dello stesso tipo.

In questo articolo viene descritto come modificare il layout e l&#39;aspetto di una casella di anteprima del record o di una pagina di record. Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/maestro/records/edit-records.md).

È necessario creare tipi di record e record prima di iniziare a modificare le pagine dei record.

Per informazioni, vedere i seguenti articoli:

* [Crea tipi di record](../architecture/create-record-types.md)

* [Crea record](/help/quicksilver/maestro/records/create-records.md)

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
   <p>Nuovo: Chiaro o superiore</p>
   Oppure
   <p>Corrente: Lavoro o versione successiva</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestione o autorizzazioni superiori per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerazioni sulla modifica delle pagine record

* Per impostazione predefinita, i dettagli e le pagine di anteprima di un record visualizzano tutti i campi associati al record.

* Non è possibile aggiungere nuovi campi per un record nella pagina di anteprima o dei dettagli. Per visualizzarli nelle pagine di anteprima e dettagli, è necessario aggiungere nuovi campi nella vista a tabella.

* È possibile aggiungere sezioni a un&#39;anteprima del record o a una pagina dei dettagli, per organizzare le informazioni in base a criteri comuni e semplificarne la ricerca.

* Le modifiche seguenti hanno effetto su tutti i record dello stesso tipo e sono visibili a tutti gli utenti che accedono a tali record:

   * Ridisposizione dei campi
   * Aggiunta o rimozione di sezioni

* Le modifiche apportate all&#39;anteprima del record sono immediatamente visibili nella pagina dei dettagli del record. Le modifiche apportate nella pagina record sono visibili anche nella casella di anteprima del record.

* L&#39;aggiunta di un&#39;immagine di copertina a un record non fa parte del layout generale dell&#39;anteprima del record o della pagina. È possibile aggiungere immagini di copertina univoche a ogni record. Per informazioni, consulta [Aggiungere una copertina a un record](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## Aggiungere sezioni a una pagina o anteprima record

Quando si aggiungono sezioni a una pagina record, tenere presente quanto segue:

* Non esiste alcun limite al numero di sezioni che è possibile includere in una pagina.
* Impossibile avere una sezione vuota. È necessario disporre di almeno un campo in una sezione.
* È possibile trascinare i campi da una sezione all&#39;altra. Per ulteriori informazioni, consulta la sezione [Ridisponi i campi nella pagina di anteprima record o dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.
* Quando rimuovi tutti i campi da una sezione, questa viene eliminata automaticamente e non può essere recuperata.

Per aggiungere una sezione a un&#39;anteprima record o a una pagina:

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome di un record.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >È possibile visualizzare **Apri dettagli** a sinistra del campo Nome di un record in una visualizzazione tabella solo quando il campo Nome è un campo primario.

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nell&#39;anteprima del record o nella pagina, posiziona il cursore del mouse sullo spazio vuoto a sinistra dei campi, quindi fai clic sul pulsante **Aggiungi sezione** icona ![](assets/add-section-icon.png) per aggiungere una sezione.
1. Fai clic sul nome della sezione e sostituisci **Sezione senza titolo** con un nome, quindi fai clic su Invio. I campi visualizzati sotto la sezione fanno automaticamente parte della nuova sezione.
1. Inizia a trascinare i campi nella nuova sezione, come descritto nella sezione [Ridisponi i campi nella pagina di anteprima record o dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.

1. (Facoltativo) Passa il puntatore del mouse sul nome di una sezione e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Facoltativo) Per modificare la sezione, effettuate una delle seguenti operazioni:

   * Clic **Rinomina** per rinominare la sezione

     >[!TIP]
     >
     > È possibile rinominare una sezione in linea facendo clic sul nome.

   * Clic **Sposta su** per spostare la sezione in alto di una posizione

     Oppure

     Clic **Sposta in basso** per spostare la sezione verso il basso di una posizione.
Tutti i campi della sezione vengono spostati insieme alla sezione.

   * Clic **Elimina** per eliminare la sezione. La sezione viene eliminata e non può essere recuperata. Tutti gli utenti che accedono ai record di questo tipo non visualizzeranno più la sezione eliminata.

1. Fare clic sulla freccia rivolta verso il basso a sinistra del nome di una sezione per comprimerla oppure sulla freccia rivolta verso destra per espanderla.
Per impostazione predefinita, tutte le sezioni vengono espanse.

1. (Facoltativo) Fai clic su **afferrare** icona ![](assets/grab-icon.png) a sinistra del nome di una sezione, quindi trascinarlo e rilasciarlo nella posizione desiderata.

   La nuova posizione della sezione viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate alle sezioni e all&#39;ordine dei campi vengono salvate automaticamente.

## Ridisponi i campi nella pagina di anteprima record o dettagli

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome di un record.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >È possibile visualizzare **Apri dettagli** a sinistra del campo Nome di un record in una visualizzazione tabella solo quando il campo Nome è un campo primario.

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nell&#39;anteprima del record o nella pagina, fare clic su **afferrare** icona ![](assets/grab-icon.png) a sinistra del nome di un campo, quindi trascinarlo e rilasciarlo nella posizione desiderata. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   La nuova posizione del campo viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate al layout dell&#39;anteprima record o del salvataggio automatico della pagina.

