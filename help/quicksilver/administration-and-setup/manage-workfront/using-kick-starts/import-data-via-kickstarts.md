---
user-type: administrator
product-area: system-administration
keywords: kickstart, kick-start, kickstart, kick-start
navigation-topic: use-kick-starts
title: Importare dati in Workfront utilizzando un modello Kick-Start
description: I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che puoi compilare con i dati che desideri importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare a tale scopo, come spiegato in Importazione dati Kick-Start.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 100%

---

# Importare dati in Workfront utilizzando un modello Kick-Start

<!--Audited: 12/2023-->

I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che puoi compilare con i dati che desideri importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare per eseguire questa operazione, come spiegato in [Importazione dati Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Questo processo è suddiviso in 3 attività principali:

* Innanzitutto, esporta un modello Kick-Start come file di foglio di calcolo
* Poi, popola il foglio di calcolo con i tuoi dati
* Infine, importa il foglio di calcolo popolato in Workfront

Ciascuna di queste procedure è descritta nell’ordine appropriato in questo articolo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitazioni

Puoi importare un numero elevato di oggetti in Workfront utilizzando un modello Kick-Start. Tuttavia, considera le seguenti limitazioni:

* Importando i dati in questo modo non si aggiornano le informazioni sui record già esistenti in Workfront.
* Puoi importare solo i nuovi record e le relative informazioni.
* Non importare più di 2.000 record alla volta per evitare il timeout dell’importazione

## Esportare un modello di Kick-Start come file di foglio di calcolo

Quando esporti un modello Kick-Start, ricevi una cartella di lavoro vuota del foglio di calcolo di Excel. Una volta scaricato il foglio di calcolo nel computer, puoi utilizzarlo per popolarlo con le informazioni e quindi importarle nuovamente in Workfront.

Per esportare un modello Kick-Start:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).
-->

1. Fai clic su **Sistema** > **Importa dati (Kick-Start)**.

1. Seleziona i tipi di informazioni che desideri includere.

   Ciascuna opzione selezionata rappresenta una raccolta di più schede nel foglio di calcolo esportato. Ad esempio, se selezioni l’opzione **Rapporto**, nel foglio di calcolo verranno inclusi tutti gli oggetti necessari per la creazione di un rapporto (viste, filtri, raggruppamenti, rapporti).

   Per importare i dati in Workfront, puoi utilizzare tutti i tipi di oggetto elencati di seguito. L’unica eccezione è rappresentata dall’opzione Livelli di accesso. La scheda dati Livelli di accesso in un’esportazione viene fornita a scopo di riferimento, in quanto consente di assegnare un livello di accesso a un nuovo account utente in base all’ID.

   Il modello per ciascuno dei tipi di oggetto può essere esportato nei formati di file seguenti e contiene i fogli riportati di seguito:

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
      <td scope="col"> <p>Dashboard</p> <p>Tutte le dashboard condivise pubblicamente nel sistema sono disponibili per l’esportazione. Le dashboard non condivise a livello di sistema non possono essere esportate. Puoi selezionare fino a 100 dashboard specifiche in una singola esportazione.</p> </td> 
      <td scope="col">Esporta come file ZIP</td> 
      <td scope="col"> <p>Parametro</p> <p>Testo descrittivo</p><p>Opzione parametro</p> <p>Raggruppa parametri</p> <p>Parametro di categoria</p> <p>Categoria</p> <p>Rapporto</p> <p>Sezione scheda del portale</p> <p>Dashboard</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapporto</p> <p>Tutti i rapporti nel sistema sono disponibili per l’esportazione. Puoi selezionare fino a 100 rapporti specifici in una singola esportazione.</p> <p>Kick-Start non supporta filtri o raggruppamenti in modalità testo. Per un’esportazione corretta, i raggruppamenti e i filtri per il reporting devono essere cambiati in modalità standard.</p> </td> 
      <td scope="col">Esporta come file ZIP </td> 
      <td scope="col"> <p scope="col">Parametro</p> <p scope="col">Testo descrittivo</p> <p scope="col">Opzione parametro</p> <p scope="col">Raggruppa parametri</p> <p scope="col">Parametro di categoria</p> <p scope="col">Categoria</p> <p scope="col">Rapporto</p> <p scope="col">Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Approvazione</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Approvatore fase</p> <p>Fase di approvazione</p> <p>Approvazione</p> <p>Processo di approvazione</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dati personalizzati</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Parametro</p> <p>Testo descrittivo</p>  <p>Opzione parametro</p> <p>Raggruppa parametri</p> <p>Parametro di categoria</p> <p>Categoria</p> <p>Preferenze</p> </td> 
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
      <td> <p> Membro del team</p> <p>Team</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Utente</p> </td> 
      <td> <p>Esporta come file Excel. Per visualizzare l’elenco completo delle opzioni, fai clic su <strong>Altre opzioni</strong>.</p> </td> 
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
      <td> <p> Spesa</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Pagina esterna</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Pagina esterna</p> <p>Preferenze </p> </td> 
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
      <td>Mansione</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Mansione</p> <p>Preferenze </p> </td> 
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
      <td> <p> Coda</p> <p>Progetto</p> <p>Regola di indirizzamento</p> <p>Argomento coda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Stima risorse</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Stima risorse</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Rischio</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Rischio</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Tipo di rischio</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Tipo di rischio</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Esporta come file Excel</td> 
      <td> <p>Domanda scorecard</p> <p>Opzione scorecard</p> <p>Scorecard</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Attività</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Attività</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Modello</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Coda</p> <p>Modello</p> <p>Regola di indirizzamento</p> <p>Argomento coda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Assegnazione modello</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Assegnazione modello</p> <p>Preferenze </p> </td> 
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
      <td>Visualizzazione </td> 
      <td> <p>Esporta come file ZIP</p> </td> 
      <td> <p> Visualizzazione</p> <p>Preferenze </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Scarica**.
