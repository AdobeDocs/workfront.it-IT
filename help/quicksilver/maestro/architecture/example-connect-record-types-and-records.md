---
title: Esempio di connessione di tipi di record e record
description: In questo articolo viene descritto un esempio di come creare una connessione tra un tipo di record Adobe Workfront Planning e un tipo di oggetto progetto Workfront. Descrive inoltre come collegare un record di Workfront Planning a un singolo progetto.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: 9b1b8d8661917946230033b661ca652f5edef734
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 0%

---

# Esempio di connessione di tipi di record e record

{{maestro-important-intro}}

Questo articolo descrive un esempio di quanto segue:

* Come creare una connessione tra due tipi di record di Workfront Planning e due record.

* Come creare una connessione tra un tipo di record di Workfront Planning e un tipo di oggetto progetto di Workfront, nonché una connessione tra un record e un progetto.

Per ulteriori informazioni, consulta anche i seguenti articoli:

* [Connetti tipi di record](../architecture/connect-record-types.md)
* [Connetti record](../records/connect-records.md)

## Collegare due tipi di record e record di Workfront Planning (esempio)

Ad esempio, il tipo di record originale è Campaign.

È inoltre disponibile un altro tipo di record denominato Prodotto, che dispone di un campo valuta denominato Budget.

Desideri creare un campo sul tipo di record Campaign in cui visualizzare i valori del campo Budget del tipo di record Prodotto.

Per eseguire questa operazione:

1. Apri la vista a tabella per il tipo di record Campaign in un’area di lavoro.
1. Fai clic su **+** nell’angolo superiore destro della vista tabella per aggiungere un nuovo campo, quindi fai clic su **Nuova connessione**, quindi fai clic su **Prodotto** nella sezione workspace selezionata.
1. Aggiungi le seguenti informazioni, ad esempio:

   * **Tipo di record**: prodotto <!--did they change the casing here?-->
   * **Nome**: assegna un nome al nuovo campo. Ad esempio, &quot;Informazioni sul prodotto&quot;. Questo è il nome del campo record collegato.
   * **Descrizione**: aggiungi una descrizione per il nuovo campo. Ad esempio, &quot;Questi sono i prodotti a cui voglio associare le mie campagne&quot;. La descrizione del campo viene visualizzata quando si passa il cursore sul campo nell’intestazione della colonna.
   * **Consenti più record**: se lasci selezionata questa opzione, gli utenti potranno selezionare più record quando il campo del tipo di record collegato (informazioni sul prodotto) viene visualizzato nei record originali (campagne). Nel nostro caso, gli utenti possono selezionare più prodotti da collegare a una campagna.
   * **Seleziona campi di ricerca**: se lasci selezionata questa opzione, il **Aggiungi campi di ricerca** Viene visualizzata la casella accanto, per consentire di collegare i campi Prodotto con il tipo di record Campaign. Puoi fare clic su **Ignora** per saltare questo passaggio e aggiungere i campi Prodotto in un secondo momento.

   ![](assets/new-connection-with-product-record-type.png)

1. (Condizionale) Se hai selezionato il **Opzione Seleziona campi di ricerca** nel passaggio precedente, dall’elenco di campi associati al **Prodotto** tipo di record, fare clic sul pulsante **+** icona per **Budget** , quindi fai clic su **Aggiungi campi**. Questo crea un campo denominato **Budget (da informazioni prodotto)**, che è il nome del campo collegato. In questo campo verranno visualizzate tutte le informazioni relative al budget prodotti per i record della campagna.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Se si desidera visualizzare il budget di tutti i prodotti selezionati come un unico numero totale, selezionare **SOMMA** nel menu a discesa a destra del nome del campo. Quando gli utenti selezionano più prodotti nella **Informazioni sul prodotto** campo record collegato, il **Budget (da informazioni prodotto)** aggiunge tutti i valori Budget e visualizza il totale. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Se si seleziona **Nessuno**, invece di **SOMMA**, i singoli budget dei prodotti selezionati verranno visualizzati separati da virgole.

   Vengono generati i campi seguenti:

   * Nella vista Tabella record Campaign e nella pagina Record Campaign di una campagna:

      * **Informazioni sul prodotto** (campo record collegato): quando vengono aggiunti, vengono visualizzati il nome o i nomi dei prodotti.
      * **Budget (da informazioni prodotto)** (campo collegato): vengono visualizzati i budget dei prodotti selezionati nel campo Informazioni prodotto.

   * Nella visualizzazione Tabella record Prodotto e nella pagina Record prodotto di un prodotto:

      * **Campagna**: indica che il tipo di record Prodotto è collegato dal tipo di record Campagna.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    I campi record collegati sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

