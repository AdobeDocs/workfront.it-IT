---
title: Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning
description: Dopo aver selezionato un tipo di record nell'area Adobe Workfront Planning, è possibile creare un modulo di richiesta e associarlo a tale tipo di record. Puoi quindi condividere un collegamento con altri utenti interni o esterni. Gli utenti con un collegamento al modulo possono compilare i valori dei campi e, inviandolo, possono aggiungere un nuovo record per il tipo di record ad esso associato.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 2%

---

# Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

È possibile creare un modulo di richiesta e associarlo a un tipo di record in Adobe Workfront Planning. Puoi quindi condividere un collegamento con altri utenti interni o esterni.

Gli utenti con un collegamento al modulo possono aggiornare i valori dei campi in esso contenuti e aggiungere nuovi record inviandolo.

In questo articolo viene descritto come un manager area di lavoro può creare un modulo di richiesta associato a un tipo di record.

Per informazioni sull&#39;invio di una richiesta a un tipo di record per la creazione di un record, vedere [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td>
   <td>
<p>Qualsiasi </p>  
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p>
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
   <ul>
   <li><p>Gestire le autorizzazioni per un’area di lavoro</p></li>
    <li><p>Gli amministratori di sistema possono gestire le aree di lavoro che non hanno creato. </p></li>
    </ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un modulo di richiesta per un tipo di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Crea modulo di richiesta**.
1. Aggiorna il nome del modulo di richiesta. Per impostazione predefinita, il nome del modulo è **Modulo senza titolo**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Facoltativo) Aggiungi una **Descrizione** per il modulo di richiesta.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Fai clic su **Crea**. Il modulo di richiesta per il tipo di record selezionato viene aperto nella scheda Modulo.

   ![](assets/campaigns-request-form-edit-mode.png)

   Per impostazione predefinita, il modulo di richiesta contiene le seguenti informazioni:

   * Campi record disponibili nella vista tabella del tipo di record selezionato. <!--they are working on removing the limitation below-->

   <!-- when we go to prod, the Preview batch below will become the only batch-->

   >[!IMPORTANT]
   >
   >I campi dei seguenti tipi non vengono visualizzati nel modulo di richiesta:
   >
   >* Creato da e Ultima modifica da
   >* Data di creazione e data dell’ultima modifica
   >* Formula
   >* Campi di ricerca di oggetti Workfront
   >* Campi di ricerca dei record connessi di Workfront Planning
   >

   <!--before release to prod: 
    > Depending on what environment you use to create a request form, the following scenarios exist:
   >
   >* Fields of the following types do not display in the request form in the Production environment: 
   >
   >    * Created by and Last modified by
   >    * Created date and Last modified date
   >    * Formula
   >    * People 
   >    * Workfront connected fields
   >    * Workfront objects' lookup fields
   >    * Workfront Planning records' connected fields
   >    * Workfront Planning connected records' lookup fields
   >    * AEM Assets connection fields-->

   * **Sezione predefinita**: questa è l&#39;interruzione di sezione predefinita che Workfront applica al modulo di richiesta. Impossibile rinominare o rimuovere la sezione predefinita.
   * Campo **Oggetto**: campo che identificherà la richiesta in Workfront. Impossibile modificare la configurazione e il valore del campo Oggetto.

     >[!TIP]
     >
     >Il campo **Subject** richiede un valore quando è visibile nel modulo di richiesta. Tuttavia, è possibile rimuovere il campo **Oggetto**, se necessario, e i richiedenti non lo visualizzeranno nel modulo al momento dell&#39;invio della richiesta.

   * Tutti i campi associati al tipo di record.

     I campi contenuti nel modulo di richiesta saranno visibili a tutti coloro che inviano una richiesta a questo tipo di record.

1. (Facoltativo) Passa il puntatore del mouse su tutti i campi del modulo che desideri rimuovere, quindi fai clic sull&#39;icona **x** per rimuoverli. Vengono aggiunti alla scheda **Campi** a sinistra del modulo.

   Rimuovere ad esempio il campo **Oggetto**, in quanto non è visibile in Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Fare clic su un campo qualsiasi, quindi utilizzare i controlli nel pannello destro del modulo per definirne le dimensioni o una delle seguenti informazioni:

   * **Etichetta**: questo è il nome del campo che verrà visualizzato nel modulo di richiesta. Questo non modifica il nome del campo record.
   * **Istruzioni**: aggiungere ulteriori informazioni sul campo.
   * **Imposta un campo obbligatorio**: se selezionata, il campo deve avere un valore. In caso contrario, il modulo non può essere inviato.
   * **Aggiungi logica**: definisci quali condizioni devono essere soddisfatte affinché il campo venga visualizzato o nascosto.

   >[!NOTE]
   >
   >   Il tipo di campo di ciascun campo viene visualizzato nella parte superiore del pannello di destra, dopo aver selezionato il campo nel modulo.
   >   
   >
   >   I campi Valuta, Numero e Percentuale vengono visualizzati come un tipo di campo di testo a riga singola. Tuttavia, il formato del campo viene mantenuto e i valori all’interno di questi campi verranno visualizzati come Valuta, Numero e Percentuale.

