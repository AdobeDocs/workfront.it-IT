---
title: Collega tipi di record
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record di Adobe Workfront Planning con i tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere lo stato attivo in un'unica applicazione.
feature: Workfront Planning
role: User
author: Alina
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 743dbef27149f42ee2328e45a76be660657a75bb
workflow-type: tm+mt
source-wordcount: '2137'
ht-degree: 1%

---


# Connetti tipi di record

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

È possibile connettere tipi di record tra loro o tipi di record con tipi di oggetto di altre applicazioni.

Questo articolo descrive come collegare due tipi di record di Workfront Planning o un tipo di record di Workfront Planning a un oggetto di un&#39;altra applicazione.

Dopo aver stabilito la connessione tra i record o i tipi di oggetto, è possibile collegare tra loro singoli record e visualizzare i campi del record o dei tipi di oggetto collegati in un record di Workfront Planning.

Per informazioni generali sui tipi di connessione, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Per informazioni sulla connessione di record o record con oggetti di altre applicazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

Per un esempio di connessione di tipi di record e record, vedere [Esempio di connessione di tipi di record e record](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <td> <p>Standard</p> 
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
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle che non hanno creato.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
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
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Connetti tipi di record

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della visualizzazione tabella, quindi fai clic sulla scheda **Nuova connessione**.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Nel campo **Tipo di record**, cercare un tipo di record oppure selezionare uno dei tipi seguenti:

   * Un altro tipo di record dall&#39;area di lavoro selezionata

     ![](assets/new-connection-tab-fields-with-another-record-selected.png)

     >[!TIP]
     >
     > 
     >Se nell&#39;area di lavoro selezionata non sono presenti altri tipi di record, la sezione area di lavoro non viene visualizzata.


   * Tipo di record di un&#39;altra area di lavoro configurata per la connessione da altre aree di lavoro. Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

     >[!TIP]
     >
     >Se non sono presenti tipi di record configurati per la connessione da un&#39;altra area di lavoro, la sezione area di lavoro non viene visualizzata.


   * **Progetto, Portfolio, Programma, Società** o **Gruppo** dalla sezione **Tipi di oggetti di Workfront**.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** dalla sezione **Adobe Applications**.

     ![](assets/aem-assets-connection-selection.png)

1. Aggiorna le seguenti informazioni:

   * **Nome**: il nome del campo connesso che verrà visualizzato nella visualizzazione tabella o nella pagina record del tipo di record originale. In questo modo viene creata la colonna del record collegato nella vista a tabella del tipo di record originale o del campo del record collegato per i record originali. Per impostazione predefinita, il nome del campo corrisponde al nome del record o dell&#39;oggetto a cui ci si connette.

   >[!TIP]
   >
   >È possibile avere più connessioni allo stesso record o tipo di oggetto. Se non si modifica il nome del campo connesso, Workfront aggiunge un numero dopo il nome del record connesso per indicare il numero di tipi di record connessi in base allo stesso nome.

   * **Descrizione**: informazioni aggiuntive sul campo record connesso. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Consenti più record**: selezionare questa opzione per indicare che gli utenti possono aggiungere più record quando il campo del tipo di record collegato viene visualizzato nei record originali. Questa opzione è selezionata per impostazione predefinita.

     Questa opzione è disponibile solo quando si collegano record di due aree di lavoro diverse o un record e un oggetto risorsa di Adobe Experience Manager.

     ![](assets/new-connection-allow-multiple-records-box.png)

   * **Tipo di connessione**: selezionare una delle opzioni seguenti per indicare il numero di record a cui è possibile connettersi e da cui connettersi:

      * Da molti a molti
      * Da uno a molti
      * Da molti a uno
      * Da uno a uno

     Questa opzione è disponibile solo quando si connettono record dello stesso workspace o di un record e un tipo di oggetto Workfront.

     ![](assets/many-to-many-connection-picker.png)

     Per ulteriori informazioni sui tipi di connessione, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Seleziona campi di ricerca**: selezionare questa opzione per aggiungere campi dal tipo di record selezionato. I campi di ricerca sono campi associati al record o al tipo di oggetto a cui si sta effettuando il collegamento. Il collegamento consente di visualizzare le informazioni del record o dell&#39;oggetto a cui si sta effettuando il collegamento nel record di cui si desidera creare il collegamento. Questa opzione è selezionata per impostazione predefinita.

     >[!TIP]
     >
     > Non è possibile aggiungere i seguenti tipi di campi come campi di ricerca:
     >
     >    * Persone
     >    * Creato da
     >    * Ultima modifica eseguita da
     >    * Campi typeahead di Workfront (inclusi campi come Proprietario progetto o Sponsor progetto)

1. (Condizionale e facoltativo) Se hai selezionato di connettere un oggetto Workfront, seleziona un **modulo personalizzato** dalla sezione **Collega solo gli oggetti che corrispondono a questi criteri**. Solo gli oggetti a cui sono allegati i moduli personalizzati selezionati possono essere collegati al tipo di record selezionato. È possibile selezionare più moduli.

   >[!NOTE]
   >
   > È necessario creare moduli personalizzati in Workfront per gli oggetti selezionati prima che vengano visualizzati in questo elenco.

1. (Condizionale) Se hai selezionato di connetterti a Experience Manager Assets, seleziona un archivio dal menu a discesa **Experience Manager repository** nella sezione **Collega risorse dal seguente archivio**. Questo campo è obbligatorio. In questo campo vengono visualizzati solo gli archivi a cui hai accesso in Experience Manager Assets.

   >[!NOTE]
   >
   >L&#39;amministratore di Workfront può mappare i campi di Workfront Planning sui campi di Experience Manager Assets tramite la mappatura dei metadati in Workfront. Per ulteriori informazioni, consulta [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Condizionale) Se hai selezionato di connetterti a Experience Manager Assets o a un tipo di record di Workfront Planning, deseleziona l&#39;opzione **Titolo** nell&#39;area **Aspetto record**, se non desideri che il titolo dei record o delle risorse connessi venga visualizzato nel campo collegato. Se questa opzione è deselezionata, nei campi collegati vengono visualizzate solo le miniature dei record. Nei record senza miniatura viene invece visualizzata un&#39;icona di immagine. L’opzione è selezionata per impostazione predefinita. Nell&#39;area **Aspetto del record** viene visualizzato un esempio di visualizzazione dei record connessi.

   >[!TIP]
   >
   >    Se si consente il collegamento di più record, la visualizzazione della sola miniatura potrebbe consentire di risparmiare spazio in aree più piccole, come le visualizzazioni record.
   >
   >Il titolo di un record è il campo principale del record. Per ulteriori informazioni, vedere [Panoramica del campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Fai clic su **Crea**.

1. (Condizionale) Se hai selezionato l&#39;impostazione **Seleziona campo di ricerca**, viene visualizzata la casella **Aggiungi campi di ricerca**.

   Fai clic sull&#39;icona **+** per aggiungere campi dall&#39;area **Campi non selezionati**.

   Oppure

   Fai clic sull&#39;icona **-** per rimuovere i campi dall&#39;area **Campi selezionati**

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   I valori dei campi collegati vengono compilati automaticamente dopo il collegamento di record o oggetti.

   >[!IMPORTANT]
   >
   >    Tutti coloro che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro possono visualizzare le informazioni nei campi collegati, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegati.


1. (Facoltativo) Fai clic su **Ignora** per saltare l&#39;aggiunta di campi dal record o dal tipo di oggetto collegato. Il **Nome** o il **Titolo** del record collegato è l&#39;unico campo visibile nella visualizzazione tabella del tipo di record da cui ci si connette.

1. (Facoltativo e condizionale) Se si seleziona di collegare un campo di tipo numero, valuta, percentuale o data, selezionare anche un valore aggregatore per riepilogare più valori. Quando gli utenti selezionano più record collegati nel campo record collegato, i valori dei campi collegati vengono visualizzati separati da virgole o come valore di riepilogo in base all&#39;aggregatore scelto.

   Se il campo di ricerca contiene più valori che non vengono riepilogati, quando si utilizza il campo in ordinamento o raggruppamento in una visualizzazione tenere presente quanto segue:

   * L’ordinamento viene eseguito dal primo valore

   * I record sono raggruppati per ogni combinazione univoca di valori di campo

   * La vista timeline viene creata in base al primo valore di data.

   >[!IMPORTANT]
   >
   >    Se si desidera che i campi siano disponibili per l&#39;aggiunta come date di inizio e di fine per le visualizzazioni Timeline e Calendario, è necessario selezionare un valore di aggregazione durante l&#39;aggiunta di campi data ricerca. Ad esempio, puoi selezionare MAX o l’aggregatore MIN per un campo data di ricerca.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Gli aggregatori non sono disponibili quando si collegano tipi di record a Experience Manager Assets.

   Selezionare una delle opzioni seguenti:

   * **Nessuno**: visualizza i valori provenienti da più record separati da virgole. Questa è la selezione predefinita.
   * **MAX**: visualizza il valore più alto di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MIN**: visualizza il valore più basso di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **SOMMA**: visualizza il totale di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MEDIA**: visualizza la media di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **UNIQUE**: rimuove i duplicati dai valori dei campi di ricerca e mostra solo i valori univoci. Questa opzione non è disponibile per i tipi di campo seguenti:
      * Paragrafo
      * Casella di controllo
      * Persone

   >[!NOTE]
   >
   >Ad esempio, puoi collegare il record Prodotto (record collegato) dal record Campagna (record originale) e denominarlo &quot;Campo prodotto&quot;. Puoi anche scegliere di collegare il campo Budget del record Prodotto dal record Campagna e chiamarlo &quot;Budget prodotto&quot;. Se è possibile selezionare più record nel &quot;Campo prodotto&quot;, è possibile selezionare il Prodotto 1 con un budget di $ 100.000 e il Prodotto 2 con un budget di $ 110.000 e il Prodotto 3 con un budget di $ 100.000. È possibile visualizzare le seguenti informazioni di Budget nel campo collegato dal record originale, a seconda dell&#39;aggregatore scelto:
   >
   >* **Nessuno**: $100.000, $110.000, $100.000
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SOMMA**: $310.000
   >* **MEDIA**: $103.000,33
   >* **UNIVOCO**: $100.000
   >

1. (Facoltativo) Utilizza l&#39;icona **ricerca** ![](assets/search-icon.png) per cercare un campo.

1. Fai clic su **Aggiungi campi** per salvare le modifiche.

   Sono aggiunti i seguenti elementi:

   * Campo record collegato sul tipo di record da cui si sta eseguendo il collegamento. Nel campo record collegato verranno visualizzati i singoli record del tipo di record collegato, dopo averli aggiunti manualmente. Per informazioni sull&#39;aggiunta di record, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md). Il nome del campo record collegato è il nome selezionato al passaggio 6. <!--accurate-->

   * Campo o campi collegati che visualizzano informazioni sul record o sui tipi di oggetto collegati dopo l&#39;aggiunta manuale dei record o degli oggetti nel campo record collegato. I campi di ricerca vengono creati solo quando l&#39;impostazione **Seleziona campi di ricerca** è selezionata durante la creazione della connessione. I campi di ricerca vengono denominati automaticamente in base a questo modello:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Ad esempio, se hai collegato un tipo di record Campaign con un tipo di record Programma e denomini il campo del record collegato al Programma &quot;Informazioni sul programma&quot;, quindi hai selezionato di visualizzare anche il campo Budget del programma nella vista a tabella di Campaign, il campo collegato viene automaticamente denominato `Budget (from Program information)` nella vista a tabella della campagna.

   * Quando si collegano tra loro tipi di record, viene aggiunto anche un campo record collegato al tipo di record a cui si desidera collegarsi. Il nome del campo record collegato nel tipo di record collegato è il nome del tipo di record da cui si esegue il collegamento.

     Ad esempio, se colleghi il tipo di record &quot;Prodotto&quot; dal tipo di record &quot;Campagna&quot; e denomini il campo connesso della campagna &quot;Prodotto collegato&quot;, viene creato un campo di record collegato &quot;Campagna&quot; per il tipo di record Prodotto.

     >[!TIP]
     >
     > Non viene creato un campo record collegato per gli oggetti di un&#39;altra applicazione al tipo di record da cui si esegue il collegamento in Workfront Planning.

1. (Facoltativo e condizionale) Nella vista tabella del tipo di record originale o del tipo di record collegato fare clic sulla freccia rivolta verso il basso nell&#39;intestazione dei campi del record collegato, quindi scegliere una delle opzioni seguenti:

   * **Modifica campo**: è possibile aggiornare **Nome** e le **Descrizione** informazioni del campo.
   * **Modifica campi di ricerca**: aggiungere o rimuovere i campi del record collegato.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Per aggiungere o rimuovere campi di ricerca, seguire le istruzioni riportate nei passaggi 16-17 precedenti. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Non è possibile aggiungere campi di ricerca appartenenti a tipi di record da cui si esegue il collegamento a tipi di oggetto da un&#39;altra applicazione.
   >
   > Ad esempio, non è possibile aggiungere il campo di ricerca &quot;Stato campagna&quot; a un progetto Workfront a cui ti stai collegando dalle campagne.

1. (Facoltativo) Fai clic sulla freccia rivolta verso il basso nell&#39;intestazione di un campo record collegato o nell&#39;intestazione di un campo di ricerca dal tipo di record da cui stai effettuando il collegamento, quindi fai clic su **Elimina**.

   Il campo record o il campo di ricerca vengono eliminati. Se si elimina un campo record, vengono eliminati anche tutti i campi di ricerca associati al record collegato.
