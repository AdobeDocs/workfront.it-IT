---
title: Esempio di connessione di tipi di record e record
description: Questo articolo descrive un esempio di come creare una connessione tra un tipo di record Adobe Maestro e un tipo di oggetto progetto Workfront. Descrive anche come collegare un record Maestro con un singolo progetto.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1742'
ht-degree: 0%

---


# Esempio di connessione di tipi di record e record

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Questo articolo descrive un esempio di quanto segue:

* Come creare una connessione tra due tipi di record Maestro e due record Maestro.

* Come creare una connessione tra un tipo di record Maestro Adobe e un tipo di oggetto progetto Workfront, nonché una connessione tra un record Maestro e un progetto.

Per ulteriori informazioni, consulta anche i seguenti articoli:

* [Connetti tipi di record](../architecture-and-fields/connect-record-types.md)
* [Collega record](../records/connect-records.md)

## Collega due tipi di record e record Maestro (esempio)

Ad esempio, il tipo di record originale è Campaign.

È inoltre disponibile un altro tipo di record denominato Prodotto, che dispone di un campo valuta denominato Budget.

Si desidera creare un campo nel tipo di record Campaign in cui è possibile visualizzare i valori del campo Budget nel tipo di record Prodotto.

Per eseguire questa operazione:

1. Aprire la vista tabella per il tipo di record Campaign.
1. Fai clic su **+** nell’angolo superiore destro della vista tabella per aggiungere un nuovo campo, quindi fai clic su **Nuova connessione**.
1. Aggiungi le seguenti informazioni, ad esempio:

   * **Tipo di record**: prodotto <!--did they change the casing here?-->
   * **Nome**: informazioni sul prodotto. Questo è il nome del campo record collegato.
   * **Descrizione**: questi sono i prodotti a cui voglio associare le mie campagne.
   * **Consenti più record**: se lasci selezionata questa opzione, gli utenti potranno selezionare più record quando il campo del tipo di record collegato (informazioni sul prodotto) viene visualizzato nei record originali (campagne). Nel nostro caso, saranno in grado di selezionare più Prodotti da collegare a una sola Campagna.
   * **Seleziona campi di ricerca**: se lasci selezionata questa opzione, il **Aggiungi campi di ricerca** Viene visualizzata la casella accanto, per consentire di collegare i campi Prodotto con il tipo di record Campaign. Puoi saltare questo passaggio e aggiungere i campi Prodotto in un secondo momento.

   ![](assets/new-connection-with-product-record-type.png)

1. (Condizionale) Se hai selezionato il **Opzione Seleziona campi di ricerca** nel passaggio precedente, dall’elenco di campi associati al **Prodotto** tipo di record, fare clic sul pulsante **+** icona per **Budget** , quindi fai clic su **Aggiungi campi**. Questo crea un campo denominato **Budget (da informazioni prodotto)**, che è il nome del campo collegato. In questo campo verranno visualizzate tutte le informazioni relative al budget prodotti per i record della campagna.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Se si desidera visualizzare il budget di tutti i prodotti selezionati come un unico numero totale, selezionare **SOMMA** nel menu a discesa a destra del nome del campo. Quando gli utenti selezionano più prodotti nella **Informazioni sul prodotto** campo record collegato, il **Budget (da informazioni prodotto)** aggiunge tutti i valori Budget e visualizza il totale. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Se si seleziona **Nessuno**, invece di **SOMMA**, i singoli budget verranno visualizzati separati da virgole.

   Vengono generati i campi seguenti:

   * Nella vista Tabella record Campaign e nella pagina Dettagli di una campagna:

      * **Informazioni sul prodotto** (campo record collegato): questo comando visualizza il nome o i nomi dei prodotti.
      * **Budget (da informazioni prodotto)** (campo collegato): vengono visualizzati i budget dei prodotti selezionati nel campo Informazioni prodotto.

   * Nella visualizzazione della tabella Record prodotto e nella pagina Dettagli di un prodotto:

      * **Campagna**: indica che il tipo di record Prodotto è collegato dal tipo di record Campagna.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    I campi record collegati sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

