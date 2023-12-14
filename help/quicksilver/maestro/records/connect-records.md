---
title: Collega record
description: Dopo aver creato connessioni tra tipi di record, è possibile collegare tra loro singoli record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: a74f9f8940a170d8e1347fd99ff2a6c816b12eca
workflow-type: tm+mt
source-wordcount: '2911'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Collega record

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

È possibile collegare tra loro record Adobe Maestro o a oggetti di altre applicazioni.

È innanzitutto necessario connettere due tipi di record o un tipo di record a un tipo di oggetto di un&#39;altra applicazione e quindi utilizzare la visualizzazione Tabella del tipo di record per connettere record tra loro o record ad altri oggetti.

Per informazioni sulla connessione di tipi di record tra loro o a tipi di oggetto di altre applicazioni, vedere [Connetti tipi di record](../architecture/connect-record-types.md).

Per un esempio di connessione dei tipi di record, vedere [Esempio di connessione di tipi di record e record](../architecture/example-connect-record-types-and-records.md).

È possibile connettere i seguenti elementi:

* Record operativi Maestro
* Gestire i record operativi per i record della tassonomia
* Gestire i record operativi e gli oggetti provenienti da altre applicazioni.

  È possibile collegare i record Maestro agli oggetti dei tipi elencati di seguito dalle seguenti applicazioni:

   * Adobe Workfront

      * Progetti
      * Portfolio
      * Programmi
      * Azienda
      * Gruppo

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
<tbody>
<td>
   <p> prodotto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td><p>Qualsiasi, per creare record Maestro</p> 
<p>Lavora o più per visualizzare i progetti in Workfront</p>
  <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Panoramica sulle licenze di Adobe Workfront</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi, per creare record Maestro</p>
<p>Accesso di visualizzazione o superiore a progetti, Portfoli e programmi</p> 
<p>Accesso aggiuntivo a gruppi e società, quando si visualizzano gruppi o società a cui gli utenti non appartengono</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti da collegare ai record Maestro  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Collega record

### Considerazioni sulla connessione dei record

* Una volta stabilita la connessione tra i tipi di record, i tipi di record collegati vengono visualizzati come campi di record collegati nella tabella dei tipi di record da cui sono collegati.
* È possibile sfogliare e aggiungere record e oggetti dei tipi di record e oggetti collegati dai campi dei record collegati.
* È possibile aggiungere campi dei tipi di record collegati alla tabella del tipo di record da cui si sta eseguendo il collegamento.
* Non è possibile aggiornare manualmente i valori dei campi collegati nei record da cui si sta effettuando il collegamento.

  I valori dei campi collegati dei record collegati popolano il record Maestro dal quale si sta effettuando il collegamento automatico.

* Tutti coloro che hanno accesso a Maestro possono vedere le connessioni che si creano tra i record Maestro o tra i record Maestro e gli oggetti Workfront. Inoltre, puoi visualizzare e modificare le connessioni di tutti gli altri. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* È possibile collegare un record Maestro a uno o più oggetti di un&#39;altra applicazione.
* Non è possibile connettere le tassonomie a tipi di record o a oggetti di un&#39;altra applicazione. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Per collegare i record Maestro agli oggetti Workfront, è necessario disporre dei seguenti elementi:

   * Oggetti Workfront. Ad esempio, devi prima creare progetti, portfolio, programmi, aziende o gruppi in Workfront.
   * Aree di lavoro Maestro, tipi di record e record. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Creare aree di lavoro](../architecture/create-workspaces.md)
      * [Crea tipi di record](../architecture/create-record-types.md)
      * [Crea record](../records/create-records.md)

   * Connessioni tra tipi di record o tra tipi di record e oggetti di altre applicazioni. Per informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md)

### Collega i record Maestro

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace da cui si desidera connettere i record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Seleziona un **Tabella** vista da **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.
1. Aggiungere una connessione a un altro record o tipo di oggetto dal tipo di record selezionato. Per informazioni, consulta [Connetti tipi di record](../architecture/connect-record-types.md).

   Viene aggiunta una nuova colonna alla tabella per visualizzare il tipo di record collegato.