1. Dalla sezione **Campagna** nella vista tabella del tipo di record, crea una campagna aggiungendo una nuova riga nella tabella della pagina del tipo di record Campaign.

1. Fai doppio clic all’interno del  **Informazioni sul prodotto** della nuova campagna.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Esegui una delle operazioni seguenti:

   * Fare clic sul nome di un prodotto connesso dall&#39;elenco per aggiungerlo al record selezionato. Il prodotto viene aggiunto automaticamente.
   * Inizia a digitare il nome di un prodotto e fai clic su di esso quando viene visualizzato nell’elenco. Il prodotto viene aggiunto automaticamente.
   * Clic **Vedi tutto** per visualizzare tutti i prodotti.

1. (Condizionale) Se hai fatto clic **Vedi tutto** nel passaggio precedente, il **Connetti oggetti** viene visualizzata la casella.

   ![](assets/connected-objects-table-for-records.png)

1. Inizia a digitare il nome di un prodotto nella casella di ricerca, quindi selezionalo quando viene visualizzato nell’elenco

   Oppure

   Seleziona i record Prodotto che desideri collegare ai record Campaign, quindi fai clic su **Connetti oggetti**.

   >[!TIP]
   >
   >    Puoi aprire la pagina record di una campagna, trovare il campo record collegato e fare clic su **+** nel campo per aggiungere prodotti dal tipo di record Prodotto connesso.

   Nella tabella dei tipi di record di Campaign sono inserite le colonne seguenti:
   * Il **Informazioni sul prodotto** viene compilato il campo relativo al record Campagna con i Prodotti selezionati.
   * **Budget (da informazioni prodotto)** viene compilato con il valore Budget per ciascun prodotto selezionato o con un totale di tutti i budget dei prodotti selezionati (se è stato selezionato SOMMA per l&#39;aggregatore).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Se non si seleziona un aggregatore per i valori multipli, tutti i valori dei prodotti selezionati vengono visualizzati separati da virgole.

1. Per popolare il **Campagna** campo da **Prodotto** vista tabella, ripetere i passaggi 5-7 a partire dalla vista tabella Tipo di record prodotto e selezionando le informazioni sulla campagna. Verrà aggiornato anche il campo Informazioni prodotto nella tabella della pagina Tipo di record campagna. <!--ensure the step numbers remain correct-->


## Collegare un tipo di record Workfront Planning a un tipo di oggetto progetto Workfront e collegare un record a singoli progetti

>[!IMPORTANT]
>
>    Tutti coloro che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro possono visualizzare le informazioni nei campi collegati, indipendentemente dalle autorizzazioni o dal livello di accesso in Workfront.

Ad esempio, il tipo di record originale è Campaign.

In Workfront sono presenti anche progetti con un campo denominato &quot;Reddito pianificato&quot;.

Si desidera creare un campo connessione nel tipo di record Campaign in cui è possibile visualizzare i valori del campo Retribuzione pianificata dei progetti in Workfront connessi alle campagne in Workfront Planning.

Per eseguire questa operazione:

1. Vai a un’area di lavoro in cui desideri collegare il tipo di record Campaign ai progetti Workfront.
1. Apri la vista a tabella per il tipo di record Campaign nell’area di lavoro selezionata.
1. Fai clic su **+** nell’angolo superiore destro della vista tabella per aggiungere un nuovo campo, quindi fai clic su **Nuova connessione**, quindi fai clic su **Progetto** nel **Tipi di oggetto Workfront** sezione.
1. Aggiungi le seguenti informazioni, ad esempio:

   * **Tipo di record**: progetto (dalla sottosezione Workfront)
   * **Nome**: assegna un nome al nuovo campo, ad esempio &quot;Informazioni sul progetto&quot;.
   * **Descrizione**: aggiungi una descrizione per il nuovo campo. Ad esempio, &quot;Questi sono i progetti a cui voglio associare le mie campagne&quot;. La descrizione viene visualizzata nella vista tabella quando passi il cursore del mouse sul nome del campo nell’intestazione della colonna.
   * 
      * **Consenti più record**: se questa opzione viene lasciata selezionata, gli utenti possono selezionare più progetti quando il campo del tipo di progetto collegato (informazioni sul progetto) viene visualizzato nei record originali (Campagne).
   * **Seleziona campi di ricerca**: se lasci selezionata questa opzione, il **Aggiungi campi di ricerca** viene visualizzata la casella accanto, che consente di collegare i campi di Project con il tipo di record Campaign. Puoi fare clic su **Ignora** per saltare questo passaggio e aggiungere i campi Progetto in un secondo momento.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Condizionale) Se hai selezionato il **Opzione Seleziona campi di ricerca** nel passaggio precedente, dall’elenco di campi associati al **Progetto** tipo di oggetto, fare clic sul pulsante **+** icona per **Reddito Pianificato** , quindi fai clic su **Aggiungi campi**. Questo crea un campo denominato **Retribuzione pianificata (da informazioni progetto)**, che è il nome del campo collegato. Tutte le informazioni contenute nel campo Retribuzione pianificata progetto verranno visualizzate automaticamente in questo campo per i record della campagna.

   >[!TIP]
   >
   >    Se desideri visualizzare la Retribuzione pianificata di tutti i progetti selezionati come un unico numero totale, seleziona **SOMMA** nel menu a discesa a destra del nome del campo. Quando gli utenti selezionano più progetti nel **Informazioni progetto** campo oggetto collegato, il **Reddito Pianificato (da informazioni prodotto)** Il campo aggiunge tutti i valori e visualizza il totale. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Se si seleziona **Nessuno**, invece di **SOMMA**, i singoli Ricavi pianificati vengono visualizzati separati da virgole.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Vengono generati i campi seguenti:

   * Nella vista Tabella record Campaign e nella pagina Record Campaign:

      * **Informazioni progetto** (campo oggetto collegato): verranno visualizzati il nome o i nomi dei progetti.
      * **Retribuzione pianificata (da informazioni progetto)** (campo collegato): visualizza le Retribuzioni pianificate dei progetti selezionati nel campo Informazioni progetto.

   >[!TIP]
   >
   >    I campi oggetto collegato sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

