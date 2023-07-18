---
user-type: administrator
product-area: system-administration
keywords: kick-start, kick-start, kick-start, kick-start
navigation-topic: use-kick-starts
title: Importare dati in Adobe Workfront utilizzando un modello di avvio
description: I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare a tale scopo, come spiegato in Importazione dati Kick-Start.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 8%

---

# Importare dati in Adobe Workfront utilizzando un modello di avvio

I Kick-Start sono cartelle di lavoro di Excel appositamente formattate che è possibile compilare con i dati che si desidera importare in Workfront. Adobe Workfront fornisce un modello Kick-Start da utilizzare a tale scopo, come spiegato in [Avvia importazione dati](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Questo processo è suddiviso in 3 attività principali:

* Innanzitutto, esportate un modello Kick-Start come file di foglio di calcolo
* In secondo luogo, il foglio di calcolo viene compilato con i dati
* Infine, puoi importare il foglio di calcolo popolato in Workfront

Ognuna di queste procedure è descritta nell&#39;ordine appropriato in questo articolo.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limitazioni

È possibile importare un numero elevato di oggetti in Workfront utilizzando un modello Kick-Start. Tuttavia, considera le seguenti limitazioni:

* L&#39;importazione dei dati in questo modo non aggiorna le informazioni sui record già esistenti in Workfront
* È possibile importare solo i nuovi record e le relative informazioni
* Non importare più di 2.000 record alla volta per evitare il timeout dell&#39;importazione

## Esportare un modello di Kick-Start come file di foglio di calcolo

Quando si esporta un modello Kick-Start, viene visualizzata una cartella di lavoro vuota del foglio di calcolo di Excel. Nelle procedure successive di questo articolo, la cartella di lavoro verrà compilata con le informazioni e quindi importata nuovamente in Workfront.

Per esportare un modello di Kick-Start:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** > **Esporta dati (Kick-Start)**.

1. Clic **Altre opzioni**, quindi selezionare i tipi di informazioni che si desidera includere.

   Ogni opzione selezionata rappresenta una raccolta di più schede nel foglio di calcolo esportato. Ad esempio, se selezioni l’opzione Rapporto, nel foglio di calcolo verranno inclusi tutti gli oggetti necessari per la creazione di un rapporto (viste, filtri, raggruppamenti, rapporti).

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
      <td scope="col"> <p>Approvatore passaggio</p> <p>Passaggio di approvazione</p> <p>Approval</p> <p>Processo di approvazione</p> <p>Preferenze</p> </td> 
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

1. Clic **Scarica**.
1. Continua con [Compilare il modello di foglio di calcolo con i dati](#populate-the-spreadsheet-template-with-your-data) per compilare il modello con le informazioni.

## Compilare il modello di foglio di calcolo con i dati {#populate-the-spreadsheet-template-with-your-data}

* [Informazioni sulle schede (fogli dati) incluse nel foglio di calcolo](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importare un record](#import-a-record)
* [Includi date](#include-dates)
* [Usa caratteri jolly](#use-wildcards)
* [Sostituzione nome attributo per ID](#attribute-name-substitution-for-ids)

### Informazioni sulle schede (fogli dati) incluse nel foglio di calcolo {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Per capire meglio come formattare le informazioni in ogni colonna quando si compila il modello di Kick-Start, è consigliabile eseguire una procedura esportando un Kick-Start con dati Workfront esistenti sugli oggetti che si sta tentando di importare. Per istruzioni, consulta [Esportare dati da Adobe Workfront tramite Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando apri un modello Kick-Start vuoto, sono disponibili diverse schede (fogli dati). Dipendono dagli oggetti selezionati per il download. Ciascuno rappresenta un oggetto nell&#39;applicazione, ad esempio progetto, attività, ore, dashboard e utenti:

Quando si apre una di queste schede, nella riga 2 vengono visualizzati i campi di ogni oggetto che è possibile impostare durante un&#39;importazione. Nell&#39;intestazione di una colonna, dopo la parola &quot;set&quot;, il nome del campo viene visualizzato come appare nel database. Questi campi fungono da intestazioni di colonna.

>[!IMPORTANT]
>
>Per evitare errori, assicurati di quanto segue:
>
>* Non eliminare o modificare questi campi in alcun modo. Ad esempio, non modificare l’ordine o i nomi.
>* Popola ogni campo con un’intestazione di colonna in grassetto. Questi rappresentano campi obbligatori.
>
>  Tuttavia, se un campo obbligatorio contiene un valore predefinito impostato nelle preferenze di sistema, non è necessario compilarlo.
>
>  Ad esempio, nella **Progetto PROJ** , la scheda **setCondition** e **setConditionType** possono essere lasciati vuoti, ma il campo **setGroupID** e **setName** le colonne non possono.
>

### Importare un record  {#import-a-record}

Ogni riga del foglio corrisponde a un oggetto univoco.

1. Completare la cella in **isNew** colonna:

   * Se l&#39;oggetto da importare è nuovo, digitare **TRUE** per importare i dati nella riga.
   * Se l&#39;oggetto è già in Workfront, digitare **FALSE** per ignorare la riga.

1. Completare la cella in **ID** in uno dei modi seguenti:

   * Se l&#39;oggetto che si sta importando è nuovo (e si è digitato **TRUE** nel **isNew** ), specifica un numero qualsiasi per l’ID. Questo numero deve essere univoco nel foglio di calcolo.

   * Se l&#39;oggetto che si sta importando esiste già nel sistema Workfront (e si è digitato **FALSE** nel **isNew** ), l&#39;ID deve essere il GUID alfanumerico esistente in Workfront per quell&#39;oggetto.

     **Esempio:** Per un progetto, il valore visualizzato nel **setGroupID** la colonna deve essere una delle seguenti:

      * GUID di un gruppo esistente nell&#39;istanza di Workfront
      * Il valore (numero) nella colonna ID sulla **Gruppo di gruppi** se si sta creando un nuovo gruppo durante l&#39;importazione

        ![ID di esempio per un gruppo](assets/kick-start-group-example.png)

1. Immetti i valori per i campi obbligatori e per tutti gli altri campi che desideri compilare durante l’importazione.
1. (Facoltativo) Per aggiungere dati personalizzati:

   * Creare una nuova colonna per ogni campo personalizzato che si desidera includere nel processo di importazione.
   * Denomina ogni nuova colonna per il campo personalizzato corrispondente come segue: **DE:[Nome del campo personalizzato visualizzato in Workfront]**.
   * Nella colonna **setCategoryID**, digitare il GUID del modulo personalizzato esistente in cui si trova il campo personalizzato. Questo campo è obbligatorio per l’importazione di dati personalizzati.
   * Per aggiungere più valori di dati nel campo personalizzato, ad esempio pulsanti di scelta, caselle di controllo o elenchi, utilizzare il delimitatore di dati personalizzato a barre verticali &quot;|&quot; elencato nella scheda Preferenze per separare i valori.

     **Esempio:** Digitare A|D nella colonna DE:Reparti per compilare il reparto A e il reparto D nel modulo personalizzato.

### Includi date  {#include-dates}

Workfront è in grado di elaborare la maggior parte dei formati di date. È tuttavia necessario assicurarsi che la colonna data nel foglio di calcolo sia formattata come data. L&#39;importazione avrà esito negativo se la colonna viene formattata come generale, un numero o un testo.

>[!TIP]
>
>Per la maggior parte delle persone è più semplice utilizzare il formato MM/GG/AAAA (ad esempio: 07/10/2022).

Workfront accetta anche valori di ora come parte della data (ad esempio: 07/10/2022 01:30 o 07/10/2022 1:00 PM).

Se si omette un&#39;ora nella data, Workfront esegue una delle operazioni seguenti:

* Presuppone le 00:00. Per visualizzare il risultato della data prevista, il fuso orario del sistema deve corrispondere al proprio.
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
   <td> <p>Se utilizzato su una <strong>setDate</strong> questo carattere jolly imposta la data come mezzanotte del giorno in cui si importa il Kick-Start.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi il lunedì della settimana in cui viene importato, indipendentemente dal giorno in cui esegui effettivamente l’importazione, puoi utilizzare <strong>$$TODAYbw</strong>. In questo modo, la data di inizio pianificata del progetto verrà impostata sulle 00.00 di domenica. Poiché la pianificazione del progetto probabilmente non consente di lavorare in quel momento, inizierà alle 9 di lunedì mattina.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Se utilizzato su una <strong>setDate</strong> questo carattere jolly imposta la data in base al momento in cui si crea il record durante l'importazione Kick-Start.</p> <p>Puoi modificare il carattere jolly utilizzando la sintassi standard consentita con il carattere jolly su un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Se desideri che un progetto inizi 3 ore dopo l’importazione, puoi utilizzare <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Se utilizzato su una <strong>setAssignedToID</strong> o un altro campo basato su userID, questo carattere jolly assegna il lavoro o associa in altro modo il record alla persona che esegue l’importazione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CLIENTE</p> </td> 
   <td> <p>Questo carattere jolly è stato aggiunto specificatamente per le importazioni utente Kick-Start. Quando si crea un account Workfront, viene creato un utente con il livello di accesso Amministratore di sistema. Il nome utente assegnato all’amministratore predefinito può essere utilizzato come prefisso durante la creazione di altri utenti nell’account.</p> <p>Poiché i nomi utente devono essere univoci in tutti i clienti, questo è utile quando esistono diversi utenti con nomi utente molto comuni, ad esempio John Smith, che potrebbero avere un nome utente "jsmith". Anteponendo l'assegnazione del nome utente al nome utente amministratore predefinito, si garantisce che ogni nome utente sia univoco (ad esempio: <strong>$$CLIENTE.jsmith</strong>).</p> <p>Suggerimento: un modo più elegante per garantire che i nomi utente siano univoci a livello di sistema consiste nell’inserire l’indirizzo e-mail dell’utente nel <strong>setUsername</strong> campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sostituzione nome attributo per ID  {#attribute-name-substitution-for-ids}

Sebbene sia una best practice utilizzare gli ID quando possibile, a volte è scomodo incrociare gli ID da un foglio all’altro durante l’impostazione di un **setAttributeID** valore. Puoi fare riferimento ai valori per nome semplicemente modificando l’intestazione della colonna.

**Esempi:**

* **(importazione progetto)**

  Durante l’importazione dei progetti, imposta **setGroupID** dei progetti mediante il collegamento **Gruppo di gruppi** , annotando i rispettivi ID gruppo e incollandoli nelle celle corrette (**setGroupID** ) sulla **Progetto PROJ** foglio.

  Questo è possibile quando si lavora con pochi gruppi e progetti, ma se si lavora con diversi di ciascuno, non è pratico.

  Per eseguire l&#39;operazione Sostituzione nome attributo per l&#39;esempio descritto in precedenza, è necessario modificare **setGroupID** intestazione di colonna a **#setGroupID GROUP****name**. È quindi possibile fare riferimento al gruppo di ogni progetto per nome.

  >[!NOTE]
  >
  >L&#39;opzione per utilizzare la sostituzione nome attributo è limitata ai riferimenti solo per i record esistenti. Non è possibile utilizzare la sostituzione del nome per gli oggetti che si stanno creando nella stessa importazione.

* **(importazione utente)**

  Quando importi gli utenti, compila il **setRoleID** da un elenco di ruoli sul **Ruolo** scheda.

  Alcuni ID Ruolo sono per i record già presenti nell’account, mentre altri vengono creati durante l’importazione.

  Per i nuovi record utente assegnati a ruoli esistenti, è possibile utilizzare la sostituzione dei nomi. Per i nuovi record utente assegnati ai nuovi ruoli importati, non è possibile.

  Ecco come utilizzare entrambi i metodi sullo stesso file di importazione:

   * Aggiungi una colonna nel foglio di calcolo a sinistra del **setRoleID** colonna.
   * Denomina la nuova colonna **#setRoleID nome RUOLO**.
   * Per le assegnazioni di ruolo a record esistenti, immettere i nomi dei ruoli nel **#setRoleID nome RUOLO** colonna.

     Per le assegnazioni di ruolo a nuovi record di ruolo, immettere l&#39;ID assegnato nel foglio Ruolo di ruolo in setRoleID.

     ![ID ruolo per gli utenti](assets/set-role-id.png)

## Importare i dati del foglio di calcolo in Workfront

Dopo aver inserito i dati nel modello di Excel, puoi caricarne i dati in Workfront.

L&#39;importazione Kick-Start supporta i seguenti tipi di file:

* Excel basato su XML (&#42;xlsx)
* Excel legacy (&#42;xls)
* Zipped (&#42;ZIP) file xlsx o xls

  >[!NOTE]
  >
  >Devi utilizzare un file ZIP per importare fogli di calcolo Excel che fanno riferimento a report, documenti e avatar o per visualizzare, filtrare o raggruppare file proprietà. Quando si utilizza un file di importazione compresso, il &#42;Il file ZIP deve avere lo stesso nome del file &#42;.xlsx o &#42;file .xls e tutto il contenuto deve trovarsi allo stesso livello di struttura del file (nessuna cartella).


Per importare i dati del foglio di calcolo del modello in Workfront:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** >**Importa dati (Kick-Start)**.

1. In **Caricare dati con il foglio di calcolo Kick-Start** , fare clic su **Scegli file**, quindi individuare e selezionare il foglio di calcolo popolato.

1. Clic **Carica.**

   Se il caricamento del file Excel in Workfront richiede più di 5 minuti, l’applicazione scade e non è possibile caricare il file.

   Prova a importare i dati in batch più piccoli di oggetti.

1. (Condizionale) Se utilizzi Workfront Fusion, ora puoi attivare i tuoi FLO o scenari.