1. Aggiungere record al tipo di record selezionato aggiungendo una nuova riga alla tabella. Per informazioni, consulta [Crea record](../../maestro/records/create-records.md).
1. Da un record elencato nella vista a tabella, vai alla colonna del record collegato e passa il puntatore del mouse sulla cella corrispondente al record che desideri collegare con altri record Maestro, quindi fai clic sul pulsante **+** icona.

   Il **Connetti oggetti** viene visualizzata la casella.

   ![](assets/connected-objects-table-for-records.png)

1. Iniziare a digitare il nome di un record nella casella di ricerca, quindi selezionarlo quando viene visualizzato nell&#39;elenco

   Oppure

   Selezionare il nome di uno o più record nella casella, quindi fare clic su **Connetti oggetti** nell&#39;angolo superiore destro della casella Connetti oggetti.

   Sono aggiunti i seguenti elementi:

   * I record collegati vengono visualizzati nel campo record collegato del record selezionato al passaggio 3. L&#39;aggiornamento dei record collegati aggiorna automaticamente i campi dei record collegati per i record da cui si sta effettuando il collegamento. <!--ensure the number of the step stays accurate-->
   * I campi collegati che appartengono ai record collegati vengono compilati automaticamente con le informazioni dei record collegati originali. Non è possibile modificare manualmente i campi collegati.

     >[!TIP]
     >
     >* Utilizziamo &quot;campi collegati&quot; e &quot;campi di ricerca&quot; in modo intercambiabile.
     >
     >* Se è stata abilitata l&#39;impostazione Consenti più record quando si sono connessi i tipi di record, i valori dei campi per i più oggetti selezionati vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.

1. (Facoltativo) Chiudi la pagina Tipo di record Maestro e passa all’area di lavoro selezionata.
1. Fare clic sulla scheda del tipo di record a cui si è collegati.

   Ad esempio, se hai collegato il record Campagna al record Prodotto, fai clic sul pulsante **Prodotto** Card.

   La scheda del tipo di record deve aprirsi nella vista Tabella.

   Il campo Record collegato Campagna visualizza i nomi delle campagne collegate ai prodotti nella pagina Tipo di record prodotto. L’aggiornamento delle informazioni della campagna aggiorna automaticamente il campo del record collegato della campagna per il tipo di record Prodotto.

### Collegare i record Maestro agli oggetti Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Dopo aver creato una connessione tra un tipo di record Maestro e un tipo di oggetto Workfront, è possibile collegare singoli record Maestro a oggetti in Workfront. I campi Workfront collegati vengono automaticamente compilati sui record Maestro da cui stai collegando gli oggetti.

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace da cui si desidera connettere i record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Seleziona un **Tabella** vista da **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.

1. (Facoltativo) Aggiungere singoli record al tipo di record selezionato aggiungendo una nuova riga alla tabella. Per informazioni, consulta [Crea record](../../maestro/records/create-records.md).
1. (Condizionale) Se il tipo di record selezionato è stato collegato a un oggetto Workfront, passare alla colonna dell&#39;oggetto collegato e passare il puntatore del mouse sulla cella corrispondente al record che si desidera collegare agli oggetti di Workfront, quindi fare clic sul pulsante **+** icona.

   Il **Connetti oggetti** viene visualizzata la casella.

   ![](assets/connect-objects-box-to-select-projects.png)

   Per ulteriori informazioni sulla connessione di tipi di record con oggetti di un&#39;applicazione di terze parti, vedere [Connetti tipi di record](../architecture/connect-record-types.md).

