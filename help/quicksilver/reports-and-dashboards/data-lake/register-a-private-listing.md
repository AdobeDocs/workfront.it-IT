---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Registra un elenco privato per Workfront Data Connect
description: Registra un’inserzione privata Snowflake per condividere i dati di Workfront Data Connect direttamente con l’account Snowflake della tua organizzazione.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 3%
---
# Registra un elenco privato per Workfront Data Connect

Puoi condividere i dati di Workfront Data Connect direttamente con l’account Snowflake della tua organizzazione registrando un’inserzione privata. Questo metodo di connessione utilizza la funzionalità di inserimento nell’elenco privato di Snowflake per condividere in modo sicuro i dati tra organizzazioni senza esporli pubblicamente e funziona tra aree geografiche e piattaforme di hosting.

Un’inserzione privata è utile quando desideri unire i dati di Workfront con altri dati nel data warehouse aziendale. Poiché i dati vengono memorizzati nel tuo account Snowflake, puoi eseguire query insieme agli altri dati.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Flusso di lavoro Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Sono inoltre necessari un account Snowflake con autorizzazioni per accettare inserzioni e creare database e un diritto a Workfront Data Connect.

## Cosa sono le azioni di un’inserzione privata

Un’inserzione privata ti permette di accedere ai seguenti elementi:

