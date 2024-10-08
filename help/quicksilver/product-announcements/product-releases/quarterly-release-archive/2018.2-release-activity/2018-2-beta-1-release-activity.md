---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.2 di Beta 1
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 1. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 22 marzo 2018. Sarà disponibile nell’ambiente di produzione a giugno 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# Attività sulla versione 2018.2 di Beta 1

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 1. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 22 marzo 2018. Sarà disponibile nell’ambiente di produzione a giugno 2018.

>[!IMPORTANT]
>
>La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.2, consulta [Panoramica delle attività sulla versione 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versione 2018.2 di Beta 1 contiene i seguenti miglioramenti:

* [Modifica date attività nel Diagramma di Gantt](#modify-task-dates-in-the-gantt-chart)
* [Accedere al diagramma di Gantt del progetto dalla scheda Aggiornamenti](#access-the-project-gantt-chart-from-the-updates-tab) (temporaneamente rimosso)

* [Vari collegamenti reintrodotti ai documenti nell&#39;elenco dei documenti](#various-links-re-introduced-to-documents-on-the-document-list)
* [Miglioramenti alla visualizzazione utente nella Programmazione delle risorse](#user-view-improvements-in-the-resource-planner)
* [Nuova esperienza elenco progetti](#new-project-list-experience)
* [Nuova scheda Cerca aggiornamenti](#new-look-for-updates-tab)
* [Miglioramenti per dispositivi mobili](#mobile-improvements)

## Modificare le date delle attività nel diagramma di Gantt {#modify-task-dates-in-the-gantt-chart}

Ora puoi trascinare il campo delle attività per modificare l’Inizio pianificato e le Date di completamento pianificate nel diagramma di Gantt. Con questa modifica, puoi applicare scenari What-If al progetto senza influire sulla timeline.

Prima di questa modifica, era possibile modificare le date delle attività solo nell&#39;elenco delle attività o a livello di attività.

Per ulteriori informazioni, vedere [Aggiornare le informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Accedere al diagramma di Gantt del progetto dalla scheda Aggiornamenti {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Questa funzionalità è stata temporaneamente rimossa dall’ambiente di anteprima.

È ora possibile accedere al nuovo diagramma di Gantt del progetto dalla scheda Aggiornamenti. Quando un utente modifica la Data di conferma di un’attività in modo da influenzare la sequenza temporale del progetto, puoi visualizzarne l’impatto nel diagramma di Gantt del progetto.

Prima di questa modifica, il collegamento Timeline progetto apriva il Grafico di Gantt legacy.

Per ulteriori informazioni, vedere [Panoramica sulla data di conferma](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Per ulteriori informazioni, vedere [Panoramica di Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Sono stati reintrodotti diversi collegamenti ai documenti nell&#39;elenco dei documenti {#various-links-re-introduced-to-documents-on-the-document-list}

Nella versione 18.1, vari collegamenti sono stati rimossi dai documenti nell’elenco e spostati in altre aree dell’interfaccia (ad esempio un pulsante accanto al nome del documento e altri in un menu a discesa sul pulsante). Con questa versione, i seguenti collegamenti vengono reintrodotti sotto il nome del documento e sono ora disponibili sui singoli documenti all’interno dell’elenco dei documenti:

* Genera bozza (disponibile quando non è ancora stata generata una bozza)
* Apri bozza (disponibile quando viene generata una bozza)
* Dettagli documento (disponibile quando non è ancora stata generata una bozza)
* Dettagli bozza (disponibili quando viene generata una bozza)
* Stampa riepilogo

Le azioni seguenti non vengono reintrodotte come collegamenti nel documento all&#39;interno dell&#39;elenco dei documenti:

* Condividi (ancora disponibile come pulsante nel menu)
* Check-Out/Check-In (disponibile nel menu a discesa Altro del menu)

Per ulteriori informazioni, vedere le sezioni seguenti:

*  in 

## Miglioramenti nella visualizzazione utente nella Programmazione delle risorse {#user-view-improvements-in-the-resource-planner}

La Visualizzazione utente della Programmazione delle risorse contiene ora i seguenti miglioramenti:

* La Vista utente è ora la vista predefinita, che sostituisce la Vista progetto.
* Sono stati migliorati i filtri che estraggono informazioni dall’intero database, anziché solo quelle visualizzate sullo schermo.
* Modalità a tutto schermo.
* Le prestazioni sono ora più veloci ed efficienti.

   * Nuovi limiti per il numero di utenti, progetti, ruoli e attività che è possibile visualizzare.
   * Caricamento lento, per un caricamento più rapido degli utenti.

La seguente funzionalità è stata temporaneamente disabilitata in Pianificazione risorse:

* Esportazione dei dati dalla Programmazione delle risorse quando si utilizza la Visualizzazione utente.

Prima di questi miglioramenti, è stato segnalato che la pianificazione delle risorse era lenta da caricare e che erano state notate incongruenze nei dati visualizzati. Grazie a questi miglioramenti, ora dovrebbero essere eliminati.

Per ulteriori informazioni sulle aree della Programmazione delle risorse, vedere [Panoramica sulla navigazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nuova esperienza nell’elenco dei progetti {#new-project-list-experience}

È ora disponibile una nuova esperienza quando visualizzi un elenco di progetti. Questa esperienza include prestazioni migliorate e una navigazione degli elenchi più fluida e veloce. Solo gli elenchi nella scheda Progetti dell’area Progetti di Workfront sono stati aggiornati a questa nuova esperienza.

Nella maggior parte dei casi, le modifiche riguardano la velocità e l&#39;efficienza dell&#39;elenco. Sono state inoltre introdotte le seguenti modifiche visibili:

* Per impostazione predefinita, l’elenco visualizza fino a 2.000 elementi.

  Prima di questo miglioramento, l’elenco mostrava 100 elementi.

* I raggruppamenti sono compressi per impostazione predefinita.

  Prima di questa modifica, i raggruppamenti venivano espansi per impostazione predefinita.

* L&#39;area per la selezione di una riga è stata estesa all&#39;intera riga.

Le seguenti funzioni sono state temporaneamente disattivate negli elenchi di progetti specificati:

* Ridimensionamento delle colonne (questa funzionalità è stata reintrodotta nella versione 2018.2 di Beta 5)
* Riordinamento colonne
* I campi dell’icona di stato vengono visualizzati come vuoti (questa funzionalità è stata reintrodotta nella versione 2018.2 di Beta 5)
* Il grafico Gantt non è accessibile (questa funzionalità è stata reintrodotta nella versione 2018.2 di Beta 3).

Per ulteriori informazioni sull&#39;utilizzo degli elenchi, vedere [Introduzione agli elenchi in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nuova scheda Cerca aggiornamenti {#new-look-for-updates-tab}

>[!NOTE]
>
>Per alcuni utenti, la nuova scheda Aggiornamenti potrebbe non essere visualizzata nell’ambiente di anteprima. Il nostro team di sviluppo sta attualmente risolvendo il problema e sta lavorando per risolverlo il prima possibile.

L’aspetto della scheda Aggiornamenti è stato modificato per essere più allineato con altre aree dell’interfaccia. Questa modifica si applica a progetti, attività, problemi e documenti.

Nella tabella seguente sono riportati gli aggiornamenti apportati alla scheda Aggiornamenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Azione utente precedente</strong> </p> </th> 
   <th> <p><strong>Azione per nuovo utente</strong> </p> </th> 
   <th> <p><strong>Per ulteriori informazioni, vedere...</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Registrazione dell’ora su una scheda orario</p> </td> 
   <td> <p>Fare clic sul collegamento Tempo di registrazione</p> </td> 
   <td> <p>Fare clic sul pulsante Tempo di registrazione</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrare ore</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Esclusione degli aggiornamenti di sistema nella scheda Aggiornamenti</p> </td> 
   <td> <p>Fai clic sul collegamento Filtra aggiornamenti sistema</p> </td> 
   <td> <p>Disattiva l’interruttore Mostra registro attività</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizzazione degli aggiornamenti di sistema nella scheda Aggiornamenti</p> </td> 
   <td> <p>Fai clic su Mostra tutti gli aggiornamenti</p> </td> 
   <td> <p>Abilita l’interruttore Mostra registro attività</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione di tag ad altri utenti in caso di aggiornamento o commento</p> </td> 
   <td> <p>Fai clic sull’icona Includi altri in questo aggiornamento</p> </td> 
   <td> <p>Aggiungere utenti e team nel campo Notifica</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Consenti solo agli utenti della tua azienda di visualizzare un oggetto</p> </td> 
   <td> <p>Fai clic sull’icona Blocca</p> </td> 
   <td> <p>Attiva/disattiva da privato a società</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegna tag ad altri utenti negli aggiornamenti</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Consenti agli utenti esterni all'azienda di visualizzare un oggetto</p> </td> 
   <td> <p>Fai clic sull’icona Blocca</p> </td> 
   <td> <p>Disattiva l'opzione Da privato a società</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegna tag ad altri utenti negli aggiornamenti</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungere una risposta o un aggiornamento a un commento o a un aggiornamento</p> </td> 
   <td> <p>Fai clic sul pulsante Commento</p> </td> 
   <td> <p>Fare clic sul pulsante Rispondi o Aggiorna</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Aggiorna lavoro</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiorna stato attività</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aggiorna condizione per attività e problemi</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Aggiungere un aggiornamento a un documento</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Miglioramenti per dispositivi mobili {#mobile-improvements}

L’app mobile contiene i seguenti miglioramenti:

* I collegamenti condivisi con te in altre app mobili ora vengono aperti nell’app mobile di Workfront.

  Per ulteriori informazioni sulla condivisione di collegamenti, vedere .

  Questo aggiornamento verrà rilasciato ad iOS a volte questa settimana, e l’aggiornamento Android dovrebbe seguire poco dopo.

* Abbiamo aggiornato i requisiti di supporto per la piattaforma iOS per supportare iPhone X.

  Per ulteriori informazioni sui dispositivi mobili e i sistemi operativi supportati, consulta la .