1. (Facoltativo) Fai clic sulla scheda **Elementi di contenuto** sul lato sinistro del modulo e aggiungi i seguenti elementi:

   * **Testo descrittivo**
   * **Interruzione di sezione**

   Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facoltativo) Fare clic su **Anteprima** per visualizzare la modalità di visualizzazione del modulo per gli altri utenti che lo utilizzeranno per inviare un nuovo record.

1. (Facoltativo) Fai clic sulla scheda **Configurazione**, quindi aggiungi almeno un utente al campo **Approvatori** per approvare nuove richieste per questo modulo record.

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Quando si associa un modulo di richiesta agli approvatori, prima di generare un nuovo record è necessario che tutte le nuove richieste vengano approvate da tutti gli approvatori.
   * Puoi aggiungere uno o più approvatori a un modulo di richiesta.
   * Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il record non viene creato.
   * Tutti gli approvatori devono prendere una decisione prima che una richiesta venga approvata o rifiutata.

     Per ulteriori informazioni sull&#39;aggiunta di approvazioni ai moduli di richiesta, vedere [Aggiungere approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Facoltativo) Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del modulo nell&#39;intestazione, quindi fai clic su **Modifica** per aggiornare il nome del modulo.
1. Fai clic su **Publish** per pubblicare il modulo e ottenere un collegamento univoco.

   Si verificano le seguenti situazioni:

   * Il pulsante **Publish** è stato rimosso.
   * Il pulsante **Annulla pubblicazione** è stato aggiunto al modulo. Facendo clic su di esso, il modulo non sarà accessibile.
   * Un pulsante **Condividi** è stato aggiunto al modulo.

1. Fai clic su **Condividi** per condividere il modulo con altri.

   ![](assets/share-box-for-request-form.png)

1. Selezionare una delle opzioni seguenti per indicare i tipi di utenti che possono accedere al modulo:

   * Chiunque con accesso alla visualizzazione, o superiore, all’area di lavoro
   * Chiunque con accesso per contribuire, o superiore, all’area di lavoro
   * Chiunque abbia il collegamento

   >[!WARNING]
   >
   >* Quando si seleziona **Chiunque disponga del collegamento** può accedere al modulo e inviare un nuovo record, anche persone esterne all&#39;organizzazione che non dispongono di un account Workfront.
   >
   > * Un modulo contenente i seguenti tipi di campi non può essere condiviso pubblicamente:
   >
   >     * Connessioni Workfront o AEM Assets
   >     * Persone
   >

1. (Condizionale) Se hai selezionato **Qualcuno con il collegamento** nel passaggio precedente, seleziona **Data di scadenza collegamento** dal calendario disponibile. Gli utenti riceveranno un errore dopo la scadenza del collegamento e, prima di poter accedere nuovamente al modulo, è necessario aggiornare la data del collegamento e generare un nuovo collegamento da condividere.

   È possibile selezionare date future entro 180 giorni dalla data corrente.

1. Fare clic su **Salva e copia collegamento** per salvare i dettagli di condivisione per il modulo. Se il modulo è stato salvato in precedenza, fare clic su **Copia collegamento**.

   Le opzioni di condivisione del modulo vengono salvate e il collegamento viene copiato negli Appunti. Ora puoi condividerlo con altri utenti.

   Per informazioni sulla creazione di record mediante un collegamento a un modulo di richiesta, vedere [Inviare richieste Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Fai clic su **Salva** nell&#39;angolo inferiore destro della scheda **Modulo** per salvare il modulo.
1. Fare clic sulla freccia rivolta a sinistra a sinistra del nome della maschera nell&#39;intestazione per chiudere la maschera.

   Viene visualizzata la pagina del tipo di record.
1. (Facoltativo) Fare clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione, quindi eseguire una delle operazioni seguenti:
   * Fai clic su **Aggiorna modulo di richiesta** per apportare eventuali modifiche al modulo di richiesta.
   * Fai clic su **Copia collegamento al modulo di richiesta** per condividere il collegamento al modulo con altri utenti.

   >[!TIP]
   >
   >In questo caso, il collegamento viene condiviso pubblicamente.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
