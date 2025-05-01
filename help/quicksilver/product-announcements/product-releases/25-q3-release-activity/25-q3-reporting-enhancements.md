---
title: Miglioramenti al reporting per il terzo trimestre 2025
description: Miglioramenti al progetto del terzo trimestre 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Miglioramenti al reporting per il terzo trimestre 2025

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2025. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2025, consulta [Panoramica sulla versione del terzo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## I caratteri jolly utente non restituiscono più risultati con un valore null durante il filtraggio

>[!NOTE]
>
>* Anteprima: 30 aprile 2025
>* Versione rapida di produzione: 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

Il comportamento dei caratteri jolly utente è stato aggiornato per escludere il valore null durante il filtraggio di un report. Questa modifica consente al filtro di produrre risultati più precisi, anziché restituire risultati che non hanno un utente configurato correttamente (un risultato nullo).

In precedenza, quando un carattere jolly utente generava un valore null, un report visualizzava tutti i record che avevano anche un valore null.

Questa modifica si applica ai seguenti filtri jolly:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

