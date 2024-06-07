---
title: Connetti tipi di record
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record di Adobe Workfront Planning con i tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere lo stato attivo in un'unica applicazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '2249'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Connetti tipi di record

{{planning-important-intro}}

È possibile utilizzare Adobe Workfront Planning per progettare aree di lavoro completamente personalizzabili che contengano i tipi di record necessari nell&#39;organizzazione. Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. È inoltre possibile collegare i tipi di record di Workfront Planning a tipi di oggetto di altre applicazioni per migliorare l&#39;esperienza degli utenti e mantenere l&#39;attenzione in un&#39;unica applicazione.

È possibile connettere tipi di record tra loro o tipi di record con tipi di oggetto di altre applicazioni.

In questo modo è possibile visualizzare i campi del record collegato o del tipo di oggetto in un record di Workfront Planning.

Questo articolo descrive come collegare due tipi di record in Workfront Planning o un tipo di record a un oggetto di un&#39;altra applicazione.

Dopo aver stabilito la connessione tra i record o i tipi di oggetto, è possibile collegare tra loro singoli record.

Per informazioni sulla connessione di un record di Workfront Planning a un oggetto di un&#39;altra applicazione, vedere [Collega record](/help/quicksilver/planning/records/connect-records.md).

Per un esempio di connessione dei tipi di record, vedere [Esempio di connessione di tipi di record e record](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Requisiti di accesso

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
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Per collegare i tipi di record di Adobe Workfront Planning a Experience Manager Assets, è necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata nell’esperienza unificata Adobe. Per informazioni, consulta <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe di esperienza unificata per Workfront</a>.</p> </td>
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
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle che non hanno creato.
</td>
  </tr>
 </tbody>
</table>


<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Considerazioni sulla connessione dei tipi di record

* È possibile connettere le seguenti entità in Adobe Workfront Planning:

   * Due tipi di record

     I tipi di record devono appartenere allo stesso workspace.
   * Tipo di record e tipo di oggetto di un&#39;altra applicazione.

* Con i tipi di record di Workfront Planning è possibile collegare i seguenti tipi di oggetto dalle applicazioni seguenti:

   * Adobe Workfront:

      * Progetti
      * Portfolio
      * Programmi
      * Aziende
      * Gruppi

   * Adobe Experience Manager Assets:

      * Immagini
      * Cartelle

     >[!IMPORTANT]
     >
     >È necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console per collegare i record di Workfront Planning ad Adobe Experience Manager Assets.
     >
     >In caso di domande sull’onboarding per Adobe Admin Console, consulta [Domande frequenti sull’esperienza unificata di Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Dopo aver creato singoli record per un tipo di record, è possibile selezionare i record a cui ci si connette dal campo del tipo di record collegato. Per informazioni, consulta [Collega record](/help/quicksilver/planning/records/connect-records.md).

* Dopo aver collegato un tipo di record a un altro tipo di record o a un tipo di oggetto di un&#39;altra applicazione, si verificano i seguenti scenari:

   * **Quando si collegano due tipi di record**: viene creato un campo record collegato sul tipo di record da cui stai effettuando la connessione. Un campo record collegato simile viene creato nel tipo di record a cui ci si connette.

     Ad esempio, se si collega il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo di record collegato denominato &quot;Prodotto collegato&quot; e nel tipo di record Prodotto viene creato automaticamente un tipo di record collegato denominato &quot;Campagna&quot;.

   * **Quando si collega un tipo di record a un tipo di oggetto di un&#39;altra applicazione**: viene creato un campo record collegato sul tipo di record da cui stai effettuando la connessione. Nessun campo record collegato viene creato automaticamente sul tipo di oggetto dell&#39;altra applicazione.

     Viene creato un nuovo tipo di record di sola lettura di Workfront Planning per l&#39;oggetto dell&#39;altra applicazione solo quando gli oggetti effettivi sono connessi ai record di Workfront Planning.

     Per ulteriori informazioni, consulta [Collega record](/help/quicksilver/planning/records/connect-records.md).

   * **Quando si aggiungono campi di ricerca del record o dell&#39;oggetto a cui ci si connette**: è possibile collegare i campi dall&#39;oggetto dell&#39;altra applicazione al tipo di record Workfront Planning. Si tratta di campi collegati o di ricerca. I campi collegati visualizzano automaticamente le informazioni dei record o degli oggetti connessi quando si collegano i record o gli oggetti. I campi di ricerca collegati sono sempre di sola lettura e vengono compilati automaticamente con i valori dei record o degli oggetti connessi.

     Ad esempio, se si collega il tipo di record &quot;Campagna&quot; a un progetto Workfront e si seleziona di inserire il campo Data di completamento pianificata del progetto nel record Pianificazione di Workfront, per la campagna viene automaticamente creato un campo collegato denominato Data di completamento pianificata (da progetto). Impossibile modificare manualmente il campo collegato. Nel campo Data di completamento pianificata (da progetto) viene visualizzata la Data di completamento pianificata dei progetti collegati.

     >[!IMPORTANT]
     >
     >    Tutti coloro che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro possono visualizzare le informazioni nei campi collegati, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegati.

* I campi record collegati sono preceduti da un&#39;icona di relazione ![](assets/relationship-field-icon.png).

  I campi collegati sono preceduti da un’icona che identifica il tipo di campo. Ad esempio, icone che indicano che un campo è un numero, un paragrafo o una data.

## Connetti tipi di record

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera connettere i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace dal quale si desidera connettere i tipi di record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Fai clic su **+** nell&#39;angolo superiore destro della vista tabella, quindi fare clic sul pulsante **Nuova connessione** scheda.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. In **Tipo di record** , cercare un tipo di record o selezionare una delle opzioni seguenti:

   * Un altro tipo di record dalla sezione dell&#39;area di lavoro selezionata

     >[!TIP]
     >
     >Solo i tipi di record dell&#39;area di lavoro selezionata sono disponibili per la connessione.
     > 
     >Se nell&#39;area di lavoro selezionata non sono presenti altri tipi di record, la sezione area di lavoro non viene visualizzata.

   * A **Progetto, Portfolio, Programma, Società**, o **Gruppo** dal **Tipi di oggetto Workfront** sezione.
   * **Experience Manager Assets** dal **Applicazioni Adobe** sezione.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Aggiorna le seguenti informazioni:

   * **Nome**: nome del campo connesso che verrà visualizzato nella visualizzazione tabella o nella pagina del record del tipo di record originale. In questo modo viene creata la colonna del record collegato nella vista a tabella del tipo di record originale o del campo del record collegato per i record originali.

   >[!TIP]
   >
   >È consigliabile includere il nome del record a cui si desidera creare il collegamento nel nome del campo record connesso per acquisire il tipo di record da cui proviene il nuovo campo. Il nome del record collegato non è visibile nel nuovo campo record collegato o nei relativi campi collegati.

   * **Descrizione**: informazioni aggiuntive sul campo record connesso. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Consenti più record**: seleziona questa opzione per indicare che gli utenti possono aggiungere più record quando il campo del tipo di record collegato viene visualizzato nei record originali. Questa opzione è selezionata per impostazione predefinita.
   * **Seleziona campi di ricerca**: seleziona questa opzione per aggiungere campi dal tipo di record selezionato. I campi di ricerca sono campi associati al record o al tipo di oggetto a cui si sta effettuando il collegamento. Il collegamento consente di visualizzare le informazioni del record o dell&#39;oggetto a cui si sta effettuando il collegamento nel record di cui si desidera creare il collegamento. Questa opzione è selezionata per impostazione predefinita.

1. (Condizionale e facoltativo) Se si è selezionato di collegare un oggetto Workfront, selezionare un **Modulo personalizzato** dal **Collega solo gli oggetti che corrispondono a questi criteri** sezione. Solo gli oggetti a cui sono allegati i moduli personalizzati selezionati possono essere collegati al tipo di record selezionato. È possibile selezionare più moduli.

   ![](assets/workfront-project-connection-selection.png)

   >[!NOTE]
   >
   > È necessario creare moduli personalizzati in Workfront per gli oggetti selezionati prima che vengano visualizzati in questo elenco.

1. (Condizionale) Se hai selezionato di connetterti a Experience Manager Assets, seleziona un archivio da **archivio Experienci Manager** menu a discesa nella **Collegare le risorse dal seguente archivio** sezione. Questo campo è obbligatorio. In questo campo vengono visualizzati solo gli archivi a cui hai accesso in Experience Manager Assets.

   <!--replace the screen shot below when they fix the permissions info icon bug-->

   ![](assets/aem-assets-connection-selection.png)

1. Fai clic su **Crea**.

1. (Condizionale) Se hai selezionato il **Seleziona campo di ricerca** impostazione, **Aggiungi campi di ricerca** viene visualizzata la casella.

   Fai clic su **+** per aggiungere campi dalla **Campi non selezionati** area.

   Oppure

   Fai clic su **-** per rimuovere i campi dal **Campi selezionati** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   I valori dei campi collegati vengono compilati automaticamente dopo il collegamento di record o oggetti.

   >[!IMPORTANT]
   >
   >    Tutti coloro che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro possono visualizzare le informazioni nei campi collegati, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegati.


1. (Facoltativo) Fai clic su **Ignora** e non aggiungere campi dal record o dall&#39;oggetto collegato. Il **Nome** del record collegato è l&#39;unico campo visibile nella visualizzazione tabella del record originale.

1. (Facoltativo e condizionale) Se si seleziona di collegare un campo di tipo numero, valuta, percentuale o data, selezionare anche un valore aggregatore. Quando gli utenti selezionano più record collegati nel campo record collegato, i valori dei campi collegati vengono visualizzati separati da virgole o come valore aggregato in base all&#39;aggregatore scelto.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Gli aggregatori non sono disponibili quando si collegano tipi di record a Experience Manager Assets.

   Selezionare una delle opzioni seguenti:

   * **Nessuno**: visualizza i valori provenienti da più record separati da virgole. Questa è la selezione predefinita.
   * **MAX**: visualizza il valore più alto tra tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MIN**: visualizza il valore più basso tra tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **SOMMA**: visualizza il totale di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MEDIA**: visualizza la media di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **UNIVOCO**: rimuove i duplicati dai valori dei campi di ricerca e mostra solo i valori univoci. Questa opzione non è disponibile per i tipi di campo seguenti:
      * Paragrafo
      * Casella di controllo
      * Persone

   >[!NOTE]
   >
   >Ad esempio, puoi collegare il record Prodotto (record collegato) dal record Campagna (record originale) e denominarlo &quot;Campo prodotto&quot;. Puoi anche scegliere di collegare il campo Budget del record Prodotto dal record Campagna e chiamarlo &quot;Budget prodotto&quot;. Se è possibile selezionare più record nel &quot;Campo prodotto&quot;, è possibile selezionare il Prodotto 1 con un budget di $ 100.000 e il Prodotto 2 con un budget di $ 110.000 e il Prodotto 3 con un budget di $ 100.000. È possibile visualizzare le seguenti informazioni di Budget nel campo collegato dal record originale, a seconda dell&#39;aggregatore scelto:
   >
   >* **Nessuno**: 100.000, 110.000, 100.000
   >* **MAX**: $ 110.000
   >* **MIN**: $ 100.000
   >* **SOMMA**: $ 310.000
   >* **MEDIA**: 103.000,33 $
   >* **UNIVOCO**: $ 100.000
   >

1. (Facoltativo) Utilizza il **ricerca** icona ![](assets/search-icon.png) per cercare un campo.

1. Clic **Aggiungi campi** per salvare le modifiche.

   Sono aggiunti i seguenti elementi:

   * Campo record collegato sul tipo di record da cui si sta eseguendo il collegamento. Nel campo record collegato verranno visualizzati i singoli record del tipo di record collegato, dopo averli aggiunti manualmente. Per informazioni sull&#39;aggiunta di record, vedere [Collega record](/help/quicksilver/planning/records/connect-records.md). Il nome del campo record collegato è il nome selezionato al passaggio 6. <!--accurate-->

   * Campo o campi collegati che visualizzano le informazioni dei campi del record o dei tipi di oggetto collegati dopo l&#39;aggiunta manuale dei record o degli oggetti nel campo record collegato. I campi collegati vengono creati solo quando **Seleziona campi di ricerca** durante la creazione della connessione. I campi collegati vengono denominati automaticamente in base a questo pattern:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Ad esempio, se hai collegato un tipo di record Campagna con un tipo di record Programma e denomini il campo del record collegato al Programma &quot;Informazioni sul programma&quot;, quindi hai selezionato di visualizzare anche il campo Budget del programma nella vista a tabella della campagna, il campo collegato viene automaticamente denominato `Budget (from Program information)` nella vista tabella della campagna.

   * Quando si collegano tra loro tipi di record, viene aggiunto anche un campo record collegato al tipo di record a cui si desidera collegarsi. Il nome del campo record collegato nel tipo di record collegato è il nome del tipo di record da cui si esegue il collegamento.

     Ad esempio, se colleghi il tipo di record &quot;Prodotto&quot; dal tipo di record &quot;Campagna&quot; e denomini il campo connesso della campagna &quot;Prodotto collegato&quot;, viene creato un campo di record collegato &quot;Campagna&quot; per il tipo di record Prodotto.

     >[!TIP]
     >
     > Non viene creato un campo record collegato per gli oggetti di un&#39;altra applicazione al tipo di record da cui si esegue il collegamento in Workfront Planning.

1. (Facoltativo e condizionale) Nella vista tabella del tipo di record originale o del tipo di record collegato fare clic sulla freccia rivolta verso il basso nell&#39;intestazione dei campi del record collegato, quindi scegliere una delle opzioni seguenti:

   * **Modifica campo**: puoi aggiornare solo il **Nome** e **Descrizione** informazioni sul campo.
   * **Modifica campi di ricerca**: aggiungi o rimuovi i campi del record collegato.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Per aggiungere o rimuovere campi di ricerca, seguire le istruzioni riportate nei passaggi 10-14 precedenti. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Non è possibile aggiungere campi di ricerca appartenenti a tipi di record da cui si esegue il collegamento a tipi di oggetto da un&#39;altra applicazione.
   >
   > Ad esempio, non è possibile aggiungere il campo di ricerca &quot;Stato campagna&quot; a un progetto Workfront a cui ti stai collegando dalle campagne.

1. (Facoltativo) Fai clic sulla freccia rivolta verso il basso nell’intestazione di un campo record collegato o nell’intestazione di un campo di ricerca dal tipo di record da cui stai eseguendo il collegamento, quindi fai clic su **Elimina**.

   Il campo record o il campo di ricerca vengono eliminati. Se si elimina un campo record, vengono eliminati anche tutti i campi di ricerca associati al record collegato.
