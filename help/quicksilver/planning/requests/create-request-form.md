---
title: Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning
description: Dopo aver selezionato un tipo di record nell'area Adobe Workfront Planning, è possibile creare un modulo di richiesta e associarlo a tale tipo di record. Puoi quindi condividere un collegamento con altri utenti interni o esterni. Gli utenti con un collegamento al modulo possono compilare i valori dei campi e, inviandolo, possono aggiungere un nuovo record per il tipo di record ad esso associato.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: c06baa45e52d77463f9f886b6f6eae4ff68e4ccd
workflow-type: tm+mt
source-wordcount: '2686'
ht-degree: 1%

---

# Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile creare un modulo di richiesta e associarlo a un tipo di record in Adobe Workfront Planning. È quindi possibile condividere il modulo con altri utenti, che possono inviare richieste per creare record di quel tipo.

In questo articolo viene descritto come un manager area di lavoro può creare un modulo di richiesta associato a un tipo di record.

Per informazioni sull&#39;invio di una richiesta a un tipo di record per la creazione di un record, vedere [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Qualsiasi pacchetto Workfront</p></li>
E
<li><p>Qualsiasi pacchetto Planning</p></li></ul>
Oppure
<ul><li><p>Qualsiasi pacchetto flusso di lavoro</p></li>
E
<li><p>Qualsiasi pacchetto Planning</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro o un tipo di record</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitazioni della visualizzazione di campi e valori nei moduli di richiesta

Dopo l’invio di una richiesta, la visualizzazione di determinati campi nel modulo di richiesta e la successiva visualizzazione dei relativi valori nei record o nella pagina dei dettagli della richiesta sono soggette a limitazioni.

Per informazioni sull&#39;invio di richieste Workfront Planning, vedere [Inviare richieste Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

* Di seguito sono riportate le limitazioni relative alla visualizzazione di determinati campi nei moduli di richiesta, nei record creati da un modulo di richiesta o nella pagina dei dettagli della richiesta:

   * Non è possibile aggiungere campi dei tipi seguenti a un modulo di richiesta:

      * Creato da, Ultima modifica da, Approvato da
      * Data di creazione, Data ultima modifica, Data approvazione
      * Campi di ricerca di oggetti Workfront
      * Campi di ricerca dei record connessi di Workfront Planning

* Di seguito sono riportate le differenze tra la visualizzazione dei formati dei campi nel generatore di moduli di richiesta e la formattazione dei valori dei campi nel record o nella pagina dei dettagli della richiesta:

   * I campi Valuta, Numero e Percentuale vengono visualizzati come un tipo di campo di testo a riga singola nel generatore di moduli.

     Tuttavia, il formato del campo viene mantenuto e i valori del campo vengono visualizzati come valuta, numeri e percentuali dopo l’invio della richiesta, nel tipo di record e nella pagina dei dettagli della richiesta.

* Di seguito viene descritto come alcuni valori di campo vengono visualizzati nei moduli di richiesta e nelle pagine dei dettagli della richiesta:

   * La formattazione speciale per i campi Valuta, Numero e Percentuale non viene mantenuta. Ad esempio, la precisione decimale non viene mantenuta per i valori di questi campi in queste aree.
   * I valori dei campi Persone vengono visualizzati come ID.
   * I campi formula che non fanno riferimento ad altri campi o calcoli non visualizzano alcun valore. Ad esempio, un campo con una formula `STRING` visualizza un valore &quot;N/D&quot;.
   * I campi formula che fanno riferimento ai campi Valuta visualizzano i valori senza tenere conto dei tassi di cambio.
   * I valori dei campi Paragrafo visualizzano un valore &quot;N/A&quot; nel modulo di richiesta e visualizzano tag HTML invece del testo formattato nella pagina dei dettagli della richiesta.

## Creare un modulo di richiesta

Per creare un modulo di richiesta, è necessario iniziare a creare il modulo, impostare i dettagli del modulo e terminare con la pubblicazione e la condivisione del modulo.

### Inizia a creare un modulo di richiesta

È possibile creare un modulo di richiesta dal tipo di record associato al modulo<!--span class="preview">, or from the Requests area of Workfront.</span>-->.

#### Creare un modulo di richiesta da un tipo di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Crea modulo di richiesta** o **Gestisci moduli di richiesta**, se disponi già di un modulo e desideri crearne di nuovi.
1. (Condizionale) Se si desidera aggiungere un altro modulo, fare clic su **Nuovo modulo di richiesta**.

   Viene visualizzata la casella Crea modulo di richiesta (Create request form).