1. Inizia a digitare il nome di un oggetto Workfront nella casella di ricerca, quindi selezionalo quando viene visualizzato nell’elenco

   Oppure

   Seleziona il nome di uno o più oggetti nella casella, quindi fai clic su **Connetti oggetti** nell&#39;angolo superiore destro della casella Connetti oggetti.

   Sono aggiunti i seguenti elementi:

   * Gli oggetti Workfront selezionati vengono aggiunti al campo record collegato.
   * Per ogni campo collegato selezionato durante l&#39;aggiunta dei campi al record collegato viene creato un nuovo campo collegato o un campo di ricerca.
   * Un nuovo tipo di record denominato &quot;&lt; Nome del tipo di oggetto Workfront >&quot; viene creato nello stesso workspace del record Maestro da cui si sta effettuando il collegamento. Il nome dell&#39;oggetto fa parte del nome di questo tipo di record. Ad esempio, il collegamento a progetti Workfront crea il **Progetto** tipo di record in Maestro.

     Si tratta di un tipo di record di sola lettura e visualizza gli oggetti Workfront selezionati nel nuovo campo oggetto collegato creato dal record Maestro. I campi collegati dell&#39;oggetto collegato vengono visualizzati anche nei record Workfront collegati di sola lettura.

     >[!IMPORTANT]
     >
     > Il tipo di record di oggetto Workfront di sola lettura viene creato solo quando singoli progetti vengono aggiunti ai record Maestro. La semplice creazione di una connessione tra un tipo di record Maestro e un tipo di oggetto Workfront non crea il tipo di record Workfront.

     Eventuali informazioni esistenti provenienti dai campi degli oggetti Workfront vengono visualizzate nei campi collegati o di ricerca.

     >[!TIP]
     >
     >
     >* Se è stata abilitata l&#39;impostazione Consenti più record, i valori dei diversi oggetti vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.
     >
     >* Non viene creato un campo record collegato ai record collegati Maestro per gli oggetti Workfront collegati in Workfront.


1. (Facoltativo) Chiudi la pagina Tipo di record Maestro e passa all’area di lavoro selezionata.
1. Fare clic sulla scheda del tipo di record oggetto Workfront. Ad esempio, fai clic su **progetto Workfront** se hai collegato a progetti Workfront. La scheda del tipo di record Workfront di sola lettura deve aprirsi nella visualizzazione Tabella.

   >[!NOTE]
   >
   >    * I record elencati nella pagina Tipo di record di Workfront sono oggetti Workfront di sola lettura. Anche i campi collegati dal tipo di record Workfront vengono visualizzati come colonne di sola lettura e vengono compilati automaticamente quando vengono inseriti in Workfront.
   >    * Non è possibile aggiornare manualmente i campi Workfront in Maestro. I campi oggetto Workfront devono essere compilati in Workfront e i valori dei campi vengono visualizzati automaticamente sul record Workfront in Maestro.
   >

1. (Facoltativo) Per aprire la pagina Dettagli record oggetto Workfront in Maestro, effettuare una delle seguenti operazioni:

   * Dal tipo di record da cui è stato eseguito il collegamento, passare al campo record collegato all&#39;oggetto Workfront e fare clic sul nome dell&#39;oggetto Workfront.
   * Dalla sezione **Tabella** nella visualizzazione della pagina tipo di record di Workfront, fare clic sul nome dell&#39;oggetto Workfront

     Oppure

     Fai clic su **Altro** a destra del nome dell&#39;oggetto Workfront, quindi fare clic su **Visualizza**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   Viene visualizzata la pagina Dettagli Maestro dell&#39;oggetto Workfront collegato. Pagina di sola lettura.

1. (Facoltativo) Per aprire l&#39;oggetto Workfront collegato in Workfront, effettuare una delle seguenti operazioni:

   * Dalla sezione **Tabella** nella visualizzazione della pagina tipo di record di Workfront, fare clic sul nome dell&#39;oggetto Workfront,

   Oppure

   Fai clic su **Altro** a destra del nome dell&#39;oggetto Workfront, quindi fare clic su **Vai all&#39;origine**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Verrà aperta la pagina degli oggetti di Workfront. Se si dispone delle autorizzazioni necessarie, è possibile modificare le informazioni sull&#39;oggetto Workfront.

1. (Facoltativo) Fai clic su **Aggiungi campi** icona ![](assets/add-fields-icon.png) nell&#39;angolo superiore destro della visualizzazione tabella della pagina tipo di record di Workfront per aggiungere o rimuovere campi di Workfront dal tipo di record di Workfront.

   >[!NOTE]
   >
   >  I campi aggiunti o rimossi nella pagina Tipo di record oggetto di Workfront non vengono aggiunti né rimossi dal tipo di record Maestro che si collega al tipo di oggetto di Workfront. I campi sono visibili solo nella pagina del tipo di record Workfront di sola lettura, quindi puoi esaminarli in Maestro.

