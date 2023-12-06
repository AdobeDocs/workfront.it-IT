---
title: Connetti tipi di record
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record Maestro a tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere l'attenzione in un'unica applicazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 98b57b08b87e47a402684428a76576455df664d7
workflow-type: tm+mt
source-wordcount: '1784'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Connetti tipi di record

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

È possibile utilizzare Adobe Maestro per progettare aree di lavoro completamente personalizzabili che contengano i tipi di record necessari nella propria organizzazione. Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record Maestro a tipi di oggetto di altre applicazioni per migliorare l&#39;esperienza degli utenti e mantenere l&#39;attenzione in un&#39;unica applicazione.

È possibile connettere i seguenti elementi:

* Tipi di record operativi Maestro
* Gestire i tipi di record operativi per i tipi di record della tassonomia
* Tipi di tassonomia Maestro per tipi di record operativi
* Gestire i tipi di record operativi e i tipi di oggetto di altre applicazioni.

In questo modo è possibile visualizzare i campi del record collegato o del tipo di oggetto su un altro record Maestro.

Questo articolo descrive come collegare due tipi di record Maestro o un tipo di record Maestro a un oggetto di un&#39;altra applicazione.

Una volta stabilita la connessione tra tipi di record o di oggetti, è possibile collegare tra loro singoli record.

Per informazioni sulla connessione di un record Maestro a un oggetto di un&#39;altra applicazione, vedere [Collega record](../records/connect-records.md).

Per un esempio di connessione dei tipi di record, vedere [Esempio di connessione di tipi di record e record](../architecture/example-connect-record-types-and-records.md).

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
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
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


## Considerazioni sulla connessione dei tipi di record

Considera quanto segue:

* In Maestro è possibile collegare le seguenti entità:

   * Due tipi di record operativi
   * Due tassonomie
   * Tipo di record operativo e tassonomia
   * Tipo di record operativo e tipo di oggetto di un&#39;altra applicazione.

     >[!TIP]
     >
     >    Non è possibile collegare un tipo di record tassonomia a un tipo di record operativo o a un tipo di oggetto di un&#39;altra applicazione.

* Con i tipi di record Maestro è possibile collegare i seguenti oggetti dalle seguenti applicazioni:

   * Adobe Workfront:

      * Progetti
      * Portfolio
      * Programmi
      * Aziende
      * Gruppi

* Dopo aver collegato un tipo di record a un altro tipo di record o a un tipo di oggetto di un&#39;altra applicazione, si verificano i seguenti scenari:

   * Quando si connettono due tipi di record: viene creato un campo Record collegato sul tipo di record da cui si esegue la connessione. Un campo record Collegato simile viene creato nel tipo di record a cui ci si connette.

     Ad esempio, se si collega il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo di record collegato denominato &quot;Prodotto collegato&quot; e nel tipo di record Prodotto viene creato automaticamente un tipo di record collegato denominato &quot;Campagna&quot;.

   * Quando si collega un campo del tipo di record con una tassonomia: viene creato un campo del record collegato sul tipo di record da cui si esegue la connessione. Non viene creato alcun campo record collegato nella tassonomia a cui ci si connette.

     Ad esempio, se colleghi il tipo di record &quot;Campagna&quot; al tipo di record della tassonomia &quot;Pubblico&quot;, nel tipo di record Campagna viene creato un campo record collegato denominato &quot;Pubblico collegato&quot;. Nel tipo di record della tassonomia Pubblico non viene creato alcun campo record collegato denominato automaticamente &quot;Campaign&quot;. <!--this might be temporary-->

   * Quando si collega un campo del tipo di record a un tipo di oggetto di un&#39;altra applicazione, viene creato un campo del record collegato nel tipo di record da cui si esegue la connessione. Nessun campo record collegato viene creato automaticamente nel progetto Workfront in Workfront. Un campo record collegato viene creato sul tipo di record oggetto di Workfront solo quando gli oggetti effettivi sono collegati ai record Maestro.

     Per ulteriori informazioni, consulta [Collega record](../records/connect-records.md).

