---
title: Panoramica sui tipi di record
description: I tipi di record sono i blocchi predefiniti di un'area di lavoro Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Panoramica sui tipi di record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

A differenza di Workfront, dove i tipi di oggetto sono predefiniti, in Adobe Workfront Planning è possibile creare tipi di oggetto personalizzati.

Ad esempio, in Workfront sono già stati creati i tipi di oggetto Programma, Portfolio, Progetto, Attività o Problema.

I tipi di oggetto di Workfront Planning sono denominati &quot;tipi di record&quot; ed esistono solo quando vengono creati dagli utenti.

I tipi di record sono i blocchi predefiniti di un&#39;area di lavoro di Workfront Planning ed è necessario crearli tutti per poterli associare al flusso di lavoro e ad altre informazioni.

I tipi di record sono organizzati in aree di lavoro.

Per informazioni sulle aree di lavoro, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

## Panoramica del tipo di record

In Workfront Planning è possibile creare tipi di record personalizzati che soddisfino le esigenze dell&#39;organizzazione.

Per informazioni sulla creazione di tipi di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

* Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono creati nelle sezioni dell&#39;area di lavoro riportate di seguito.

   * **Tipi di record operativi**: tipi di record che rappresentano piani strategici, iniziative o lavoro pianificato. Ad esempio, Campaign, Activity, Tactic, Opportunity sono tipi di record operativi.
   * **Tassonomie**: tipi di record che acquisiscono attributi relativi a un tipo di record operativo. Ad esempio, Area geografica, Indirizzo e Pubblico sono tassonomie.

  È possibile rinominare o eliminare sezioni e tipi di record oppure crearne altri.

* Quando si crea un tipo di record in un&#39;area di lavoro creata da zero, è possibile inserire il tipo di record in qualsiasi sezione creata nell&#39;area di lavoro.
* Quando si crea un tipo di record, solo l&#39;utente e gli utenti a cui sono state assegnate le autorizzazioni di accesso all&#39;area di lavoro potranno accedervi.
* È necessario creare un&#39;area di lavoro prima di poter creare i tipi di record per l&#39;area di lavoro.

  Per informazioni sui limiti relativi al numero di tipi di record che è possibile avere in un&#39;istanza dell&#39;area di lavoro o di Workfront, vedere [Panoramica sui limiti degli oggetti di Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
* Per utilizzare i tipi di record in più aree di lavoro, è possibile designare i tipi di record come globali o collegabili.

   * I tipi di record globali possono essere aggiunti come tipi di record esistenti ad altre aree di lavoro.
   * I tipi di record collegabili possono essere collegati ad altre aree di lavoro.

  Per ulteriori informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
