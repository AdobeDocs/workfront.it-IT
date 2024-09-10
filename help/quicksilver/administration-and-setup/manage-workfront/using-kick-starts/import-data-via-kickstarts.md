---
user-type: administrator
product-area: system-administration
keywords: kick-start, kick-start, kick-start, kick-start
navigation-topic: use-kick-starts
title: Importare dati in Workfront utilizzando un modello di avvio
description: I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare a tale scopo, come spiegato in Importazione dati Kick-Start.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '2750'
ht-degree: 6%

---

# Importare dati in Workfront utilizzando un modello di avvio

<!--Audited: 12/2023-->

I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare per eseguire questa operazione, come spiegato in [Importazione dati Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Questo processo è suddiviso in 3 attività principali:

* Innanzitutto, esportate un modello Kick-Start come file di foglio di calcolo
* In secondo luogo, il foglio di calcolo viene compilato con i dati
* Infine, puoi importare il foglio di calcolo popolato in Workfront

Ognuna di queste procedure è descritta nell&#39;ordine appropriato in questo articolo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p> Nuovo: Standard</p>
   oppure
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitazioni

È possibile importare un numero elevato di oggetti in Workfront utilizzando un modello Kick-Start. Tuttavia, considera le seguenti limitazioni:

* Questa importazione di dati non aggiorna le informazioni sui record già esistenti in Workfront.
* È possibile importare solo i nuovi record e le relative informazioni.
* Non importare più di 2.000 record alla volta per evitare il timeout dell&#39;importazione

## Esportare un modello di Kick-Start come file di foglio di calcolo

Quando si esporta un modello Kick-Start, viene visualizzata una cartella di lavoro vuota del foglio di calcolo di Excel. Una volta scaricato il foglio di calcolo nel computer, è possibile utilizzarlo per compilare le informazioni e quindi importarle nuovamente in Workfront.

Per esportare un modello di Kick-Start:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  -->

1. Fare clic su **Sistema** > **Importa dati (Kick-Start)**.

1. Selezionare i tipi di informazioni che si desidera includere.

   Ogni opzione selezionata rappresenta una raccolta di più schede nel foglio di calcolo esportato. Se ad esempio si seleziona l&#39;opzione **Report**, nel foglio di calcolo verranno inclusi tutti gli oggetti necessari per la creazione di un report (visualizzazioni, filtri, raggruppamenti, report).

   Per importare i dati in Workfront, è possibile utilizzare tutti i tipi di oggetto elencati di seguito. L&#39;unica eccezione è rappresentata dall&#39;opzione Livelli di accesso. La scheda dati Livelli di accesso in un&#39;esportazione viene fornita a scopo di riferimento, in quanto consente di assegnare un livello di accesso a un nuovo account utente in base all&#39;ID.)

   Il modello per ciascuno dei tipi di oggetto può essere esportato nei formati di file seguenti e contiene i fogli riportati di seguito.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Oggetto</strong> </p> </th> 
      <th> <p><strong>Esporta come</strong> </p> </th> 
      <th> <p><strong>Fogli nel foglio di calcolo esportato</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Dashboard</p> <p>Tutte le dashboard del sistema sono disponibili per l’esportazione. È possibile selezionare fino a 100 dashboard specifici in una singola esportazione.</p> </td> 
      <td scope="col">Esporta come file ZIP</td> 
      <td scope="col"> <p>Parametro</p> <p>Testo descrittivo</p><p>Opzione Parametro</p> <p>Gruppo di parametri</p> <p>Parametro di Categoria</p> <p>Categoria</p> <p>Rapporto</p> <p>La Sezione della Liguetta Portale</p> <p>Dashboard</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapporto</p> <p>Tutti i report nel sistema sono disponibili per l'esportazione. Puoi selezionare fino a 100 rapporti specifici in una singola esportazione.</p> <p>Kick-Start non supporta i filtri in modalità testo. Per una corretta esportazione, i filtri di reporting devono essere commutati in modalità Standard.</p> </td> 
      <td scope="col">Esporta come file ZIP </td> 
      <td scope="col"> <p scope="col">Parametro</p> <p scope="col">Testo descrittivo</p> <p scope="col">Opzione Parametro</p> <p scope="col">Gruppo di parametri</p> <p scope="col">Parametro di Categoria</p> <p scope="col">Categoria</p> <p scope="col">Rapporto</p> <p scope="col">Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Approvazione</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Approvatore fase</p> <p>Fase di approv.</p> <p>Approvazione</p> <p>Processo di approvazione</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dati personalizzati</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Parametro</p> <p>Testo descrittivo</p>  <p>Opzione Parametro</p> <p>Gruppo di parametri</p> <p>Parametro di Categoria</p> <p>Categoria</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Tipo di spesa</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td> <p>Tipo di spesa</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Tipo di ora</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td> <p>Tipo di ora</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Team</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td> <p> Membro team</p> <p>Team</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Utente</p> </td> 
      <td> <p>Esporta come file Excel. Per visualizzare l'elenco completo delle opzioni, fare clic su <strong>Altre opzioni</strong>.</p> </td> 
      <td> <p>Utente</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td>Livello di accesso</td> 
      <td>Esporta come file Excel</td> 
      <td> <p>Livello di accesso</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td>Assegnazione</td> 
      <td>Esporta come file Excel</td> 
      <td> <p>Assegnazione</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td>Azienda</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Azienda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Modello e-mail</td> 
      <td>Esporta come file Excel</td> 
      <td> <p>Modello e-mail</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Spesa</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Spesa'</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Pagina Esterna</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Pagina Esterna</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Filtro</td> 
      <td>Esporta come file ZIP</td> 
      <td> <p> Filtro</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Gruppo</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Gruppo</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Raggruppamento</td> 
      <td>Esporta come file ZIP</td> 
      <td> <p> Raggruppamento</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Ora</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Ora</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Problema</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Problema</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Ruolo</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Ruolo</p> <p>Preferenze </p> </td> 
     </tr>

   <tr> 
      <td>Percorso milestone</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Milestone</p> <p>Percorso milestone</p> <p>Preferenze </p> </td> 
     </tr>

   <tr> 
      <td>Nota</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Nota</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Portfolio</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Progetto</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Coda</p> <p>Progetto</p> <p>Regola di Istradamento</p> <p>Argomento coda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Stima Risorse</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Stima Risorse</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Rischio</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Rischio</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Tipo Rischio</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Tipo Rischio</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Esporta come file Excel</td> 
      <td> <p>Domanda Scorecard</p> <p>Opzione scorecard</p> <p>Scorecard</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Attività</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Attività</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Modello</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Coda</p> <p>Modello</p> <p>Regola di Istradamento</p> <p>Argomento coda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Assegnazione Modello</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Assegnazione Modello</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Attività modello</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Attività modello</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Scheda orario</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Profilo scheda orario</p> <p>Scheda orario</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Visualizza </td> 
      <td> <p>Esporta come file ZIP</p> </td> 
      <td> <p> Visualizza</p> <p>Preferenze </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Scarica**.
1. Continua con [Inserisci i tuoi dati nel modello di foglio di calcolo](#populate-the-spreadsheet-template-with-your-data) per inserire le tue informazioni nel foglio di calcolo del modello vuoto.

## Compilare il modello di foglio di calcolo con i dati {#populate-the-spreadsheet-template-with-your-data}

* [Panoramica delle schede (fogli dati) incluse nel foglio di calcolo](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importa un record](#import-a-record)
* [Includi date](#include-dates)
* [Usa caratteri jolly](#use-wildcards)
* [Sostituzione nome attributo per ID](#attribute-name-substitution-for-ids)

### Panoramica delle schede (fogli dati) incluse nel foglio di calcolo

>[!TIP]
>
>Per capire meglio come formattare le informazioni in ogni colonna quando si compila il modello di Kick-Start, è consigliabile eseguire una procedura esportando un Kick-Start con dati Workfront esistenti sugli oggetti che si sta tentando di importare. Per istruzioni, consulta [Esportare dati da Adobe Workfront tramite Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando apri un modello Kick-Start vuoto, sono disponibili diverse schede (fogli dati). Dipendono dagli oggetti selezionati per il download. Ciascuno rappresenta un oggetto nell&#39;applicazione, ad esempio progetto, attività, ore, dashboard e utenti:

Quando si apre una di queste schede, nella riga 2 vengono visualizzati i campi di ogni oggetto che è possibile impostare durante un&#39;importazione. Nell&#39;intestazione di una colonna, dopo la parola &quot;set&quot;, il nome del campo viene visualizzato come appare nel database. Questi campi fungono da intestazioni di colonna.

>[!IMPORTANT]
>
>Per evitare errori, assicurati di quanto segue:
>
>* Non eliminare la prima riga vuota di un foglio di calcolo di avvio.
>* Non eliminare, modificare o ridisporre questi campi (intestazioni di colonna) in alcun modo. Ad esempio, non modificare l’ordine o i nomi.
>* Aggiungi valori a ogni campo visualizzato in grassetto nell’intestazione della colonna. Questi rappresentano campi obbligatori.
>
>     Tuttavia, se un campo obbligatorio contiene un valore predefinito impostato nelle preferenze di sistema, non è necessario compilarlo.
>
>     Ad esempio, nella scheda **Progetto PROJ** i campi **setCondition** e **setConditionType** possono essere lasciati vuoti, ma non le colonne **setGroupID** e **setName**.
>
>* Alcuni campi, tra cui **setResourceRevenue** e **setEnteredByID**, vengono generati automaticamente dal sistema. Se si immettono dati per questi campi nel foglio di calcolo, il processo di avvio lo ignorerà quando si carica il foglio di calcolo.

### Importare un record  {#import-a-record}

Ogni riga del foglio corrisponde a un oggetto univoco.

1. Aggiungi informazioni nella colonna **isNew**:

   * Se l&#39;oggetto che si sta importando è nuovo, digitare **TRUE** per importare i dati nella riga. Questo valore fa distinzione tra maiuscole e minuscole e deve essere sempre in lettere maiuscole
   * Se l&#39;oggetto è già in Workfront, digitare **FALSE** nella colonna **isNew** per ignorare la riga. Questo valore fa distinzione tra maiuscole e minuscole e deve essere sempre in lettere maiuscole

      * I record già esistenti in Workfront non vengono aggiornati.
      * Se hai scaricato un modello con dati da Workfront, gli oggetti esistenti sono già contrassegnati con **FALSE**.
      * Se è stato scaricato un modello vuoto, non è necessario aggiungere nuove righe per gli oggetti esistenti.

1. Aggiungere informazioni nella colonna **ID** in uno dei modi seguenti:

   * Se l&#39;oggetto che si sta importando è nuovo e si è digitato **TRUE** nella colonna **isNew**, digitare un numero qualsiasi per l&#39;ID. Questo numero deve essere univoco nel foglio di calcolo. Ad esempio, se importi tre oggetti, puoi assegnare loro rispettivamente l’ID 1, 2, 3.

   * Se l&#39;oggetto esiste già in Workfront (e **FALSE** si trova nella colonna **isNew**) e si stanno importando nuove informazioni sugli oggetti esistenti, l&#39;ID deve essere il GUID alfanumerico esistente in Workfront per tale oggetto.

   >[!TIP]
   >
   > Per individuare il GUID univoco di un oggetto in Workfront, è possibile creare un report per tale oggetto e aggiungere la colonna ID al report. Il valore di ogni oggetto nella colonna è il GUID dell&#39;oggetto.

   * I record già esistenti in Workfront non vengono aggiornati.
   * Se è stato scaricato un modello con dati, gli oggetti esistenti contengono già il GUID come ID.
   * È possibile importare un nuovo oggetto basato su un oggetto esistente modificando **FALSE** in **TRUE** nella colonna **isNew**, modificando l&#39;ID e apportando le modifiche necessarie ai dati prima dell&#39;importazione.

   ![ID campione per un gruppo](assets/kick-start-group-example.png)

   * Quando si importa un progetto, è necessario indicare un ID gruppo.

      * Se il gruppo esiste già in Workfront, è necessario aggiungerne l&#39;ID univoco al campo **setGroupID** per il progetto.
      * Se il gruppo non esiste in Workfront, è possibile aggiungere il foglio **GROUP** al file di importazione, impostare il campo **isNew** su **TRUE** nel foglio Gruppo e indicare un ID numerico per il nuovo gruppo nella colonna **ID**. Il campo **setGroupID** per il nuovo progetto deve corrispondere al valore numerico **ID** per il nuovo gruppo.

     **Esempio:** Per un progetto, il valore visualizzato nella colonna **setGroupID** deve essere uno dei seguenti:

      * GUID di un gruppo esistente nell&#39;istanza di Workfront
      * Il valore (numero) nella colonna ID del foglio **GROUP** se si sta creando un nuovo gruppo durante l&#39;importazione

1. Immetti i valori per i campi obbligatori e per tutti gli altri campi che desideri compilare durante l’importazione.
1. (Facoltativo) Per aggiungere dati personalizzati:

   * Creare una nuova colonna per ogni campo personalizzato che si desidera includere nel processo di importazione.
   * Assegnare un nome a ogni nuova colonna per il campo personalizzato corrispondente nel modo seguente: **DE:[Nome del campo personalizzato visualizzato in Workfront]**. Ad esempio, puoi creare il seguente campo personalizzato: &quot;DE: Dipartimenti&quot;.
   * Nella colonna **setCategoryID** digitare il GUID del modulo personalizzato esistente in cui si trova il campo personalizzato. Questo campo è obbligatorio per l’importazione di dati personalizzati.
   * Per aggiungere più valori di dati nel campo personalizzato, ad esempio pulsanti di scelta, caselle di controllo o elenchi, utilizzare il delimitatore di dati personalizzato a barre verticali &quot;|&quot; elencato nella scheda Preferenze per separare i valori.

     **Esempio:** Digitare A|D nella colonna DE:Dipartimenti per compilare il reparto A e il reparto D nel modulo personalizzato.

### Includi date  {#include-dates}

Workfront è in grado di elaborare la maggior parte dei formati di date. È tuttavia necessario assicurarsi che la colonna data nel foglio di calcolo sia formattata come data. L&#39;importazione avrà esito negativo se la colonna viene formattata come generale, un numero o un testo.

>[!TIP]
>
>Il formato più diffuso è il formato MM/GG/AAAA.
>
>Ad esempio: 07/10/2023.

Workfront accetta anche i valori di ora come parte della data.

Ad esempio: 07/10/2022 01:30 o 07/10/2022 1:00 PM.

Se si omette un&#39;ora nella data, Workfront esegue una delle operazioni seguenti:

* Presuppone che l’ora sia le 00:00. Per visualizzare il risultato della data prevista, il fuso orario del sistema deve corrispondere al proprio.
* Se si trova su un oggetto associato a una pianificazione, il tempo si riferisce alla prima volta consentita dalla pianificazione.

>[!NOTE]
>
>Quando si utilizza un timestamp UNIX, è necessario includere tre zeri aggiuntivi alla fine del valore.
>
>Ad esempio, se la marca temporale è 7336899000, immettere 7336899000000 nella cella.

### Usa caratteri jolly {#use-wildcards}

È possibile utilizzare i seguenti caratteri jolly durante la compilazione del foglio di calcolo del modello di Kick-Start:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Carattere jolly</strong> </p> </th> 
   <th> <p><strong>Comportamento</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$OGGI</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setDate</strong>, questo carattere jolly imposta la data come mezzanotte del giorno in cui si importa il Kick-Start.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi il lunedì della settimana in cui viene importato, indipendentemente dal giorno in cui esegui effettivamente l'importazione, puoi utilizzare <strong>$$TODAYbw</strong>. In questo modo, la data di inizio pianificata del progetto verrà impostata sulle 00.00 di domenica. Poiché la pianificazione del progetto probabilmente non consente di lavorare in quel momento, inizierà alle 9 di lunedì mattina.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setDate</strong>, questo carattere jolly imposta la data in base al momento della creazione del record durante l'importazione Kick-Start.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi 3 ore dopo l'importazione, puoi utilizzare <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setAssignedToID</strong> o in un altro campo basato su userID, questo carattere jolly assegna il lavoro o associa in altro modo il record alla persona che esegue l'importazione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CLIENTE</p> </td> 
   <td> <p>Questo carattere jolly è stato aggiunto specificatamente per le importazioni utente Kick-Start. Quando si crea un account Workfront, viene creato un utente con il livello di accesso Amministratore di sistema. Il nome utente assegnato all’amministratore predefinito può essere utilizzato come prefisso durante la creazione di altri utenti nell’account.</p> <p>Poiché i nomi utente devono essere univoci in tutti i clienti, questo è utile quando esistono diversi utenti con nomi utente molto comuni, ad esempio John Smith, che potrebbero avere un nome utente "jsmith". Anteponendo l'assegnazione del nome utente con il nome utente amministratore predefinito, si garantisce che ogni nome utente sia univoco (ad esempio: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Suggerimento: un modo più elegante per garantire che i nomi utente siano univoci a livello di sistema consiste nell'inserire l'indirizzo e-mail dell'utente nel campo <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sostituzione nome attributo per ID  {#attribute-name-substitution-for-ids}

Anche se è consigliabile utilizzare gli ID quando possibile, a volte può risultare scomodo eseguire un riferimento incrociato tra gli ID da un foglio all&#39;altro quando si imposta un valore **setAttributeID**. Puoi fare riferimento ai valori per nome semplicemente modificando l’intestazione della colonna.

**Esempi:**

* **Importazione progetto**

  Durante l&#39;importazione dei progetti, impostare **setGroupID** dei progetti accedendo al foglio **GROUPGroup**, analizzando i rispettivi ID gruppo e incollandoli nelle celle corrette (**setGroupID**) del foglio **PROJ Project**.

  Questo è possibile quando si lavora con pochi gruppi e progetti, ma se si lavora con diversi di ciascuno, non è pratico.

  Per eseguire la sostituzione del nome attributo per l&#39;esempio descritto in precedenza, modificare l&#39;intestazione di colonna **setGroupID** in **#setGroupID nome GRUPPO**. È quindi possibile fare riferimento al gruppo di ogni progetto per nome.

  >[!NOTE]
  >
  >L&#39;opzione per utilizzare la sostituzione nome attributo è limitata ai riferimenti solo per i record esistenti. Non è possibile utilizzare la sostituzione del nome per gli oggetti che si stanno creando nella stessa importazione.

* **Importazione utente**

  Durante l&#39;importazione degli utenti, compilare il **setRoleID** da un elenco di ruoli nella scheda **ROLE Role**.

  Alcuni ID Ruolo sono per i record già presenti nell’account, mentre altri vengono creati durante l’importazione.

  Per i nuovi record utente assegnati a ruoli esistenti, è possibile utilizzare la sostituzione dei nomi. Per i nuovi record utente assegnati ai nuovi ruoli importati, non è possibile.

  Ecco come utilizzare entrambi i metodi sullo stesso file di importazione:

   * Aggiungi una colonna nel foglio di calcolo a sinistra della colonna **setRoleID**.
   * Denomina la nuova colonna **#setRoleID nome RUOLO**.
   * Per le assegnazioni di ruolo a record esistenti, immettere i nomi dei ruoli nella colonna **#setRoleID nome RUOLO**.

     Per le assegnazioni di ruolo a nuovi record di ruolo, immettere l&#39;ID assegnato nel foglio Ruolo di ruolo in setRoleID.

     ![ID ruolo per utenti](assets/set-role-id.png)

## Importare i dati del foglio di calcolo in Workfront

Dopo aver popolato il modello Excel con i tuoi dati, puoi caricarne i dati in Workfront.

L&#39;importazione Kick-Start supporta i seguenti tipi di file:

* Excel (.xls o .xlsx)
* File ZIP compresso (contenente solo file xlsx o xls)

  >[!NOTE]
  >
  >È necessario utilizzare un file .ZIP per importare fogli di calcolo Excel che fanno riferimento ai seguenti oggetti:
  >
  >* Report
  >* Documenti
  >* Avatar
  >* Visualizzare, filtrare o raggruppare i file di proprietà
  >
  >Quando si utilizza un file di importazione compresso, il file .ZIP deve avere lo stesso nome del file .xlsx o .xls e tutti i file devono trovarsi allo stesso livello di struttura (nessuna cartella).

Per importare i dati del foglio di calcolo del modello in Workfront:

<!--1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Importa dati (Kick-Start)**.

1. Nella sezione **Carica dati con foglio di calcolo di avvio**, fai clic su **Scegli file**, quindi individua e seleziona il foglio di calcolo popolato.

1. Fai clic su **Carica.**

   Se il caricamento del file Excel in Workfront richiede più di 5 minuti, l’applicazione va in timeout e Workfront non può caricare il file.

   Prova a importare i dati in batch più piccoli di oggetti.

1. (Condizionale) Se utilizzi Workfront Fusion, ora puoi attivare i tuoi FLO o scenari.
