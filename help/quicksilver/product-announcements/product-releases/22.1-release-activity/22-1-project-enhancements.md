---
title: Miglioramenti al progetto 22.1
description: Miglioramenti al progetto 22.1
author: Luke
draft: Probably
feature: Product Announcements
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# Miglioramenti al progetto 22.1

Questa pagina descrive tutti i miglioramenti apportati a Project con la versione 22.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, vedi [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Modificare l&#39;opzione predefinita per i predecessori durante la copia o lo spostamento delle attività

Per ridurre al minimo il numero di passaggi manuali durante la copia o lo spostamento delle attività, sono state aggiornate le informazioni che vengono copiate o spostate con l&#39;attività per impostazione predefinita. Ora, tutti i predecessori vengono copiati o spostati con l&#39;attività per impostazione predefinita, in quanto l&#39;opzione Tutti i predecessori è selezionata per impostazione predefinita.

Prima di questo miglioramento, l&#39;opzione Tutti i predecessori era deselezionata per impostazione predefinita durante la copia o lo spostamento di un&#39;attività.

Per ulteriori informazioni, consulta gli articoli:

* [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Barra degli strumenti aggiornata nell’elenco del dashboard e nei rapporti nelle dashboard

La barra degli strumenti su quattro pagine del dashboard ora presenta un aspetto moderno che corrisponde ad altri elenchi di Workfront, ad esempio progetti, attività e problemi. Questa barra degli strumenti intuitiva semplifica l’aggiunta, la modifica, la condivisione, la copia e l’eliminazione delle dashboard.

Le pagine con la barra degli strumenti aggiornata sono le seguenti:

* Rapporti attività (visualizzati nelle dashboard)
* Elenco Tutte le dashboard
* Elenco delle mie dashboard
* Elenco delle dashboard condivise

Per ulteriori informazioni, consulta [Creazione e gestione di dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Aggiunta e modifica del pannello Riepilogo moduli personalizzati per i documenti

È ora possibile aggiungere e modificare moduli personalizzati direttamente nel pannello Riepilogo del documento.

Con questa modifica verrà visualizzato anche un nuovo aspetto nel riepilogo del documento. È disponibile una nuova sezione Panoramica , che contiene la miniatura dell’immagine e i dettagli del documento. È inoltre possibile archiviare o estrarre i documenti nella sezione dei dettagli del documento.

In precedenza era necessario passare alla scheda Moduli personalizzati in Dettagli documento per apportare modifiche o aggiungere moduli personalizzati.

Per ulteriori informazioni, consulta [Panoramica del riepilogo dei documenti](../../../documents/managing-documents/summary-for-documents.md).

## Nuova esperienza durante la copia di una o più attività

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Adobe Workfront, durante la copia di un’attività è stata riprogettata l’interfaccia . Questa opzione è attualmente disponibile quando si copia un&#39;attività a livello di attività o si copia una o più attività in un elenco.

Alcuni dei miglioramenti includono:

* Tutte le informazioni che è necessario aggiornare prima di copiare l’attività vengono visualizzate su una pagina continua.
* Workfront controlla se puoi accedere al progetto di destinazione subito dopo aver scelto il progetto. Prima di questo miglioramento, veniva visualizzato un messaggio di avviso che indica che non disponi dell’accesso corretto dopo la conferma della copia, che comportava passaggi aggiuntivi e che la copia non era consentita.
* Possibilità di richiedere l&#39;accesso per un progetto in cui si desidera copiare l&#39;attività senza uscire dalla casella Copia attività.

Per ulteriori informazioni, consulta [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nuova esperienza durante lo spostamento di una o più attività da un elenco

Per offrire un’esperienza coerente durante l’esecuzione della stessa attività, è stata aggiornata l’interfaccia per lo spostamento di una o più attività da un elenco in modo che corrispondano all’esperienza durante lo spostamento dell’attività a livello di attività. (Avevamo aggiornato l’esperienza per spostare un’attività a livello di attività in una versione precedente di Preview).

Per ulteriori informazioni, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nuova esperienza durante lo spostamento di un&#39;attività a livello di attività

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per lo spostamento di un’attività. Questa opzione è attualmente disponibile quando si sposta un&#39;attività a livello di attività. In una versione successiva, questa nuova progettazione verrà estesa allo spostamento di un’attività da un elenco.

Alcuni dei miglioramenti di questa nuova interfaccia riprogettata includono:

* Tutte le informazioni da aggiornare prima dello spostamento vengono visualizzate su una pagina continua.
* Workfront verificherà se hai accesso al progetto di destinazione immediatamente dopo aver scelto il progetto. Prima di questo miglioramento, Workfront ti ha avvisato che non disponi dell’accesso corretto dopo aver confermato lo spostamento, il che causava passaggi aggiuntivi e lo spostamento non era consentito.
* Possibilità di richiedere l&#39;accesso per un progetto in cui si desidera spostare l&#39;attività senza uscire dalla casella Sposta attività.

Per ulteriori informazioni, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nuova esperienza durante la conversione di un problema in un progetto utilizzando un modello a livello di problema

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente pubblicato in un roll-out graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Questa funzione è ora disponibile in Anteprima e Produzione per tutti i clienti. (Per gli ultimi aggiornamenti sullo stato di questa funzione rilasciata in Produzione, consulta [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per la conversione di un problema in un progetto quando si utilizza un modello quando lo si converte dalla pagina del problema.

Ora puoi accedere più facilmente all’elenco dei preferiti immediatamente dopo aver selezionato per convertire il problema.

L’interfaccia riprogettata corrisponde all’esperienza acquisita durante la creazione di un progetto da un modello, anch’esso aggiornato di recente.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convertire i problemi in progetti utilizzando un modello da elenchi, rapporti e dashboard

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 4 marzo 2022. È stato successivamente pubblicato in un roll-out graduale a partire dal 28 aprile 2022. L’implementazione è stata completata il 5 maggio 2022. Questa funzione è ora disponibile in Anteprima e Produzione per tutti i clienti. (Per gli ultimi aggiornamenti sullo stato di questa funzione rilasciata in Produzione, consulta [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Per aumentare l’efficienza del lavoro e semplificare la conversione dei problemi in un ambiente ad alta velocità, abbiamo aggiunto la possibilità di convertire un problema in un progetto utilizzando un modello da un elenco, un rapporto o un dashboard.

Prima di questo miglioramento, questa funzionalità esisteva solo quando il problema era stato convertito dalla pagina del problema.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Filtra per elenco di utenti nelle bacheche mobili mostra gli utenti con la maggior parte delle assegnazioni per primi

>[!NOTE]
>
>Questa funzione non sarà inclusa nella versione 22.1. È stato rimosso dall’ambiente di anteprima.

Ora il filtro mostra gli utenti con il maggior numero di assegnazioni, in modo che siano più facili da individuare senza scorrere l&#39;elenco.

Precedentemente, il filtro per elenco di utenti nelle bacheche Kanban e Scrum veniva visualizzato in ordine alfabetico.

Per ulteriori informazioni, consulta le seguenti informazioni

* [Filtrare per utente sulla scheda Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrare per utente sulla scheda Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limitare la possibilità di aggiungere documenti a un modello condiviso

A volte le persone aggiungono documenti a un modello di progetto pensando di aggiungerli a un progetto. Ora è possibile evitare questa situazione: quando condividi un modello con accesso Visualizza, puoi disattivare la nuova impostazione avanzata Aggiungi documenti. Questo disabilita la possibilità dei destinatari di aggiungere documenti al modello.

Per istruzioni sulla condivisione di un modello, vedi [Condividere i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Per informazioni sulla nuova impostazione avanzata Aggiungi documenti, consulta la sezione nell’articolo [Condivisione di un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Condivisione di una cartella di documenti

Ora è possibile condividere una cartella di documenti e il relativo contenuto dall&#39;area Documenti. In precedenza non era possibile: era necessario condividere separatamente ogni documento in una cartella.

Per ulteriori informazioni, consulta [Condivisione di una cartella di documenti](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

