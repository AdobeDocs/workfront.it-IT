---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Correggere il giorno di inizio della settimana lavorativa per le schede orario
description: Il giorno di inizio della settimana nella scheda orario non corrisponde al giorno di inizio settimanale previsto.
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Correggere il giorno di inizio della settimana lavorativa per le schede orario

<!--Audited: 5/2025-->

## Problema

Il giorno di inizio della settimana nella scheda orario non corrisponde al giorno di inizio settimanale previsto.

Ciò si verifica in genere quando non si è assegnati a un profilo Scheda orario e la scheda orario è stata creata manualmente.


## Soluzione

L&#39;amministratore di Workfront deve creare profili di schede orario e assegnare tutti a un profilo, come descritto in [Creare, modificare e assegnare profili di schede orario](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). L’amministratore di Workfront potrebbe definire la data di inizio di una scheda orario in un giorno diverso dalla data di inizio settimanale prevista. Rivolgiti a loro per scoprire la data di inizio di un profilo Scheda orario per la tua scheda orario.

Se la scheda orario è stata creata manualmente, il giorno di inizio della settimana nella scheda orario utilizza le impostazioni di Impostazioni internazionali e-mail nel profilo dell&#39;utente, come descritto nell&#39;articolo [Configura impostazioni personali](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Ad esempio, con Email Locale impostato su Inglese (Stati Uniti), la settimana nella scheda orario inizia di domenica. In alternativa, con Email Locale impostato su Inglese (Regno Unito), la settimana nella scheda orario inizia di lunedì.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


