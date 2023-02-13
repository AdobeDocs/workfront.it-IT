---
user-type: administrator
product-area: system-administration
keywords: kickstart, calcio d'inizio, kickstart, calcio d'inizio
navigation-topic: use-kick-starts
title: Importare dati in Adobe Workfront utilizzando un modello Click-Start
description: Le Kick-Starts sono cartelle di lavoro Excel formattate appositamente che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start che puoi utilizzare per eseguire questa operazione, come spiegato in Importazione dati Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 4912349cbbc74a6f7587312e83297169ecd52f51
workflow-type: tm+mt
source-wordcount: '2412'
ht-degree: 8%

---

# Importare dati in Adobe Workfront utilizzando un modello Click-Start

Le Kick-Starts sono cartelle di lavoro Excel formattate appositamente che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start che puoi utilizzare per eseguire questa operazione, come spiegato in [Importazione dati Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Questo processo è suddiviso in 3 attività principali:

* Innanzitutto, puoi esportare un modello Click-Start come file di foglio di calcolo
* In secondo luogo, compila il foglio di calcolo con i tuoi dati
* Infine, puoi importare il foglio di calcolo popolato in Workfront

Ognuna di queste procedure è descritta nell&#39;ordine corretto del presente articolo.

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limitazioni

È possibile importare un gran numero di oggetti in Workfront utilizzando un modello Click-Start. Tuttavia, considera le seguenti limitazioni:

* L&#39;importazione di dati in questo modo non aggiorna le informazioni sui record già esistenti in Workfront
* È possibile importare solo i nuovi record e le relative informazioni
* Importa non più di 2.000 record alla volta per garantire che l&#39;importazione non si interrompa

## Esportare un modello Click-Start come file di foglio di calcolo

Quando si esporta un modello Click-Start si riceve una cartella di lavoro vuota del foglio di calcolo Excel. Nelle procedure successive di questo articolo, la cartella di lavoro verrà compilata con le informazioni e quindi importata nuovamente in Workfront.

Per esportare un modello di avvio rapido:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Esportare i dati (Kick-Starts)**.

1. Fai clic su **Altre opzioni**, quindi seleziona i tipi di informazioni da includere.

   Ogni opzione selezionata rappresenta una raccolta di più schede nel foglio di calcolo esportato. Ad esempio, se selezioni l’opzione Rapporto , tutti gli oggetti necessari per creare un rapporto verranno inclusi nel foglio di calcolo (visualizzazioni, filtri, raggruppamenti, rapporti).

   È possibile utilizzare tutti i tipi di oggetto elencati di seguito per importare i dati in Workfront. (L&#39;unica eccezione è l&#39;opzione Livelli di accesso. Il foglio dati Livelli di accesso in un&#39;esportazione viene fornito a scopo di riferimento, che consente di assegnare un livello di accesso a un nuovo account utente in base all&#39;ID.)

   Il modello per ciascuno dei tipi di oggetto può essere esportato nei seguenti formati di file e contiene i seguenti fogli:

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
      <td scope="col"> <p>Parametro</p> <p>Opzione Parametro</p> <p>Gruppo di parametri</p> <p>Parametro di Categoria</p> <p>Categoria</p> <p>Rapporto</p> <p>La Sezione della Liguetta Portale</p> <p>Dashboard</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapporto</p> <p>Tutti i report nel sistema sono disponibili per l'esportazione. Puoi selezionare fino a 100 rapporti specifici in una singola esportazione.</p> </td> 
      <td scope="col">Esporta come file ZIP </td> 
      <td scope="col"> <p scope="col">Parametro</p> <p scope="col">Opzione Parametro</p> <p scope="col">Gruppo di parametri</p> <p scope="col">Parametro di Categoria</p> <p scope="col">Categoria</p> <p scope="col">Rapporto</p> <p scope="col">Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Approval</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Approvatore del passaggio</p> <p>Passaggio di approvazione</p> <p>Approval</p> <p>Processo di approvazione</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dati personalizzati</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td scope="col"> <p>Parametro</p> <p>Opzione Parametro</p> <p>Gruppo di parametri</p> <p>Parametro di Categoria</p> <p>Categoria</p> <p>Preferenze</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Tipo di Spesa</p> </td> 
      <td scope="col"> <p>Esporta come file Excel</p> </td> 
      <td> <p>Tipo di Spesa</p> <p>Preferenze</p> </td> 
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
      <td> <p> Coda</p> <p>Progetto</p> <p>Regola di Istradamento</p> <p>Argomento Coda</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Stima Risorse</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Stima Risorse</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Gruppo di risorse</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Gruppo di risorse</p> <p>Preferenze </p> </td> 
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
      <td> <p>Domande Scorecard</p> <p>Opzione scorecard</p> <p>Scorecard</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Attività</td> 
      <td>Esporta come file Excel</td> 
      <td> <p> Attività</p> <p>Preferenze </p> </td> 
     </tr> 
     <tr> 
      <td>Modello</td> 
      <td> Esporta come file Excel</td> 
      <td> <p> Coda</p> <p>Modello</p> <p>Regola di Istradamento</p> <p>Argomento Coda</p> <p>Preferenze </p> </td> 
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
1. Continua con [Compilare il modello del foglio di calcolo con i dati](#populate-the-spreadsheet-template-with-your-data) per compilare il modello con le tue informazioni.

## Compilare il modello del foglio di calcolo con i dati {#populate-the-spreadsheet-template-with-your-data}

* [Informazioni sulle schede (fogli dati) incluse nel foglio di calcolo](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importare un record](#import-a-record)
* [Includi date](#include-dates)
* [Usa caratteri jolly](#use-wildcards)
* [Sostituzione del nome dell&#39;attributo per gli ID](#attribute-name-substitution-for-ids)

### Informazioni sulle schede (fogli dati) incluse nel foglio di calcolo {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Per comprendere meglio come sarà necessario formattare le informazioni in ogni colonna quando si compila il modello Kick-Start, è consigliabile eseguire una pratica esportando un Kick-Start con i dati Workfront esistenti sugli oggetti che si sta tentando di importare. Per istruzioni, consulta [Esportare dati da Adobe Workfront tramite Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando si apre un modello Kick-Starts vuoto, sono disponibili diverse schede (fogli dati). Dipendono dagli oggetti selezionati per il download. Ciascuno rappresenta un oggetto nell&#39;applicazione, ad esempio un progetto, attività, ore, dashboard e utenti:

Quando si apre una di queste schede, nella riga 2 vengono visualizzati i campi di ciascun oggetto che è possibile impostare durante un&#39;importazione. Nell&#39;intestazione di una colonna, dopo la parola &quot;set&quot;, il nome del campo viene visualizzato così come appare nel database. Questi campi fungono da intestazioni di colonna.

>[!IMPORTANT]
>
>Per evitare errori, accertati di quanto segue:
>
>* Non eliminare o modificare in alcun modo questi campi. Ad esempio, non modificare il loro ordine o i loro nomi.
>* Compilare ogni campo con un’intestazione di colonna in grassetto. che rappresentano i campi obbligatori.
>
>  Tuttavia, se un campo obbligatorio contiene un valore predefinito impostato nelle preferenze di sistema, non è necessario compilarlo.
>
>  Ad esempio, nella **Progetto PROJ** scheda **setCondition** e **setConditionType** i campi possono essere lasciati vuoti, ma la **setGroupID** e **setName** Le colonne non possono.

### Importare un record  {#import-a-record}

Ogni riga del foglio corrisponde a un oggetto univoco.

1. Completa la cella nel **isNew** colonna:

   * Se l&#39;oggetto da importare è nuovo, digitare **TRUE** per importare i dati nella riga .
   * Se l’oggetto è già in Workfront, digitare **FALSE** per ignorare la riga.

1. Completa la cella nel **ID** in uno dei seguenti modi:

   * Se l&#39;oggetto da importare è nuovo (e hai digitato **TRUE** in **isNew** ), specifica un numero qualsiasi per l&#39;ID. Questo numero deve essere univoco nel foglio di calcolo.

   * Se l&#39;oggetto da importare esiste già nel sistema Workfront (e hai digitato **FALSE** in **isNew** (colonna), l&#39;ID deve essere il GUID alfanumerico esistente in Workfront per l&#39;oggetto.

      **Esempio:** Per un progetto, il valore visualizzato nel **setGroupID** la colonna deve avere una delle caratteristiche seguenti:

      * GUID di un gruppo esistente nell&#39;istanza Workfront
      * Il valore (numero) nella colonna ID nella colonna **Gruppo** foglio se si sta creando un nuovo gruppo durante l&#39;importazione

         ![](assets/verysimplekickstartprojectimport-350x31.png)

1. Immetti i valori dei campi obbligatori e di tutti gli altri campi che desideri compilare durante l’importazione.
1. (Facoltativo) Per aggiungere dati personalizzati:

   * Crea una nuova colonna per ogni campo personalizzato che desideri includere nel processo di importazione.
   * Denomina ogni nuova colonna per il relativo campo personalizzato come segue: **DE:[Nome del campo personalizzato come visualizzato in Workfront]**.
   * Nella colonna **setCategoryID**, digitare il GUID del modulo personalizzato esistente in cui si trova il campo personalizzato. Questo campo è obbligatorio durante l’importazione di dati personalizzati.
   * Se è necessario aggiungere più valori di dati nel campo personalizzato, ad esempio pulsanti di scelta, caselle di controllo o elenchi, utilizzare il delimitatore di dati personalizzato &quot;|&quot; della barra verticale elencato nella scheda Preferenze per separare i valori.

      **Esempio:** Digitare A|D nella colonna DE:Departments per compilare il reparto A e il reparto D nel modulo personalizzato.

### Includi date  {#include-dates}

Workfront è in grado di elaborare la maggior parte dei formati di data. Tuttavia, è necessario assicurarsi che la colonna data nel foglio di calcolo sia formattata come data. L’importazione avrà esito negativo se la colonna viene formattata come generale, come numero o come testo.

>[!TIP]
>
>Per la maggior parte delle persone è più semplice utilizzare il formato MM/GG/AAAA (ad esempio: 10/07/2022).

Workfront accetta anche valori di ora come parte della data (ad esempio: 10/07/2022 01:30 o 07/10/2022 1:00 PM).

Se ometti un’ora nella data, Workfront effettua una delle seguenti operazioni:

* Presuppone le 12:00. Per visualizzare il risultato della data previsto, il fuso orario del sistema deve corrispondere al tuo fuso orario.
* Se si trova in un oggetto associato a una pianificazione, l&#39;ora si estende al primo tempo consentito dalla pianificazione.

>[!NOTE]
>
>Quando si utilizza un timestamp UNIX, è necessario includere tre zeri aggiuntivi alla fine del valore.
>
>Ad esempio, se la marca temporale è 7336899000, immettere 7336899000000 nella cella.

### Usa caratteri jolly {#use-wildcards}

È possibile utilizzare i seguenti caratteri jolly durante la compilazione del foglio di calcolo del modello Kick-Start:

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
   <td> <p>Quando viene utilizzato su un <strong>setDate</strong> Questo carattere jolly imposta la data come mezzanotte del giorno in cui si importa l’avvio rapido.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly presente in un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi il lunedì della settimana in cui viene importato, indipendentemente dal giorno in cui esegui effettivamente l’importazione, puoi utilizzare <strong>$$OGGIbw</strong>. In questo modo la data di inizio prevista del progetto verrà impostata alle 12:00 di domenica. Poiché il programma del progetto probabilmente non consente il lavoro in quel momento, inizierà alle 9 del mattino del lunedì mattina.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Quando viene utilizzato su un <strong>setDate</strong> Questo carattere jolly imposta la data in base al momento in cui si crea il record durante l'importazione Kick-Start.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly presente in un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi 3 ore dopo l’importazione, puoi utilizzare <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Quando viene utilizzato su un <strong>setAssignedToID</strong> Per un altro campo basato su userID, questo carattere jolly assegna il lavoro o in altro modo associa il record all'utente che esegue l'importazione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CLIENTE</p> </td> 
   <td> <p>Questo carattere jolly è stato aggiunto specificatamente per le importazioni di utenti Kick-Start. Quando viene creato un account Workfront, viene creato un utente con il livello di accesso amministratore di sistema. Il nome utente assegnato all’amministratore predefinito può essere utilizzato come prefisso durante la creazione di altri utenti nell’account.</p> <p>Poiché i nomi utente devono essere univoci per tutti i clienti, questo è utile quando hai diversi individui con nomi utente molto comuni come John Smith, che potrebbero avere un nome utente "jsmith". Anteponendo l’assegnazione del nome utente con il nome utente amministratore predefinito, garantisci che ogni nome utente sia univoco (ad esempio: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Suggerimento: Un modo più elegante per garantire che i nomi utente siano univoci a livello di sistema è quello di inserire l'indirizzo e-mail del singolo utente nel <strong>setUsername</strong> campo .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sostituzione del nome dell&#39;attributo per gli ID  {#attribute-name-substitution-for-ids}

Anche se è consigliabile utilizzare gli ID ogni volta che è possibile, talvolta è scomodo effettuare riferimenti incrociati agli ID da un foglio all’altro quando si imposta un **setAttributeID** valore. È possibile fare riferimento ai valori per nome semplicemente modificando l’intestazione della colonna.

**Esempi:**

* **(importazione del progetto)**

   Durante l’importazione dei progetti, imposta le **setGroupID** dei progetti andando al **Gruppo** , annotando i rispettivi ID di gruppo e incollandoli nelle celle corrette (**setGroupID** nella colonna **Progetto PROJ** foglio.

   Questo è possibile quando si lavora con pochi gruppi e progetti, ma se si lavora con diversi di essi, non è pratico.

   Per eseguire la sostituzione del nome dell&#39;attributo per l&#39;esempio sopra descritto, modificare la **setGroupID** intestazione colonna a **#setGroupID GROUP****name**. A questo punto puoi fare riferimento a ciascun gruppo del progetto per nome.

   >[!NOTE]
   >
   >L&#39;opzione per utilizzare Sostituzione nome attributo è limitata ai riferimenti solo per i record esistenti. Non è possibile utilizzare la sostituzione del nome per gli oggetti creati nella stessa importazione.

* **(importazione utente)**

   Durante l’importazione degli utenti, compila **setRoleID** da un elenco di ruoli nel **Ruolo RUOLO** scheda .

   Alcuni degli ID ruolo sono per i record già esistenti nell&#39;account e altri vengono creati durante l&#39;importazione.

   Per i nuovi record utente assegnati ai ruoli esistenti, è possibile utilizzare la sostituzione del nome. Per i nuovi record utente assegnati a nuovi ruoli importati, non è possibile.

   È possibile utilizzare entrambi i metodi sullo stesso file di importazione:

   * Aggiungi una colonna nel foglio di calcolo a sinistra del **setRoleID** colonna.
   * Denomina la nuova colonna **#setRoleID Nome RULE**.
   * Per le assegnazioni di ruolo a record esistenti, immettere i nomi di ruolo nel **#setRoleID Nome RULE** colonna.

      Per le assegnazioni di ruolo a nuovi record di ruolo, inserisci l&#39;ID assegnato nel foglio Ruolo ROLE nel setRoleID.

      ![](assets/setroleid-350x66.png)

## Importare i dati del foglio di calcolo in Workfront

Dopo aver compilato il modello Excel con i dati, puoi caricarli in Workfront.

L’importazione Kick-Start supporta i seguenti tipi di file:

* Excel basato su XML (&#42;.xlsx)
* Excel legacy (&#42;.xls)
* Ritagliato (&#42;ZIP) file xlsx o xls

   >[!NOTE]
   >
   >Devi utilizzare un file ZIP per importare fogli di calcolo Excel che fanno riferimento a report, documenti e avatar o per visualizzare, filtrare o raggruppare file proprietà. Quando utilizzi un file di importazione ZIP, la &#42;Il file ZIP deve avere lo stesso nome del file &#42;xlsx o &#42;.xls e tutti i contenuti devono trovarsi allo stesso livello di struttura del file (nessuna cartella).


Per importare i dati del foglio di calcolo del modello in Workfront:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** >**Importa dati (Kick-Starts)**.

1. In **Caricare dati con il foglio di calcolo Click-Start** sezione, fai clic su **Scegli file**, quindi individua e seleziona il foglio di calcolo popolato.

1. Fai clic su **Carica.**

   Se il file Excel richiede più di 5 minuti per essere caricato in Workfront, l&#39;applicazione si interrompe e il file non può essere caricato.

   Provare a importare i dati in batch più piccoli di oggetti.

1. (Condizionale) Se utilizzi Workfront Fusion, ora puoi attivare gli FLO o gli scenari.
