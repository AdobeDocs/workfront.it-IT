---
title: Gestire la pagina record
description: In Adobe Workfront Planning è possibile modificare il layout della casella record e della pagina.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d3778d52f9a3afa12a7bdf348f7400693f8f7ab
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gestire la pagina record

{{maestro-important-intro}}

In Adobe Workfront Planning è possibile modificare il layout della casella record e della pagina. È possibile visualizzare la casella record in una visualizzazione record.

La casella record è una visualizzazione ridotta della pagina record visualizzata nella visualizzazione di un tipo di record.

Quando si modifica il layout di una casella record e di una pagina, la casella e la pagina vengono modificate per tutti i record dello stesso tipo.

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
<p>La tua organizzazione deve essere iscritta al programma beta di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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

* La ridisposizione dei campi nella casella record o nella pagina comporta la ridisposizione dei campi per tutti i record di quel tipo e per tutti gli utenti che accedono a tali record.
* L&#39;aggiunta di un&#39;immagine di copertina a un record non fa parte del layout complessivo della casella di record o della pagina. È possibile aggiungere immagini di copertina univoche a ogni record.

## Ridisposizione dei campi nella casella record o nella pagina

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome di un record.

   La casella del record viene visualizzata nella vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >È possibile visualizzare **Apri dettagli** a sinistra del campo Nome di un record in una visualizzazione tabella solo quando il campo Nome è un campo primario.

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro della casella record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nella casella di record o nella pagina fare clic sull&#39;icona di cattura ![](assets/grab-icon.png) a sinistra del nome di un campo, quindi trascinarlo e rilasciarlo nella posizione desiderata.

   La nuova posizione del campo viene aggiornata sia nella casella che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate al layout della casella di record o della pagina vengono salvate automaticamente.


## Aggiungere un&#39;immagine di copertina alla casella record o alla pagina

È possibile personalizzare un record aggiungendo un&#39;immagine di copertina nella parte superiore della casella del record o della pagina.

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome di un record.

   La casella del record viene visualizzata nella vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >È possibile visualizzare **Apri dettagli** a sinistra del campo Nome di un record in una visualizzazione tabella solo quando il campo Nome è un campo primario.

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro della casella record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nella casella o nella pagina del record fare clic su **Aggiungi copertina**. <!--check the casing here; I logged a bug for this-->
Il **Registra copertina** viene visualizzata la casella.

1. Clic **Seleziona per caricare** e cercare un&#39;immagine nel computer per selezionarla, aggiungerla, quindi fare clic su **Usa immagine**.

   L’immagine viene caricata nella parte superiore della casella o della pagina di record e le modifiche vengono salvate automaticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Facoltativo) Passa il puntatore sull&#39;immagine, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell&#39;angolo inferiore destro dell&#39;immagine di copertina, quindi eseguire una delle operazioni seguenti:

   * Clic **Carica** se si desidera sostituire l&#39;immagine di copertina e ripetere il passaggio 6 per caricare e salvare una nuova immagine.
   * Clic **Riposiziona**, e utilizzare il **Riposiziona** strumento ![](assets/reposition-tool-icon.png) per centrare l&#39;immagine di copertina, quindi fare clic su **Salva** al termine.
   * Clic **Rimuovi** per rimuovere l&#39;immagine di copertina

   Tutte le modifiche hanno effetto immediato.