1. Continua con [Popola il modello di foglio di calcolo con i tuoi dati](#populate-the-spreadsheet-template-with-your-data) per inserire le tue informazioni nel foglio di calcolo del modello vuoto.

## Popola il modello di foglio di calcolo con i tuoi dati {#populate-the-spreadsheet-template-with-your-data}

* [Panoramica delle schede (fogli dati) incluse nel foglio di calcolo](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importare un record](#import-a-record)
* [Includere le date](#include-dates)
* [Utilizzare i caratteri jolly](#use-wildcards)
* [Sostituzione nome attributo per ID](#attribute-name-substitution-for-ids)

### Panoramica delle schede (fogli dati) incluse nel foglio di calcolo

>[!TIP]
>
>Per capire meglio come formattare le informazioni di ciascuna colonna quando popoli il modello di Kick-Start, è consigliabile eseguire una prova esportando un Kick-Start con i dati Workfront esistenti sugli oggetti che stai tentando di importare. Per istruzioni, consulta [Esportare dati da Adobe Workfront tramite Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando apri un modello Kick-Start vuoto, sono disponibili diverse schede (fogli dati). Queste dipendono dagli oggetti selezionati per il download. Ciascuna rappresenta un oggetto nell’applicazione, ad esempio progetto, attività, ore, dashboard e utenti:

Quando ne apri una, nella 2° riga vengono visualizzati i campi di ciascun oggetto che è possibile impostare durante un’importazione. Nell’intestazione di una colonna, dopo la parola “impostazione”, il nome del campo viene visualizzato così come appare nel database. Questi campi fungono da intestazioni di colonna.

>[!IMPORTANT]
>
>Per evitare errori, assicurati di quanto segue:
>
>* Non eliminare la prima riga vuota di un foglio di calcolo Kick-Start.
>* Non eliminare, modificare o ridisporre questi campi (intestazioni di colonna) in alcun modo. Ad esempio, non modificarne l’ordine o i nomi.
>* Aggiungi valori a ciascun campo visualizzato in grassetto nell’intestazione della colonna. Questi rappresentano campi obbligatori.
>
>     Tuttavia, se un campo obbligatorio contiene un valore predefinito impostato nelle preferenze di sistema, non è necessario compilarlo.
>
>     Ad esempio, nella scheda **Progetto PROJ** i campi **setCondition** e **setConditionType** possono essere lasciati vuoti, ma non le colonne **setGroupID** e **setName**.
>
>* Alcuni campi, tra cui **setResourceRevenue** e **setEnteredByID**, vengono generati automaticamente dal sistema. Se iserisci i dati per questi campi nel foglio di calcolo, il processo Kick-Start li sovrascriverà durante il caricamento del foglio di calcolo.

### Importare un record  {#import-a-record}

Ciascuna riga del foglio corrisponde a un oggetto univoco.

1. Aggiungi informazioni nella colonna **isNew**:

   * Se l’oggetto che stai importando è nuovo, digita **TRUE** per importare i dati nella riga. Questo valore fa distinzione tra maiuscole e minuscole e deve essere sempre in lettere maiuscole
   * Se l’oggetto è già in Workfront, digita **FALSE** nella colonna **isNew** per ignorare la riga. Questo valore fa distinzione tra maiuscole e minuscole e deve essere sempre in lettere maiuscole

      * I record già esistenti in Workfront non vengono aggiornati.
      * Se hai scaricato un modello con dati da Workfront, gli oggetti esistenti sono già contrassegnati con **FALSE**.
      * Se hai scaricato un modello vuoto, non è necessario aggiungere nuove righe per gli oggetti esistenti.

1. Aggiungi informazioni nella colonna **ID** in uno dei modi seguenti:

   * Se l’oggetto che stai importando è nuovo, ed hai digitato **TRUE** nella colonna **isNew**, digita un numero qualsiasi per l’ID. Questo numero deve essere univoco nel foglio di calcolo. Ad esempio, se importi tre oggetti, puoi assegnare loro rispettivamente l’ID 1, 2, 3.

   * Se l’oggetto esiste già in Workfront (e **FALSE** si trova nella colonna **isNew**) e stai importando nuove informazioni sugli oggetti esistenti, l’ID deve essere il GUID alfanumerico esistente in Workfront per tale oggetto.

   >[!TIP]
   >
   > Per individuare il GUID univoco di un oggetto in Workfront, puoi creare un rapporto per tale oggetto e aggiungervi la colonna ID. Il valore di ciascun oggetto nella colonna è il GUID dell’oggetto.

   * I record già esistenti in Workfront non vengono aggiornati.
   * Se hai scaricato un modello con i dati, gli oggetti esistenti contengono già il GUID come ID.
   * Puoi importare un nuovo oggetto basato su un oggetto esistente modificando **FALSE** in **TRUE** nella colonna **isNew**, modificando l’ID e apportando le modifiche necessarie ai dati prima dell’importazione.

   ![ID di esempio per un gruppo](assets/kick-start-group-example.png)

   * Quando importi un progetto, è necessario indicare un ID gruppo.

      * Se il gruppo esiste già in Workfront, è necessario aggiungerne l’ID univoco al campo **setGroupID** per il progetto.
      * Se il gruppo non esiste in Workfront, puoi aggiungere il foglio **GROUP** al file di importazione, impostare il campo **isNew** su **TRUE** nel foglio Gruppo e indicare un ID numerico per il nuovo gruppo nella colonna **ID**. Il campo **setGroupID** del nuovo progetto deve corrispondere al valore numerico **ID** del nuovo gruppo.

     **Esempio:** per un progetto, il valore visualizzato nella colonna **setGroupID** deve essere uno dei seguenti:

      * Il GUID di un gruppo esistente nell’istanza di Workfront
      * Il valore (numero) nella colonna ID del foglio **GROUP** se stai creando un nuovo gruppo durante l’importazione

1. I valori di input per i campi obbligatori e per qualsiasi altro campo che desideri compilare durante l’importazione.
1. (Facoltativo) Per aggiungere dati personalizzati:

   * Crea una nuova colonna per ciascun campo personalizzato che desideri includere nel processo di importazione.
   * Assegna un nome a ciascuna nuova colonna per il campo personalizzato corrispondente nel modo seguente: **DI:[nome del campo personalizzato visualizzato in Workfront]**. Ad esempio, puoi creare il seguente campo personalizzato: “DI: Reparti”.
   * Nella colonna **setCategoryID** digita il GUID del modulo personalizzato esistente in cui si trova il campo personalizzato. Questo campo è obbligatorio per l’importazione di dati personalizzati.
   * Per aggiungere più valori di dati nel campo personalizzato, ad esempio pulsanti di scelta, caselle di controllo o elenchi, utilizza il delimitatore di dati personalizzati a barre verticali “|” elencato nella scheda Preferenze per separare i valori.

     **Esempio:** digita A|D nella colonna DI:Departments per compilare il repartto A e il reparto D nel modulo personalizzato.

     >[!NOTE]
     >
     >Utilizza solo il delimitatore “|” per separare i valori dei campi personalizzati. Non è possibile utilizzarlo in altre colonne del foglio di calcolo, incluso **setCategoryID**.

### Includere date  {#include-dates}

Workfront è in grado di elaborare la maggior parte dei formati di date. Tuttavia, devi assicurarti che la colonna della data nel foglio di calcolo sia formattata come data. L’importazione avrà esito negativo se la colonna viene formattata come generale, un numero o un testo.

>[!TIP]
>
>Il formato più diffuso è quello di MM/GG/AAAA.
>
>Ad esempio 07/10/2023.

Workfront accetta anche i valori di ora come parte della data.

Ad esempio: 07/10/2022 01:30 o 07/10/2022 13:00.

Se ometti l’ora nella data, Workfront esegue una delle operazioni seguenti:

* Presuppone che l’ora sia 00:00. Per visualizzare il risultato della data prevista, il fuso orario del sistema deve corrispondere al tuo fuso orario.
* Se si trova su un oggetto associato a una pianificazione, l’ora si riferisce alla prima ora consentita dalla pianificazione.

>[!NOTE]
>
>Quando utilizzi una marca temporale UNIX, è necessario includere tre zeri aggiuntivi alla fine del valore.
>
>Ad esempio, se la marca temporale è 7336899000, inserisci 7336899000000 nella cella.

### Utilizzare caratteri jolly {#use-wildcards}

Durante la compilazione del foglio di calcolo del modello Kick-Start, puoi utilizzare i seguenti caratteri jolly:

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
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setDate</strong>, questo carattere jolly imposta la data come mezzanotte del giorno in cui importi il Kick-Start.</p> <p>Puoi modificarlo utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>se desideri che un progetto inizi il lunedì della settimana in cui viene importato, indipendentemente dal giorno in cui esegui effettivamente l’importazione, puoi utilizzare <strong>$$TODAYbw</strong>. In questo modo, la data di inizio pianificata del progetto verrà impostata sulle 00.00 di domenica. Poiché la pianificazione del progetto probabilmente non consente di lavorare in quel momento, inizierà alle 9:00 di lunedì mattina.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setDate</strong>, questo carattere jolly imposta la data in base al momento della creazione del record durante l’importazione Kick-Start.</p> <p>Puoi modificarlo utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>se desideri che un progetto inizi 3 ore dopo l’importazione, puoi utilizzare <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Se utilizzato in un campo <strong>setAssignedToID</strong> o in un altro campo basato su userID, questo carattere jolly assegna il lavoro o associa in altro modo il record all’individuo che esegue l’importazione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Questo carattere jolly è stato aggiunto specificatamente per le importazioni utente Kick-Start. Durante la creazione di un account Workfront, viene creato un utente con il livello di accesso Amministratore di sistema. Il nome utente assegnato all’amministratore predefinito può essere utilizzato come prefisso durante la creazione di altri utenti nell’account.</p> <p>Poiché i nomi utente devono essere univoci tra tutti i clienti, questo è utile quando disponi di diversi individui con nomi utente molto comuni, ad esempio John Smith, che potrebbero avere un nome utente “jsmith”. Anteponendo l’assegnazione del nome utente con il nome utente amministratore predefinito, assicuri che ciascun nome utente sia univoco (ad esempio: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Suggerimento: un modo più elegante per garantire che i nomi utente siano univoci a livello di sistema consiste nell’inserire l’indirizzo e-mail dell’individuo nel campo <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sostituzione nome attributo per ID  {#attribute-name-substitution-for-ids}

Anche se la best prctice consiste nell’utilizzare gli ID quando possibile, a volte può risultare scomodo eseguire un riferimento incrociato tra gli ID da un foglio all’altro durante l’impostazione di un valore **setAttributeID**. Puoi fare riferimento ai valori per nome semplicemente modificando l’intestazione della colonna.

**Esempi:**

* **Importazione progetti**

  Durante l’importazione dei progetti, imposta il **setGroupID** dei progetti accedendo al foglio **GROUPGroup**, annotando i rispettivi ID gruppo e incollandoli nelle celle corrette (**setGroupID**) sul foglio **PROJ Project**.

  Questo è possibile quando vengono utlizzati pochi gruppi e progetti, ma quando sono diversi per ciascuno, non è pratico.

  Per eseguire la sostituzione del nome attributo per l’esempio descritto in precedenza, modifica l’intestazione di colonna **setGroupID** in **#setGroupID GROUP name**. Puoi quindi fare riferimento al gruppo di ciascun progetto per nome.

  >[!NOTE]
  >
  >L’opzione per utilizzare la sostituzione nome attributo è limitata ai riferimenti solo per i record esistenti. Non puoi utilizzare la sostituzione del nome per gli oggetti che stai creando nella stessa importazione.

* **Importazione utenti**

  Durante l’importazione degli utenti, compila **setRoleID** da un elenco di ruoli nella scheda **ROLE Role**.

  Alcuni ID Ruolo sono per i record già presenti nell’account, mentre altri vengono creati durante l’importazione.

  Per i nuovi record utente assegnati a ruoli esistenti, puoi utilizzare la sostituzione dei nomi. Per i nuovi record utente assegnati ai nuovi ruoli importati, non è possibile.

  Ecco come utilizzare entrambi i metodi sullo stesso file di importazione:

   * Aggiungi una colonna nel foglio di calcolo a sinistra della colonna **setRoleID**.
   * Denomina la nuova colonna **#setRoleID ROLE name**.
   * Per le assegnazioni di ruolo a record esistenti, inserisci i nomi dei ruoli nella colonna **#setRoleID ROLE name**.

     Per le assegnazioni di ruolo a nuovi record di ruolo, inserisci l’ID assegnato nel foglio di ruolo ROLE in setRoleID.

     ![ID ruolo per utenti](assets/set-role-id.png)

## Importare i dati del foglio di calcolo in Workfront

Dopo aver popolato il modello Excel con i tuoi dati, puoi caricarli in Workfront.

L’importazione Kick-Start supporta i seguenti tipi di file:

* Excel (.xls o .xlsx)
* File compresso (.ZIP) (contenente solo file .xlsx o .xls)

  >[!NOTE]
  >
  >Devi utilizzare un file .ZIP quando importi fogli di calcolo Excel che fanno riferimento ai seguenti oggetti:
  >
  >* Rapporti
  >* Documenti
  >* Avatar
  >* Visualizzare, filtrare o raggruppare i file di proprietà
  >
  >Quando utilizzi un file di importazione compresso, il file .ZIP deve avere lo stesso nome del file .xlsx o .xls e tutti i file devono trovarsi allo stesso livello di struttura (nessuna cartella).

Per importare i dati del foglio di calcolo del modello in Workfront:

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Importa dati (Kick-Start)**.

1. Nella sezione **Carica dati con foglio di calcolo Kick-Start**, fai clic su **Scegli il file**, quindi sfoglia e seleziona il foglio di calcolo popolato.

   Il file viene caricato automaticamente e viene visualizzata una notifica di completamento dell’importazione.

   Se il caricamento del file Excel in Workfront richiede più di 5 minuti, l’applicazione va in timeout e Workfront non riesce a caricare il file. Prova a importare i dati in batch di oggetti più piccoli.

1. (Condizionale) Se l’importazione non viene completata correttamente, viene visualizzato un messaggio di errore in cui viene indicato il problema. Cerca di identificare il campo, il foglio e il numero di riga in cui è stato riscontrato il problema e correggi le informazioni nel file di Excel. Prova quindi a importare il file un’altra volta.
1. (Condizionale) Se utilizzi Workfront Fusion, ora puoi attivare i FLO o gli scenari al termine dell’importazione.
