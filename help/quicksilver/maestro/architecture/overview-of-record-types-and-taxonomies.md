---
title: Panoramica dei tipi di record
description: I tipi di record sono i blocchi predefiniti di un'area di lavoro Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b2ec979cf9aa2431c8c908440c227758d9dab521
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Panoramica dei tipi di record

{{maestro-important-intro}}

A differenza di Workfront, dove i tipi di oggetto sono predefiniti, in Adobe Workfront Planning è possibile creare tipi di oggetto personalizzati. In Workfront, ad esempio, sono già stati creati i tipi di oggetto Programma, Portfolio, Progetto, Attività o Problema.

I tipi di oggetto di Workfront Planning sono denominati &quot;tipi di record&quot; e possono essere creati e personalizzati tutti. I tipi di record sono i blocchi predefiniti di un&#39;area di lavoro di Workfront Planning. Per informazioni sulle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

## Panoramica del tipo di record

In Workfront Planning è possibile creare tipi di record personalizzati che soddisfino le esigenze dell&#39;organizzazione.

* Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono creati nelle sezioni dell&#39;area di lavoro riportate di seguito.

   * [Tipi di record operativi](#operational-record-type): tipo di record che rappresenta piani strategici, iniziative o lavoro pianificato. Ad esempio, Campaign, Activity, Tactic, Opportunity può essere un tipo di record operativo.
   * [Tassonomie](#taxonomy): tipi di record che acquisiscono attributi relativi a un tipo di record operativo. Ad esempio, Area geografica, Indirizzo e Pubblico possono essere tassonomie.

* Quando si crea un tipo di record in un&#39;area di lavoro creata da zero, è possibile inserire il tipo di record in qualsiasi sezione creata nell&#39;area di lavoro.
* Quando si crea un tipo di record, solo l&#39;utente e coloro ai quali sono state assegnate le autorizzazioni di accesso all&#39;area di lavoro possono visualizzare il tipo di record.
* È necessario creare un&#39;area di lavoro prima di poter creare i tipi di record per l&#39;area di lavoro.
* È possibile avere un totale di 1.000 tipi di record in un&#39;area di lavoro, indipendentemente dal numero di sezioni dell&#39;area di lavoro. Sono inclusi i tipi di record creati da zero o quando si utilizza un modello.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

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
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->