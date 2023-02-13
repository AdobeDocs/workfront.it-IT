---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Correggere il giorno di inizio della settimana lavorativa per i fogli presenze
description: Il giorno di inizio della settimana nella scheda attività non corrisponde al giorno di inizio della settimana configurato nel profilo della scheda attività.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Correggere il giorno di inizio della settimana lavorativa per i fogli presenze

## Problema

Il giorno di inizio della settimana nella scheda attività non corrisponde al giorno di inizio della settimana configurato nel profilo della scheda attività (come descritto in [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Soluzione

Il giorno iniziale della settimana di una scheda attività in Adobe Workfront utilizza le impostazioni della lingua e delle impostazioni internazionali nel browser per determinare il giorno della settimana. Per questo motivo, è necessario aggiornare le impostazioni della lingua e delle impostazioni internazionali del browser. 

Ad esempio, con la lingua del browser impostata su Inglese e le impostazioni internazionali impostate su Stati Uniti, la settimana inizia la domenica. In alternativa, il giorno di inizio è lunedì se la lingua del browser è impostata su Inglese e le impostazioni internazionali sono impostate su Regno Unito.

Questa impostazione influisce anche sul giorno iniziale della settimana nei calendari pop-up in tutto il sistema.

La modifica delle impostazioni internazionali non influisce sul giorno iniziale della settimana sulla griglia delle risorse (o sulla vista griglia delle risorse). La settimana inizia sempre di domenica.

Di seguito sono riportate le istruzioni per modificare le impostazioni della lingua e delle impostazioni internazionali per vari browser supportati con Workfront.

* **Chrome:** Copia e incolla il seguente collegamento nel browser Chrome: `chrome://settings/languages` poi vai a Lingue.
* **Firefox:**copia e incolla il seguente collegamento nel browser Firefox: `about:preferences#content` poi vai a Lingue.
* **IE 11:** Strumenti -> Opzioni Internet -> Generale -> Lingue
* **Safari:** Sfortunatamente, Safari non consente di modificare le lingue di navigazione web senza modificare anche l&#39;intera lingua del sistema operativo. Probabilmente è più semplice installare un altro browser come Chrome o Firefox.

 
