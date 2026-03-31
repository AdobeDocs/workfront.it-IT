---
title: Gestire la vista a elenco in Adobe Workfront Planning
description: In Adobe Workfront Planning è possibile visualizzare gli oggetti e i relativi campi in una vista a elenco quando si accede a tali oggetti nella pagina Record collegati di un record. Questo articolo descrive come creare o modificare una visualizzazione elenco nella pagina Record collegati di un record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: ddf10844646a79c43accaffa1789caf24290cc8a
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---


# Gestire la vista elenco in Adobe Workfront Planning

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile visualizzare gli oggetti nella vista a elenco nelle seguenti aree di Workfront Planning:

* Pagina record connessi per i progetti nell&#39;area dei dettagli di un record

  ![Progetti nella pagina dei record connessi nella vista a elenco](assets/projects-on-connected-records-page-list-view.png)

* Elenco di moduli di richiesta a livello di tipo di record

  ![Moduli di richiesta nella vista a elenco](assets/request-forms-in-list-view.png)

In questo articolo viene descritto come spostarsi, creare o modificare una vista elenco che visualizza gli oggetti in Workfront Planning. <!--change 'projects' to other objects when they become available and the location of the list view-->

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
<p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p> Standard per creare ed eliminare viste</p>
   <p>Collaboratore o versione successiva per aggiornare gli elementi di visualizzazione</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Autorizzazioni di visualizzazione a una visualizzazione per modificare temporaneamente le impostazioni di visualizzazione o per duplicarla</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Considerazioni sulle visualizzazioni elenco

* Considerare quanto segue per la visualizzazione elenco delle pagine dei record connessi:

   * È possibile visualizzare i progetti solo nella vista a elenco della pagina record connessi di un record. La visualizzazione elenco non è disponibile per altri tipi di oggetto o record in una pagina di record connessi.

  Per informazioni sulla creazione di una pagina di record connessi, vedere [Aggiungere una pagina di record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
   * Prima di poter visualizzare una vista elenco in una pagina di record connessi di un record, è necessario collegare i progetti Workfront con i tipi di record di Planning. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
   * È possibile creare più visualizzazioni elenco per i progetti nella pagina record connessi di un record.

* Considera quanto segue per la visualizzazione elenco dei moduli di richiesta:

   * Non è possibile creare o modificare visualizzazioni elenco aggiuntive per i moduli di richiesta di Planning. Workfront crea una vista elenco per i moduli di richiesta. <!--this will change-->

     Per informazioni sui moduli di richiesta, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* A seconda della posizione in cui viene visualizzata, non tutte le visualizzazioni elenco presentano gli stessi elementi descritti in questo articolo.


## Gestire una vista a elenco {#manage-a-list-view}

Le visualizzazioni elenco sono simili agli elenchi avanzati. La maggior parte degli elementi delle viste avanzate è disponibile anche nelle viste elenco in Workfront Planning.

Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Passare a una visualizzazione elenco in una delle aree seguenti:

   * Pagina Record collegati nell&#39;area dei dettagli di un record
   * Pagina Moduli di richiesta di un record

1. (Condizionale) Se disponibile, effettuare una delle seguenti operazioni per modificare la vista a elenco:

   1. Espandere il menu delle viste a discesa nell&#39;angolo superiore sinistro dell&#39;elenco per selezionare un&#39;altra vista oppure fare clic su **Nuova vista** e crearne un&#39;altra.

      Le visualizzazioni sono condivise in tutto il sistema. Se si crea una visualizzazione Progetti per un tipo di record, è possibile visualizzarla su altri tipi di record che visualizzano progetti collegati.

   1. Passa il puntatore del mouse sul nome di una visualizzazione esistente e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:
      * **Rinomina**, per assegnare un nuovo nome alla visualizzazione
      * **Condividi**, per condividere la visualizzazione con altri
      * **Elimina**, per eliminare la visualizzazione.

      >[!NOTE]
      >
      >* Per poter modificare, condividere o eliminare una visualizzazione, è necessario disporre delle autorizzazioni di gestione.
      >
      >* Non è possibile modificare le visualizzazioni di sistema.
      >
      >* <span class="preview">È possibile reimpostare una visualizzazione condivisa con l&#39;utente che dispone solo delle autorizzazioni di visualizzazione, dopo averla modificata per ripristinarne le preferenze originali, oppure è possibile copiarla con le modifiche e condividere la copia. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

      <!--
        And hide everything else below for these elements, after moving it to the Use enhanced lists article: 
        1. <span class="preview">To update one of the following view elements, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md):</span>
            <div class="preview">
            * Filter
            * Columns
            * Format cells
            * Row height
            </div>
        -->

   1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) per aggiungere un filtro alla visualizzazione. I risultati vengono filtrati immediatamente nell’elenco. Non è possibile salvare e denominare i filtri. I filtri vengono ricordati quando accedi alla pagina in futuro e fanno parte di visualizzazioni condivise.
   1. Fai clic sull&#39;icona **Colonne** ![Icona Colonne](assets/columns-icon.png) per selezionare le colonne da visualizzare o da nascondere nella visualizzazione.
   1. Passa il puntatore del mouse sul nome di una colonna, fai clic sulla freccia rivolta verso il basso a sinistra del nome della colonna, quindi fai clic su una delle seguenti opzioni:
      * **Rinomina**, per aggiungere una **etichetta personalizzata** per la colonna. Il nome del campo originale in Workfront non cambia.
      * **Ordina**, per ordinare l&#39;elenco in base al campo selezionato. All’intestazione della colonna viene aggiunta un’icona di ordinamento che indica la direzione dell’ordinamento.
   1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro dell&#39;elenco per aggiungere o rimuovere colonne dall&#39;elenco, quindi fai clic su **Salva**.

      Verrà aperto **Gestione colonne**.

      È possibile aggiungere solo campi esistenti alla visualizzazione elenco.
