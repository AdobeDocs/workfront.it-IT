---
title: Panoramica della gerarchia e delle breadcrumb
description: È possibile creare più gerarchie di aree di lavoro tra i tipi di record di un'area di lavoro.
hide: true
hidefromtoc: true
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '752'
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

Le gerarchie sono connessioni tra tipi di record o tra tipi di record e un progetto Workfront.

Per informazioni sulla creazione di gerarchie, vedere [Creare gerarchie di aree di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Di seguito sono riportati i vantaggi dell’utilizzo delle gerarchie nelle aree di lavoro:

* Organizzare il lavoro in modo che rifletta il modo in cui i team pianificano, operano e distribuiscono.
* Per consentire agli utenti di capire dove si trovano, come si connettono i tipi di record e come la strategia fluisce nell’esecuzione facendo riferimento a un set di breadcrumb che indicano la loro posizione nel sistema.
* Per migliorare la navigazione e creare chiarezza e continuità in tutti i flussi di lavoro.
* Definire flussi che si adattino al funzionamento dell&#39;organizzazione, supportando flessibilità e coerenza in tutte le fasi del lavoro.

## Considerazioni durante l’utilizzo delle gerarchie

* È possibile creare più gerarchie per un&#39;area di lavoro.
* In una gerarchia è possibile connettere fino a 4 tipi di record e di oggetti.
* In una gerarchia di workspace è possibile connettere solo i seguenti tipi di oggetto:
   * Tipi di record che appartengono all&#39;area di lavoro in cui si stanno creando le gerarchie.
   * Progetti Workfront. I progetti Workfront non possono essere aggiunti come elementi padre di altri tipi di record. Sono sempre l&#39;ultimo figlio di una gerarchia.
* Non è possibile aggiungere i seguenti tipi di oggetto in una gerarchia:
   * Tipi di record di altre aree di lavoro, anche se impostati come tipi di record collegabili o globali. È possibile aggiungere tipi di record globali alle gerarchie solo quando sono stati aggiunti all&#39;area di lavoro da cui si sta creando la gerarchia.
   * Tutti gli altri oggetti di Workfront.
   * AEM Assets
* Le gerarchie possono includere contemporaneamente sia i tipi di record di Planning che i progetti Workfront.

      È ad esempio possibile avere un tipo di record Campaign con Planning Tactics e Workfront Projects come figli nella stessa gerarchia dell&#39;area di lavoro.
  * Se esiste già una connessione tra i tipi di record selezionati, il sistema riutilizza la connessione esistente.
* Se non esiste alcuna connessione, Workfront ne creerà una come parte dell’impostazione della gerarchia.
* L&#39;impostazione **Crea campo corrispondente nel tipo di record collegato** deve essere attivata per il campo connesso per i record e gli oggetti che si desidera includere in una gerarchia.
* Di seguito sono riportate le regole per l&#39;impostazione della gerarchia:
   * Un tipo di record può avere un solo tipo di record padre in una determinata area di lavoro.

     Ad esempio, un tipo di record Tattico non può avere come padre sia un tipo di record Campagna che un tipo di record Obiettivo nella stessa area di lavoro.
   * Un tipo di record può essere il padre in più gerarchie.

     Ad esempio, puoi avere tre gerarchie diverse in un’area di lavoro e ciascuna di esse può avere Campagne come tipo di record principale.
   * Un record può essere connesso a più record padre dello stesso tipo quando si connette uno a molti o molti a molti tipi di record.
Ad esempio, la tattica A può appartenere sia alla campagna X che alla campagna Y.
   * Un tipo di record può connettersi a più tipi di record figlio.

     Ad esempio, un tipo di record Campaign può essere padre di più altri tipi di record, come Tattiche, Test e altri tipi di record.
   * I tipi di record globali possono essere visualizzati in più aree di lavoro all&#39;interno di più gerarchie, dopo essere stati aggiunti a tali aree.

     Ad esempio, se una campagna è un tipo di record globale e fa parte di una gerarchia in Workspace 1, può essere aggiunta come tipo di record esistente a Workspace 2 e può far parte di una gerarchia. Tuttavia, non può far parte di una gerarchia in Workspace 2 solo se designato come tipo di record globale in Workspace 1, ma non aggiunto a Workspace 2.


## Considerazioni durante la visualizzazione delle breadcrumb

Quando si creano gerarchie tra tipi di record, vengono generate breadcrumb per i record che appartengono a tali tipi di record.

Ad esempio, se si crea una gerarchia e si collegano Campagne con Tattiche, quindi con Attività e quindi con Progetti, quando si passa a un record di qualsiasi tipo connesso nella gerarchia, è possibile visualizzare la posizione del record nella gerarchia.

Considera quanto segue:

* Se un tipo di record fa parte di più gerarchie, è possibile passare da una gerarchia all&#39;altra dalla breadcrumb del record nella pagina del record.
* Le breadcrumb funzionano in Workfront e Planning.

  Ad esempio, quando si esamina un progetto connesso alle campagne e alle tattiche di Planning, nonché ai portfolio e ai programmi di Workfront, è possibile passare sia dal tipo di oggetto Planning che da quello di Workfront dalla breadcrumb.

  Per ulteriori informazioni, vedere [Creare gerarchie area di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


