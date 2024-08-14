---
title: Connetti record
description: Dopo aver creato connessioni tra tipi di record, è possibile collegare tra loro singoli record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '2495'
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

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connetti record

{{planning-important-intro}}

È possibile collegare tra loro record di Adobe Workfront Planning o a oggetti di altre applicazioni.

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

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Per collegare i record di Adobe Workfront Planning a Experience Manager Assets, è necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience. Per informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
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
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un'area di lavoro per connettere i record </p>  
   <p>Consente di visualizzare o autorizzazioni superiori per un'area di lavoro per visualizzare tutte le connessioni a oggetti e campi da altre applicazioni, indipendentemente dall'accesso all'altra applicazione. </p>
   <p>Visualizza o autorizzazioni superiori per gli oggetti che si desidera collegare da Workfront o Experience Manager Assets. </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle che non hanno creato.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerazioni sulla connessione dei record

* Dopo aver connesso i tipi di record, i tipi di record collegati vengono visualizzati come campi di record collegati nella tabella dei tipi di record da cui sono collegati e nelle pagine dei record.
* È possibile sfogliare e aggiungere record e oggetti dei tipi di record e oggetti collegati dai campi dei record collegati.
* È possibile aggiungere campi (campi di ricerca) dei tipi di record collegati nella tabella del tipo di record da cui si sta effettuando il collegamento.

  È possibile aggiungere campi (campi di ricerca) dei tipi di record da cui si esegue il collegamento nella tabella del tipo di record a cui si esegue il collegamento.

  Ad esempio, se colleghi il tipo di record Prodotto dal tipo di record Campagna, puoi visualizzare i campi Prodotto per le campagne e Campagna per i prodotti.
* Non è possibile aggiornare manualmente i valori dei campi di ricerca nei record da cui si sta effettuando il collegamento.

  I valori dei campi di ricerca dei record collegati popolano il record di Workfront Planning da cui si sta effettuando il collegamento automatico dal record o dall&#39;oggetto originale.

* Tutti coloro che dispongono dell&#39;accesso a Workfront Planning and View o delle autorizzazioni di livello superiore per l&#39;area di lavoro possono visualizzare le connessioni tra record o tra record e oggetti di altre applicazioni. Possono visualizzare i record e gli oggetti connessi indipendentemente dalle autorizzazioni di cui dispongono nelle applicazioni a cui ci si connette.
* Se si dispone delle autorizzazioni di gestione per l&#39;area di lavoro in cui si trovano i record connessi, è possibile visualizzare e modificare le connessioni di tutti gli altri utenti.
* È possibile connettere un record a uno o più oggetti di un&#39;altra applicazione.
* È possibile connettere oggetti da Workfront a record di Workfront Planning nelle seguenti aree:
   * Da un record Planning in Workfront Planning.
   * Dalla sezione Planning di un oggetto Workfront.

* È possibile collegare i record di Workfront Planning a Experience Manager Assets nelle seguenti aree:

   * Da un record di Planning in Workfront Planning

## Prerequisiti per il collegamento di record

Per collegare record ad altri record o oggetti, è necessario disporre dei seguenti elementi:

* Almeno un&#39;area di lavoro, tipo di record e record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)
   * [Crea record](/help/quicksilver/planning/records/create-records.md)

* Connessioni tra tipi di record o tra tipi di record e oggetti di altre applicazioni. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

## Connetti record da Workfront Planning

