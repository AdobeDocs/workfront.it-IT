---
user-type: administrator
product-area: system-administration;setup
title: Importare schede tariffarie da un modello
description: Puoi utilizzare un file modello per creare le schede tariffa in Excel e importarle in Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: 3b05ab91619e8a2d2ae451d2f0f4cd38e58c7440
workflow-type: tm+mt
source-wordcount: '1696'
ht-degree: 2%

---

# Importare le schede tariffa da un modello

{{highlighted-preview-article-level}}

Puoi utilizzare un file modello per creare le schede dei tassi in Excel e importarle in Adobe Workfront, invece di aggiungere manualmente tutti i ruoli e i tassi.

Per visualizzare le schede di frequenza di esempio descritte in questo articolo, scarica il [file di esempio](assets/rate-cards-sample.zip).

Per ulteriori informazioni sulle schede tariffarie, vedere [Gestione delle schede tariffarie](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Regole importanti per l’utilizzo del file modello

* Inserire la mansione O la categoria di risorse non manodopera, ma non entrambe.
* La sequenza della scheda Rate Card della scheda RATE_RTCRD deve corrispondere all&#39;ordine delle schede della scheda RTCRD (1 per la prima, 2 per la seconda, ecc.).
* Le date di inizio e di fine devono seguire i formati consentiti.
* Le schede delle tariffe possono essere importate senza tariffe e aggiornate in un secondo momento.
* Gli attributi personalizzati (Agenzia, Centro di costo, ecc.) possono variare. Per informazioni sui requisiti, rivolgiti all’amministratore di sistema.
* Le righe eliminate nel modello non elimineranno i record esistenti nel sistema.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a [!UICONTROL Rate Cards]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compila il file modello

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Fai clic su **Nuova scheda tariffa**, quindi fai clic su **Scarica modello Excel**.
1. Seguire le istruzioni del browser per salvare il file modello nel computer.
1. Apri il file modello in Excel.

   >[!TIP]
   >
   > Salvare il file con un nuovo nome se si desidera conservare il file modello vuoto e riutilizzarlo in un secondo momento.

   Il modello ha due schede. Entrambe le schede devono avere le informazioni corrette per importare correttamente le schede di frequenza.

   * RTCRD: definire le schede tariffarie (informazioni di base)
   * RATE_RTCRD: Definisci i tassi dettagliati associati a ciascuna scheda tasso

### Compila la scheda RTCRD (Rate Card Setup).

Crea ed elenca tutte le schede su questa scheda. Ogni riga rappresenta una scheda tariffa.

![Scheda RTCRD nel file modello di importazione scheda tariffe](assets/rate-card-import-template-tab1.png)

1. Immettere le informazioni per una scheda tariffaria su ogni riga:

   * **Nome** (obbligatorio): nome della scheda tariffe, ad esempio &quot;Fatturazione globale 2025&quot;.

     Questo nome è l’identificatore principale della scheda tariffa. Ogni scheda tariffa deve avere un nome univoco.

   * **Descrizione** (facoltativo): una descrizione in formato libero della scheda tariffaria. Utilizzate questa opzione per descrivere scopo, ambito o validità, ad esempio &quot;Si applica ai progetti nordamericani&quot;.
   * **Società** (facoltativo): può essere il nome della società o l&#39;ID della società. L’importazione riconoscerà entrambi.

     Esempio: Coffesta o _68c0234e00000541dd8c0757723daa68_

   * **Gruppo** (facoltativo): può essere il nome o l&#39;ID del gruppo. L’importazione riconoscerà entrambi.

     Esempio: Marketing o _68c0234e00000541dd8c0757723daa68_

   * **Campi personalizzati** (facoltativo): se l&#39;ambiente presenta requisiti specifici, è possibile aggiungere colonne aggiuntive con nomi di campi personalizzati.

   >[!NOTE]
   >
   >* È necessario immettere almeno il Nome per ogni scheda tariffaria.
   >* A ogni scheda viene assegnato automaticamente un numero di sequenza in base alla posizione della riga. Ad esempio, la prima scheda tasso definita (nella riga 2) è la sequenza 1, la successiva è 2 e così via. Questi numeri di sequenza vengono utilizzati nella scheda RATE_RTCRD per allegare le tariffe.

### Compila la scheda RATE_RTCRD (Impostazione tariffe)

Definisci tutte le tariffe che appartengono alle schede su questa scheda.

Ogni riga della scheda definisce una tariffa specifica. È possibile creare più tariffe con la stessa scheda ripetendo la sequenza della scheda.

Assicurati che le date non si sovrappongano a meno che non sia previsto.

![Scheda RATE_RTCRD nel file modello di importazione scheda tariffe](assets/rate-card-import-template-tab2.png)

1. Immettere le informazioni per un tasso su ogni riga:

   * **Nome** (obbligatorio): etichetta per la riga della tariffa.

     La best practice prevede di riutilizzare il nome della scheda tariffa per maggiore chiarezza, ad esempio &quot;Global Billing 2025 - Developer Rate&quot; (Fatturazione globale 2025 - Tasso sviluppatori).

   * **Riferimento scheda tariffa** (obbligatorio): il numero di sequenza della scheda tariffa a cui appartiene la tariffa.

     Se la scheda tariffe è la prima che hai elencato nella scheda RTCRD (riga 2), immetti 1. Se si trattava del secondo, immettere 2 e così via.

   * **Ruolo** (obbligatorio se non viene utilizzata la categoria di risorse non manodopera): la mansione a cui si applica la tariffa. Può essere il nome o l’ID della mansione. L’importazione riconoscerà entrambi.

     Esempio: Designer o _68c0234e00000541dd8c0757723daa68_

   * **Categoria risorsa non manodopera** (obbligatorio se non si utilizza la mansione): categoria di risorsa non manodopera a cui si applica la tariffa. Può essere il nome della categoria o l’ID della categoria. L’importazione riconoscerà entrambi.

     Esempio: fotocamera o _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >Impossibile immettere dati nelle colonne **Mansione** e **Categoria risorse non manodopera**. Uno è obbligatorio.

   * **Data inizio** (facoltativo): la data in cui la tariffa diventa effettiva.

     La data deve seguire uno dei formati supportati (a seconda della posizione): MM/gg/aaaa, gg/MM/aaaa, MM/GG/AA, GG/MM/AAA, M/gg/aa, gg/M/aaaa, aaaa/MM/gg, aaaa/gg/MM, aaaa-MM-gg, aaaa-gg-MM

     Esempio: 01/01/2025

     Per ulteriori informazioni, consulta [Requisiti di formattazione della data](#date-formatting-requirements), di seguito.

   * **Data di fine** (facoltativo): la data in cui la tariffa smette di essere effettiva.

     Questa data deve seguire gli stessi formati supportati della data di inizio.

     Per ulteriori informazioni, consulta [Requisiti di formattazione della data](#date-formatting-requirements), di seguito.

   * **Valore** (facoltativo): valore della velocità numerica, ad esempio 150. Il valore predefinito è 0.
   * **Valuta** (facoltativo): la valuta per il tasso, ad esempio USD, EUR, GBP. Il valore predefinito è la valuta di sistema.
   * **Bloccato** (facoltativo): indica se la tariffa è bloccata. I valori validi sono True o False.
   * **Attributi** (facoltativo/personalizzato): le ultime colonne (Agenzia, Posizione, Centro di costo, ecc.) sono Attributi di tasso che differiscono in base alla configurazione del cliente. Si tratta di campi personalizzabili che possono variare a seconda dell’ambiente del cliente.

     Esempio: Agenzia = &quot;1: Agenzia&quot;, Posizione = &quot;Chicago&quot;, Centro di costo = &quot;22: Centro di costo&quot;

### Compila la scheda RSAL (Rate Card Alias)

Crea ed elenca tutti gli alias in questa scheda. Ogni riga rappresenta un alias.

Quando la scheda tariffa è collegata a un progetto, l&#39;alias viene visualizzato in informazioni quali assegnazioni segnaposto, spese e rapporti, anziché nel nome della mansione interna. Può esistere un solo alias per ogni mansione e combinazione di attributi all&#39;interno di una singola scheda tariffa.

Un alias viene aggiunto al sistema, ma non è connesso a una mansione in base alle informazioni disponibili in questa scheda.

![Scheda RSAL nel file modello di importazione scheda tariffe](assets/rsals-tab-rate-card-import.png)

1. Immettere il nome di un alias in ogni riga.

   Immettere un solo nome alias per riga: un alias di mansione, un alias di categoria di risorse non manodopera o un alias di tipo spesa.

### Compila la scheda RCRMET_RTCRD_RSAL (Metadati scheda tariffa)

In questa scheda puoi definire le connessioni tra risorse e alias per una scheda tariffa specifica.

![Scheda RCRMET_RTCRD_RSAL nel file modello importazione scheda tariffe](assets/rcrmet-tab-rate-card-import.png)

1. Immettere le informazioni su ogni riga:

   * **Scheda tariffa** (obbligatorio): nome o numero di sequenza della scheda tariffa a cui appartengono la risorsa e l&#39;alias. La scheda tariffa deve essere elencata nella scheda RTCRD.

     Per un numero di sequenza: se la scheda delle tariffe è la prima che hai elencato nella scheda RTCRD (riga 2), immetti 1. Se si trattava del secondo, immettere 2 e così via.

   * **Mansione** (obbligatorio se non si utilizzano il tipo di spesa e la categoria di risorse non manodopera): la mansione a cui è connesso l&#39;alias. Può essere il nome o l’ID della mansione. L’importazione riconoscerà entrambi.

     Esempio: Designer o _68c0234e00000541dd8c0757723daa68_

   * **Tipo di spesa** (obbligatorio se non si utilizzano la mansione e la categoria di risorse non manodopera): il tipo di spesa a cui è connesso l&#39;alias. Può essere il nome del tipo di spesa o l&#39;ID del tipo di spesa. L’importazione riconoscerà entrambi.

     Esempio: viaggio o _68c0234e00000541dd8c0757723daa68_

   * **Categoria risorsa non manodopera** (obbligatorio se non si utilizzano la mansione e il tipo di spesa): la categoria della risorsa non manodopera a cui è connesso l&#39;alias. Può essere il nome della categoria o l’ID della categoria. L’importazione riconoscerà entrambi.

     Esempio: fotocamera o _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >Impossibile immettere tutte e tre le colonne **Mansione**, **Tipo di spesa** e **Categoria risorse non manodopera**. Uno è obbligatorio.

   * **Alias risorsa**: alias immesso nella scheda RSAL.

### Requisiti di formattazione della data

Durante la preparazione dei dati della scheda tariffe per l&#39;importazione, è necessario assicurarsi che le colonne di data siano formattate come **Generale** e non come **Data**.

Se le colonne sono impostate sul formato Data, il sistema potrebbe interpretare erroneamente i valori durante il processo di importazione, causando errori o caricamenti non riusciti. L’utilizzo del formato Generale mantiene la rappresentazione numerica o testuale non elaborata della data, consentendo al sistema di convalidare e applicare correttamente i valori.

Seguendo questi passaggi si eviteranno problemi inutili e si garantirà un&#39;importazione fluida e accurata dei dati sui tassi.

1. Prima di salvare o caricare il file, seleziona le colonne della data nel foglio di calcolo.
1. Cambia il formato della colonna in **Generale**.
1. Verifica che i valori vengano ancora visualizzati correttamente (ad esempio, 01/01/2025 o 2025-01-01).

## Importa il file modello

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Fai clic su **Nuova scheda**, quindi fai clic su **Importa nuove schede**.
1. Trascina e rilascia il file nella finestra di dialogo oppure fai clic su **Seleziona un file Excel** per passare al file nel computer.
1. Fai clic su **Inizia importazione**.

   Se il file non presenta problemi, viene visualizzato un messaggio di conferma e le nuove schede vengono visualizzate nell’elenco.

1. Se il file contiene problemi, viene visualizzato un messaggio di errore. Fai clic su **Visualizza problemi** per visualizzare i problemi in una schermata separata.

   È necessario correggere i problemi nel file Excel e importarlo nuovamente prima che le schede di frequenza esistano in Workfront.

## Aggiorna le schede delle tariffe esistenti

Puoi aggiornare le tariffe nelle schede delle tariffe esistenti utilizzando lo stesso modello Excel e caricare tali modifiche in Workfront.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Fai clic su **Nuova scheda**, quindi fai clic su **Importa aggiornamenti scheda**.
1. Trascina e rilascia il file nella finestra di dialogo oppure fai clic su **Seleziona un file Excel** per passare al file nel computer.
1. Fai clic su **Inizia importazione**.

   Se il file non presenta problemi, viene visualizzato un messaggio di conferma e le nuove schede vengono visualizzate nell’elenco.

1. Se il file contiene problemi, viene visualizzato un messaggio di errore. Fai clic su **Visualizza problemi** per visualizzare i problemi in una schermata separata.

   È necessario correggere i problemi nel file Excel e importarlo nuovamente prima che gli aggiornamenti delle schede di frequenza esistano in Workfront.


