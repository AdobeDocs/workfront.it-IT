---
content-type: reference
navigation-topic: get-started-with-workfront
title: Lingue supportate in Adobe Workfront
description: Puoi modificare la lingua in cui vengono visualizzati Adobe Workfront e le e-mail provenienti da Workfront, regolando le preferenze di lingua sul browser e le impostazioni e-mail predefinite in Workfront.
feature: Get Started with Workfront
author: Becky
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: eb5296348c27f806dd50b997970166ebae4c97f4
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 97%

---

# Lingue supportate in Adobe Workfront

Puoi modificare la lingua in cui vengono visualizzati Adobe Workfront e le e-mail provenienti da Workfront, regolando le preferenze di lingua sul browser (se l’organizzazione non ha effettuato la migrazione ad Adobe Admin Console) o le preferenze di lingua del profilo Adobe Experience Cloud (se su Adobe Admin Console) e le impostazioni locali e-mail predefinite in Workfront.

Per modificare la lingua in cui visualizzi Workfront, consulta [Modificare la lingua](#change-the-language) in questo articolo.

La terminologia di Workfront viene aggiornata per le lingue supportate a ogni aggiornamento di Workfront.

Workfront supporta le seguenti lingue:

* Inglese (en-US)
* Francese (fr-FR)
* Tedesco (de-DE)
* Giapponese (ja-JP)
* Spagnolo (es-ES)
* Italiano (it-IT)
* Portoghese (pt-BR)
* Coreano (ko-KR)
* Cinese - semplificato (zh-CN)
* Cinese - Tradizionale (zh-TW)

La lingua utilizzata per visualizzare Workfront nel browser è controllata dalle impostazioni della lingua del browser, se l’organizzazione non è nel Adobe Admin Console, o dalla lingua del profilo Adobe Experience Cloud, se l’organizzazione è in Adobe Admin Console. In entrambi i casi, assicurati di selezionare una lingua elencata nell’elenco di lingue supportate.

Per visualizzare le e-mail in uscita in una delle lingue supportate, modifica le impostazioni locali e-mail utente o le informazioni cliente in Workfront.\
Per modificare le impostazioni di Informazioni cliente devi essere un amministratore di Workfront.\
Per ulteriori informazioni sulla modifica delle informazioni cliente e delle impostazioni locali e-mail utente, consulta [Modificare le impostazioni locali e-mail utente e Workfront](#change-the-workfront-and-user-locales).

Puoi affidare a terzi la traduzione in altre lingue dell’interfaccia di Workfront e delle e-mail in uscita da Workfront. Queste traduzioni non sono supportate da Workfront come anche qualsiasi lingua al di fuori di quelle elencate sopra.

>[!NOTE]
>
>Parti dell’interfaccia potrebbero non essere ancora tradotte per quanto segue:
>
>* Quando si utilizza una lingua non supportata, l’interfaccia viene visualizzata in inglese
>* Il menu Aiuto e il contenuto della guida accessibile da tale menu vengono visualizzati in inglese
>* Il testo inserito dall’utente rimane nella lingua originale. Può includere, tra l’altro:
>
>   * Nomi progetti
>   * Nomi attività
>   * Nomi problemi
>   * Nomi portfolio
>   * Nomi programmi
>   * Nomi approvazione
>   * Descrizioni
>   * Campi modulo personalizzati
>   * Nomi tipi di ora
>   * Tipi di spesa
>   * Le Milestone
>   * Schede personalizzate
>   * Stati
>   * Nomi dei rapporti
>

## Differenze di lingua supportate durante l’uso di bozze

Il Visualizzatore di bozze web di Workfront supporta la maggior parte delle lingue supportate in Workfront.

Le lingue seguenti non sono supportate nello strumento bozza:

* Cinese - Tradizionale (zh-TW)
* Coreano (ko-KR)

Per accedere al Visualizzatore di bozze Web, l’azienda deve acquistarne una licenza.

Per ulteriori informazioni sulla bozza, consulta [Bozza](../review-and-approve-work/proofing/proofing.md).

Quando visualizzi Workfront in una lingua non supportata nello strumento di bozza, il visualizzatore di bozze web viene mostrato in inglese.

Se utilizzi Workfront Proof (strumento di bozze autonomo) in una lingua non supportata in Workfront, il visualizzatore di bozze web in Workfront viene mostrato in inglese.\
Per ulteriori informazioni sulle lingue supportate in Workfront Proof, consulta [Impostazioni lingua in Workfront Proof](../workfront-proof/wp-getstarted/system-information/language-settings.md).

## Lingua supportata in Adobe Workfront Fusion

Attualmente, Workfront Fusion supporta solo l’inglese.

* Tutti i contenuti in Workfront Fusion ed eventuali guide relative a Workfront Fusion vengono visualizzati in inglese.
* Workfront Fusion non supporta l’utilizzo di caratteri di testo non inglesi nei campi inseriti dall’utente.

Per poter accedere a Workfront Fusion, l’azienda deve acquistare la relativa licenza.\
Per ulteriori informazioni su Workfront Fusion, consulta [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

## Modificare la lingua

Puoi modificare la lingua in cui visualizzi Workfront e quella delle e-mail in uscita modificando le seguenti impostazioni:

<!--* DELETE THIS SECTION MARCH 2026 The language on your browser (for users not on the Adobe Admin Console)-->
* La lingua principale e secondaria del profilo AEM (per gli utenti su Adobe Admin Console)
* Le impostazioni locali e-mail utente e le Informazioni cliente nel tuo account Workfront.

Per visualizzare tutte le traduzioni disponibili per la lingua scelta, le impostazioni locali di Workfront e del browser dovrebbero essere sulla stessa lingua.

Per determinare se la tua organizzazione ha effettuato la migrazione ad Adobe Admin Console, esamina l’URL utilizzato per visualizzare Workfront.

| URL | Adobe Experience | Controllo lingua |
|---|---|---|
| (CompanyName).my.workfront.com | Migrazione non effettuata ad Adobe Admin Console | [Modificare la lingua del browser](#change-the-browser-language) |
| experience.adobe.com | Migrazione effettuata ad Adobe Admin Console | [Modificare la lingua di Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) |

* [Modificare la lingua del browser](#change-the-browser-language)
* [Modificare la lingua di Adobe Experience Cloud](#change-the-adobe-experience-cloud-language)
* [Modificare le impostazioni locali e-mail utente e Workfront](#change-the-workfront-and-user-locales)

<!--DELETE THIS SECTION MARCH 2026-->

<!--

### Change the browser language {#change-the-browser-language}

If your organization has not been migrated to the Adobe Admin Console, when you change the browser language, your Workfront interface displays in that language.   
For more information about what languages are supported by Workfront, see [Supported languages in Adobe Workfront](#supported-languages).

The browser language must be changed on an individual user basis.

See the "Help" menu for your browser for specific information about how to change the language of your browser.-->

### Modificare la lingua di Adobe Experience Cloud

Se nell’organizzazione è stata effettuata la migrazione ad Adobe Admin Console, la lingua del profilo Adobe Experience Cloud determina quella mostrata in Workfront.

1. Fai clic sull’immagine del tuo profilo all’estrema destra della barra degli strumenti di Adobe Experience Cloud, quindi su **Preferenze**. La barra degli strumenti di Adobe Experience Cloud si trova direttamente sopra quella principale di Workfront.

1. In **Profilo** sotto il nome e l’indirizzo e-mail, fai clic sul nome della lingua attualmente selezionata.

1. Seleziona le lingue preferite nei menu a discesa **Prima lingua** e **Seconda lingua**. La prima lingua è la tua scelta predefinita, mentre la seconda viene visualizzata solo se la prima non è supportata da un’applicazione specifica.

### Modificare le impostazioni locali e-mail utente e Workfront {#change-the-workfront-and-user-locales}

* [Modificare le impostazioni locali e-mail predefinite di Workfront](#change-the-workfront-locale)
* [Modificare le impostazioni locali e-mail utente](#change-the-user-locale)

### Modificare le impostazioni internazionali e-mail predefinite di Workfront {#change-the-workfront-locale}

Quando modifichi la lingua e-mail predefinita di Workfront, modifichi anche lingua, data e formato numerico utilizzati nei messaggi in uscita per tutti gli utenti di Workfront. Queste impostazioni diventano predefinite per ogni nuovo utente creato.

Per modificare le impostazioni locali e-mail predefinite di Workfront:

1. Effettua l’accesso a Workfront come amministratore.

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente.**

1. Nella sezione **Informazioni di base**, fai clic sull’elenco a discesa **Lingua e-mail predefinita** per selezionare la lingua in cui desideri visualizzare le e-mail di Workfront.

1. Fai clic su **Salva**.

### Modificare le impostazioni locali e-mail utente {#change-the-user-locale}

<!--


When changing your User Email Locale, you modify the language, date, and number format used in your outgoing messages. These settings override the system settings selected in the Customer Info area of Setup.-->

>[!NOTE]
>
>Le preferenze della lingua vengono memorizzate nel profilo Adobe e le impostazioni internazionali dell’e-mail non vengono utilizzate. Consulta [Modificare la lingua di Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) in questo articolo.

<!--To change your User Email Locale:

{{step1-click-main-menu}}

1. Click your user profile picture.

1. Click the More menu ![](assets/more-icon.png), then click **Edit**.

1. In the **Preferences** section, click the **Email Locale** drop-down list to select the language that you want Workfront emails to display in.

1. Click **Save Changes**.-->