### Collegare i record di Adobe Workfront Planning

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Fare clic sul nome di una visualizzazione **Tabella** per aprirla.
1. (Facoltativo) Aggiungere record al tipo di record selezionato aggiungendo una nuova riga alla tabella. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
1. (Condizionale) Dopo aver collegato il tipo di record selezionato con un altro tipo di record, passare alla colonna del record collegato e fare doppio clic sulla cella corrispondente al record che si desidera collegare con altri record.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Esegui una delle operazioni seguenti:

   * Fare clic sul nome di un record connesso nell&#39;elenco per aggiungerlo al record selezionato. Il record viene aggiunto automaticamente.
   * Iniziare a digitare il nome di un record e fare clic su di esso quando viene visualizzato nell&#39;elenco. Il record viene aggiunto automaticamente.

   <!--1. (Optional) If you cannot find a record to connect, and you want to add it, click **+ Add** to add a new record. For more information, see the "Create records by connecting them" in the article [Create records](/help/quicksilver/planning/records/create-records.md). -->

   >[!TIP]
   >
   >    È possibile aprire la pagina di un record facendo clic sul nome del record nella visualizzazione, trovare il campo record collegato e fare doppio clic sul campo (se sono già presenti record connessi) oppure fare clic su **Connetti record** (se il campo è vuoto) per aggiungere record dal record o dal tipo di oggetto connesso.
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
   >* Se è stata abilitata l&#39;impostazione **Consenti più record** quando sono stati connessi i tipi di record, i valori dei campi per i più oggetti selezionati vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.

1. (Facoltativo) Chiudere la pagina del tipo di record e passare all&#39;area di lavoro selezionata.
1. Fare clic sulla scheda del tipo di record a cui si è collegati.

   Ad esempio, se hai connesso il record **Campaign** al record Prodotto, fai clic sulla scheda **Prodotto**.

   La scheda del tipo di record deve aprirsi nella vista Tabella. In caso contrario, selezionare una vista tabella.

   Il campo record collegato **Campagna** visualizza i nomi delle campagne collegate ai prodotti nella pagina Tipo record prodotto. L’aggiornamento delle informazioni della campagna aggiorna automaticamente il campo del record collegato della campagna per il tipo di record Prodotto.

### Collegare i record di Adobe Workfront Planning agli oggetti Workfront

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
   >* Quando si abilita l&#39;impostazione Consenti più record, i valori dei campi di ricerca vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.
   >
   >* Non viene creato un campo record collegato per gli oggetti Workfront collegati in Workfront.

1. (Facoltativo) Nella vista a tabella del tipo di record, posizionare il puntatore del mouse sull&#39;intestazione di colonna dell&#39;oggetto Workfront collegato e fare clic sul menu a discesa, quindi scegliere **Modifica campi di ricerca**.

1. Aggiungi campi oggetto Workfront dall&#39;area **Campi non selezionati**

   Oppure

   Rimuovi i campi oggetto Workfront dall&#39;area **Campi selezionati**.

   Questa operazione consente di aggiungere o rimuovere campi collegati dai record di Workfront Planning. Le informazioni associate ai campi rimossi rimangono in Workfront.


### Collegare i record di Workfront Planning agli oggetti di Adobe Experience Manager

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
     >* Se è stata abilitata l&#39;impostazione Consenti più record, i valori dei diversi oggetti vengono visualizzati separati da virgole o aggregati in base all&#39;aggregatore scelto.
     >
     >* Non viene creato un campo record collegato ai record collegati di Workfront Planning per le risorse Experienci Manager collegate nell&#39;applicazione Experience Manager Assets.

1. (Facoltativo) Vai al tipo di record da cui hai collegato Experience Manager Assets e fai clic sul nome di una risorsa nel campo del record collegato. I dettagli di Experience Manager della risorsa vengono visualizzati in una finestra a comparsa. <!--update screen shot with hi-rez picture-->

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

## Connetti record da oggetti Workfront

Per connettere i record di Workfront Planning dagli oggetti di Workfront, è necessario disporre delle seguenti informazioni:

* Connessioni tra tipi di record e tipi di oggetti Workfront.
* Almeno una connessione tra un record e un oggetto Workfront.
* L&#39;amministratore del Workfront o del gruppo deve aggiungere la sezione Planning ai tipi di oggetto di Workfront che possono connettersi ai tipi di record di Planning.

Per ulteriori informazioni, vedere [Gestire i record nella sezione Pianificazione degli oggetti Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
