---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Miglioramenti al progetto 2019.2
description: Questa pagina descrive tutti i miglioramenti al progetto inclusi nella versione 2019.2. La funzionalità sarà disponibile nell’ambiente di produzione la settimana del 20 maggio 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# Miglioramenti al progetto 2019.2

Questa pagina descrive tutti i miglioramenti al progetto inclusi nella versione 2019.2. La funzionalità sarà disponibile nell’ambiente di produzione la settimana del 20 maggio 2019.

Per un elenco di tutte le modifiche apportate in 2019.2, consulta [Panoramica delle attività sulla versione 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Ricerca Più Rapida Dei Gruppi Durante La Personalizzazione Degli Stati

Il menu a discesa nella scheda Stati nell’area Configurazione è ora un menu typeahead. Questo consente di cercare e trovare rapidamente qualsiasi gruppo nel sistema, semplificando la personalizzazione degli stati.

In precedenza, il menu a discesa mostrava un numero limitato di gruppi. Se il gruppo desiderato non è visualizzato, è necessario passare a Configurazione > Gruppi e trovare il gruppo specifico per personalizzare gli stati del gruppo.

Per ulteriori informazioni, vedere [Creare o modificare uno stato](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Allega alle attività i processi di approvazione e Forms personalizzati predefiniti

È ora possibile configurare moduli personalizzati predefiniti e processi di approvazione da allegare alle attività quando si aggiungono attività a un progetto. Puoi configurare le impostazioni predefinite a livello di progetto.

Per informazioni sulla configurazione di moduli personalizzati predefiniti e sui processi di approvazione per le attività a livello di progetto, vedi la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Visualizzare l&#39;intera riga di un task padre in grassetto in un elenco di task

In un elenco di attività, la riga contenente un&#39;attività padre viene visualizzata in grassetto. Questa modifica è visibile quando l’elenco è ordinato in base alla struttura Work Breakdown (Raggruppamento del lavoro) o al numero di attività in ordine crescente.

## Inverti modifiche negli elenchi di task

Un nuovo pulsante di salvataggio automatico nell&#39;elenco dei task consente di scegliere se salvare automaticamente le modifiche apportate o se visualizzare gli effetti delle modifiche prima di salvarle. Questa impostazione si applica sia all&#39;elenco delle attività che al diagramma di Gantt.

Prima di questo miglioramento, tutte le modifiche venivano sempre salvate automaticamente.

Per informazioni sulla modifica delle attività in un elenco attività, vedere [Modifica attività](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Per informazioni sulla modifica delle attività nel diagramma di Gantt, vedere [Aggiornare le informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nuovi valori predefiniti per la larghezza di colonna nei nuovi elenchi

Ora Workfront regola automaticamente la larghezza delle colonne in base alle informazioni sul formato del valore in ogni colonna. Ad esempio, le colonne che visualizzano un numero sono più larghe di quelle che visualizzano il campo Descrizione.

Prima di questo miglioramento, la larghezza delle colonne nelle nuove viste progetto e attività era impostata su 100 pixel, salvo diversa indicazione.

Per informazioni sulla larghezza delle colonne, vedere [Modificare la larghezza e l&#39;ordine delle colonne](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Disattiva oggetti inutilizzati

>[!NOTE]
>
>Questa funzione è stata rilasciata direttamente nell’ambiente di produzione durante il periodo di anteprima 2019.2.

Se sono presenti oggetti non più utilizzati, è ora possibile disattivarli per nasconderli dagli elenchi per impedire agli utenti di associarli ad altri oggetti.

Ora, quando si modifica uno qualsiasi degli oggetti riportati di seguito, è possibile indicare se devono essere attivi. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti. Gli oggetti non impostati su Attivo non sono visibili nei menu a discesa e nei campi di completamento automatico da associare ad altri oggetti.

* Processi di approvazione
* Aziende
* Moduli personalizzati
* Percorsi milestone
* Portfolio
* Programmi
* Modelli

Tutto ciò che disattivi e attualmente in uso continua a funzionare come sempre, e non viene rimosso o bloccato.

>[!IMPORTANT]
>
>Quando si creano questi oggetti tramite l’API di Workfront, il valore predefinito per il parametro &quot;isActive&quot; è true. Questo è un nuovo campo per tutti gli oggetti e non è disponibile per la modifica prima della versione 11 dell’API. Questo campo esisteva già per Portfolio, tranne per il fatto che il valore predefinito era falso; passerà al valore predefinito true a partire dalla versione 11 dell’API.

## Visualizza il costo preventivato del lavoro programmato (BCWS) e eseguito (BCWP) nelle visualizzazioni

È ora possibile visualizzare il Costo preventivato del lavoro programmato (BCWS) e il Costo preventivato del lavoro eseguito (BCWP) nelle visualizzazioni dei progetti e delle attività.

Anche se queste metriche delle prestazioni del progetto sono state utilizzate in precedenza nei calcoli finanziari in Workfront, non erano visibili nel sistema prima di questo miglioramento.

Per informazioni sul calcolo di BCWS, vedere [Calcolare il costo preventivato del lavoro programmato (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Per informazioni sul calcolo del valore BCWP, vedere [Calcolare il costo preventivato del lavoro eseguito (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

