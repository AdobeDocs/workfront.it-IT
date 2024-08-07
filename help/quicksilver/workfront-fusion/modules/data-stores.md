---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Archivi dati in [!DNL Adobe Workfront Fusion]
description: Un archivio dati, simile a un database o a una semplice tabella, può memorizzare i dati di scenari, rendendo possibile il trasferimento di dati tra scenari singoli o l’esecuzione di scenari singoli. È possibile utilizzare un archivio dati per memorizzare nuovi dati provenienti da vari sistemi durante la sincronizzazione.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 00a969175626d27b70d516921097725fdf818799
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# Archivi dati in [!DNL Adobe Workfront Fusion]

Un archivio dati, simile a un database o a una semplice tabella, può memorizzare i dati di scenari, rendendo possibile il trasferimento di dati tra scenari singoli o l’esecuzione di scenari singoli. È possibile utilizzare un archivio dati per memorizzare nuovi dati provenienti da vari sistemi durante la sincronizzazione.

I moduli dell&#39;archivio dati consentono di eseguire le azioni seguenti sui record dell&#39;archivio dati [!DNL Adobe Workfront Fusion]:

* Aggiungi
* Sostituisci
* Aggiorna
* Recupera
* Elimina
* Ricerca
* Conta

Per informazioni sull&#39;utilizzo dei moduli di archivio dati, vedere [[!UICONTROL Moduli di archivio dati]](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Per un video introduttivo sugli archivi dati in Workfront Fusion, vedi:

* [Archivi dati](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Corrente: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Legacy: qualsiasi </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Nuovo:</p> <ul><li>Piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Il piano [!DNL Workfront Fusion] è incluso.</li></ul>
   <p>Oppure</p>
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Spazio dati disponibile

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

Se l’organizzazione utilizza il nuovo modello di piano Workfront (pacchetti Select, Prime e Ultimate), il piano dell’organizzazione influisce sulle dimensioni e sul numero di archivi di dati disponibili per l’istanza di Fusion.

### Piano Ultimate

Le istanze di Fusion sul pacchetto Ultimate ricevono:

* 100 MB di spazio
* 50 archivi dati

### Seleziona e crea piani

Le istanze di Fusion nei pacchetti Select o Prime ricevono:—>

* 100 MB per le prime operazioni 500K.

* 10 MB per ogni 100.000 operazioni aggiuntive.

  Ad esempio, un’organizzazione con 600.000 operazioni riceve 110 MB.

La tua organizzazione può avere fino a 50 archivi di dati. La dimensione combinata di questi archivi dati non può superare la dimensione totale dell’archivio dati dell’organizzazione.

## Crea un archivio dati in [!DNL Workfront Fusion]

* [Configurare l’archivio dati](#set-up-the-data-store)
* [Impostare la struttura dati](#set-up-the-data-structure)

### Configurare l’archivio dati

Prima di poter utilizzare un archivio dati in un modulo, è necessario creare l&#39;archivio dati in [!DNL Workfront Fusion].

>[!NOTE]
>
>La tua organizzazione dispone di un numero limitato di archivi di dati. Se si tenta di creare un numero di archivi dati superiore a quello disponibile, [!DNL Workfront] restituisce un errore [!UICONTROL Numero massimo di archivi raggiunto].
>
>Per ulteriori informazioni, vedere [Numero massimo di archivi raggiunto l&#39;errore](#maximum-stores-reached-error) in questo articolo.

1. Accedi al tuo account [!DNL Workfront Fusion].
1. Fai clic su **[!UICONTROL Archivi dati]** nel pannello di navigazione a sinistra.
1. Fai clic su **[!UICONTROL Aggiungi archivio dati]** nell&#39;angolo superiore destro della schermata.
1. Immetti le impostazioni per il nuovo archivio dati.

   Un titolo in grassetto in un campo di un modulo [!DNL Workfront Fusion] indica un&#39;impostazione obbligatoria.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome archivio dati] </td> 
      <td> <p>Immettere un nome per l'archivio dati. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data Structure]</p> </td> 
      <td> <p>Una struttura di dati è un elenco delle colonne di una tabella. Questo elenco indica il nome della colonna e il tipo di dati.</p> <p>Esegui una delle operazioni seguenti:</p> 
       <ul> 
        <li style="font-weight: bold;">Seleziona una struttura dati già creata</li> 
        <li> <p style="font-weight: bold;">Aggiungere una nuova struttura dati</p> <p>Fare clic su <strong>[!UICONTROL Add]</strong> per creare una nuova struttura dati.</p> <p>Per ulteriori informazioni, vedere la sezione <a href="#set-up-the-data-structure" class="MCXref xref">Configurare la struttura dati</a> in questo articolo.</p> </li> 
        <li style="font-weight: bold;"> <p>Lascia vuoto il campo</p> <p style="font-weight: normal;">Se non si seleziona o non si aggiunge una struttura dati, il database conterrà solo la chiave primaria. Questo tipo di database è utile se desideri salvare solo le chiavi e vuoi sapere solo se nel database esiste o meno una chiave specifica.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Dimensioni archiviazione dati in MB]</p> </td> 
      <td> <p>Alloca le dimensioni per l’archivio dati dal totale dell’archiviazione interna dei dati.</p> <p> Il valore predefinito è 10 MB. Se hai meno di 10 MB di spazio non allocato per l'archivio dati dall'assegnazione di 95 MB, la dimensione predefinita è la quantità di spazio non allocato.  <p>Nota: l'importo prenotato può essere modificato in qualsiasi momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Impostare la struttura dati

1. Durante la creazione o la modifica di un archivio dati, fare clic su **[!UICONTROL Aggiungi]**.
1. Nella casella **[!UICONTROL Aggiungi struttura dati]** visualizzata, configura i campi seguenti:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome struttura dati]</td> 
      <td> <p> Immettere un nome per la nuova struttura dati.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Per impostare le colonne dell'archivio dati, eseguire una delle operazioni seguenti.</p> 
       <ul> 
        <li> <p>Fare clic su <strong>[!UICONTROL Add item]</strong> per specificare manualmente le proprietà di una colonna.</p> <p>Immettere <strong>[!UICONTROL Name]</strong> e <strong>[!UICONTROL Type]</strong> per la colonna dell'archivio dati e definire le proprietà corrispondenti.</p> </li> 
        <li> <p>Fare clic su <strong>[!UICONTROL Generator]</strong> per determinare le colonne dai dati di esempio forniti.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Esempio: </b></span></span> 
          <p>Ad esempio, i seguenti dati di esempio JSON creano tre colonne: nome, età e numero di telefono. Il numero di telefono è una raccolta di numeri di telefono cellulare e di rete fissa.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>Le colonne vuote nella vista archivio dati:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>È quindi possibile aggiungere valori all'archivio dati manualmente o utilizzando i moduli dell'archivio dati [!DNL Workfront Fusion].</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Abilita questa opzione per garantire che il payload corrisponda alle strutture di dati. I payload che contengono elementi aggiuntivi non specificati nella struttura dati vengono rifiutati.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modificare un archivio dati esistente

Puoi modificare le proprietà e il contenuto di un archivio dati esistente nell&#39;area [!UICONTROL Archivio dati] di [!DNL Workfront Fusion].

* [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store)
* [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store)

### Modificare le proprietà di un archivio dati

Le proprietà di un archivio dati includono la struttura dati utilizzata dall’archivio dati e le relative dimensioni.

1. Fai clic su **[!UICONTROL Archivio dati]** ![](assets/data-store-icon.png) nel pannello di navigazione a sinistra per aprire l&#39;area [!UICONTROL Archivio dati].
1. Fai clic su **[!UICONTROL Modifica]** ![](assets/data-store-edit.png) accanto all&#39;archivio dati che desideri modificare.
1. (Facoltativo) Se desideri modificare la struttura dati utilizzata da questo archivio dati in un&#39;altra struttura dati esistente, selezionala dal menu a discesa **[!UICONTROL Struttura dati]**.

   Oppure

   (Facoltativo) Se desideri modificare la struttura dati utilizzata da questo archivio dati in una struttura dati completamente nuova, consulta [Configurare la struttura dati](#set-up-the-data-structure) in questo articolo.

1. (Facoltativo) Modificare le dimensioni dell&#39;archivio dati immettendo le nuove dimensioni nel campo **[!UICONTROL Dimensioni archiviazione dati in MB]**.
1. Fai clic su **[!UICONTROL Salva]**.

### Modificare il contenuto di un archivio dati

1. Fai clic sull&#39;icona ![](assets/data-store-icon.png) dell&#39;**[!UICONTROL Archivio dati]** nel pannello di navigazione a sinistra per aprire l&#39;area [!UICONTROL Archivio dati].
1. Fai clic su **[!UICONTROL Sfoglia]** accanto all&#39;archivio dati che desideri modificare.
1. (Facoltativo) Riordinare le colonne trascinandole nella posizione desiderata.
1. (Facoltativo) [!UICONTROL Modificare] una singola cella facendo clic sull&#39;icona **[!UICONTROL Modifica]** nella cella, quindi immettendo il valore desiderato.
1. (Facoltativo) Aggiungere un nuovo elemento all&#39;archivio dati facendo clic su **[!UICONTROL Aggiungi]**, quindi immettendo le informazioni per il nuovo elemento.
1. Fai clic su **[!UICONTROL Salva]**.

## Risoluzione dei problemi

* [Ripristino dei dati persi da un archivio dati](#restoring-lost-data-from-a-data-store)
* [Errore di spazio insufficiente](#out-of-space-error)
* [Numero massimo di archivi raggiunti dall&#39;errore](#maximum-stores-reached-error)

### Ripristino dei dati persi da un archivio dati

Attualmente non esiste uno strumento in grado di automatizzare il ripristino dei dati persi.

#### Soluzione alternativa

1. Esamina tutti i registri di esecuzione degli scenari in cui sono stati inseriti elementi nell’archivio dati.

   Per ulteriori informazioni sull&#39;esame dei log di esecuzione, vedere [Visualizzare la cronologia di esecuzione di uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copia i dati.
1. Inserisci nuovamente i dati nell’archivio dati.

   Per informazioni sull&#39;inserimento di dati in un archivio dati, vedere [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store) in questo articolo.

### [!UICONTROL Spazio insufficiente] errore

Si è verificato un errore di [!UICONTROL Spazio esaurito] perché gli archivi dati creati in precedenza sono già stati assegnati all&#39;archivio dati allocato.

#### Soluzione alternativa

1. Modifica uno qualsiasi degli archivi dati esistenti per utilizzare meno spazio. In questo modo sarà possibile liberare spazio per il nuovo archivio dati.

   Per ulteriori informazioni, vedere [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store) in questo articolo.

>[!NOTE]
>
>È consigliabile non assegnare tutto lo spazio a un singolo archivio dati, a meno che non si sia certi di non richiedere altri archivi dati.

### [!UICONTROL Numero massimo di archivi raggiunto] errore

Si è verificato un errore di [!UICONTROL numero massimo di archivi raggiunti] perché l&#39;organizzazione ha utilizzato tutti gli archivi dati disponibili. Un’organizzazione dispone di un numero di archivi di dati disponibili pari al doppio del numero di scenari disponibili. Pertanto, il numero totale di archivi dati disponibili dipende dal piano acquistato.

Ad esempio, se la tua organizzazione ha acquistato un piano con 15 scenari, può disporre di un massimo di 30 archivi di dati.

#### Soluzione alternativa

Per ridurre il numero di archivi dati esistenti, eseguire una delle operazioni seguenti:

* Combina archivi dati esistenti
* Elimina archivi dati inutilizzati