1. Per popolare il **Informazioni sul prodotto** campo, da **Campagna** nella vista tabella del tipo di record, crea una campagna aggiungendo una nuova riga nella tabella della pagina del tipo di record Campaign.
1. Fai clic su **+** all&#39;interno del  **Informazioni sul prodotto** della nuova campagna. Il **Connetti oggetti** viene visualizzata la casella. Il nome del tipo di record a cui si desidera collegare (Product) viene visualizzato nell&#39;angolo superiore sinistro della casella.

   ![](assets/connect-objects-box-to-select-other-maestro-records-example-for-product-record.png)

1. Seleziona i record Prodotto che desideri collegare ai record Campaign, quindi fai clic su **Connetti oggetti**.

   Nella tabella dei tipi di record di Campaign sono inserite le colonne seguenti:
   * Il **Informazioni sul prodotto** viene compilato il campo relativo al record Campagna con i Prodotti selezionati.
   * **Budget (da informazioni prodotto)** viene compilato con il valore Budget per ciascun Prodotto selezionato o con un totale di tutti i budget dei prodotti selezionati.

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Se non si seleziona un aggregatore per i valori multipli, tutti i valori vengono visualizzati separati da virgole.

1. Per popolare il **Campagna** campo da **Prodotto** vista tabella, ripetere i passaggi 5-7 a partire dalla vista tabella Tipo di record prodotto e selezionando le informazioni sulla campagna. Verrà aggiornato anche il campo Informazioni prodotto nella tabella della pagina Tipo di record campagna. <!--ensure the step numbers remain correct-->


## Collegare un tipo di record Maestro a un tipo di oggetto progetto Workfront e un record a singoli progetti

Ad esempio, il tipo di record originale è Campaign.

In Workfront sono presenti anche progetti con un campo denominato &quot;Entrate pianificate&quot;.

Desideri creare un campo connessione nel tipo di record Campaign in cui visualizzare i valori del campo Retribuzione pianificata nel progetto in Workfront per determinate campagne.

Per eseguire questa operazione:

1. Vai a un’area di lavoro in cui desideri collegare il tipo di record Campaign ai progetti Workfront.
1. Apri la vista a tabella per il tipo di record Campaign nell’area di lavoro selezionata.
1. Fai clic su **+** nell’angolo superiore destro della vista tabella per aggiungere un nuovo campo, quindi fai clic su **Nuova connessione**.
1. Aggiungi le seguenti informazioni, ad esempio:

   * **Tipo di record**: progetto Workfront (dalla sottosezione Workfront) <!--did they change the casing here for the field label and did they take "Workfront" out of the name of the object?-->
   * **Nome**: informazioni sul progetto. Questo è il nome del campo oggetto collegato.
   * **Descrizione**: questi sono i progetti a cui voglio associare le mie campagne.
   * 
      * **Consenti più record**: se lasci selezionata questa opzione, gli utenti potranno selezionare più oggetti quando il campo del tipo di oggetto collegato (informazioni sul progetto) viene visualizzato nei record originali (Campagne).
   * **Seleziona campi di ricerca**: se lasci selezionata questa opzione, il **Aggiungi campi di ricerca** viene visualizzata la casella accanto, che consente di collegare i campi di Project con il tipo di record Campaign. Puoi saltare questo passaggio e aggiungere i campi Progetto in un secondo momento.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Condizionale) Se hai selezionato il **Opzione Seleziona campi di ricerca** nel passaggio precedente, dall’elenco di campi associati al **Progetto** tipo di oggetto, fare clic sul pulsante **+** icona per **Reddito Pianificato** , quindi fai clic su **Aggiungi campi**. Questo crea un campo denominato **Retribuzione pianificata (da informazioni progetto)**, che è il nome del campo collegato. In questo campo verranno visualizzate tutte le informazioni del campo Ricavi progetto relative ai record della campagna.

   >[!TIP]
   >
   >    Se desideri visualizzare la Retribuzione pianificata di tutti i progetti selezionati come un unico numero totale, seleziona **SOMMA** nel menu a discesa a destra del nome del campo. Quando gli utenti selezionano più progetti nel **Informazioni progetto** campo oggetto collegato, il **Reddito Pianificato (da informazioni prodotto)** Il campo aggiunge tutti i valori e visualizza il totale. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Se si seleziona **Nessuno**, invece di **SOMMA**, i singoli Ricavi pianificati vengono visualizzati separati da virgole.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Vengono generati i campi seguenti:

   * Nella vista Tabella record Campaign e nella pagina Dettagli di una campagna:

      * **Informazioni progetto** (campo oggetto collegato): verranno visualizzati il nome o i nomi dei progetti.
      * **Retribuzione pianificata (da informazioni progetto)** (campo collegato): visualizza le Retribuzioni pianificate dei progetti selezionati nel campo Informazioni progetto.

   >[!TIP]
   >
   >    I campi oggetto collegato sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

