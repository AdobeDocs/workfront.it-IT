---
title: Panoramica della gerarchia e delle breadcrumb
description: Dopo aver connesso i tipi di record, è possibile creare più gerarchie di aree di lavoro tra i tipi di record di un'area di lavoro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---



# Panoramica della gerarchia e delle breadcrumb

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

In qualità di responsabile del workspace, in Adobe Workfront Planning è possibile definire gerarchie flessibili ma strutturate tra tipi di record connessi e altri tipi di oggetti.

Le gerarchie sono connessioni tra tipi di record o tra tipi di record e un progetto Workfront.

Per informazioni sulla creazione di gerarchie, vedere [Creare gerarchie di aree di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Di seguito sono riportati i vantaggi dell’utilizzo delle gerarchie nelle aree di lavoro:

* Organizzare il lavoro in modo che rifletta il modo in cui i team pianificano, operano e distribuiscono.
* Per consentire agli utenti di capire dove si trovano, come si connettono i tipi di record e come la strategia fluisce nell’esecuzione facendo riferimento a un set di breadcrumb che indicano la loro posizione nel sistema.
* Per migliorare la navigazione e creare chiarezza e continuità in tutti i flussi di lavoro.
* Definire flussi che si adattino al funzionamento dell&#39;organizzazione, supportando flessibilità e coerenza in tutte le fasi del lavoro.

## Considerazioni durante l’utilizzo delle gerarchie

* Puoi creare fino a 5 gerarchie per un’area di lavoro.
* In una gerarchia è possibile connettere fino a 4 tipi di record e di oggetti.
* In una gerarchia di workspace è possibile connettere solo i seguenti tipi di oggetto:
   * Tipi di record che appartengono all&#39;area di lavoro in cui si stanno creando le gerarchie.
   * Progetti Workfront. I progetti Workfront non possono essere aggiunti come elementi padre di altri tipi di record. Sono sempre l&#39;ultimo tipo di oggetto in una gerarchia.
* Non è possibile aggiungere i seguenti tipi di oggetto in una gerarchia:
   * Tipi di record di altre aree di lavoro, anche se impostati come tipi di record collegabili o globali. È possibile aggiungere tipi di record globali alle gerarchie solo quando sono stati aggiunti all&#39;area di lavoro da cui si sta creando la gerarchia.
   * Tutti gli altri oggetti di Workfront.
   * AEM Assets.
* Le gerarchie possono includere contemporaneamente sia i tipi di record di Planning che i progetti Workfront.

  È possibile, ad esempio, disporre di un tipo di record Campaign con Tattiche di pianificazione e Progetti Workfront come elementi figlio nella stessa gerarchia dell&#39;area di lavoro.

* Se esiste già una connessione tra i tipi di record selezionati, il sistema riutilizza la connessione esistente.
* Se non esiste alcuna connessione, Workfront ne creerà una come parte dell’impostazione della gerarchia.
* L&#39;impostazione **Crea campo corrispondente nel tipo di record collegato** deve essere attivata per il campo connesso per i record e i tipi di oggetto che si desidera includere in una gerarchia.
* Non è possibile eliminare un tipo di record se fa parte di una gerarchia.
* Non è possibile eliminare un campo di connessione se il tipo di record a cui si fa riferimento nel campo fa parte di una gerarchia. Prima di eliminare il tipo di record, è necessario rimuovere il tipo di record dalla gerarchia o eliminare la gerarchia.
* È possibile eliminare un campo di ricerca da un tipo di record connesso. Impossibile recuperare le informazioni nel campo.
* Di seguito sono riportate le regole per l&#39;impostazione della gerarchia:
   * Un tipo di record può avere un solo tipo di record padre in una determinata area di lavoro.

     Ad esempio, un tipo di record Tattico non può avere come padre sia un tipo di record Campagna che un tipo di record Obiettivo nella stessa area di lavoro.
   * Un tipo di record può essere il padre in più gerarchie.

     Ad esempio, puoi avere tre gerarchie diverse in un’area di lavoro e ciascuna di esse può avere Campagne come tipo di record principale.
   * Un record può essere connesso a più record padre dello stesso tipo quando si connette uno a molti o molti a molti tipi di record.

     Ad esempio, la tattica A può appartenere sia alla campagna X che alla campagna Y.
   * Un tipo di record può connettersi a un solo tipo di record figlio alla volta. Un tipo di record figlio può anche essere padre di un altro tipo di record.

     Ad esempio, un tipo di record Campaign può essere padre di un solo altro tipo di record nella stessa gerarchia (Tactics) e Tactics può essere a sua volta padre di Programmi che possono essere padre di Progetti.
   * Un tipo di record non può essere il padre in una gerarchia e il figlio in un&#39;altra gerarchia nello stesso workspace.
   * I tipi di record globali possono essere visualizzati in più aree di lavoro all&#39;interno di più gerarchie, dopo essere stati aggiunti a tali aree.

     Ad esempio, se una campagna è un tipo di record globale e fa parte di una gerarchia in Workspace 1, può essere aggiunta come tipo di record esistente a Workspace 2 e può far parte di una gerarchia. Tuttavia, non può far parte di una gerarchia in Workspace 2 solo se designato come tipo di record globale in Workspace 1, ma non aggiunto a Workspace 2.
   * Quando i tipi di record connessi fanno parte di gerarchie, è possibile collegare un record da un tipo di record figlio a un massimo di 10 record da un tipo di record padre.

     Ad esempio, se crei una gerarchia tra Campagne come record principale e Persona come record secondario, puoi collegare la stessa persona a un massimo di 10 campagne.

## Considerazioni durante la visualizzazione delle breadcrumb

Quando si creano gerarchie tra tipi di record, vengono generate breadcrumb per i record che appartengono a tali tipi di record.

Ad esempio, se si crea una gerarchia e si collegano Campagne con Tattiche, quindi con Attività e quindi con Progetti, quando si passa a un record di qualsiasi tipo connesso nella gerarchia, è possibile visualizzare la posizione del record nella gerarchia.

![Breadcrumb](assets/breadcrumbs-on-project.png)

Considera quanto segue:

* Se un tipo di record fa parte di più gerarchie, è possibile passare da una gerarchia all&#39;altra dalla breadcrumb del record nella pagina del record.
* Se il tipo di record in una gerarchia dispone di più record, è possibile selezionare i record dalla breadcrumb.
* Le breadcrumb funzionano in Workfront e Planning.

  Ad esempio, quando si esamina un progetto connesso alle campagne e alle tattiche di Planning, nonché ai portfolio e ai programmi di Workfront, è possibile passare sia dal tipo di oggetto Planning che da quello di Workfront dalla breadcrumb.

  Per ulteriori informazioni, vedere [Creare gerarchie area di lavoro](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* Quando si modifica un record, le modifiche sono visibili da tutte le aree di lavoro e da tutte le gerarchie di cui fa parte il record.