1. Nella casella Crea modulo di richiesta aggiornare il nome del modulo. Per impostazione predefinita, il nome del modulo è **Modulo senza titolo**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Facoltativo) Aggiungi una **Descrizione** per il modulo di richiesta.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Fai clic su **Crea**.

   Il modulo di richiesta per il tipo di record selezionato viene aperto nella scheda Modulo.
1. Continua con [Configurare il modulo](#configure-the-form).

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### Imposta i dettagli per il modulo di richiesta

I dettagli del modulo sono suddivisi in schede.

* La scheda **Modulo** consente di aggiungere campi ed elementi di contenuto al modulo
* La scheda **Configurazione** consente di impostare un processo di approvazione per il modulo e di impostare le opzioni di completamento richieste&lt;.
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### Imposta dettagli modulo

1. Inizia a creare o modificare un modulo di richiesta, come descritto nella sezione [Inizia a creare un modulo di richiesta](#begin-creating-a-request-form).

   Il modulo di richiesta per il tipo di record selezionato viene aperto nella scheda Modulo.

   ![Modalità di modifica modulo richiesta campagne](assets/campaigns-request-form-edit-mode.png)

   Per impostazione predefinita, il modulo di richiesta contiene le seguenti informazioni:

   * Campi record disponibili nella vista tabella del tipo di record selezionato. <!--they are working on removing the limitation below-->

   * **Sezione predefinita**: questa è l&#39;interruzione di sezione predefinita che Workfront applica al modulo di richiesta. Tutti i campi record vengono visualizzati nell&#39;area **Sezione predefinita**.
   * Campo **Oggetto**: campo che identificherà la richiesta in Workfront. Impossibile modificare la configurazione e il valore del campo Oggetto.

     >[!NOTE]
     >
     >* Il campo **Subject** richiede un valore quando è visibile nel modulo di richiesta. Tuttavia, è possibile rimuovere il campo **Oggetto**, se necessario, e i richiedenti non lo visualizzeranno nel modulo al momento dell&#39;invio della richiesta.
     >* Quando in un modulo di richiesta manca il campo Oggetto, ma è presente un campo Nome per il nome del record futuro, al nome della richiesta viene automaticamente assegnato lo stesso nome del record creato.
     >* Quando nel modulo di richiesta mancano i campi Oggetto e Nome, la richiesta viene denominata in base al seguente pattern: `< Record name > request form < Entry date of the request >`; il record è denominato **Senza titolo**.

   * Tutti i campi associati al tipo di record.

     I campi contenuti nel modulo di richiesta saranno visibili a tutti coloro che inviano una richiesta a questo tipo di record.

1. (Facoltativo) Passa il puntatore del mouse su tutti i campi del modulo che desideri rimuovere, quindi fai clic sull&#39;icona **x** per rimuoverli. Vengono aggiunti alla scheda **Campi** a sinistra del modulo.

   Rimuovere ad esempio il campo **Oggetto**, in quanto non è visibile in Workfront Planning. <!--remove this example if this becomes visible in Planning?-->

1. (Facoltativo) Per rimuovere la **sezione predefinita** dal modulo, eseguire le operazioni seguenti:

   1. Rimuovi tutti i campi dalla sezione predefinita.
   1. Fai clic su **Elementi di contenuto** e aggiungi una nuova sezione, quindi aggiungi un nome per la sezione.
   1. Aggiungi campi alla nuova sezione.
   1. Fai clic sull&#39;icona **x** per rimuovere la **sezione predefinita**.
1. Fare clic su un campo qualsiasi, quindi utilizzare i controlli nel pannello destro del modulo per definirne le dimensioni o una delle seguenti informazioni:

   * **Etichetta**: questo è il nome del campo che verrà visualizzato nel modulo di richiesta. Questo non modifica il nome del campo record.
   * **Istruzioni**: aggiungere ulteriori informazioni sul campo.
   * **Imposta un campo obbligatorio**: se selezionata, il campo deve avere un valore. In caso contrario, il modulo non può essere inviato.
   * **Aggiungi logica**: definisci quali condizioni devono essere soddisfatte affinché il campo venga visualizzato o nascosto.

   >[!TIP]
   >
   >   Il tipo di campo di ciascun campo viene visualizzato nella parte superiore del pannello di destra, dopo aver selezionato il campo nel modulo.
   >     

1. (Facoltativo) Fai clic sulla scheda **Elementi di contenuto** sul lato sinistro del modulo e aggiungi i seguenti elementi:

   * **Testo descrittivo**
   * **Interruzione di sezione**

   Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facoltativo) Fare clic su **Anteprima** per visualizzare la modalità di visualizzazione del modulo per gli altri utenti che lo utilizzeranno per inviare un nuovo record.
1. Passa a [Imposta dettagli configurazione](#set-up-configuration-details) se desideri configurare ulteriori dettagli per il modulo o passa a [Completa creazione modulo richiesta](#complete-request-form-creation).

#### Configurare i dettagli della configurazione

Nella scheda Configurazione puoi impostare il processo di approvazione e configurare quando una richiesta creata da questo modulo verrà contrassegnata come Completata.

1. Inizia a creare o modificare un modulo di richiesta, come descritto nella sezione [Inizia a creare un modulo di richiesta](#begin-creating-a-request-form).

   Il modulo di richiesta per il tipo di record selezionato viene aperto nella scheda Modulo.
1. (Facoltativo) Configura i dettagli del modulo come descritto in [Configura dettagli modulo](#set-up-form-details).

1. (Facoltativo) Fai clic sulla scheda **Configurazione**, quindi aggiungi almeno un utente o un team al campo **Approvatori** per approvare nuove richieste per questo modulo record.

   ![Scheda Configurazione](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Quando si associa un modulo di richiesta agli approvatori, prima di generare un nuovo record è necessario che tutte le nuove richieste vengano approvate da tutti gli approvatori.
   * Puoi aggiungere uno o più approvatori a un modulo di richiesta.
   * Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il record non viene creato.
   * Tutti gli approvatori devono prendere una decisione prima che una richiesta venga approvata o rifiutata.
   * Se un team è impostato come approvatore, è necessaria una sola decisione del team.

     Per ulteriori informazioni sull&#39;aggiunta di approvazioni ai moduli di richiesta, vedere [Aggiungere approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Condizionale) Se desideri che il record venga creato dopo l&#39;approvazione di uno qualsiasi degli approvatori, seleziona la casella di controllo **È necessaria una sola decisione**.

1. Specificare se si desidera che una richiesta creata da questo modulo venga contrassegnata come completata al momento della creazione dell&#39;oggetto richiesto o quando l&#39;oggetto richiesto viene completato.
1. (Condizionale) Se hai selezionato la richiesta da contrassegnare come completata quando l’oggetto richiesto è completato, seleziona il campo e il valore che indicano quando l’oggetto è completo. Ad esempio, è possibile selezionare il campo Stato e il valore Completo per completare la richiesta quando lo stato dell&#39;oggetto creato è impostato su Completo.
1. Passa a <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Creazione modulo di richiesta completata](#complete-request-form-creation).

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### Creazione modulo di richiesta completa

1. Creare e configurare il modulo come descritto in [Iniziare a creare un modulo di richiesta](#begin-creating-a-request-form) e [Configurare i dettagli per il modulo di richiesta](#set-up-details-for-the-request-form).
1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del modulo nell&#39;intestazione, quindi fai clic su **Modifica** per aggiornare il nome del modulo.

1. Fai clic su **Pubblica** per pubblicare il modulo e ottenere un collegamento univoco.

   Si verificano le seguenti situazioni:

   * Il pulsante **Pubblica** è stato rimosso.
   * Il pulsante **Annulla pubblicazione** è stato aggiunto al modulo. Facendo clic su di esso, il modulo non sarà accessibile.
   * Un pulsante **Condividi** è stato aggiunto al modulo.
   * Il modulo diventa disponibile nell’area Richieste del menu Principale in Workfront.

1. Fai clic su **Condividi** per condividere il modulo con altri.

   Per informazioni sulla condivisione di un modulo di richiesta, vedere la sezione [Condividere un modulo di richiesta](#share-a-request-form) in questo articolo
1. Fare clic sulla freccia rivolta a sinistra a sinistra del nome della maschera nell&#39;intestazione per chiudere la maschera.

   Viene aperta la vista tabella **Moduli di richiesta** alla quale viene aggiunto il modulo.

## Gestire i moduli di richiesta esistenti


1. Fare clic sull&#39;area di lavoro in cui si desidera gestire i moduli di richiesta.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Gestisci moduli di richiesta**.

   Tutte le maschere di richiesta associate al tipo di record vengono visualizzate in una vista tabella.

1. (Facoltativo) Passa il puntatore del mouse sul nome di un modulo di richiesta nella visualizzazione tabella, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del modulo e fai clic su una delle seguenti opzioni:

   * **Modifica modulo**: fare clic qui per modificare ulteriormente le informazioni nel modulo.
   * **Annulla pubblicazione**: fare clic qui per annullare la pubblicazione del modulo che lo rimuove dall&#39;area Richieste di Workfront.
   * **Condividi**: fare clic qui per modificare gli utenti che hanno accesso al modulo.
   * **Copia collegamento**: fare clic qui per copiare rapidamente il collegamento del modulo di richiesta senza aprire il modulo.
   * **Elimina**: fare clic qui per eliminare il modulo. Tutte le richieste e i record aggiunti utilizzando il modulo non vengono eliminati. Impossibile recuperare il modulo.

   ![Altro menu nel modulo di richiesta dall&#39;elenco dei moduli di richiesta](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Fare clic sulla freccia rivolta a sinistra a sinistra di **Moduli di richiesta** nell&#39;intestazione per chiudere la tabella dei moduli di richiesta.

   Viene visualizzata la pagina del tipo di record.
1. (Facoltativo e condizionale) Fare clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione, quindi eseguire una delle operazioni seguenti:

   1. Fai clic su **Aggiorna modulo di richiesta** per apportare modifiche al modulo di richiesta, quindi fai clic su un modulo di richiesta per aprirlo e modificarlo.
   1. Fai clic su **Copia collegamento al modulo di richiesta** per condividere il collegamento al modulo con altri utenti.

1. (Facoltativo) Vai all&#39;area **Richieste** in Workfront e trova il modulo condiviso per inviare una richiesta. Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Condivisione di un modulo di richiesta

1. Creare un modulo di richiesta come descritto nella sezione [Creare un modulo di richiesta per un tipo di record](#create-a-request-form-for-a-record-type) in questo articolo.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del modulo di richiesta nella pagina del tipo di record.
1. Fai clic su **Condividi** per condividere il modulo con altri.

1. Per condividere il modulo internamente, selezionare la scheda **Condivisione interna**, cercare il nome di un utente, team, mansione, gruppo o società nel campo **Concedi l&#39;accesso per inviare il modulo**, quindi selezionarlo quando viene visualizzato nell&#39;elenco. L&#39;autorizzazione **Invia** è selezionata per impostazione predefinita per ogni entità.

   ![Casella di condivisione per il modulo di richiesta](assets/share-box-for-request-form.png)

1. (Facoltativo) Fai clic sul menu a discesa dopo il nome di un&#39;entità, quindi fai clic su **Rimuovi** per rimuoverli dall&#39;elenco e interrompere la condivisione del modulo con loro.

   >[!NOTE]
   >
   >Oltre a team, gruppi, aziende e ruoli, puoi condividere solo con gli utenti che sono stati aggiunti al Adobe Admin Console. Non è possibile aggiungere utenti solo Workfront. Per informazioni, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. Nella sezione **Chi può inviare richieste tramite questo modulo**, selezionare una delle opzioni seguenti per indicare i tipi di utenti che possono accedere al modulo:

   * Possono accedere solo le persone invitate
   * Chiunque con accesso alla visualizzazione, o superiore, all’area di lavoro
   * Chiunque con accesso per contribuire, o superiore, all’area di lavoro
1. (Facoltativo) Fai clic su **Copia collegamento** per condividere il collegamento al modulo con gli utenti che possono accedervi. Il collegamento viene copiato negli Appunti.
1. Per condividere il modulo pubblicamente, seleziona la scheda **Condivisione pubblica**, quindi abilita l&#39;impostazione **Crea collegamento pubblico**.

   ![Condivisione pubblica per modulo di richiesta](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* Quando si abilita l&#39;impostazione **Crea collegamento pubblico**, chiunque può accedere al modulo e inviare un nuovo record, anche persone esterne all&#39;organizzazione che non dispongono di un account Workfront.
   >
   >* Un modulo contenente i seguenti tipi di campi non può essere condiviso pubblicamente:
   >
   >     * Connessioni Workfront o AEM Assets
   >     * People
   >

1. Scegli una **data di scadenza collegamento**.

   È possibile selezionare date future entro 180 giorni dalla data corrente.

   >[!TIP]
   >
   >Dopo la scadenza della data di condivisione, il modulo di richiesta non è più disponibile nell’area Richieste di Workfront e i collegamenti condivisi con altri utenti non sono più accessibili.

   Gli utenti riceveranno un errore dopo la scadenza del collegamento e, prima di poter accedere nuovamente al modulo, è necessario aggiornare la data del collegamento e generare un nuovo collegamento da condividere.


1. (Facoltativo e condizionale) Fare clic su **Salva** per salvare i dettagli di condivisione per il modulo.
1. (Condizionale) Se il modulo è stato salvato in precedenza, fare clic su **Copia collegamento**.

   Le opzioni di condivisione del modulo vengono salvate e il collegamento viene copiato negli Appunti. Ora puoi condividerlo con altri utenti.

   Per informazioni sulla creazione di record mediante un collegamento a un modulo di richiesta, vedere [Inviare richieste Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Fai clic su **Salva** nell&#39;angolo inferiore destro della scheda **Modulo** per salvare il modulo.
