---
content-type: release-notes
keywords: note, trimestrale, aggiornamento, versione
navigation-topic: 2021-2-release-activity
title: 21. 2 Miglioramenti al reporting
description: Questa pagina descrive tutti i miglioramenti apportati alla funzione di reporting nell’ambiente di anteprima con la versione 21.2. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2 Miglioramenti al reporting

Questa pagina descrive tutti i miglioramenti apportati alla funzione di reporting nell’ambiente di anteprima con la versione 21.2. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, vedi [Panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Limitare la modifica delle ore nei progetti e nei rapporti

Per fornire un maggiore controllo sulla modifica delle ore nella scheda Ore di un progetto e dei rapporti sulle ore, è stata aggiunta un’impostazione che consente agli amministratori di Workfront di limitare la modifica delle ore ai proprietari delle ore e agli amministratori di sistema.

In precedenza, gli utenti con fogli presenze e ore abilitate nel livello di accesso potevano modificare le ore.

Per ulteriori informazioni, consulta [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nuovo aspetto del campo Assegnazioni in elenchi e rapporti aggiornati

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per ottenere l’aspetto moderno di altre aree della nuova esperienza Workfront, lo stile del campo Assegnazioni è stato modificato in elenchi e rapporti aggiornati. Questa riprogettazione include:

* Avatar arrotondato per immagini di profilo utente, ruoli di lavoro e team
* Visualizzazione delle iniziali per gli utenti senza immagini del profilo
* Icona del nuovo ruolo
* Una nuova icona Persone per le assegnazioni avanzate
* Una nuova icona Accesso limitato
* Altre modifiche di progettazione minori

Per ulteriori informazioni sulle assegnazioni negli elenchi, vedere [Assegnare le attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md) o [Assegnare i problemi](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nuovo aspetto dei campi typeahead in elenchi e rapporti aggiornati

>[!NOTE]
>
>È stata temporaneamente rimossa dall’ambiente di produzione il 20 maggio 2021.

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per ottenere l’aspetto moderno di altre aree della nuova esperienza Workfront, lo stile dei campi typeahead in elenchi e rapporti aggiornati è stato modificato. Queste modifiche includono:

* L’icona Typeahead è stata rimossa dal campo .
* Quando si fa clic su un campo typeahead, viene visualizzato il menu suggerimenti prima di immettere il testo.
* Il menu dei suggerimenti è più reattivo alla lunghezza dei valori e questi valori vengono ora troncati alla fine quando il limite dei caratteri viene soddisfatto invece che al centro del valore.

Per informazioni sugli elenchi aggiornati, consulta la sezione [Differenza tra gli elenchi aggiornati e quelli legacy](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) sezione dell&#39;articolo [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Rapporto sugli aggiornamenti di sistema

Il nuovo rapporto Scrittura contabile consente una maggiore verificabilità consentendo di eseguire un drill-through degli aggiornamenti di sistema, tra cui:

* Lo stato cambia in un progetto, un&#39;attività o un problema
* Attività o problemi eliminati
* Valori nei campi personalizzati
* Date di completamento pianificate
* Modifiche al proprietario del progetto

Ad esempio, puoi impostare questo rapporto per mostrare l’attività intorno a un campo personalizzato specifico, incluso il progetto per il campo personalizzato, quando è stato immesso un valore, quale era tale valore, quando il campo è stato aggiornato, quale era il valore precedente, quale era il nuovo valore immesso, quali utenti hanno completato queste azioni, ecc.

In precedenza era possibile creare rapporti sugli aggiornamenti di sistema solo tramite l’API Workfront.

Per ulteriori informazioni su questo rapporto e su cosa può essere utilizzato, consulta [Rapporto sull’area Aggiornamenti](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