* Oltre 100 visualizzazioni dati per oggetti Workfront. Per la descrizione di ogni visualizzazione, vedere [Dizionario dati Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* Le visualizzazioni dati `*_event`, che contengono ogni transazione di modifica consegnata alle pipeline dati di Data Connect.
* Valori di dati personalizzati per oggetti estensibili ai dati. Ad esempio, vedi l&#39;esempio di query di dati personalizzate in [Esempi di query Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Differenze rispetto a una connessione dell&#39;account di lettura

Un’inserzione privata condivide un set di visualizzazioni diverso rispetto a una connessione a un account di lettura e i dati arrivano secondo una pianificazione diversa. Considera le seguenti differenze:

* Un&#39;inserzione privata condivide solo le `*_event` visualizzazioni. Le visualizzazioni `*_current` e `*_daily_history` sono disponibili tramite un account di lettura, ma non tramite un elenco privato. Puoi crearli nel tuo account Snowflake. Per ulteriori informazioni, vedere [Configurare le visualizzazioni Cronologia corrente e Cronologia giornaliera](#set-up-current-and-daily-history-views) in questo articolo.
* Un’inserzione privata potrebbe non includere tutte le visualizzazioni disponibili tramite un account di lettura. Esempi di visualizzazioni non condivise includono oggetti di Workfront Planning, `MONITORING_DATA_REFRESHES`, `BOOKINGS` e `CLASSIFIER`. Questo elenco non è esaustivo.
* Data Connect carica gli eventi di modifica ogni 4 ore. Poiché un’inserzione privata richiede un ulteriore passaggio di replica per far emergere i dati, l’arrivo dei dati dovrebbe richiedere circa 1 ora in più rispetto a quando avviene tramite un account di lettura.
* La replica dei dati viene eseguita alle 01:01, 05:01, 09:01, 13:01, 17:01 e 21:01 UTC. I dati sono generalmente disponibili entro circa 10 minuti dopo ogni esecuzione.
* Le visualizzazioni `MONITORING_DATA_REFRESHES` e `JOB_HISTORY` non riflettono le volte in cui i dati diventano disponibili tramite un&#39;inserzione privata. Sebbene la visualizzazione `JOB_HISTORY` sia condivisa tramite l&#39;elenco privato, è consigliabile leggerla tramite un account di lettura per identificare più rapidamente i processi non riusciti.

## Registra un&#39;inserzione privata

Per registrare un’inserzione privata, raccogli innanzitutto i dettagli del tuo account Snowflake, quindi aggiungi l’inserzione in Workfront.

### Raccogli i dettagli del tuo account Snowflake

Workfront utilizza i dettagli del tuo account Snowflake per indirizzare l’inserzione al tuo account. Raccogli i seguenti dettagli:

* Localizzatore account
* URL account
* Organizzazione dell’account
* Nome account

Ciascuno di questi valori è disponibile dalla finestra modale Dettagli account in Snowflake.

Per trovare i dettagli dell&#39;account:

1. Dopo aver effettuato l’accesso al tuo account Snowflake, fai clic sul menu utente nell’angolo in basso a sinistra.

1. Seleziona l&#39;account nella sezione **Account** del menu.

1. Fare clic su **Visualizza dettagli account** per l&#39;account.

1. Registra ciascuno dei valori elencati sopra.

Decidi anche il nome del database tramite il quale desideri accedere ai dati Workfront collegati. Immetti questo nome al momento della registrazione dell&#39;inserzione.

### Aggiungere l’inserzione privata in Workfront

Registra l’inserzione privata tramite l’interfaccia di Adobe Workfront.

>[!IMPORTANT]
>
>Puoi creare una sola inserzione privata per ogni identificatore di account.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Setup**.

1. Nel pannello a sinistra, fai clic su **Sistema** > **Connessione dati**.

1. Fare clic sulla scheda **connessioni Snowflake**.

1. Fai clic su **Aggiungi inserzione privata**.

1. Completa il modulo con i dettagli dell’account raccolti, compreso il nome del database preferito.

1. Fai clic su **Aggiungi inserzione privata**.

### Connettersi all’elenco in Snowflake

Nel tuo account Snowflake, stabilisci una connessione all’inserzione privata come origine dati esterna. Puoi quindi eseguire una query sui dati Workfront insieme al resto dei dati.

## Impostare le visualizzazioni Cronologia corrente e Cronologia giornaliera

Una connessione dell&#39;account di lettura fornisce tre visualizzazioni dati per ogni tabella di oggetti:

* **Corrente**: una rappresentazione a bassa latenza dei dati attualmente presenti nell&#39;applicazione di origine.
* **Cronologia giornaliera** — una rappresentazione dei dati così come erano alle 23:59 UTC per ogni giorno.
* **Evento**: ogni transazione di modifica recapitata alle pipeline dati di connessione dati.

Un’inserzione privata condivide solo la vista Evento. In questa sezione vengono fornite istruzioni SQL per creare le visualizzazioni Corrente, Cronologia giornaliera ed Evento nel proprio account Snowflake.

Tutte le visualizzazioni evento incluse nell’elenco dispongono dei campi necessari per la logica di visualizzazione riportata di seguito. In questi esempi si presuppone che sia stato creato un nuovo database e uno schema a scelta nell&#39;account Snowflake di destinazione e che venga utilizzata la visualizzazione `projects_event`. In ogni esempio, sostituisci `<listing_db>` e `<listing_schema>` con i tuoi valori.

>[!TIP]
>
>Si consiglia di sostituire `select *` con un elenco delle colonne utilizzate per l&#39;analisi. Se si utilizza `select *` e le colonne vengono aggiunte successivamente alla visualizzazione eventi dell&#39;elenco, è necessario ricreare la visualizzazione per abilitare le nuove colonne.

### Visualizzazioni correnti

La visualizzazione corrente di un oggetto è l&#39;ultimo record evento di modifica memorizzato in Connessione dati. Se l&#39;ultimo record è in stato Eliminato, il record viene omesso dalla visualizzazione Corrente. Tutte le visualizzazioni evento hanno la stessa struttura.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

Le colonne `deleted` e `end_effective_timestamp` non sono necessarie nella visualizzazione corrente. La visualizzazione filtra i dati in un singolo valore e rimuove completamente il record se viene eliminato.

### Visualizzazioni cronologia giornaliera

La visualizzazione Cronologia giornaliera identifica il record dell&#39;evento di modifica attivo al 23:59:59 di una data specificata, in modo da poter generare tendenze sullo stato del record nel tempo. Nell&#39;esempio seguente viene indicato lo stato di un record di progetto alla fine di ogni giorno di calendario.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Visualizzazioni evento

Per coerenza, si consiglia di creare una copia della visualizzazione evento dal database delle voci e di inserirla nello stesso schema delle visualizzazioni Cronologia corrente e Cronologia giornaliera.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
