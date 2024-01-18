---
title: 22.1 Miglioramenti al progetto
description: 22.1 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# 22.1 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 22.1 di Project. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, consulta [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Modifica dell&#39;opzione predefinita per i predecessori durante la copia o lo spostamento delle attività

Per ridurre al minimo il numero di passaggi manuali durante la copia o lo spostamento delle attività, sono state aggiornate le informazioni copiate o spostate con l&#39;attività per impostazione predefinita. Ora, tutti i predecessori vengono copiati o spostati con l&#39;attività per impostazione predefinita, in quanto l&#39;opzione Tutti i predecessori è selezionata per impostazione predefinita.

Prima di questo miglioramento, l’opzione Tutti i predecessori era deselezionata per impostazione predefinita durante la copia o lo spostamento di un’attività.

Per ulteriori informazioni, consulta gli articoli:

* [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## È stata aggiornata la barra degli strumenti nell’elenco delle dashboard e nei report nelle dashboard

La barra degli strumenti su quattro pagine del dashboard ora ha un aspetto moderno che corrisponde ad altri elenchi di Workfront come progetti, attività e problemi. Questa barra degli strumenti intuitiva semplifica l’aggiunta, la modifica, la condivisione, la copia e l’eliminazione delle dashboard.

Le pagine con la barra degli strumenti aggiornata sono:

* Rapporti sulle attività (visualizzati nei dashboard)
* Elenco di tutti i dashboard
* Elenco Dashboard personali
* Elenco dashboard condivisi

Per ulteriori informazioni, consulta [Creare e gestire le dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Aggiungi e modifica moduli personalizzati Pannello di riepilogo per i documenti

È ora possibile aggiungere e modificare moduli personalizzati direttamente nel pannello Riepilogo del documento.

Con questa modifica, nel Riepilogo del documento verrà inoltre visualizzato un nuovo aspetto. È disponibile una nuova sezione Panoramica, che contiene la miniatura dell’immagine e i dettagli del documento. È inoltre possibile archiviare ed estrarre i documenti nella sezione dei dettagli dei documenti.

In precedenza, per apportare modifiche o aggiungere moduli personalizzati era necessario passare alla scheda Moduli personalizzati in Dettagli documento.

Per ulteriori informazioni, consulta [Panoramica del riepilogo dei documenti](../../../documents/managing-documents/summary-for-documents.md).

## Nuova esperienza durante la copia di una o più attività

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Adobe Workfront, abbiamo riprogettato l’interfaccia durante la copia di un’attività. Questa opzione è attualmente disponibile quando si copia un&#39;attività a livello di attività o si copia una o più attività in un elenco.

Alcuni dei miglioramenti includono:

* Tutte le informazioni da aggiornare prima di copiare l&#39;attività vengono visualizzate in una pagina continua.
* Workfront controlla se hai accesso al progetto di destinazione subito dopo aver scelto il progetto. Prima di questo miglioramento, veniva visualizzato un messaggio di avviso che indicava che non disponevi dell’accesso corretto dopo la conferma della copia, causando passaggi aggiuntivi e la mancata autorizzazione della copia.
* Possibilità di richiedere l&#39;accesso per un progetto in cui si desidera copiare l&#39;attività senza uscire dalla casella Copia attività.

Per ulteriori informazioni, consulta [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nuova esperienza durante lo spostamento di una o più attività da un elenco

Per offrire un’esperienza coerente quando si esegue la stessa attività, ora è stata aggiornata l’interfaccia per spostare una o più attività da un elenco in modo che corrisponda all’esperienza quando si sposta l’attività a livello di attività. L’esperienza per lo spostamento di un’attività a livello di attività era stata aggiornata in una versione precedente di anteprima.

Per ulteriori informazioni, consulta [Sposta le attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nuova esperienza durante lo spostamento di un’attività a livello di attività

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per lo spostamento di un’attività. Questa funzione è attualmente disponibile quando si sposta un’attività a livello di attività. In una versione successiva, questa riprogettazione verrà estesa allo spostamento di un’attività da un elenco.

Alcuni dei miglioramenti apportati a questa nuova interfaccia includono:

* Tutte le informazioni da aggiornare prima che lo spostamento venga visualizzato in una pagina continua.
* Dopo aver scelto il progetto, Workfront verifica se hai accesso al progetto di destinazione. Prima di questo miglioramento, Workfront ti aveva avvisato che non disponi dell’accesso corretto dopo aver confermato lo spostamento, che ha comportato passaggi aggiuntivi e che lo spostamento non era consentito.
* Possibilità di richiedere l&#39;accesso per un progetto in cui si desidera spostare l&#39;attività senza uscire dalla casella Sposta attività.

Per ulteriori informazioni, consulta [Sposta le attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nuova esperienza durante la conversione di un problema in un progetto utilizzando un modello a livello di problema

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente rilasciato in un rollout graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Ora è disponibile in Anteprima e Produzione per tutti i clienti. (Per gli ultimi aggiornamenti sullo stato del rilascio di questa funzione in produzione, consulta [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Workfront, è stata riprogettata l’interfaccia per convertire un problema in un progetto quando si utilizza un modello convertito dalla pagina del problema.

Ora è possibile accedere più facilmente all’elenco dei preferiti subito dopo aver selezionato per convertire il problema.

L’interfaccia riprogettata corrisponde all’esperienza acquisita durante la creazione di un progetto a partire da un modello, anch’esso aggiornato di recente.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convertire i problemi in progetti utilizzando un modello da elenchi, report e dashboard

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente rilasciato in un rollout graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Ora è disponibile in Anteprima e Produzione per tutti i clienti. (Per gli ultimi aggiornamenti sullo stato del rilascio di questa funzione in produzione, consulta [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Per aumentare l’efficienza del lavoro e facilitare la conversione dei problemi in un ambiente in rapida evoluzione, è stata aggiunta la possibilità di convertire un problema in un progetto utilizzando un modello da un elenco, un report o un dashboard.

Prima di questo miglioramento, questa funzionalità esisteva solo quando il problema veniva convertito dalla pagina del problema.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## L’elenco Filtra per utente nelle bacheche Agile mostra gli utenti con la maggior parte delle assegnazioni

>[!NOTE]
>
>Questa funzione non sarà inclusa nella versione 22.1. È stato rimosso dall’ambiente di anteprima.

Ora il filtro mostra prima gli utenti con il maggior numero di assegnazioni, in modo che siano più facili da individuare senza scorrere l’elenco.

In precedenza, l’elenco dei filtri per utente nelle bacheche Kanban e Scrum veniva visualizzato in ordine alfabetico.

Per ulteriori informazioni, vedere le informazioni seguenti

* [Filtra per utente sulla bacheca Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtra per utente sulla bacheca Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limitare la possibilità di aggiungere documenti a un modello condiviso

A volte gli utenti aggiungono documenti a un modello di progetto pensando di aggiungerli a un progetto. È ora possibile evitare che ciò si verifichi, poiché quando si condivide un modello con accesso in visualizzazione, è possibile disattivare la nuova impostazione avanzata Aggiungi documenti. Questo disabilita la possibilità dei destinatari di aggiungere documenti al modello.

Per istruzioni sulla condivisione di un modello, consulta [Condividere modelli di progetto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Per informazioni sulla nuova impostazione avanzata Aggiungi documenti, vedi la sezione nell’articolo [Condivisione di un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Condividere una cartella documenti

È ora possibile condividere una cartella documenti e il relativo contenuto dall&#39;area Documenti. In precedenza non era possibile: era necessario condividere ogni documento in una cartella separatamente.

Per ulteriori informazioni, consulta [Condividere una cartella documenti](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

