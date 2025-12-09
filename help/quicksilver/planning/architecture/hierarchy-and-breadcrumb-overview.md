---
title: Panoramica della gerarchia e delle breadcrumb
description: È possibile creare più gerarchie di aree di lavoro tra i tipi di record di un'area di lavoro.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Panoramica della gerarchia e delle breadcrumb

In qualità di responsabile del workspace, in Adobe Workfront Planning è possibile definire gerarchie flessibili ma strutturate tra tipi di record e altri tipi di oggetto.

Le gerarchie sono connessioni tra tipi di record. In una gerarchia è possibile connettere fino a 4 tipi di record e di oggetti.

Per informazioni sulla creazione di gerarchie, vedere [Creare gerarchie di aree di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Di seguito sono riportati i vantaggi dell’utilizzo delle gerarchie nelle aree di lavoro:

* Organizzare il lavoro in modo che rifletta il modo in cui i team pianificano, operano e distribuiscono.
* Per consentire agli utenti di capire dove si trovano, come si connettono i tipi di record e come la strategia fluisce nell’esecuzione facendo riferimento a un set di breadcrumb che indicano la loro posizione nel sistema.
* Per migliorare la navigazione e creare chiarezza e continuità in tutti i flussi di lavoro.
* Definire flussi che si adattino al funzionamento dell&#39;organizzazione, supportando flessibilità e coerenza in tutte le fasi del lavoro.

## Considerazioni durante l’utilizzo delle gerarchie

* In qualità di responsabile dell&#39;area di lavoro, puoi creare più gerarchie per un&#39;area di lavoro.
* Se esiste già una connessione tra i tipi di record selezionati, il sistema riutilizza la connessione esistente.
* Se non esiste alcuna connessione, Workfront ne creerà automaticamente una come parte dell’impostazione della gerarchia.
* Di seguito sono riportate le regole per l&#39;impostazione della gerarchia:
   * Un tipo di record può avere un solo tipo di record padre in una determinata area di lavoro.

     Ad esempio, un tipo di record Tattico non può avere come padre sia un tipo di record Campagna che un tipo di record Obiettivo nella stessa area di lavoro.
   * Un record può essere connesso a più record padre dello stesso tipo quando si connette uno a molti o molti a molti tipi di record.
Ad esempio, la tattica A può appartenere sia alla campagna X che alla campagna Y.
   * Un tipo di record può connettersi a più tipi di record figlio.

     Ad esempio, un tipo di record Campaign può essere padre di più altri tipi di record, come Tattiche, Test e altri tipi di record.
   * Le gerarchie possono includere sia i tipi di record di Planning che i tipi di oggetto di Workfront.

     È ad esempio possibile avere un tipo di record Campagna con Tattiche di pianificazione e Progetti Workfront come figli.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * I tipi di record globali possono essere visualizzati in più aree di lavoro all&#39;interno di più gerarchie. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * I tipi di oggetto Workfront possono inoltre essere visualizzati in più gerarchie e in aree di lavoro diverse.
   * I tipi di record globali non possono far parte di gerarchie in aree di lavoro diverse.

     Ad esempio, se una campagna è un tipo di record globale e fa parte di una gerarchia in Workspace 1, può essere aggiunta come tipo di record esistente a Workspace 2 ma non può far parte di una gerarchia. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * Anche i tipi di record con connessioni che non creano un campo corrispondente nei tipi di record collegati possono far parte di gerarchie. Per impostazione predefinita, le nuove connessioni create durante l&#39;impostazione della gerarchia creeranno sempre un campo corrispondente nei tipi di record collegati.

## Considerazioni durante la visualizzazione delle breadcrumb

Quando si creano gerarchie tra tipi di record, vengono generate breadcrumb per i record che appartengono a tali tipi di record.

Ad esempio, se si crea una gerarchia e si connettono Campagne con Tattiche con Programmi e quindi Progetti, quando si passa a un record di qualsiasi tipo connesso nella gerarchia, è possibile visualizzare la posizione nella gerarchia in cui è posizionato il record.

Considera quanto segue:

* Se un tipo di record fa parte di più gerarchie in più aree di lavoro, è possibile passare da una gerarchia all&#39;altra dalla breadcrumb del record nella pagina del record.
* Le breadcrumb funzionano in Workfront e Planning.

  Ad esempio, quando si esamina un progetto connesso alle campagne e alle tattiche di Planning, nonché ai portfolio e ai programmi di Workfront, è possibile passare dalla gerarchia di Planning a quella di Workfront e viceversa.

  Per ulteriori informazioni, vedere [Creare gerarchie area di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


