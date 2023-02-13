---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Creare e gestire visualizzazioni personalizzate in [!DNL Workfront Proof]
description: Puoi creare visualizzazioni personalizzate dei file e delle bozze per elencare gli elementi desiderati nel modo desiderato. Puoi anche esportare le informazioni nella visualizzazione Personalizzato come rapporto (in CSV, valori separati da virgole, formato file).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2457'
ht-degree: 1%

---

# Creare e gestire visualizzazioni personalizzate in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Puoi creare visualizzazioni personalizzate dei file e delle bozze per elencare gli elementi desiderati nel modo desiderato. Puoi anche esportare le informazioni nella visualizzazione Personalizzato come rapporto (in CSV, valori separati da virgole, formato file).

>[!NOTE]
>
>Le visualizzazioni personalizzate sono disponibili solo nei piani Select e Premium. Contatta il nostro team di vendita per un preventivo.

## Creazione di una vista personalizzata

Quando crei una visualizzazione personalizzata, puoi scegliere:

* Includere bozze, file o entrambi
* Colonne visualizzate
* Quale colonna ordinare in base a
* Ordine della colonna (crescente o decrescente)
* Quali tipi di filtri utilizzare per determinare quali informazioni sono incluse nella visualizzazione

Dopo la creazione della visualizzazione personalizzata, questa può essere utilizzata immediatamente. Il nome della nuova visualizzazione è incluso anche nel menu a discesa sotto l’intestazione Le mie viste personalizzate (sotto le viste Standard).

Per creare una visualizzazione personalizzata:

1. Vai a **[!UICONTROL Viste]** pagina.
1. Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Effettua una delle seguenti operazioni, a seconda che desideri creare una nuova visualizzazione personalizzata da zero o crearne una nuova personalizzata basata su una visualizzazione standard esistente:

   * Per creare una nuova visualizzazione personalizzata basata su una visualizzazione standard esistente: Dal menu a discesa, seleziona la visualizzazione standard esistente da utilizzare come base per la nuova visualizzazione personalizzata. Fai clic sul pulsante **[!UICONTROL Visualizza impostazioni]** icona, quindi fai clic su **[!UICONTROL Copia]** alla nuova visualizzazione personalizzata.

   * ![](assets/proof-custom-view-icon.png)

   * Per creare una nuova visualizzazione personalizzata da zero: Fai clic sul pulsante **[!UICONTROL Nuova vista]** icona.
   * ![](assets/proof-newview.png)

1. In **[!UICONTROL Dettagli]** specificare le seguenti informazioni:

   * **[!UICONTROL Nome]** (obbligatorio): Nome della nuova visualizzazione. Usa un nome univoco in modo che gli utenti possano trovare facilmente la visualizzazione personalizzata nel menu a discesa Visualizzazioni .
   * **[!UICONTROL Elementi]**: Selezionare se si desidera includere nella visualizzazione solo le bozze e i file, solo le bozze o i file. Per impostazione predefinita, sono inclusi sia le bozze che i file.

