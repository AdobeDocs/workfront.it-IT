---
title: Miglioramenti al reporting per il terzo trimestre 2025
description: Miglioramenti al progetto del terzo trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/XN5rfSeje0azVxpC4uBSDn5mg2C9Oyik2awD5pQy3Jo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 4%

---

# Miglioramenti al reporting per il terzo trimestre 2025

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2025. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2025, consulta [Panoramica sulla versione del terzo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Sicurezza migliorata della consegna dei rapporti

* Anteprima: 26 giugno 2025
* Produzione: rollout graduale dal 26 giugno 2025 al 9 luglio 2025

Abbiamo migliorato la consegna dei rapporti pianificata per garantire che le notifiche Workfront vengano inviate solo ai domini e-mail approvati nel inserisco nell&#39;elenco Consentiti di.

In precedenza, se la tua organizzazione avesse definito un limite su quali domini e-mail vengono inviate le notifiche Workfront, effettueremmo un controllo in base al inserisco nell&#39;elenco Consentiti di aggiunta delle e-mail al momento dell’aggiunta delle e-mail all’e-mail.

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