* Dopo aver connesso i tipi di record, è possibile collegare più campi da un tipo di record a un altro. Questi campi sono denominati &quot;campi collegati&quot; o &quot;campi di ricerca&quot;.
* I campi record collegati sono preceduti da un&#39;icona di relazione ![](assets/relationship-field-icon.png).
* Dopo aver creato singoli record per un tipo di record, è possibile selezionare i record a cui ci si connette dal campo del tipo di record collegato. Per informazioni, consulta [Collega record](../records/connect-records.md).
* Non è possibile modificare le informazioni dei campi collegati dal tipo di record da cui si sta effettuando il collegamento, in quanto vengono automaticamente compilati dal tipo di record originale a cui appartengono non appena si selezionano i record collegati.

## Connetti tipi di record

<!--when changes here, also update the article for "Connect records"-->

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](assets/dots-main-menu.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](assets/lines-main-menu.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Maestro]**.

   Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un&#39;area di lavoro esistente e selezionare l&#39;area di lavoro da cui si desidera connettere i tipi di record.
1. Fare clic sulla scheda di un tipo di record per aprire la pagina del tipo di record.
1. Fai clic su **+** nell&#39;angolo superiore destro della vista tabella, quindi fare clic sul pulsante **Nuova connessione** scheda.

   ![](assets/new-connection-tab-with-workfront-option.png)
1. In **Tipo di record** , selezionare una delle opzioni seguenti: <!--is the field name spelled right? lowercase "t"?-->

   * Altro tipo di record operativo
   * Una tassonomia
   * Un progetto, un Portfolio, un programma, una società o un gruppo Workfront.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)

   >[!TIP]
   >
   > Solo i tipi di record e le tassonomie dell&#39;area di lavoro selezionata sono disponibili per la selezione.

1. Aggiorna le seguenti informazioni:

   * **Nome**: nome del campo connesso che verrà visualizzato nella visualizzazione tabella o nella pagina Dettagli del tipo di record originale. In questo modo viene creata la colonna del record collegato nella vista a tabella del tipo di record originale o del campo del record collegato per i record originali. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >È consigliabile includere il nome del record a cui si desidera creare il collegamento nel nome del campo record connesso per acquisire il tipo di record da cui proviene il nuovo campo. Il nome del record collegato non è visibile nel nuovo campo record collegato o nei relativi campi collegati.

   * **Descrizione**: informazioni aggiuntive sul campo record connesso. La descrizione di un campo viene visualizzata quando si passa il cursore sulla colonna del campo in una tabella.
   * **Consenti più record**: seleziona questa opzione per indicare che gli utenti possono aggiungere più record quando il campo del tipo di record collegato viene visualizzato nei record originali. Questa opzione è selezionata per impostazione predefinita.
   * **Seleziona campi di ricerca**: seleziona questa opzione per aggiungere campi dal tipo di record selezionato. Questa opzione è selezionata per impostazione predefinita.

1. Clic **Crea**.

1. (Condizionale) Se hai selezionato l’impostazione Seleziona campo di ricerca nel passaggio precedente, il **Aggiungi campi di ricerca** viene visualizzata la casella.

   Fai clic su **+** per aggiungere campi dalla **Campi non selezionati** area.

   Oppure

   Fai clic su **-** per rimuovere i campi dal **Campi selezionati** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!NOTE]
   >
   >Se non selezioni alcun campo, il campo **Nome** del record collegato è l&#39;unico campo visibile nella visualizzazione tabella del record originale. Il **Nome** non può essere rimosso.