1. In **[!UICONTROL Colonne]** determina le colonne da includere nella visualizzazione personalizzata.

   1. Fai clic sull’icona a forma di freccia destra.
   1. ![](assets/proof-view-rightarrow.png)

   1. Fare doppio clic sul nome della colonna selezionata.
   1. È necessario selezionare almeno una colonna e aggiungerne una solo una.
   1. Seleziona una colonna dal **[!UICONTROL Colonne disponibili]** area da includere nella nuova visualizzazione.
   1. Le colonne vengono spostate dal **[!UICONTROL Colonne disponibili]** all&#39;elenco **[!UICONTROL Colonne selezionate]** elenco.

   1. È possibile selezionare tra le colonne standard oppure scegliere i campi personalizzati e i motivi delle decisioni come colonne nella visualizzazione personalizzata. (Se questi sono stati configurati nel tuo account, vengono visualizzati nell&#39;area standard dell&#39;elenco delle colonne disponibili.)
   1. Colonne standard da includere

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nome dell'area di visualizzazione attiva</strong></td>   
      <td>Nome dello stadio attivo nel flusso di lavoro automatizzato.</td>  
      </tr>  
      <tr>   
      <td><strong>Commenti</strong></td>   
      <td>Numero di osservazioni ricevute.</td>
      </tr>  
      <tr>   
      <td><strong>Contatore</strong></td>
      <td>Mostra una serie di prove che sono state caricate sul tuo account (devi aver abilitato un'opzione di contatore delle prove in Impostazioni account).</td>
      </tr>
      <tr>
      <td><strong>Creazione completata</strong></td>
      <td>Data e ora di creazione dell’elemento.</td>
      </tr>
      <tr>
      <td><strong>Creatore</strong></td>
      <td>Utente che ha creato l’elemento.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Data aggiunta alla bozza]</strong></td>
      <td>Data di aggiunta alla bozza. </td>
      </tr>
      <tr>
      <td><strong>Scadenza</strong></td>
      <td>Il termine per l'intera prova.</td>
      </tr>
      <tr>
      <td><strong>Decisioni</strong></td>
      <td>Numero di decisioni prese rispetto al numero previsto (ad esempio 0 di 1, 1 di 1, ecc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Download]</strong></td>
      <td>Il numero di volte in cui il file originale è stato scaricato.</td>
      </tr>
      <tr>
      <td><strong>Nome file</strong></td>
      <td>Nome del file o della bozza.</td>
      </tr>
      <tr>
      <td><strong>Cartella</strong></td>
      <td>La cartella contenente l'elemento.</td>
      </tr>
      <tr>
      <td><strong>Ultima attività</strong></td>
      <td>Data e ora dell’ultima attività sull’elemento.</td>
      </tr>
      <tr>
      <td><strong>Decisione più recente</strong></td>
      <td>Data e ora dell'ultima decisione presa.</td>
      </tr>
      <tr>
      <td><strong>La mia scadenza</strong></td>
      <td>La tua scadenza sulle bozze in cui sei esplicitamente aggiunto come Revisore/Approvatore (se applicato).</td>
      </tr>
      <tr>
      <td><strong>Proprietario</strong></td>
      <td>Il proprietario dell'elemento.</td>
      </tr>
      <tr>
      <td><strong>Paese proprietario</strong></td>
      <td>Il paese registrato nel sistema per il proprietario della prova. </td>
      </tr>
      <tr>
      <td><strong>Prova principale</strong></td>
      <td>Nome della bozza padre.</td>
      </tr>
      <tr>
      <td><strong>Avanzamento</strong></td>
      <td><p>Barra di avanzamento. Visualizza le bozze non ancora Avviate, Aperte, Commentate o Decise.</p><p>Queste informazioni non vengono ordinate in base a.</p></td>
      </tr>
      <tr>
      <td><strong>Nome bozza</strong></td>
      <td>Nome della bozza.</td>
      </tr>
      <tr>
      <td><strong>Tipo di bozza</strong></td>
      <td><p>Tipo di prova: File statico, pagina web statica, Web interattivo (.zip upload), pagina web interattiva (https), video, audio e altro. </p><p>Le prove combinate sono identificate come "Tipo di prova combinato". Tipo di file della bozza.</p></td>
      </tr>
      <tr>
      <td><strong>Dimensioni file (MB)</strong></td>
      <td><p>Dimensione del file della bozza in relazione alla quota di utilizzo del disco.</p><p>Queste informazioni fornivano la versione corrente della bozza. Se non è presente alcuna versione corrente, questa verrà utilizzata per la versione più recente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Termine fase attiva</strong></p></td>
      <td>Termine delle fasi del flusso di lavoro automatizzato.</td>
      </tr>
      <tr>
      <td><strong>Nome della fase</strong></td>
      <td>Nome di ogni fase del flusso di lavoro automatizzato. Ciò include le fasi passate, le fasi attive e future.</td>
      </tr>
      <tr>
      <td><strong>Stato</strong></td>
      <td>Attivo, Bloccato, Bozza o Inviato.</td>
      </tr>
      <tr>
      <td><strong>Stato</strong></td>
      <td>In sospeso, modifiche richieste, approvate con modifiche, approvate o non rilevanti.</td>
      </tr>
      <tr>
      <td><strong>Tag</strong></td>
      <td>Qualsiasi tag associato all’elemento.</td>
      </tr>
      <tr>
      <td><strong>Prossimi nomi di stage</strong></td>
      <td> Nome di ogni fase non ancora avviata nel flusso di lavoro automatizzato. </td>
      </tr>
      <tr>
      <td><strong>Contatore delle versioni</strong></td>
      <td> Numero di versioni dell'elemento. </td>
      </tr>
      <tr>
      <td><strong>Numero della versione di prova</strong></td>
      <td><i>Numero di versione della bozza.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Facoltativo) Per spostare la colonna nel **[!UICONTROL Colonne selezionate]** area in modo che sia inclusa nella nuova visualizzazione:

      * Riordina le colonne nel **[!UICONTROL Colonne selezionate]** elenco.
      * L’ordine in cui vengono visualizzate le colonne nel **[!UICONTROL Colonne selezionate]** determina l’ordine di visualizzazione delle colonne nella visualizzazione personalizzata.
      * Le colonne sono visibili nella **[!UICONTROL Colonne selezionate]** nell’ordine in cui li hai aggiunti dal **[!UICONTROL Colonne disponibili]** elenco.

      * Per riordinare una colonna nel **[!UICONTROL Colonne selezionate]** selezionare il nome della colonna e trascinarla verso l’alto o verso il basso nell’elenco.

      * Rimuovi una colonna dal **[!UICONTROL Colonne selezionate]** facendo clic sul nome della colonna selezionata, quindi facendo clic sul pulsante **[!UICONTROL Sinistra]** freccia. In alternativa, è possibile fare doppio clic sul nome della colonna selezionata (la colonna viene spostata di nuovo nel **[!UICONTROL Colonne disponibili]** elenco).

      * È possibile aggiungere una colonna una sola volta. Ad esempio, se si sposta la colonna Commenti da [!UICONTROL Disponibile] a [!UICONTROL Colonne selezionate] elenco, il nome di questa colonna scompare [!UICONTROL Colonne disponibili] elenco.

