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
source-git-commit: 259ffbbaeddeea64ea2e7f77db258472162c9d8d
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 1%

---

# Archivi dati in [!DNL Adobe Workfront Fusion]

Un archivio dati, simile a un database o a una semplice tabella, può memorizzare i dati di scenari, rendendo possibile il trasferimento di dati tra scenari singoli o l’esecuzione di scenari singoli. È possibile utilizzare un archivio dati per memorizzare nuovi dati provenienti da vari sistemi durante la sincronizzazione.

I moduli dell’archivio dati ti consentono di eseguire le seguenti azioni sui record nel [!DNL Adobe Workfront Fusion] archivio dati:

* Aggiungi
* Sostituisci
* Aggiorna
* Recupera
* Elimina
* Ricerca
* Count

Per informazioni sull’utilizzo dei moduli dell’archivio dati, consulta [[!UICONTROL Archivio dati] moduli](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Creare un archivio dati in [!DNL Workfront Fusion]

* [Configurare l’archivio dati](#set-up-the-data-store)
* [Impostare la struttura dati](#set-up-the-data-structure)

### Configurare l’archivio dati

Prima di poter utilizzare un archivio dati in un modulo, è necessario creare l’archivio dati in [!DNL Workfront Fusion].

>[!NOTE]
>
>La tua organizzazione dispone di un numero limitato di archivi di dati. Se tenti di creare più archivi dati di quanti ne hai a disposizione, [!DNL Workfront] restituisce un [!UICONTROL Numero massimo di archivi raggiunto] errore.
>
>Per ulteriori informazioni, consulta [Numero massimo di archivi raggiunti dall&#39;errore](#maximum-stores-reached-error) in questo articolo.

1. Accedi al tuo [!DNL Workfront Fusion] account.
1. Clic **[!UICONTROL Archivi dati]** nel pannello di navigazione a sinistra.
1. Clic **[!UICONTROL Aggiungi archivio dati]** nell&#39;angolo superiore destro dello schermo.
1. Immetti le impostazioni per il nuovo archivio dati.

   Titolo in grassetto in un campo di una [!DNL Workfront Fusion] indica un&#39;impostazione richiesta.

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
        <li> <p style="font-weight: bold;">Aggiungere una nuova struttura dati</p> <p>Clic <strong>[!UICONTROL Add]</strong> per creare una nuova struttura dati.</p> <p>Per ulteriori informazioni, vedere <a href="#set-up-the-data-structure" class="MCXref xref">Impostare la struttura dati</a> in questo articolo.</p> </li> 
        <li style="font-weight: bold;"> <p>Lascia vuoto il campo</p> <p style="font-weight: normal;">Se non si seleziona o non si aggiunge una struttura dati, il database conterrà solo la chiave primaria. Questo tipo di database è utile se desideri salvare solo le chiavi e vuoi sapere solo se nel database esiste o meno una chiave specifica.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Dimensioni archiviazione dati in MB]</p> </td> 
      <td> <p>Alloca le dimensioni per l’archivio dati dal totale dell’archiviazione interna dei dati.</p> <p> Il valore predefinito è 10 MB. Se hai meno di 10 MB di spazio non allocato per l'archivio dati dall'assegnazione di 500 MB, la dimensione predefinita è la quantità di spazio non allocato.  <p>Nota: l'importo prenotato può essere modificato in qualsiasi momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Impostare la struttura dati

1. Durante la creazione o la modifica di un archivio dati, fai clic su **[!UICONTROL Aggiungi]**.
1. In **[!UICONTROL Aggiungi struttura dati]** che viene visualizzata, configura i campi seguenti:

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
        <li> <p>Clic <strong>[!UICONTROL Add item]</strong> per specificare manualmente le proprietà di una colonna.</p> <p>Inserisci il <strong>[!UICONTROL Name]</strong> e <strong>[!UICONTROL Type]</strong> per la colonna dell’archivio dati e definisci le proprietà corrispondenti.</p> </li> 
        <li> <p>Clic <strong>[!UICONTROL Generator]</strong> per determinare le colonne dai dati di esempio forniti.</p> 
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
          <p>È quindi possibile aggiungere valori all’archivio dati manualmente o utilizzando [!DNL Workfront Fusion] moduli dell’archivio dati.</p> 
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

Puoi modificare le proprietà e il contenuto di un archivio dati esistente in [!UICONTROL Archivio dati] area di [!DNL Workfront Fusion].

* [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store)
* [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store)

### Modificare le proprietà di un archivio dati

Le proprietà di un archivio dati includono la struttura dati utilizzata dall’archivio dati e le relative dimensioni.

1. Clic **[!UICONTROL Archivio dati]** ![](assets/data-store-icon.png) nel pannello di navigazione a sinistra per aprire [!UICONTROL Archivio dati] area.
1. Clic **[!UICONTROL Modifica]** ![](assets/data-store-edit.png) accanto all&#39;archivio dati che si desidera modificare.
1. (Facoltativo) Se desideri modificare la struttura dati utilizzata da questo archivio dati in un’altra struttura dati esistente, selezionala dall’elenco **[!UICONTROL Struttura dei dati]** a discesa.

   Oppure

   (Facoltativo) Se desideri modificare la struttura dati utilizzata da questo archivio dati in una struttura dati completamente nuova, consulta [Impostare la struttura dati](#set-up-the-data-structure) in questo articolo.

1. (Facoltativo) Modifica le dimensioni dell’archivio dati inserendo le nuove dimensioni nella **[!UICONTROL Dimensioni di archiviazione dati in MB]** campo.
1. Fai clic su **[!UICONTROL Salva]**.

### Modificare il contenuto di un archivio dati

1. Fai clic su **[!UICONTROL Archivio dati]** icona ![](assets/data-store-icon.png) nel pannello di navigazione a sinistra per aprire [!UICONTROL Archivio dati] area.
1. Clic **[!UICONTROL Sfoglia]**  accanto all&#39;archivio dati che si desidera modificare.
1. (Facoltativo) Riordinare le colonne trascinandole nella posizione desiderata.
1. (Facoltativo) [!UICONTROL Modifica] una singola cella facendo clic sul pulsante **[!UICONTROL Modifica]** nella cella, quindi immettendo il valore desiderato.
1. (Facoltativo) Aggiungi un nuovo elemento all’archivio dati facendo clic su **[!UICONTROL Aggiungi]**, quindi immettere le informazioni per il nuovo elemento.
1. Fai clic su **[!UICONTROL Salva]**.

## Risoluzione dei problemi

* [Ripristino dei dati persi da un archivio dati](#restoring-lost-data-from-a-data-store)
* [Errore di spazio insufficiente](#out-of-space-error)
* [Numero massimo di archivi raggiunti dall&#39;errore](#maximum-stores-reached-error)

### Ripristino dei dati persi da un archivio dati

Attualmente non esiste uno strumento in grado di automatizzare il ripristino dei dati persi.

#### Soluzione alternativa

1. Esamina tutti i registri di esecuzione degli scenari in cui sono stati inseriti elementi nell’archivio dati.

   Per ulteriori informazioni sull’esame dei registri di esecuzione, consulta [Visualizzare la cronologia di esecuzione di uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copia i dati.
1. Inserisci nuovamente i dati nell’archivio dati.

   Per informazioni sull&#39;inserimento di dati in un archivio dati, vedere [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store) in questo articolo.

### [!UICONTROL Spazio insufficiente] errore

Un [!UICONTROL Spazio insufficiente] si verifica un errore perché gli archivi dati creati in precedenza sono già stati assegnati all’archivio dati allocato.

#### Soluzione alternativa

1. Modifica uno qualsiasi degli archivi dati esistenti per utilizzare meno spazio. In questo modo sarà possibile liberare spazio per il nuovo archivio dati.

   Per ulteriori informazioni, consulta [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store) in questo articolo.

>[!NOTE]
>
>È consigliabile non assegnare tutto lo spazio a un singolo archivio dati, a meno che non si sia certi di non richiedere altri archivi dati.

### [!UICONTROL Numero massimo di archivi raggiunto] errore

A [!UICONTROL Numero massimo di archivi raggiunto] si verifica un errore perché l’organizzazione ha utilizzato tutti gli archivi dati disponibili. Un’organizzazione dispone di un numero di archivi di dati disponibili pari al doppio del numero di scenari disponibili. Pertanto, il numero totale di archivi dati disponibili dipende dal piano acquistato.

Ad esempio, se la tua organizzazione ha acquistato un piano con 15 scenari, può disporre di un massimo di 30 archivi di dati.

#### Soluzione alternativa

Per ridurre il numero di archivi dati esistenti, eseguire una delle operazioni seguenti:

* Combina archivi dati esistenti
* Elimina archivi dati inutilizzati
