---
title: Miglioramenti alla creazione di rapporti per il terzo trimestre 2025
description: Miglioramenti dei progetti del terzo trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 5%

---

# Miglioramenti alla creazione di rapporti per il terzo trimestre 2025

Questa pagina descrive tutti i miglioramenti di reporting apportati con la versione del terzo trimestre 2025 all’ambiente Preview. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto nel ciclo di rilascio del terzo trimestre 2025, vedere [Panoramica sulle versioni del terzo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Sicurezza avanzata di recapito dei report

* Anteprima: 26 giugno 2025
* Produzione: rollout graduale dal 26 giugno 2025 al 9 luglio 2025

Abbiamo migliorato la consegna pianificata dei report per garantire che le notifiche Workfront vengano inviate solo ai domini e-mail approvati nell&#39;elenco Consentiti.

In precedenza, se la tua organizzazione avesse definito una limitazione su quali domini e-mail vengono inviate le notifiche Workfront, eseguiremmo una verifica rispetto all’elenco Consentiti durante l’aggiunta delle e-mail.

Ora eseguiamo anche un controllo durante l&#39;invio dell&#39;e-mail per assicurarci che l&#39;indirizzo e-mail inserito sia conforme all&#39;elenco di indirizzi consentiti. Questa verifica migliorata si applica sia agli indirizzi e-mail associati agli utenti che alle e-mail ad hoc aggiunte all’elenco dei destinatari del report.

Per ulteriori informazioni, vedere [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## I caratteri jolly utente non restituiscono più risultati con un valore null durante il filtraggio

>[!NOTE]
>
>* Anteprima: 30 aprile 2025
>* Rilascio rapido in produzione: venerdì 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È stato aggiornato il comportamento dei caratteri jolly dell’utente per escludere un valore null durante il filtraggio di un report. Questa modifica consente al filtro di produrre risultati più accurati, anziché restituire risultati per i quali un utente non è configurato correttamente (risultato nullo).

In precedenza, quando un carattere jolly dell&#39;utente generava un valore null, in un report venivano visualizzati tutti i record che avevano anche un valore null.

Questa modifica si applica ai seguenti filtri jolly:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
