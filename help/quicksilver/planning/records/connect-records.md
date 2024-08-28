---
title: Collega record
description: Dopo aver creato connessioni tra tipi di record, è possibile collegare tra loro singoli record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: a3006a05b7003e638596c2754b77e914083a5643
workflow-type: tm+mt
source-wordcount: '2714'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting records to one another, you can also connect records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->


# Connetti record

{{planning-important-intro}}

È possibile collegare tra loro record di Adobe Workfront Planning o a oggetti di altre applicazioni.

Questo articolo descrive come collegare i record. Per ulteriori informazioni generali sulla connessione dei record, vedere [Panoramica sui record collegati](/help/quicksilver/planning/records/connected-records-overview.md).

È innanzitutto necessario collegare due tipi di record tra loro o un tipo di record a un tipo di oggetto di un&#39;altra applicazione. In questo modo vengono creati campi record collegati. È quindi possibile collegare record tra loro o record ad altri oggetti da altre applicazioni utilizzando i campi dei record collegati.

La connessione dei record è simile alla connessione dei record agli oggetti di un&#39;altra applicazione.

Per informazioni sulla connessione di tipi di record tra loro o a tipi di oggetto da altre applicazioni, vedere [Connettere tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

Per un esempio di connessione dei tipi di record, vedere [Esempio di connessione dei tipi di record e dei record](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

È possibile connettere i seguenti elementi:

* Record di Adobe Workfront Planning
* Adobe Workfront Planning registra gli oggetti di altre applicazioni.

  È possibile collegare record agli oggetti dei tipi elencati di seguito dalle applicazioni seguenti:

   * Adobe Workfront

      * Progetti
      * Portfolio
      * Programmi
      * Azienda
      * Gruppo

   * Adobe Experience Manager Assets

      * File immagine
      * Cartelle

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<p>Qualsiasi </p> 
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
   <td> Standard
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
   <td>   <p>Gestire le autorizzazioni per un'area di lavoro per connettere i record </p>  
   <p>Consente di visualizzare o autorizzazioni superiori per un'area di lavoro per visualizzare tutte le connessioni a oggetti e campi da altre applicazioni, indipendentemente dall'accesso all'altra applicazione. </p>
   <p>Visualizza o autorizzazioni superiori per gli oggetti che si desidera collegare da Workfront o Experience Manager Assets. </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle che non hanno creato.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>To connect Adobe Workfront Planning records with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace to connect records </p>  
   <p>View or higher permissions to a workspace to view all connections to objects and fields from other applications, regardless of your access in the other application. </p>
   <p>View or higher permissions to the objects you want to link from Workfront or Experience Manager Assets. </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++

## Prerequisiti per la connessione dei record

Per collegare i record ad altri record o oggetti, è necessario disporre dei seguenti elementi:

* Almeno un&#39;area di lavoro, tipo di record e record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)
   * [Crea record](/help/quicksilver/planning/records/create-records.md)

* Connessioni tra tipi di record o tra tipi di record e oggetti di altre applicazioni. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

## Connetti record da Workfront Planning

È possibile collegare record da Workfront Planning nelle seguenti aree di un record Planning:

* Campi record connessi nella visualizzazione tabella.
* L&#39;anteprima o la pagina del record nei campi del record collegato nella scheda Dettagli.
* L&#39;anteprima o la pagina del record nella scheda Connessioni.

### Collegare i record di Adobe Workfront Planning dalla vista tabella o dalla scheda Dettagli della pagina record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Fare clic sul nome di una vista tabella per aprirla.
1. (Facoltativo) Aggiungere record al tipo di record selezionato aggiungendo una nuova riga alla tabella. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
1. (Condizionale) Dopo aver collegato il tipo di record selezionato con un altro tipo di record, passare alla colonna del record collegato e fare doppio clic sulla cella corrispondente al record che si desidera collegare con altri record.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Esegui una delle operazioni seguenti:

   * Fare clic sul nome di un record connesso nell&#39;elenco per aggiungerlo al record selezionato. Il record viene aggiunto automaticamente.
   * Iniziare a digitare il nome di un record e fare clic su di esso quando viene visualizzato nell&#39;elenco. Il record viene aggiunto automaticamente.

1. (Facoltativo) Se non è possibile trovare un record o un oggetto da connettere e si desidera aggiungerlo, fare clic su **+ Aggiungi** per aggiungere un nuovo record. Per ulteriori informazioni, vedere l&#39;articolo [Creare record](/help/quicksilver/planning/records/create-records.md) in cui è possibile creare record durante la connessione.

   >[!TIP]
   >
   >    È possibile aprire la pagina di un record e connettere altri record eseguendo le operazioni seguenti nella vista a tabella:
   >1. Fare clic sul nome del record nella visualizzazione.
   >1. Trovare il campo record collegato e fare doppio clic sul campo (se sono già presenti record connessi)
   >Oppure
   >Fare clic su **Connetti record** (se il campo è vuoto) per aggiungere record dal record o dal tipo di oggetto connesso.
   >
   >![](assets/connect-records-from-record-page-field.png)

1. (Facoltativo) Fai clic su **Visualizza tutti** per visualizzare tutti i record.

1. (Condizionale) Se hai fatto clic su **Visualizza tutti** nel passaggio precedente, viene visualizzata la casella **Connetti oggetti**.

   ![](assets/connected-objects-table-for-records.png)

1. Iniziare a digitare il nome di un record nella casella di ricerca, quindi selezionarlo quando viene visualizzato nell&#39;elenco

   Oppure

   Selezionare il nome di uno o più record nella casella, quindi fare clic su **Connetti oggetti**.

   Sono aggiunti i seguenti elementi:

   * I record collegati vengono visualizzati nel campo record collegato del record selezionato in un passaggio precedente.
   * I campi collegati vengono compilati con le informazioni dei record collegati, se sono stati aggiunti campi di ricerca collegati al momento della connessione dei tipi di record.

   L&#39;aggiornamento dei record collegati aggiorna automaticamente i campi collegati per i record da cui si sta effettuando il collegamento. Non è possibile modificare manualmente i campi collegati.

   >[!TIP]
   >
   >* Utilizziamo &quot;campi collegati&quot; e &quot;campi di ricerca&quot; in modo intercambiabile.
   >
   >* Quando si sceglie di connettere più record durante la connessione dei tipi di record, i valori dei campi dei diversi oggetti vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto durante la connessione dei tipi di record.

1. (Facoltativo) Chiudere la pagina del tipo di record e passare all&#39;area di lavoro selezionata.
1. Fare clic sulla scheda del tipo di record a cui si è collegati.

   Ad esempio, se hai connesso il record **Campaign** al record Prodotto, fai clic sulla scheda **Prodotto**.

   La scheda del tipo di record deve aprirsi nella vista tabella. In caso contrario, selezionare una vista tabella.

   Il campo record collegato **Campagna** visualizza i nomi delle campagne collegate ai prodotti nella pagina Tipo record prodotto. L’aggiornamento delle informazioni della campagna aggiorna automaticamente il campo del record collegato della campagna per il tipo di record Prodotto.

### Collegare i record di Adobe Workfront Planning agli oggetti di Workfront dalla vista tabella o dalla scheda Dettagli della pagina record

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Dopo aver creato una connessione tra un tipo di record e un tipo di oggetto Workfront, è possibile collegare singoli record agli oggetti in Workfront. I campi Workfront connessi vengono automaticamente compilati nei record da cui si collegano gli oggetti.

>[!NOTE]
>
>Non è possibile connettere tipi di oggetto Workfront con tipi di record di Workfront Planning da Workfront.


{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Selezionare una visualizzazione **Tabella** dal menu a discesa **Visualizzazione**.

1. Fare clic su **Nuovo record** per aggiungere singoli record al tipo di record selezionato. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

1. (Condizionale) Dopo aver collegato il tipo di record selezionato a un tipo di oggetto Workfront, passare alla colonna oggetto collegato e fare doppio clic sulla cella corrispondente al record che si desidera collegare agli oggetti da Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Esegui una delle operazioni seguenti:

   * Fare clic su un oggetto dall&#39;elenco per aggiungerlo al record selezionato. Gli oggetti sono elencati in ordine alfabetico. L&#39;oggetto viene aggiunto automaticamente.
   * Iniziare a digitare il nome di un oggetto e fare clic su di esso quando viene visualizzato nell&#39;elenco. L&#39;oggetto viene aggiunto automaticamente.

   >[!TIP]
   >
   >È possibile aprire la pagina di un record dalla visualizzazione, fare doppio clic sul campo del record collegato oppure fare clic su **Connetti** nel campo per aggiungere oggetti dal tipo di oggetto connesso.

1. (Facoltativo) Se non riesci a trovare un oggetto da connettere e vuoi aggiungerlo, fai clic su **+ Aggiungi** per creare e aggiungere un nuovo progetto o portfolio.

   È possibile aggiungere progetti senza un modello o portafogli solo quando si collegano ai record di Planning. Non è possibile aggiungere nuovi programmi, utenti o società.

1. (Facoltativo) Fai clic su **Visualizza tutti** per visualizzare tutti gli oggetti per i quali disponi almeno delle autorizzazioni di visualizzazione.

1. (Condizionale) Se hai fatto clic su **Visualizza tutti** nel passaggio precedente, viene visualizzata la casella **Connetti oggetti**.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Inizia a digitare il nome di un oggetto Workfront nella casella di ricerca, quindi selezionalo quando viene visualizzato nell’elenco

   Oppure

   Selezionare il nome di uno o più oggetti nella casella, quindi fare clic su **Connetti oggetti**.

   >[!IMPORTANT]
   >
   >* È possibile aggiungere solo oggetti Workfront a cui si ha accesso per la visualizzazione.
   >
   >* Dopo aver aggiunto gli oggetti Workfront, tutti gli utenti con autorizzazioni di visualizzazione o superiori all&#39;area di lavoro possono visualizzare gli oggetti Workfront e le relative informazioni di campo, indipendentemente dalle autorizzazioni o dall&#39;accesso in Workfront.

   Sono aggiunti i seguenti elementi:

   * Gli oggetti Workfront selezionati vengono aggiunti al campo record collegato.
   * Se sono stati aggiunti quando il tipo di record è stato connesso a Workfront, i campi collegati (o i campi di ricerca) degli oggetti Workfront vengono automaticamente compilati con le informazioni di Workfront.

   Per ulteriori informazioni sulla connessione di tipi di record con oggetti di un&#39;altra applicazione, vedere [Connettere tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Facoltativo) Fare clic sul nome di un oggetto Workfront connesso a un record di Workfront Planning nel campo collegato di una vista tabella o nel campo collegato della pagina del record.

   Se si dispone almeno delle autorizzazioni di visualizzazione per l&#39;oggetto, verrà aperto l&#39;oggetto Workfront in Workfront.

   >[!TIP]
   >
   >* Quando si sceglie di connettere più record durante la connessione dei tipi di record, i valori dei campi di ricerca vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.
   >
   >* Non viene creato un campo record collegato per gli oggetti Workfront collegati in Workfront.

1. (Facoltativo) Nella vista a tabella del tipo di record, posizionare il puntatore del mouse sull&#39;intestazione di colonna dell&#39;oggetto Workfront collegato e fare clic sul menu a discesa, quindi scegliere **Modifica campi di ricerca**.

1. Aggiungi campi oggetto Workfront dall&#39;area **Campi non selezionati**

   Oppure

   Rimuovi i campi oggetto Workfront dall&#39;area **Campi selezionati**.

   Questa operazione consente di aggiungere o rimuovere campi collegati dai record di Workfront Planning. Le informazioni associate ai campi rimossi rimangono in Workfront.


### Collegare i record di Workfront Planning agli oggetti di Adobe Experience Manager dalla vista tabella o dalla scheda Dettagli della pagina record

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>È necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console per poter collegare i record di Workfront Planning ad Adobe Experience Manager Assets.
>
>Se hai domande sull&#39;onboarding in Adobe Admin Console, consulta le [Domande frequenti sull&#39;esperienza unificata di Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Dopo aver creato una connessione tra un tipo di record e Adobe Experience Manager Assets, puoi collegare singoli record alle risorse di Experience Manager. I campi della risorsa connessi da Experience Manager Assets al momento della creazione della connessione vengono compilati automaticamente sul tipo di record da cui è stato effettuato il collegamento.

>[!NOTE]
>
>I record di pianificazione e i relativi campi sono accessibili da Experience Manager Assets quando l’amministratore Workfront configura la mappatura dei metadati tramite l’integrazione tra Workfront e Adobe Experience Manager Assets. Per ulteriori informazioni, consulta [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

Per collegare i record con le risorse AEM:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Selezionare una visualizzazione **Tabella** dal menu a discesa **Visualizzazione** nell&#39;angolo superiore destro della pagina del tipo di record.

1. (Facoltativo) Fare clic su **Nuovo record** per aggiungere nuovi record al tipo di record selezionato. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
1. (Condizionale) Dopo aver connesso il tipo di record selezionato con Experience Manager Assets, passa alla colonna dell&#39;oggetto collegato e passa il puntatore del mouse sulla cella corrispondente al record che desideri collegare ad altri oggetti da Experience Manager, quindi fai clic sull&#39;icona **+**.

   >[!TIP]
   >
   >  È possibile aggiungere fare clic sull&#39;icona **+** nel campo oggetto collegato nella pagina del record per connettere le risorse al record.

   Viene visualizzata la casella **Seleziona Assets**. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Fai clic su per selezionare alcuni dei seguenti tipi di risorse:

   * Immagini
   * Cartelle

   Puoi selezionare più risorse.

   >[!IMPORTANT]
   >
   > Puoi collegare solo le risorse a cui hai accesso per visualizzare in Experience Manager. Una volta connessi, tutti gli utenti di Workfront Planning possono visualizzare le risorse in Workfront Planning, indipendentemente dal loro accesso in Experience Manager Assets.

1. Fai clic su **Seleziona**. <!-- we might change this to Connect-->

   Sono aggiunti i seguenti elementi:

   * Le risorse Experienci Manager selezionate vengono aggiunte al campo record collegato.
   * I campi collegati (o campi di ricerca) si compilano con le informazioni provenienti dall’Experience Manager risorse collegate.

     Eventuali informazioni esistenti provenienti dai campi delle risorse Experience Manager vengono visualizzate automaticamente nei campi collegati o di ricerca.

     >[!TIP]
     >
     >* Quando si sceglie di connettere più record durante la connessione dei tipi di record, i valori dei diversi oggetti vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.
     >
     >* Non viene creato un campo record collegato ai record collegati di Workfront Planning per le risorse Experienci Manager collegate nell&#39;applicazione Experience Manager Assets.

1. (Facoltativo) Vai al tipo di record da cui hai collegato Experience Manager Assets e fai clic sul nome di una risorsa nel campo del record collegato. I dettagli di Experience Manager della risorsa vengono visualizzati in una finestra a comparsa.

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Per un file di immagine vengono visualizzati i seguenti campi:

   * Miniatura dell&#39;immagine
   * Nome del file di immagine
   * Dimensioni
   * Dimensione
   * Descrizione
   * Percorso del file nell’Experience Manager
   * Tipo di risorsa
   * Data di creazione
   * Data modificata

1. (Facoltativo) Per aprire la pagina di record Experience Manager assets in Experience Manager, vai alla pagina del tipo di record del record da cui stai effettuando il collegamento, fai clic sul nome di una risorsa nel campo del record collegato per aprire la finestra a comparsa, quindi fai clic sull&#39;icona **Apri in AEM** ![](assets/open-asset-icon.png) per aprire la risorsa.

   Verrà aperta la risorsa Experience Manager in Adobe Experience Manager Assets.

1. (Facoltativo) Nella vista a tabella del tipo di record, passa il puntatore del mouse sull&#39;intestazione di colonna della risorsa di Experience Manager collegata e fai clic sul menu a discesa, quindi fai clic su **Modifica campi di ricerca**.

1. Aggiungi campi oggetto Experience Manager Assets dall&#39;area **Campi non selezionati**

   Oppure

   Rimuovi i campi oggetto Workfront dall&#39;area **Campi selezionati**.

   Questa operazione consente di aggiungere o rimuovere campi collegati dai record. Le informazioni associate ai campi rimossi rimangono in Adobe Experience Assets.

### Collegare i record di Workfront Planning ad altri record o oggetti dalla scheda Connessioni della pagina dei record

1. Passare a una visualizzazione di un tipo di record connesso ad altri tipi di record o tipi di oggetto di Planning da altre applicazioni.
1. Seguire i passaggi descritti nelle sottosezioni precedenti per trovare un record nella visualizzazione che si desidera connettere ad altri record o oggetti.
1. Fare clic sul nome di un record.

   Viene visualizzata la pagina di anteprima.
1. (Facoltativo) Fai clic sull&#39;icona ![](assets/open-details-in-a-new-tab-icon.png) di **Apri in una nuova scheda** per aprire la pagina del record.
1. Fare clic sulla scheda **Connessioni** nell&#39;anteprima o nella pagina del record.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

   Tutti i tipi di record o di oggetti collegati al tipo di record selezionato vengono visualizzati come sezioni. I record o gli oggetti collegati vengono visualizzati sotto i nomi dei record o dei tipi di oggetto sulle schede.

   >[!TIP]
   >
   >    Per impostazione predefinita, vengono visualizzati solo i record connessi con singoli record.

1. (Facoltativo) Fare clic su **Mostra tutte le connessioni** per visualizzare tutti i tipi di record connessi, inclusi quelli senza record connessi.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a sinistra di una sezione per comprimerla.

1. (Condizionale) Fare clic su **Connetti** per aggiungere altri record o oggetti dello stesso tipo.
1. Seguire i passaggi descritti nelle sezioni precedenti per connettere i record da Workfront Planning o gli oggetti da Workfront o Experience Manager Assets.
I record e gli oggetti vengono aggiunti immediatamente.
1. (Facoltativo) Passa il puntatore del mouse sulla scheda connessa di un record o di un oggetto, quindi fai clic sull&#39;icona **Disconnetti record** **-** per disconnetterlo dal record selezionato.

   ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   Il record viene immediatamente disconnesso da tutte le aree di Workfront Planning o da altre applicazioni in cui potrebbe essere visualizzato come connesso. Vengono rimossi anche eventuali valori dei campi di ricerca.

## Connetti record da oggetti Workfront

Per connettere i record di Workfront Planning dagli oggetti di Workfront, è necessario disporre delle seguenti informazioni:

* Connessioni tra tipi di record e tipi di oggetto Workfront stabiliti in Workfront Planning.
* L&#39;amministratore del Workfront o del gruppo deve aggiungere la sezione Pianificazione ai progetti, ai portfolio e ai programmi Workfront nel modello di layout.

Per ulteriori informazioni, vedere [Gestire i record nella sezione Pianificazione degli oggetti Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
