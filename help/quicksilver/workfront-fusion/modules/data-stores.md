---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Archivia dati in [!DNL Adobe Workfront Fusion]
description: Un archivio dati, simile a un database o a una tabella semplice, può memorizzare dati da scenari, consentendo il trasferimento di dati tra scenari o esecuzioni di scenari individuali. È possibile utilizzare un archivio dati per memorizzare i nuovi dati provenienti da diversi sistemi durante la sincronizzazione.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Archivia dati in [!DNL Adobe Workfront Fusion]

Un archivio dati, simile a un database o a una tabella semplice, può memorizzare dati da scenari, consentendo il trasferimento di dati tra scenari o esecuzioni di scenari individuali. È possibile utilizzare un archivio dati per memorizzare i nuovi dati provenienti da diversi sistemi durante la sincronizzazione.

I moduli di archiviazione dati consentono di eseguire le seguenti azioni sui record nel [!DNL Adobe Workfront Fusion] archivio dati:

* Aggiungi
* Sostituisci
* Aggiorna
* Recupera
* Elimina
* Ricerca
* Count

Per informazioni sull&#39;utilizzo dei moduli di archivio dati, vedi [[!UICONTROL Archiviazione dati] moduli](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Crea un archivio dati in [!DNL Workfront Fusion]

