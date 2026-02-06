---
title: Gestire la vista a elenco in Adobe Workfront Planning
description: In Adobe Workfront Planning è possibile visualizzare gli oggetti e i relativi campi in una vista a elenco quando si accede a tali oggetti nella pagina Record collegati di un record. Questo articolo descrive come creare o modificare una visualizzazione elenco nella pagina Record collegati di un record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---


# Gestire la vista elenco in Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning è possibile visualizzare gli oggetti e i relativi campi in una vista a elenco quando si accede a tali oggetti nella pagina Record collegati di un record.

In questo articolo viene descritto come creare o modificare una visualizzazione elenco nella pagina Record collegati di un record e come modificare gli oggetti nella visualizzazione.

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
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p> Standard per creare ed eliminare viste</p>
   <p>Collaboratore o versione successiva per aggiornare gli elementi di visualizzazione</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
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

* Non è possibile visualizzare i record nelle pagine dei tipi di record in una visualizzazione elenco. È possibile visualizzare i seguenti oggetti in una vista a elenco solo quando vengono visualizzati nella pagina Record collegati di un record:

   * Progetti Workfront

  Per informazioni sulla creazione di una pagina di record connessi, vedere [Aggiungere una pagina di record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Prima di poter visualizzare una vista elenco in una pagina di record connessi di un record, è necessario collegare i progetti Workfront con i tipi di record di Planning. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* Le visualizzazioni elenco sono simili agli elenchi Avanzati. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Gestire una vista a elenco {#manage-a-list-view}

Per ulteriori informazioni sulla gestione delle visualizzazioni elenco in Workfront, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Fai clic su una scheda dell’area di lavoro, quindi fai clic su una scheda del tipo di record.
1. Da qualsiasi visualizzazione, fare clic sul nome di un record per aprire la pagina di anteprima o i dettagli del record.
1. Aggiungere una **pagina Record connessi** per i progetti connessi come descritto nell&#39;articolo [Aggiungere una pagina Record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   Nella pagina Record collegati vengono visualizzati i progetti connessi al record nella vista a elenco.

   ![Progetti nella pagina dei record connessi nella vista a elenco](assets/projects-on-connected-records-page-list-view.png)

1. (Facoltativo) Per modificare la vista a elenco, effettuate una delle seguenti operazioni:

   1. Espandere il menu delle viste a discesa nell&#39;angolo superiore destro dell&#39;elenco per selezionare un&#39;altra vista oppure fare clic su **Nuova vista** e crearne un&#39;altra.

      Le visualizzazioni sono condivise in tutto il sistema. Se si crea una visualizzazione Progetti per un tipo di record, è possibile visualizzarla su altri tipi di record che visualizzano progetti collegati.

   1. Passa il puntatore del mouse sul nome di una visualizzazione esistente e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:
      * **Rinomina**, per assegnare un nuovo nome alla visualizzazione
      * **Condividi**, per condividere la visualizzazione con altri
      * **Elimina**, per eliminare la visualizzazione.

      >[!NOTE]
      >
      >Per poter modificare, condividere o eliminare una visualizzazione, è necessario disporre delle autorizzazioni di gestione.
      >
      >Non è possibile modificare le visualizzazioni di sistema.
      >
   1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) per aggiungere un filtro alla visualizzazione. I risultati vengono filtrati immediatamente nell’elenco. Non è possibile salvare e denominare i filtri. I filtri vengono ricordati quando accedi alla pagina in futuro e fanno parte di visualizzazioni condivise.
   1. Fai clic sull&#39;icona **Colonne** ![Icona Colonne](assets/columns-icon.png) per selezionare le colonne da visualizzare o da nascondere nella visualizzazione.
   1. Passa il puntatore del mouse sul nome di una colonna, fai clic sulla freccia rivolta verso il basso a sinistra del nome della colonna, quindi fai clic su una delle seguenti opzioni:
      * **Rinomina**, per aggiungere una **etichetta personalizzata** per la colonna. Il nome del campo originale in Workfront non cambia.
      * **Ordina**, per ordinare l&#39;elenco in base al campo selezionato. All’intestazione della colonna viene aggiunta un’icona di ordinamento che indica la direzione dell’ordinamento.
   1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro dell&#39;elenco per aggiungere o rimuovere colonne dall&#39;elenco, quindi fai clic su **Salva**.

      Verrà aperto **Gestione colonne**.

      È possibile aggiungere solo campi esistenti alla visualizzazione elenco.
Non è possibile rimuovere il campo principale nella vista a elenco visualizzato nella prima colonna.
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

   Seleziona uno o più elementi e osserva la barra delle azioni nella parte inferiore dell’elenco, quindi fai clic su una delle seguenti opzioni:

   * **Elimina** per eliminare il progetto. Quando si elimina un progetto, questo viene disconnesso dal record e spostato nel Cestino di Workfront. Gli amministratori di Workfront possono recuperare i progetti eliminati fino a 30 giorni dopo la loro eliminazione.
   * **Disconnetti** per disconnettere il progetto dal record. Se si disconnette un progetto, verranno rimossi anche tutti i valori dei campi di ricerca dal record corrente.

   ![Barra delle azioni nella visualizzazione Elenco della pagina Record connessi](assets/actions-bar-connected-records-page-list-view.png)