1. (Facoltativo e condizionale) Se sono stati aggiunti almeno due campi data all&#39;oggetto Workfront, fare clic su **Visualizza** nella pagina tipo di record oggetto di Workfront e selezionare il **Timeline** visualizzare o **Crea visualizzazione** per creare una vista timeline.  Per informazioni, consulta [Gestire la visualizzazione della timeline](/help/quicksilver/maestro/views/manage-the-timeline-view.md).

   Gli oggetti collegati di Workfront vengono visualizzati nella vista timeline.


### Collegare i record Maestro agli oggetti Adobe Experience Manager

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Dopo aver creato una connessione tra un tipo di record Maestro e Adobe Experience Manager Assets, puoi collegare singoli record Maestro ad Experienci Manager di risorse. I campi della risorsa connessi da Experience Manager Assets al momento della creazione della connessione vengono automaticamente popolati sul tipo di record Maestro da cui è stato effettuato il collegamento.

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace da cui si desidera connettere i record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Seleziona un **Tabella** vista da **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.

1. (Facoltativo) Aggiungere singoli record al tipo di record selezionato aggiungendo una nuova riga alla tabella. Per informazioni, consulta [Crea record](../../maestro/records/create-records.md).
1. (Condizionale) Se il tipo di record selezionato è stato collegato a Experience Manager Assets, passare alla colonna dell&#39;oggetto collegato e passare il puntatore del mouse sulla cella corrispondente al record che si desidera collegare ad altri oggetti da Experience Manager, quindi fare clic sul pulsante **+** icona.

   Il **Seleziona risorse** viene visualizzata la casella. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Per ulteriori informazioni sulla connessione di tipi di record con oggetti di un&#39;applicazione di terze parti, vedere [Connetti tipi di record](../architecture/connect-record-types.md).

1. Fai clic su per selezionare alcuni dei seguenti tipi di risorse:

   * Immagini
   * Raccolte
   * Cartelle

   Puoi selezionare più risorse.

   >[!IMPORTANT]
   >
   > Puoi collegare solo le risorse a cui hai accesso per visualizzare in Experience Manager.

1. Clic **Seleziona**.

   Sono aggiunti i seguenti elementi:

   * Le risorse Experienci Manager selezionate vengono aggiunte al campo record collegato.
   * Per ogni campo collegato selezionato durante l&#39;aggiunta dei campi al record collegato viene creato un nuovo campo collegato o un campo di ricerca.
   * Un nuovo tipo di record denominato &quot;Experience Manager Assets&quot; viene creato nello stesso spazio di lavoro del record Maestro da cui si sta effettuando il collegamento.

     Si tratta di un tipo di record di sola lettura e visualizza gli oggetti Experienci Manager selezionati nel nuovo campo oggetto collegato creato dal record Maestro. I campi collegati dell&#39;oggetto collegato vengono visualizzati anche nei record di Experience Manager collegati di sola lettura.

     >[!IMPORTANT]
     >
     > Il tipo di record Experience Manager Assets di sola lettura viene creato solo quando le singole risorse vengono aggiunte ai record Maestro. La semplice creazione di una connessione tra un tipo di record Maestro e Experience Manager Assets non crea il tipo di record Experience Manager Assets.

     Eventuali informazioni esistenti provenienti dai campi delle risorse Experience Manager vengono visualizzate nei campi collegati o di ricerca.

     >[!TIP]
     >
     >
     >* Se è stata attivata l&#39;impostazione Consenti più record, i valori dei diversi oggetti vengono visualizzati separati da virgole.
     >
     >* Non viene creato un campo record collegato ai record collegati Maestro per le risorse Experienci Manager collegate nell’applicazione Experience Manager Assets.


1. (Facoltativo) Chiudi la pagina Tipo di record Maestro e passa all’area di lavoro selezionata.
1. Fare clic sulla scheda del tipo di record Experience Manager Assets. La scheda del tipo di record Experience Manager Assets di sola lettura deve aprirsi nella visualizzazione Tabella.

   >[!NOTE]
   >
   >    * I record elencati nella pagina Tipo di record di Experience Manager Assets sono risorse di sola lettura. Anche i campi collegati dal tipo di record Experience Manager Assets vengono visualizzati come colonne di sola lettura e vengono compilati automaticamente quando vengono compilati in Experience Manager.
   >    * Non è possibile aggiornare manualmente i campi Experience Manager in Maestro. I campi delle risorse di Experience Manager devono essere compilati in Experience Manager e i valori dei campi vengono visualizzati automaticamente sul record Experience Manager Assets in Maestro.
   >