1. In **[!UICONTROL Ordinamento]** specificare le seguenti informazioni:

   * **Ordina per:** Utilizza la [!UICONTROL Ordinamento] per impostare un ordine particolare in cui gli elementi sono elencati nella visualizzazione personalizzata. Se non si seleziona una colonna per l’ordinamento, il valore predefinito è No (No), ovvero nessuna colonna o ordine di ordinamento speciale.
   * Solo le colonne selezionate nella [!UICONTROL Colonne] sono incluse nella scheda [!UICONTROL Ordina per colonna] elenco a discesa.
   * **Crescente o decrescente:** Seleziona se ordinare la colonna in senso crescente o decrescente per impostazione predefinita.

1. Utilizza la **[!UICONTROL Filtri]** per definire uno o più criteri per la selezione degli elementi da includere nella visualizzazione personalizzata. I filtri sono particolarmente utili se desideri utilizzare la visualizzazione personalizzata come rapporto.
1. Per includere tutti gli elementi nella visualizzazione personalizzata, ignora **[!UICONTROL Filtri]** sezione .
1. Filtri disponibili:

   * **Campo:** Selezionare il campo Campo per questo filtro (Commenti è il campo predefinito). L’elenco Campo contiene tutti i campi Standard, come nel [!UICONTROL Colonne] ). L’elenco non è limitato alle colonne selezionate per la visualizzazione.
   * **Operatore:** Gli operatori disponibili per il filtro dipendono dal tipo di campo selezionato. Selezionare un operatore che mostri la relazione tra il campo Campo e il campo valore. Compila queste informazioni più tardi.
   * **Valore:** Selezionare o immettere il valore scelto in questo campo, in base al campo e all&#39;operatore selezionato. A seconda dell&#39;operatore scelto, potrebbe essere presente un campo Valore o due campi o nessuno. Vedi gli esempi seguenti.
   * **I filtri vengono applicati utilizzando la logica seguente:** L’operatore AND consente di filtrare i criteri tra campi diversi. Per i criteri di filtro multipli che utilizzano lo stesso campo viene utilizzato l’operatore OR per lo stesso campo.

      Se si desidera visualizzare solo le bozze con zero commenti, selezionare i seguenti valori:

      * Campo: Commenti
      * Operatore: Uguale
      * Campo valore: 0

      Se si desidera visualizzare solo le bozze con due o più commenti, selezionare i seguenti valori:

      * Campo: Commenti
      * Operatore: Maggiore o uguale a
      * Campo valore: 2

      Se si desidera visualizzare solo le bozze con un numero di commenti compreso tra 1 e 4, selezionare i seguenti valori:

      * Campo: Commenti
      * Operatore: Tra
      * Campo valore (primo campo): 1
      * Campo valore (secondo campo): 4

         Per modificare un filtro aggiunto alla visualizzazione personalizzata senza problemi o rimuoverlo, fai clic sull’icona a croce accanto alla [!UICONTROL setup] , se necessario.

         Poiché l’elenco Campo non è limitato alle colonne selezionate nella [!UICONTROL Colonne] , fai attenzione quando crei un filtro che include una colonna che non hai selezionato per la visualizzazione personalizzata. Ad esempio, il seguente filtro per la visualizzazione selezionerà tutte le bozze con un valore del contatore Versione pari o superiore a 2:

         * Campo = contatore delle versioni
         * Operatore = Maggiore o uguale a
         * Campo valore = 2

            >[!NOTE]
            >
            >Per modificare un filtro aggiunto alla visualizzazione personalizzata senza problemi o rimuoverlo, fai clic sull’icona a croce accanto alla [!UICONTROL setup] , se necessario.





