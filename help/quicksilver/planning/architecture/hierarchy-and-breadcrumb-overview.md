---
title: Panoramica della gerarchia e delle breadcrumb
description: È possibile creare più gerarchie di aree di lavoro tra i tipi di record di un'area di lavoro.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

Di seguito sono riportati i vantaggi dell’utilizzo delle gerarchie nelle aree di lavoro:

* Organizzare il lavoro in modo che rifletta il modo in cui i team pianificano, operano e distribuiscono.
* Gli utenti capiscono dove si trovano, come si connettono i tipi di record e come la strategia fluisce nell’esecuzione facendo riferimento a un set di breadcrumb che indicano la loro posizione nel sistema.
* Offri una navigazione migliore e crea chiarezza e continuità in tutti i flussi di lavoro.
* Le gerarchie non impongono una struttura rigida definita dal sistema, ma consentono di definire flussi che si adattano al funzionamento dell’organizzazione, supportando sia la flessibilità che la coerenza in tutte le fasi del lavoro.

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
   * I tipi di record globali possono essere visualizzati in più aree di lavoro all&#39;interno di più gerarchie.
   * I tipi di oggetto Workfront possono inoltre essere visualizzati in più gerarchie e in aree di lavoro diverse.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Anche i tipi di record con connessioni che non creano un campo corrispondente nei tipi di record collegati possono far parte di gerarchie. Per impostazione predefinita, le nuove connessioni create durante l&#39;impostazione della gerarchia creeranno sempre un campo corrispondente nei tipi di record collegati.

## Considerazioni durante la visualizzazione delle breadcrumb


