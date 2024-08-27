---
title: Gestire il layout della pagina record
description: È possibile modificare il layout dell'anteprima record e della pagina in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '1356'
ht-degree: 0%

---


# Gestire il layout della pagina record

{{planning-important-intro}}

È possibile modificare il layout dell&#39;anteprima record e della pagina in Adobe Workfront Planning.

L&#39;anteprima del record è una visualizzazione ridotta della pagina del record visualizzata nella visualizzazione di un tipo di record.

Quando si modifica il layout di un&#39;anteprima record e di una pagina, le modifiche hanno effetto sulle caselle di anteprima e sulle pagine dei dettagli di tutti i record dello stesso tipo.

In questo articolo viene descritto come modificare il layout e l&#39;aspetto di una casella di anteprima del record o di una pagina di record. Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

È necessario creare tipi di record e record prima di iniziare a modificare le pagine dei record.

Per informazioni, vedere i seguenti articoli:

* [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)

* [Crea record](/help/quicksilver/planning/records/create-records.md)

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

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
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td>
   <td>
<p>Qualsiasi</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni piano di Workfront Planning, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Determinazione prezzi e packaging di Adobe Workfront</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale e l'area Planning per i progetti, i portfolio e i programmi. </p> Per ulteriori informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla modifica delle pagine record

* Per impostazione predefinita, i dettagli e le pagine di anteprima di un record visualizzano tutti i campi associati al record.

* Non è possibile aggiungere nuovi campi per un record nella pagina di anteprima o dei dettagli. Per visualizzarli nelle pagine di anteprima e dettagli, è necessario aggiungere nuovi campi nella vista a tabella.

* È possibile aggiungere sezioni a un&#39;anteprima del record o a una pagina dei dettagli, per organizzare le informazioni in base a criteri comuni e semplificarne la ricerca.

* Le modifiche seguenti hanno effetto su tutti i record dello stesso tipo e sono visibili a tutti gli utenti che accedono a tali record:

   * Ridisposizione dei campi
   * Aggiunta o rimozione di sezioni

* Le modifiche apportate all&#39;anteprima del record sono immediatamente visibili nella pagina dei dettagli del record. Le modifiche apportate nella pagina record sono visibili anche nella casella di anteprima del record.

* L&#39;aggiunta di un&#39;immagine di copertina o di una miniatura a un record non fa parte del layout generale dell&#39;anteprima del record o della pagina. È possibile aggiungere immagini di copertina o miniature univoche a ciascun record. Per informazioni, vedere [Aggiungere un&#39;immagine di copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) e [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Aggiungere sezioni a una pagina o anteprima record

Quando si aggiungono sezioni a una pagina record, tenere presente quanto segue:

* Non esiste alcun limite al numero di sezioni che è possibile includere in una pagina.
* Impossibile avere una sezione vuota. È necessario disporre di almeno un campo in una sezione.
* È possibile trascinare i campi da una sezione all&#39;altra. Per ulteriori informazioni, vedere la sezione [Ridisponi campi nell&#39;anteprima record o nella pagina dei dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.
* Quando rimuovi tutti i campi da una sezione, questa viene eliminata automaticamente e non può essere recuperata.

Per aggiungere una sezione a un&#39;anteprima record o a una pagina:

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella fare clic sull&#39;icona ![](assets/open-details-icon-in-table-name-field.png) **Apri dettagli** nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record. Per impostazione predefinita, viene visualizzata la scheda Dettagli (Details).

   ![](assets/details-page.png)

1. Nella scheda **Dettagli** dell&#39;anteprima del record o della pagina, passa il puntatore del mouse sullo spazio vuoto a sinistra dei campi, quindi fai clic sull&#39;icona **Aggiungi sezione** ![](assets/add-section-icon.png) per aggiungere una sezione.
1. Fare clic nel nome della sezione e sostituire **Sezione senza titolo** con un nome, quindi fare clic su Invio. I campi visualizzati sotto la sezione fanno automaticamente parte della nuova sezione.
1. Inizia a trascinare i campi nella nuova sezione, come descritto nella sezione [Ridisponi i campi nell&#39;anteprima del record o nella pagina dei dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.

1. (Facoltativo) Passa il puntatore del mouse sul nome di una sezione e fai clic sul menu **Altro** ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Facoltativo) Per modificare la sezione, effettuate una delle seguenti operazioni:

   * Fai clic su **Rinomina** per rinominare la sezione

     >[!TIP]
     >
     > È possibile rinominare una sezione in linea facendo clic sul nome.

   * Fai clic su **Sposta su** per spostare la sezione in alto di una posizione

     Oppure

     Fare clic su **Sposta in basso** per spostare la sezione in basso di una posizione.
Tutti i campi della sezione vengono spostati insieme alla sezione.

   * Fai clic su **Elimina** per eliminare la sezione. La sezione viene eliminata e non può essere recuperata. Tutti gli utenti che accedono ai record di questo tipo non visualizzeranno più la sezione eliminata.

1. Fare clic sulla freccia rivolta verso il basso a sinistra del nome di una sezione per comprimerla oppure sulla freccia rivolta verso destra per espanderla.
Per impostazione predefinita, tutte le sezioni vengono espanse.

1. (Facoltativo) Fai clic sull&#39;icona **grab** ![](assets/grab-icon.png) a sinistra del nome di una sezione, quindi trascinala e rilasciala nel punto desiderato.

   La nuova posizione della sezione viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate alle sezioni e all&#39;ordine dei campi vengono salvate automaticamente.

1. (Facoltativo) Fai clic sull&#39;icona **Esporta** ![](assets/export-icon-in-record-details-page.png) per esportare la scheda Dettagli in un file Word. Per ulteriori informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facoltativo) Fai clic sulla scheda **Connessioni** accanto alla scheda **Dettagli**. Potrebbe essere necessario fare clic su **Altro** prima di fare clic sulla scheda **Connessioni**.

   Tutti i record o gli oggetti connessi al record selezionato vengono visualizzati con i nomi del tipo di record o dell&#39;applicazione a cui appartengono.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facoltativo) Selezionare l&#39;impostazione **Mostra tutti i record** nell&#39;angolo superiore destro della scheda Connessioni. Vengono visualizzati tutti i tipi di record connessi, inclusi quelli che non dispongono ancora di record connessi. Per impostazione predefinita, l&#39;interruttore è deselezionato e i tipi di record senza record collegati sono nascosti.

1. (Facoltativo) Fai clic su **Connetti** per aggiungere altri record ai tipi di record connessi. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi di ricerca di Workfront connessi al record Planning.

## Ridisporre i campi nell&#39;anteprima o nella pagina del record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella fare clic sull&#39;icona ![](assets/open-details-icon-in-table-name-field.png) **Apri dettagli** nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nell&#39;anteprima del record o nella pagina, fare clic sull&#39;icona **grab** ![](assets/grab-icon.png) a sinistra del nome di un campo, quindi trascinarla e rilasciarla in un punto desiderato. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   La nuova posizione del campo viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate al layout dell&#39;anteprima record o del salvataggio automatico della pagina.

