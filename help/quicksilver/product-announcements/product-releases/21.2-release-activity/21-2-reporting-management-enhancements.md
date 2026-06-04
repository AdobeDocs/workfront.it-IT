---
content-type: release-notes
keywords: note,trimestrale,aggiornamento,rilascio
navigation-topic: 2021-2-release-activity
title: ​21. 2 Miglioramenti per il reporting
description: Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 21.2 di Reporting. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
TQID: https://experienceleague.adobe.com/-fD0kFEB6ka8-DojDCkBnveHBncaLh3ppK0DIe9-vus
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 560
ht-degree: 1%

---

# &#x200B;21. 2 Miglioramenti per il reporting

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 21.2 di Reporting. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta la [panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Limita la modifica delle ore in progetti e report

Per fornire un maggiore controllo sulla modifica delle ore nella scheda Ore in un progetto e nei rapporti sulle ore, abbiamo aggiunto un’impostazione che consente agli amministratori di Workfront di limitare la modifica delle ore ai proprietari e agli amministratori di sistema.

In precedenza, gli utenti con le schede orario e le ore abilitate nel loro livello di accesso potevano modificare le ore.

Per ulteriori informazioni, consulta [Configurare le preferenze di orario e scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nuovo aspetto del campo Assegnazioni negli elenchi e nei report aggiornati

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per mantenere l’aspetto moderno delle altre aree della nuova esperienza Workfront, è stato modificato lo stile del campo Assegnazioni negli elenchi e nei rapporti aggiornati. Questa riprogettazione include:

* Un avatar arrotondato per le immagini del profilo utente, i ruoli e i team
* Visualizzazione delle iniziali per gli utenti senza immagini del profilo
* Icona di una nuova mansione
* Una nuova icona Persone per le assegnazioni avanzate
* Icona Un nuovo accesso con restrizioni
* Altre modifiche di progettazione minori

Per ulteriori informazioni sulle assegnazioni negli elenchi, consulta [Assegnare attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md) o [Assegnare problemi](../../../manage-work/issues/manage-issues/assign-issues.md).

![Aggiornamenti assegnazioni](assets/assignments-updates-350x193.png)

## Nuovo aspetto per i campi typeahead negli elenchi e nei report aggiornati

>[!NOTE]
>
>Temporaneamente rimosso dall’ambiente di produzione il 20 maggio 2021.

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per conferire un aspetto moderno alle altre aree della nuova esperienza Workfront, è stato modificato lo stile dei campi typeahead negli elenchi e nei report aggiornati. Queste modifiche includono:

* L’icona Typeahead è stata rimossa dal campo.
* Quando fai clic su un campo di completamento automatico, ora viene visualizzato il menu dei suggerimenti prima di immettere il testo.
* Il menu dei suggerimenti è più reattivo alla lunghezza dei valori, che ora vengono troncati alla fine quando viene raggiunto il limite di caratteri anziché al centro del valore.

Per informazioni sugli elenchi aggiornati, vedere la sezione [Differenza tra gli elenchi aggiornati e quelli legacy](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) nell&#39;articolo [Introduzione agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![Campo automatico](assets/typeahead-updates-350x336.png)

## Rapporto sugli aggiornamenti di sistema

Il nuovo rapporto Scrittura contabile offre una maggiore verificabilità consentendo di eseguire il drill-in agli aggiornamenti del sistema, tra cui:

* Modifiche di stato su un progetto, un’attività o un problema
* Attività o problemi eliminati
* Valori nei campi personalizzati
* Date di completamento pianificate
* Modifiche del proprietario del progetto

Ad esempio, puoi impostare questo rapporto in modo da mostrare l’attività intorno a un campo personalizzato specifico, incluso il progetto per il campo personalizzato, quando è stato immesso un valore, di che valore si trattava, quando il campo è stato aggiornato, qual era il valore precedente, qual era il nuovo valore immesso, quali utenti hanno completato queste azioni, ecc.

In precedenza, era possibile creare rapporti sugli aggiornamenti di sistema solo tramite l’API Workfront.

Per ulteriori informazioni su questo report e sui motivi per cui è possibile utilizzarlo, vedere [Report sull&#39;area Aggiornamenti con un report sulle voci diario](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

