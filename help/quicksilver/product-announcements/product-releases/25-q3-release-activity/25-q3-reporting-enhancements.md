---
title: Miglioramenti al reporting per il terzo trimestre 2025
description: Miglioramenti al progetto del terzo trimestre 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Miglioramenti al reporting per il terzo trimestre 2025

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2025. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2025, consulta [Panoramica sulla versione del terzo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Sicurezza migliorata della consegna dei rapporti

* Anteprima: 26 giugno 2025
* Produzione: rollout graduale dal 26 giugno 2025 al 9 luglio 2025

Abbiamo migliorato la consegna dei rapporti pianificata per garantire che le notifiche Workfront vengano inviate solo ai domini e-mail approvati nel inserisco nell&#39;elenco Consentiti di.

Precedentemente, se la tua organizzazione avesse definito un limite sui domini e-mail per le notifiche Workfront, effettueremmo un controllo in base al inserisco nell&#39;elenco Consentiti di aggiunta delle e-mail durante la procedura di e-mail.

Ora viene eseguito anche un controllo durante l’invio dell’e-mail per verificare che l’indirizzo e-mail inserito sia conforme al inserisco nell&#39;elenco Consentiti di e-mail di. Questo controllo migliorato si applica sia agli indirizzi e-mail associati agli utenti che alle e-mail ad hoc aggiunte all’elenco dei destinatari del rapporto.

Per ulteriori informazioni, consulta [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


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