1. (Facoltativo e condizionale) Se si seleziona di collegare un campo di tipo numero, valuta, percentuale o data, selezionare anche un valore aggregatore. Quando gli utenti selezionano più record collegati nel campo record collegato, i valori dei campi collegati vengono visualizzati separati da virgole o come valore aggregato in base all&#39;aggregatore scelto.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   Selezionare una delle opzioni seguenti:

   * **Nessuno**: visualizza i valori provenienti da più record separati da virgole. Questa è la selezione predefinita.
   * **MAX**: visualizza il valore più alto tra tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MIN**: visualizza il valore più basso tra tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **SOMMA**: visualizza il totale di tutti i valori provenienti da più record selezionati nel campo record collegato.
   * **MEDIA**: visualizza la media di tutti i valori provenienti da più record selezionati nel campo record collegato.

   >[!NOTE]
   >
   >Ad esempio, puoi collegare il record Prodotto (record collegato) dal record Campagna (record originale) e denominarlo &quot;Campo prodotto&quot;. Puoi anche scegliere di collegare il campo Budget del record Prodotto dal record Campagna e chiamarlo &quot;Budget prodotto&quot;. Se hai consentito di selezionare più record nel &quot;Campo prodotto&quot;, puoi selezionare il Prodotto 1 con un Budget di $ 120.000 e il Prodotto 2 con un Budget di $ 100.000. È possibile visualizzare le seguenti informazioni di Budget nel campo collegato dal record originale, a seconda dell&#39;aggregatore scelto:
   >
   >* **Nessuno**: $ 120.000, $ 100.000
   >* **MAX**: $ 120.000
   >* **MIN**: $ 100.000
   >* **SOMMA**: $ 220.000
   >* **MEDIA**: $ 110.000
   >

1. (Facoltativo) Utilizza il **ricerca** icona ![](assets/search-icon.png) per cercare un campo.

1. (Facoltativo) Fai clic su **Ignora** se non si desidera aggiungere campi dal tipo di record connesso.

1. Clic **Aggiungi campi** per salvare le modifiche.

   Sono aggiunti i seguenti elementi:

   * Campo record collegato che visualizzerà i record del tipo di record collegato, dopo averli aggiunti manualmente. Il nome del campo record collegato è il nome selezionato al passaggio 6. <!-- ensure this is still accurate-->

   * Il campo o i campi collegati che visualizzeranno le informazioni dei campi del tipo di record collegato dopo l&#39;aggiunta manuale dei record nel campo del record collegato. I campi collegati vengono creati solo quando **Seleziona campi di ricerca** durante la creazione della connessione. I campi collegati sono denominati in base a questo pattern:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Un campo record collegato sul tipo di record a cui si sta effettuando il collegamento. Il nome del campo record collegato nel tipo di record collegato è il nome del tipo di record da cui si esegue il collegamento.

     Ad esempio, se colleghi il tipo di record &quot;Prodotto&quot; dal tipo di record &quot;Campagna&quot; e denomini il campo connesso della campagna &quot;Prodotto collegato&quot;, viene creato un campo di record collegato &quot;Campagna&quot; per il tipo di record Prodotto.

1. (Facoltativo) Nella visualizzazione per tabella del tipo di record originale o del tipo di record collegato fare clic sulla freccia rivolta verso il basso nell&#39;intestazione dei campi del record collegato, quindi scegliere una delle opzioni seguenti:

   * **Modifica campo**: puoi aggiornare solo il **Nome** e **Descrizione** informazioni sul campo.
   * **Modifica campi di ricerca**: aggiungi o rimuovi i campi del record collegato.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Per aggiungere o rimuovere campi di ricerca, seguire le istruzioni riportate nei passaggi 7-12 precedenti. <!--ensure these step numbers stay accurate-->

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso nell&#39;intestazione del campo record collegato dal tipo di record da cui si sta eseguendo il collegamento, quindi fare clic su **Elimina**.

   Il campo record ed eventuali campi di ricerca collegati aggiuntivi vengono eliminati e non è possibile recuperare i campi e le relative informazioni.

   >[!TIP]
   >
   >    Il campo del record collegato nel tipo di record a cui si sta effettuando il collegamento non viene eliminato. <!-- is this still accurate?! -->
