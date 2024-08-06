---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Correggere il giorno di inizio della settimana lavorativa per le schede orario
description: Il giorno di inizio della settimana nella scheda orario non corrisponde al giorno di inizio della settimana configurato nel profilo della scheda orario.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Correggere il giorno di inizio della settimana lavorativa per le schede orario

## Problema

Il giorno di inizio della settimana nella scheda attività non corrisponde al giorno di inizio della settimana configurato nel mio profilo scheda attività (come descritto in [Creare, modificare e assegnare profili scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).)

## Soluzione

Il giorno di inizio della settimana di una scheda orario in Adobe Workfront utilizza le impostazioni della lingua e delle impostazioni internazionali nel browser per determinare il giorno della settimana. Per questo motivo, è necessario aggiornare le impostazioni della lingua e delle impostazioni internazionali del browser.

Ad esempio, con la lingua del browser impostata su Inglese e la lingua impostata su Stati Uniti, la settimana inizia di domenica. In alternativa, se la lingua del browser è impostata su Inglese e la lingua è impostata su Regno Unito, il giorno di inizio è Lunedì.

Questa impostazione ha effetto anche sul giorno di inizio della settimana nei calendari popup nel sistema.

La modifica delle impostazioni internazionali non ha effetto sul giorno di inizio della settimana nella griglia risorse o nella visualizzazione griglia risorse. La settimana inizia sempre la domenica.

Di seguito sono riportate le istruzioni per la modifica delle impostazioni della lingua e delle impostazioni internazionali per i vari browser supportati con Workfront.

* **Chrome:** Copia e incolla il seguente collegamento nel browser Chrome: `chrome://settings/languages`, quindi passa a Lingue.
* **Firefox:**copia e incolla il seguente collegamento nel browser Firefox: `about:preferences#content`, quindi passa a Lingue.
* **IE 11:** Strumenti -> Opzioni Internet -> Generale -> Lingue
* **Safari:** Sfortunatamente, Safari non consente la modifica delle lingue di esplorazione Web senza modificare anche l&#39;intera lingua del sistema operativo. Probabilmente è più facile semplicemente installare un altro browser come Chrome o Firefox.