1. In **[!UICONTROL Condivisione]** seleziona gli utenti nel tuo account che potranno visualizzare la tua visualizzazione personalizzata.
1. Le visualizzazioni personalizzate sono specifiche per l’utente che le crea. Per impostazione predefinita, la nuova vista Personalizzato è visibile solo per il relativo creatore; tuttavia, puoi scegliere di condividere la visualizzazione personalizzata scegliendo una delle seguenti opzioni:

   * **Solo questa visualizzazione personalizzata** (predefinito): Seleziona questa opzione se desideri che la visualizzazione personalizzata sia disponibile solo per te.
   * **Tutti gli utenti possono visualizzare questa visualizzazione personalizzata**: Seleziona questa opzione per rendere disponibile la visualizzazione personalizzata a tutti gli utenti dell’account.
   * **Seleziona gli utenti che possono visualizzare questa visualizzazione personalizzata**: Seleziona questa opzione per rendere la visualizzazione personalizzata disponibile solo per utenti specifici.
   * Inizia a digitare il nome o l’indirizzo e-mail dell’utente che desideri accedere alla visualizzazione personalizzata, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
   * Se a questo punto scegli di non condividere la visualizzazione con altri utenti, puoi farlo in un secondo momento modificando la visualizzazione personalizzata.

1. Fai clic su **[!UICONTROL Crea]**.
1. La vista Personalizzato viene visualizzata ed è disponibile nella sezione [!DNL Views] pagina. Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nel [!DNL Views] Ingresso pagina [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Modifica delle visualizzazioni personalizzate

È possibile modificare facilmente una visualizzazione personalizzata. Per modificare una visualizzazione personalizzata:

1. Vai a **[!UICONTROL Viste]** pagina.\
   Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Fai clic sul pulsante [!UICONTROL Viste] pulsante (1)
1. Seleziona la visualizzazione da modificare dal menu a discesa.\
   ![](assets/proof-view-edit.png)

1. Fai clic sul pulsante **[!UICONTROL Opzioni di visualizzazione]** quindi fai clic su **[!UICONTROL Modifica visualizzazione]**.\
   ![](assets/proof-view-options.png)\
   Viene visualizzata la pagina Modifica visualizzazione personalizzata.

1. Fai clic sul pulsante [!UICONTROL Azioni] menu. (3)\
   Questo pulsante è disponibile solo se nella visualizzazione è inclusa la colonna Nome bozza.
1. Seleziona [!UICONTROL Modifica visualizzazione] dal menu. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. Viene visualizzata la pagina Modifica visualizzazione personalizzata.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Se si modifica la visualizzazione personalizzata, le colonne dell&#39;elenco Colonne selezionate verranno disposte automaticamente in ordine alfabetico. Se necessario, è necessario riorganizzarli prima di aggiornare la visualizzazione.


## Copia delle visualizzazioni personalizzate

La funzione Copia vista consente di creare facilmente una copia di una visualizzazione personalizzata esistente. Questo è molto utile, ad esempio, se desideri impostare viste separate per tutti i tuoi designer, con ogni visualizzazione uguale tranne il proprietario della bozza (designer).

Per copiare una visualizzazione personalizzata:

1. Vai a **[!UICONTROL Viste]** pagina.\
   Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Fai clic sul pulsante **[!UICONTROL Viste]** pulsante . (1)
1. Seleziona la visualizzazione personalizzata dall’elenco. (2)
1. Fai clic sul pulsante **[!UICONTROL Azioni]** menu. (3)\
   Questo pulsante è disponibile solo se nella visualizzazione è inclusa la colonna Nome bozza.

1. Seleziona [!UICONTROL Copia] dal menu. (4)\
   ![copy_custom_view.png](assets/copying-custom-view-350x258.png)

1. Nella pagina Copia visualizzazione personalizzata vengono compilate tutte le impostazioni originali. Modifica la visualizzazione personalizzata in base alla tua scelta e fai clic sul pulsante **[!UICONTROL Copia vista]** pulsante . Verrà immediatamente visualizzata la nuova visualizzazione.\
   ![](assets/copy-custom-view-page-350x542.png)

## Condivisione di visualizzazioni personalizzate

La funzione di visualizzazione Condividi consente di condividere una visualizzazione con altri utenti nel tuo account se non li hai già selezionati nella sezione Condivisione della visualizzazione. Quando condividi una visualizzazione personalizzata con altri utenti, la visualizzazione viene visualizzata nella [!UICONTROL Viste personalizzate] nel menu a discesa Viste.

Per condividere una visualizzazione personalizzata con altri utenti:

1. Vai a **[!UICONTROL Viste]** pagina.\
   Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Fai clic sul pulsante **[!UICONTROL Viste]** pulsante (1)
1. Seleziona la visualizzazione personalizzata dall&#39;elenco (2)
1. Fai clic sul pulsante **[!UICONTROL Azioni]** menu. (3)\
   Questo pulsante è disponibile solo se nella visualizzazione è inclusa la colonna Nome bozza.

1. Seleziona [!UICONTROL Visualizzazione Condividi] dal menu (4)
1. Viene visualizzata la pagina Modifica visualizzazione personalizzata.
1. In [!UICONTROL Condivisione] Seleziona gli utenti con cui vuoi condividere la visualizzazione e fai clic su **[!UICONTROL Aggiorna visualizzazione]**.

   ![Edit_custom_view_page_1_.png](assets/edit-custom-view-page--1--350x543.png)

## Esportazione di visualizzazioni personalizzate in file CSV

Per esportare i dati da una visualizzazione personalizzata in un file CSV:

1. Vai a **[!UICONTROL Viste]** pagina.\
   Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Fai clic sul pulsante **[!UICONTROL Viste]** pulsante . (1)
1. Seleziona la visualizzazione personalizzata dall’elenco. (2)
1. Fai clic sul pulsante **[!UICONTROL Azioni]** menu. (3)\
   Questo pulsante è disponibile solo se nella visualizzazione è inclusa la colonna Nome bozza.

1. Seleziona [!UICONTROL Esportazione in formato CSV] dal menu. (4)\
   ![export_custom_view.png](assets/exporting-custom-view-350x258.png)\
   In una finestra del browser separata, &#39;Generazione del rapporto: 100%&quot; appare più il numero di record (il numero di elementi inclusi nel rapporto dalla visualizzazione personalizzata)

1. (Condizionale) Se viene visualizzato un messaggio di sicurezza che indica che il download del report è attualmente bloccato, fai clic su per consentire il proseguimento del download.
1. Fai clic su **[!UICONTROL Salva]** quando viene visualizzata la finestra Download file che chiede se si desidera aprire o salvare il file.
1. Selezionare un percorso nel computer e salvare il file.

## Eliminazione di visualizzazioni personalizzate

È possibile eliminare facilmente una visualizzazione personalizzata. Per eseguire questa operazione:

1. Vai a **[!UICONTROL Viste]** pagina.\
   Per ulteriori informazioni sulle visualizzazioni, vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Fai clic sul pulsante **[!UICONTROL Viste]** pulsante .
1. Seleziona la visualizzazione personalizzata dall’elenco
1. Fai clic sul pulsante **[!UICONTROL Azioni]** menu. (3)\
   Questo pulsante è disponibile solo se nella visualizzazione è inclusa la colonna Nome bozza.

1. Seleziona [!UICONTROL Elimina] dal menu. (4)\
   ![delete_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Fai clic su **[!UICONTROL Elimina]** (5) per confermare che si desidera eliminare la visualizzazione personalizzata corrente\
   ![delete_1_.png](assets/delete--1--350x187.png)

1. Viene visualizzata la vista predefinita Tutti gli elementi e la vista personalizzata eliminata non viene più visualizzata nella **[!UICONTROL Viste]** menu a discesa.