1. (Facoltativo) Vai al tipo di record da cui hai collegato Experience Manager Assets e fai clic sul nome di una risorsa nel campo del record collegato. I dettagli di Experience Manager della risorsa vengono visualizzati in una finestra a comparsa. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Per un file di immagine vengono visualizzati i seguenti campi:

   * Miniatura dell&#39;immagine
   * Nome del file di immagine
   * Dimension
   * Dimensione
   * Descrizione
   * Percorso del file nell’Experience Manager
   * Tipo di risorsa
   * Data di creazione
   * Data modificata

1. (Facoltativo) Per aprire la pagina Dettagli record Experience Manager Assets in Maestro, effettuare le seguenti operazioni:

   1. Vai a **Experience Manager Assets** Scheda del tipo di record Maestro nello stesso workspace selezionato in origine e fare clic per aprire la pagina del tipo di record.
La pagina del tipo di record Experience Manager Assets Maestro è di sola lettura.
   1. Dalla vista tabella, fai clic sul nome di una risorsa

      Oppure

      Passa il puntatore del mouse sul nome di una risorsa, fai clic su **Altro** menu ![](assets/more-menu.png) a destra del nome della risorsa, quindi fai clic su **Visualizza**.\
      Questo apre il Maestro della risorsa **Dettagli** pagina. Pagina di sola lettura.
1. (Facoltativo) Per aprire la pagina Dettagli record cespiti di Experience Manager in Experience Manager, effettuare una delle seguenti operazioni:

   * Vai alla pagina del tipo di record Maestro del record da cui stai effettuando il collegamento, fai clic sul nome di una risorsa nel campo del record collegato per aprire la finestra a comparsa, quindi fai clic su **Apri** icona ![](assets/open-asset-icon.png) per aprire la risorsa.
   * Vai a **Experience Manager Assets** Carta Maestro del tipo di record nello stesso spazio di lavoro che hai selezionato originariamente e fai clic per aprire la pagina del tipo di record, fai clic sul nome di una risorsa per aprire Maestro **Dettagli** , quindi fai clic su **Vai all&#39;origine** nell&#39;angolo superiore destro dello schermo.

     ![](assets/go-to-source-asset-maestro-details-page.png)
   * Vai a **Experience Manager Assets** La scheda del tipo di record Maestro si trova nello stesso workspace selezionato in origine e fai clic sulla scheda per aprire la pagina del tipo di record di Experience Manager Assets, passa il puntatore del mouse sul nome di una risorsa e fai clic sulla **Altro** , quindi fai clic su **Vai all&#39;origine**.

     ![](assets/go-to-source-option-on-table-view.png)

   La risorsa viene aperta in Experience Manager Assets.

1. (Facoltativo) Fai clic su **Aggiungi campi** icona ![](assets/add-fields-icon.png) per aggiungere o rimuovere campi di Experience Manager nell&#39;angolo superiore destro della visualizzazione tabella della pagina tipo di record di Experience Manager Assets.

   >[!NOTE]
   >
   >  I campi aggiunti o rimossi nella pagina del tipo di record di Experience Manager Assets non vengono aggiunti né rimossi dal tipo di record Maestro che collega alla risorsa Experience Manager. I campi sono visibili solo nella pagina del tipo di record Experience Manager Assets di sola lettura, quindi puoi esaminarli in Maestro.

1. (Facoltativo e condizionale) Se hai aggiunto almeno due campi data alla risorsa collegata dell’Experience Manager, fai clic su **Visualizza** nella pagina tipo di record di Experience Manager Assets e selezionare il **Timeline** visualizzare o **Crea visualizzazione** per creare una vista timeline.  Per informazioni, consulta [Gestire la visualizzazione della timeline](/help/quicksilver/maestro/views/manage-the-timeline-view.md).
Le risorse collegate di Experience Manager Assets vengono visualizzate nella vista timeline.