---
title: Panoramica dei tipi di record e delle tassonomie
description: I tipi di record sono gli elementi costitutivi di uno spazio di lavoro Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Panoramica dei tipi di record e delle tassonomie

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

A differenza di Workfront, dove i tipi di oggetto sono predefiniti, in Adobe Maestro potete creare tipi di oggetto personalizzati. In Workfront, ad esempio, sono già stati creati i tipi di oggetto Programma, Portfolio, Progetto, Attività o Problema.

I tipi di oggetto Maestro sono denominati &quot;tipi di record&quot;. I tipi di record sono gli elementi costitutivi di uno spazio di lavoro Maestro. Per informazioni sulle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

## Panoramica del tipo di record

In Maestro, puoi creare tipi di record personalizzati che soddisfano le esigenze della tua organizzazione.

* I tipi di record Maestro sono i seguenti:

   * [Tipo di record operativo](#operational-record-type): tipo di record che rappresenta piani strategici, iniziative o lavoro pianificato. Ad esempio, Campaign, Activity, Tactic, Opportunity può essere un tipo di record operativo.
   * [Tassonomia](#taxonomy): tipi di record che acquisiscono attributi relativi a un tipo di record operativo. Ad esempio, Area geografica, Indirizzo e Pubblico possono essere tassonomie.

* Quando si crea un tipo di record, solo l&#39;utente e coloro ai quali sono state assegnate le autorizzazioni di accesso all&#39;area di lavoro possono visualizzare il tipo di record.
* È necessario creare un&#39;area di lavoro prima di poter creare i tipi di record per l&#39;area di lavoro.
* In un&#39;unica area di lavoro è possibile ottenere un totale combinato di 1.000 tipi di record operativi e tassonomie. Sono inclusi i tipi di record o le tassonomie creati da zero o importati da altri sistemi.

### Tipo di record operativo{#operational-record-type}

Un tipo di record operativo è un tipo di record Maestro che rappresenta oggetti correlati al lavoro.

![](assets/operational-record-type-blank.png)

Per ulteriori informazioni sui tipi di record operativi, inclusa la relativa creazione, vedere [Crea tipi di record](../architecture/create-record-types.md).

### Tassonomia{#taxonomy}

Una tassonomia è un tipo di record che acquisisce attributi relativi a un tipo di record operativo.

![](assets/taxonomy-record-type-blank.png)

Per ulteriori informazioni sui tipi di record di tassonomia, vedere [Creare una tassonomia](../architecture/create-a-taxonomy.md).

Sebbene la creazione delle tassonomie sia identica alla creazione dei tipi di record operativi, Maestro distingue concettualmente tra un tipo di record operativo e un tipo di record tassonomia. Lo scopo delle tassonomie è migliorare i tipi di record operativi. Le tassonomie non devono rappresentare direttamente oggetti di lavoro.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

Ad esempio, Pubblico, Area o Indirizzo possono essere tipi di record di tipo tassonomia.

Per ulteriori informazioni, consulta [Creare una tassonomia](../architecture/create-a-taxonomy.md).

## Somiglianze e differenze tra tipi di record operativi e tassonomie

Nella tabella seguente vengono illustrate alcune analogie e differenze tra i tipi di record operativi e le tassonomie:

| Tipo di record e caratteristica | Tipo di record operativo | Tipo di record tassonomia |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| Fanno parte di un’area di lavoro | ✓ | ✓ |
| Puoi crearli automaticamente da un modello di workspace | ✓ | ✓ |
| Puoi crearli manualmente, da zero | ✓ | ✓ |
| È possibile crearli copiando e incollando le informazioni da un file o da un elenco esterno | ✓ | ✓ |
| Puoi creare importando un file Excel o CSV | ✓ |                     |
| È possibile creare tipi di record di sola lettura connettendosi a tipi di oggetto di altre applicazioni | ✓ |                     |
| Rappresentano oggetti correlati al lavoro | ✓ |                      |
| Rappresentano attributi relativi a oggetti correlati al lavoro |                         | ✓ |
| Puoi creare da zero | ✓ | ✓ |
| Puoi creare importando un file Excel o CSV | ✓ |                      |
| È possibile collegare il tipo di record a un oggetto da un&#39;applicazione di terze parti | ✓ |                      |
| È possibile connettersi ad altri tipi di record Maestro | ✓ |                    |
| È possibile visualizzare i record associati in una vista tabella | ✓ | ✓ |
| È possibile visualizzare i record associati in una visualizzazione timeline | ✓ | ✓ |