* [Configurare l&#39;archivio dati](#set-up-the-data-store)
* [Impostare la struttura dati](#set-up-the-data-structure)

### Configurare l&#39;archivio dati

Prima di poter utilizzare un archivio dati in un modulo, è necessario creare l&#39;archivio dati in [!DNL Workfront Fusion].

>[!NOTE]
>
>La tua organizzazione dispone di un numero limitato di archivi dati disponibili. Se si tenta di creare più archivi di dati di quanti ne siano disponibili, [!DNL Workfront] restituisce [!UICONTROL Numero massimo di archivi raggiunti] errore.
>
>Per ulteriori informazioni, consulta [Numero massimo di archivi raggiunto errore](#maximum-stores-reached-error) in questo articolo.

1. Accedi al tuo [!DNL Workfront Fusion] conto.
1. Fai clic su **[!UICONTROL Archiviazione dati]** nel pannello di navigazione a sinistra.
1. Fai clic su **[!UICONTROL Aggiungi archivio dati]** nell&#39;angolo superiore destro dello schermo.
1. Immettere le impostazioni per il nuovo archivio dati.

   Titolo in grassetto su un campo in un [!DNL Workfront Fusion] Il modulo indica un’impostazione obbligatoria.

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
      <td> <p>Una struttura dati è un elenco delle colonne di una tabella. Questo elenco indica il nome della colonna e il tipo di dati.</p> <p>Esegui una delle operazioni seguenti:</p> 
       <ul> 
        <li style="font-weight: bold;">Selezionare una struttura dati già creata</li> 
        <li> <p style="font-weight: bold;">Aggiungi una nuova struttura dati</p> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong> per creare una nuova struttura dati.</p> <p>Per ulteriori informazioni, consulta la sezione <a href="#set-up-the-data-structure" class="MCXref xref">Impostare la struttura dati</a> in questo articolo.</p> </li> 
        <li style="font-weight: bold;"> <p>Lascia vuoto il campo</p> <p style="font-weight: normal;">Se non si seleziona o si aggiunge una struttura dati, il database conterrà solo la chiave primaria. Tale tipo di database è utile se si desidera salvare solo le chiavi e si desidera sapere solo se esiste una chiave specifica nel database.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Dimensioni archiviazione dati in MB]</p> </td> 
      <td> <p>Alloca le dimensioni dell’archivio dati dal totale dell’archiviazione dati interna.</p> <p>Nota: L'importo riservato può essere modificato in qualsiasi momento.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Impostare la struttura dati

1. Quando crei o modifichi un archivio dati, fai clic su **[!UICONTROL Aggiungi]**.
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
      <td> <p>Per impostare le colonne dell'archivio dati, effettuare una delle seguenti operazioni.</p> 
       <ul> 
        <li> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong> per specificare manualmente le proprietà di una colonna.</p> <p>Inserisci il <strong>[!UICONTROL Name]</strong> e <strong>[!UICONTROL Type]</strong> per la colonna dell’archivio dati e definire le proprietà corrispondenti.</p> </li> 
        <li> <p>Fai clic su <strong>[!UICONTROL Generator]</strong> per determinare le colonne dai dati di esempio forniti.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Esempio: </b></span></span> 
          <p>Ad esempio, i seguenti dati di esempio JSON creano tre colonne: nome, età e numero di telefono. Il numero di telefono è una raccolta di numeri di cellulare e di telefono fisso.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>Le colonne vuote nella visualizzazione archivio dati:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>È quindi possibile aggiungere valori all'archivio dati manualmente o utilizzando il [!DNL Workfront Fusion] moduli di archiviazione dati.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Abilita questa opzione per assicurarti che il payload corrisponda alle strutture di dati. I payload contenenti elementi aggiuntivi non specificati nella struttura dati vengono rifiutati.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modificare un archivio dati esistente

Puoi modificare le proprietà e il contenuto di un archivio dati esistente nella sezione [!UICONTROL Archiviazione dati] area [!DNL Workfront Fusion].

* [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store)
* [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store)

### Modificare le proprietà di un archivio dati

Le proprietà di un archivio dati includono la struttura dati utilizzata dall&#39;archivio dati e le dimensioni dell&#39;archivio dati.

1. Fai clic su **[!UICONTROL Archiviazione dati]** ![](assets/data-store-icon.png) nel pannello di navigazione a sinistra per aprire [!UICONTROL Archiviazione dati] area.
1. Fai clic su **[!UICONTROL Modifica]** ![](assets/data-store-edit.png) accanto all’archivio dati da modificare.
1. (Facoltativo) Se desideri modificare la struttura dati utilizzata da questo archivio dati in un&#39;altra struttura dati esistente, selezionala dal **[!UICONTROL Struttura dati]** a discesa.

   Oppure

   (Facoltativo) Per modificare la struttura dati utilizzata da questo archivio dati in una struttura dati completamente nuova, consultare [Impostare la struttura dati](#set-up-the-data-structure) in questo articolo.

1. (Facoltativo) Modifica le dimensioni dell’archivio dati immettendo la nuova dimensione nel **[!UICONTROL Dimensioni di archiviazione dei dati in MB]** campo .
1. Fai clic su **[!UICONTROL Salva]**.

### Modificare il contenuto di un archivio dati

1. Fai clic sul pulsante **[!UICONTROL Archiviazione dati]** icona ![](assets/data-store-icon.png) nel pannello di navigazione a sinistra per aprire [!UICONTROL Archiviazione dati] area.
1. Fai clic su **[!UICONTROL Sfoglia]** ![](assets/browse-data-store.png) accanto all’archivio dati da modificare.
1. (Facoltativo) Riordinare le colonne trascinandole nella posizione desiderata.
1. (Facoltativo) [!UICONTROL Modifica] una singola cella facendo clic sul pulsante **[!UICONTROL Modifica]** icona ![](assets/data-store-edit.png)in quella cella, quindi immetti il valore desiderato.
1. (Facoltativo) Aggiungi un nuovo elemento all’archivio dati facendo clic su **[!UICONTROL Aggiungi]**, quindi immettendo le informazioni per il nuovo elemento.
1. Fai clic su **[!UICONTROL Salva]**.

## Risoluzione dei problemi

* [Ripristino dei dati persi da un archivio dati](#restoring-lost-data-from-a-data-store)
* [Errore di spazio esaurito](#out-of-space-error)
* [Numero massimo di archivi raggiunto errore](#maximum-stores-reached-error)

### Ripristino dei dati persi da un archivio dati

Attualmente non esiste uno strumento che possa automatizzare il ripristino dei dati persi.

#### Soluzione alternativa

1. Esamina tutti i registri di esecuzione degli scenari in cui sono stati inseriti elementi nell’archivio dati.

   Per ulteriori informazioni sull’esame dei registri di esecuzione, vedi [Visualizzare la cronologia di esecuzione di uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copia i dati.
1. Inserisci nuovamente i dati nell&#39;archivio dati.

   Per informazioni sull&#39;inserimento di dati in un archivio dati, consulta [Modificare il contenuto di un archivio dati](#edit-the-contents-of-a-data-store) in questo articolo.

### [!UICONTROL Spazio esaurito] errore

Un [!UICONTROL Spazio esaurito] si verifica un errore perché agli archivi dati creati in precedenza è già stato assegnato lo spazio di archiviazione dati allocato.

#### Soluzione alternativa

1. Modifica uno qualsiasi degli archivi dati esistenti per utilizzare meno spazio. Questo consente di liberare spazio per il nuovo archivio dati.

   Per ulteriori informazioni, consulta [Modificare le proprietà di un archivio dati](#edit-the-properties-of-a-data-store) in questo articolo.

>[!NOTE]
>
>È consigliabile non assegnare tutto lo spazio a un singolo archivio dati a meno che non si sia certi di non richiedere più archivi dati.

### [!UICONTROL Numero massimo di archivi raggiunti] errore

A [!UICONTROL Numero massimo di archivi raggiunti] si verifica un errore perché l&#39;organizzazione ha utilizzato tutti gli archivi dati disponibili. Un&#39;organizzazione dispone di un numero di archivi di dati disponibili pari al doppio del numero di scenari disponibili. Pertanto, il numero totale di archivi dati disponibili dipende dal piano acquistato.

Ad esempio, se l’organizzazione ha acquistato un piano con 15 scenari, l’organizzazione può disporre di un massimo di 30 archivi dati.

#### Soluzione alternativa

Per ridurre il numero di archivi dati esistenti, effettuare una delle seguenti operazioni:

* Combinare archivi dati esistenti
* Elimina archivi dati non utilizzati