Non è possibile rimuovere il campo principale nella vista a elenco visualizzato nella prima colonna.

   1. <span class="preview">Fare clic sull&#39;icona **Formatta celle** ![Formatta celle](assets/format-cells-icon.png). Viene visualizzata la casella **Formato**.</span> <!--change the name of the box when they update it-->
      <span class="preview">Effettuare le seguenti operazioni: </span>

      1. Fai clic su **Aggiungi condizione**.
      1. <span class="preview">Nella riga **If**, selezionare un campo, scegliere un valore di campo e aggiungere un modificatore. I modificatori cambiano a seconda del tipo di campo scelto. </span>

         >[!TIP]
         >
         ><span class="preview">Per la formattazione condizionale sono disponibili solo i campi visibili nella visualizzazione elenco.</span>

      1. <span class="preview">(Facoltativo) Anziché aggiungere un valore di campo, fare clic sull&#39;icona **Confronta con un altro campo** ![Confronta con un altro campo](assets/compare-to-another-field-icon.png) e scegliere un campo di cui si desidera confrontare il valore con il valore del campo selezionato. Ad esempio, puoi filtrare i progetti il cui Proprietario progetto corrisponde allo Sponsor del progetto. </span>

         >[!TIP]
         >
         ><span class="preview">Per la formattazione condizionale sono disponibili solo i campi visibili nella visualizzazione elenco.</span>

      1. <span class="preview">(Facoltativo) Fare clic su **Aggiungi condizione** nella riga **If** per aggiungere altre condizioni alla stessa regola.</span>

         >[!TIP]
         >
         ><span class="preview">È possibile aggiungere fino a 10 condizioni in una regola di condizionamento e disporre di un massimo di 20 regole per un campo.</span>

      <div class="preview">

      1. Fare clic sul connettore **Or** tra le condizioni per passare a **And** e indicare che è necessario soddisfare più condizioni contemporaneamente. **Or** è il connettore predefinito.
      1. Nella riga **Formato** selezionare un campo per indicare la colonna da formattare. <!--edit this area, if it changes names??-->
      1. (Facoltativo) Fai clic sull&#39;icona **cerchio colore** ![icona cerchio colore](assets/color-circle.png) accanto al campo selezionato, per espanderlo e scegliere un altro colore <!--for a cell or the text of the cell that matches your criteria-->. <!--is this where the bold, italic is? I had no UI for this when I wrote it-->
      1. Attivare l&#39;impostazione **Applica a riga** per applicare la formattazione all&#39;intera riga del campo che soddisfa le condizioni.
      1. (Facoltativo) Fai clic su **Aggiungi condizione** nella casella **Formato** per aggiungere un&#39;altra regola per un altro campo e ripetere i passaggi precedenti.
      1. (Facoltativo) Fai clic su **Cancella tutto** per rimuovere tutta la formattazione.
      1. Fare clic all&#39;esterno della casella **Formato** per chiuderla.

         In questo modo si ritorna alla vista elenco.
La formattazione viene applicata immediatamente alla visualizzazione elenco.
Accanto all&#39;icona **Formatta celle** è presente un punto blu per indicare che alla visualizzazione è applicata una formattazione speciale.

      </div>

   <!--leave these here-->

1. (Facoltativo) Aggiungi una parola chiave nella casella di ricerca nell’angolo superiore destro dell’elenco per cercare un elemento.

   Gli elementi che corrispondono al termine di ricerca sono evidenziati nell&#39;elenco.

1. (Facoltativo) Per aggiungere altri elementi all&#39;elenco e collegarli automaticamente al record selezionato, eseguire una delle operazioni seguenti:

   * Fai clic su **Connetti record** nell&#39;angolo superiore destro dell&#39;elenco per aggiungere elementi esistenti.
   * Fai clic su **Nuova riga** in fondo all&#39;elenco per aggiungere nuovi elementi.
1. Fare clic sul nome di un elemento collegato nell&#39;elenco per aprirlo in un&#39;altra scheda del browser.
1. Fare doppio clic all&#39;interno di una cella dell&#39;elenco per modificare le informazioni di un campo, quindi premere Invio per salvare le modifiche.

   Alcuni campi sono di sola lettura. Ad esempio, la percentuale di completamento di un progetto è un campo calcolato dal sistema e non è possibile modificarlo manualmente.

1. Passa il puntatore del mouse sul nome di un elemento nell&#39;elenco e fai clic sul menu **Altro** [Altro menu](assets/more-menu.png) e fai clic su **Visualizza** per aprire il progetto in un&#39;altra scheda

   Oppure

   Seleziona uno o più elementi e osserva la barra delle azioni nella parte inferiore dell’elenco, quindi fai clic su uno dei seguenti, se disponibile:

   * **Elimina** per eliminare l&#39;elemento. Quando si elimina un progetto, questo viene disconnesso dal record e spostato nel Cestino di Workfront. Gli amministratori di Workfront possono recuperare i progetti eliminati fino a 30 giorni dopo la loro eliminazione. L’eliminazione di un modulo non comporta l’eliminazione delle richieste o dei record creati al momento dell’invio del modulo.
   * **Disconnetti** per disconnettere il progetto dal record. Se si disconnette un progetto, verranno rimossi anche tutti i valori dei campi di ricerca dal record corrente.

   ![Barra delle azioni nella visualizzazione Elenco della pagina Record connessi](assets/actions-bar-connected-records-page-list-view.png)