1. Dalla sezione **Campagna** tipo di record vista tabella, crea una campagna aggiungendo una nuova riga nella tabella.

1. Fai doppio clic all’interno del  **Informazioni progetto** della nuova campagna.

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Esegui una delle operazioni seguenti:

   * Fare clic sul nome di un progetto nell&#39;elenco per aggiungerlo al record selezionato. Il progetto viene aggiunto automaticamente.
   * Inizia a digitare il nome di un progetto e fai clic su di esso quando viene visualizzato nell’elenco. Il progetto viene aggiunto automaticamente.
   * Clic **Vedi tutto** per visualizzare tutti i progetti.

1. (Condizionale) Se hai fatto clic **Vedi tutto** nel passaggio precedente, il **Connetti oggetti** viene visualizzata la casella.

   ![](assets/connect-projects-larger-box.png)

1. Inizia a digitare il nome di un progetto nella casella di ricerca, quindi selezionalo quando viene visualizzato nell’elenco

   Oppure

   Seleziona i record di Project che desideri connettere ai record di Campaign, quindi fai clic su **Connetti oggetti**.

   >[!TIP]
   >
   >    Puoi aprire la pagina di una campagna, trovare il campo del progetto collegato e fare clic su **+** nel campo per aggiungere progetti dal tipo di record Prodotto connesso.

   Questa operazione aggiunge quanto segue all&#39;area di lavoro selezionata:

   * Nella tabella del tipo di record di Campaign:
      * Il **Informazioni progetto** Il campo viene compilato per il record Campaign con i progetti selezionati.
      * Il **Reddito Pianificato (da informazioni prodotto)** viene compilato con il valore Budget per ciascun Prodotto selezionato. Questo campo è di sola lettura.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Se non si seleziona un aggregatore per i valori multipli e si selezionano più oggetti nel campo collegato a oggetti, tutti i valori vengono visualizzati separati da virgole.

1. Fare clic sul nome di un progetto nel campo record connesso.

   Verrà aperta la pagina del progetto di sola lettura Woekfront Planning.
Rivedi le informazioni sul progetto. Nella pagina del record vengono visualizzati solo i campi progetto selezionati.

1. Clic **Vai all&#39;origine** nell’angolo in alto a destra dello schermo per aprire il progetto in Workfront, se disponi almeno delle autorizzazioni di visualizzazione per il progetto.
1. (Facoltativo) Se disponi delle autorizzazioni necessarie, aggiorna le informazioni sul progetto in Workfront.

1. (Facoltativo) Dalla vista della tabella Campaign, passa il puntatore del mouse su **Informazioni progetto** e fare clic sulla freccia rivolta verso il basso, quindi su **Modificare i campi di ricerca.**
1. Fai clic su **+** per i campi del progetto che si desidera aggiungere al record Workfront Planning del progetto in **Campi non selezionati** sezione.
1. Fai clic su **-** per i campi del progetto che si desidera rimuovere dal record Workfront Project Planning nel **Campi selezionati** sezione.
1. Fai clic su **Salva**.

   Campi collegati aggiuntivi vengono aggiunti al tipo di record Campaign.