1. Per popolare il **Informazioni progetto** campo, da **Campagna** tipo di record vista tabella, crea una campagna aggiungendo una nuova riga nella tabella.
1. Fai clic su **+** all&#39;interno del  **Informazioni progetto** della nuova campagna. Il **Connetti oggetti** viene visualizzata la casella. Il nome del tipo di oggetto a cui si sta effettuando il collegamento (Workfront Project) viene visualizzato nell&#39;angolo superiore sinistro della casella.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Seleziona il progetto o i progetti a cui vuoi collegare i record di Campaign, quindi fai clic su **Connetti oggetti**.

   Nell&#39;area di lavoro selezionata vengono aggiunti gli elementi seguenti:

   * Nella tabella del tipo di record di Campaign:
      * Il **Informazioni progetto** Il campo viene compilato per il record Campaign con i progetti selezionati.
      * Il **Reddito Pianificato (da informazioni prodotto)** viene compilato con il valore Budget per ciascun Prodotto selezionato. Questo campo è di sola lettura.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Se non si seleziona un aggregatore per i valori multipli e si selezionano più oggetti nel campo collegato a oggetti, tutti i valori vengono visualizzati separati da virgole.

   * Tipo di record di Workfront Project di sola lettura per l&#39;area di lavoro selezionata.

1. Fare clic sulla freccia rivolta all&#39;indietro a sinistra del nome del record nell&#39;intestazione della pagina per passare all&#39;area di lavoro che si sta aggiornando.
1. Apri **Progetto Workfront** scheda tipo di record per aprire la pagina tipo di record.

   Osservare quanto segue per la pagina Tipo di record Progetto Workfront:

   * Si tratta di un tipo di record Maestro di sola lettura che non è possibile eliminare o aggiornare.
   * I progetti selezionati per la connessione alle campagne vengono visualizzati come record separati nella pagina Tipo di record progetto Workfront. I record del progetto sono anche di sola lettura e le relative informazioni vengono aggiornate automaticamente durante l’aggiornamento dei progetti in Workfront. È necessario aggiungere altri progetti dal record Maestro connesso per visualizzarli nel tipo di record Progetto Workfront.
   * Nel campo Record collegato alla campagna vengono inseriti i nomi delle campagne connesse ai progetti dalla pagina Tipo di record Campagna.

1. (Facoltativo) Fai clic su **Altro** icona ![](assets/more-menu.png) a destra del nome del tipo di record di Workfront Project e fare clic su **Rinomina** per rinominare il tipo di record.

   >[!TIP]
   >
   >È possibile rinominare un nome di tipo di record facendo clic sul nome nell&#39;intestazione del tipo di record.

1. Fai clic sull’icona Aggiungi campi ![](assets/add-fields-icon.png) nell’angolo superiore destro della tabella dei tipi di record di Workfront Project per aggiungere altri campi di progetto al tipo di record Workfront Project Maestro.
1. Fai clic su **+** per qualsiasi campo di progetto che desideri aggiungere al record Workfront Project Maestro in **Campi non selezionati** sezione.
1. Fai clic su **-** per i campi del progetto che si desidera rimuovere dal record Workfront Project Maestro in **Campi selezionati** sezione.
1. Fai clic su **Salva**.

   >[!TIP]
   >
   >    I campi aggiunti al record Workfront Project Maestro vengono aggiunti solo nella pagina Progetto Workfront e non nella pagina Tipo di record Campagna, come campi collegati. Per visualizzare i campi relativi alle campagne, aggiungi i campi del progetto dal campo Informazioni progetto connesso a un oggetto del tipo di record Campagna.

1. (Facoltativo e condizionale) Se hai selezionato di visualizzare almeno due campi data per i progetti, fai clic sul pulsante **Visualizza** nella tabella dei tipi di record di Workfront Project, quindi **Crea visualizzazione** > **Timeline** > **Crea** per creare una vista timeline e visualizzare i progetti su una timeline.



