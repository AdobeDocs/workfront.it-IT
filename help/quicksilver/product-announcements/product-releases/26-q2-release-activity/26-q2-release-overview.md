---
title: Panoramica sulla versione del secondo trimestre 2026
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2026. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9e7b94201705ce96dbc38fc6d9246461e4d4d7ea
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---

# Panoramica sulla versione del secondo trimestre 2026

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2026 pianificata per aprile 2026.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che la versione del secondo trimestre 2026 si avvicina alla versione di produzione pianificata.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>26.2 (12 febbraio 2026)</li><li>26.3 (12 marzo 2026)</li><li>26.4 (15 aprile 2026)</li></ul> | <ul><li>26.1 (16 aprile 2026)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (26.4 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo (15 aprile 2026).
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront


* [Altri miglioramenti](#other-enhancements)



### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzionalità</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Esperienza unificata Adobe ora disponibile per altre organizzazioni Workfront</a><p></p>
            <p>Per consentire alle organizzazioni di accedere ai vantaggi di Adobe Unified Experience, continuiamo a renderla disponibile ai clienti Workfront esistenti.</p>
        </td>
        <td><p>venerdì 11 dicembre 2025</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
    <tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## Note sulla versione per altre aree

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività sulla versione del secondo trimestre 2026 per Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md).

A questo punto della versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenario
* Bozza
* Obiettivi

## Aggiornamenti del visualizzatore per la verifica del desktop

### Versione 2.1.54

**Versione di produzione per tutti i clienti: 11 dicembre 2025**

Il Visualizzatore bozze desktop è stato aggiornato a da 2.1.52 a 2.1.54. Questo aggiornamento includeva aggiornamenti interni degli strumenti e non influiva sulle funzionalità dell’utente finale.

La versione 2.1.53 includeva anche modifiche interne alla strumentazione.

Questo aggiornamento è sia per Mac che per Windows.

## Annunci

### API versione 21

La versione 21 dell’API di Workfront è stata rilasciata il 23 ottobre 2025. Per API versione 21, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

>[!IMPORTANT]
>
>Questa modifica della versione API comporta una modifica che potrebbe influire sulle chiamate API esistenti. Ciò è dovuto al fatto che API versione 21 utilizza sottoscrizioni evento versione 2.
>
> Per i campi a selezione multipla, la versione 2 delle sottoscrizioni eventi invia sempre come array. La versione 1 ha inviato un array se sono selezionati più valori. Se è stato selezionato un solo valore, viene inviata una stringa.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 21](/help/quicksilver/wf-api/api/new-api-version-21.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Altre transizioni all&#39;integrazione di Workfront

Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, le seguenti integrazioni non saranno disponibili dopo il **28 febbraio 2026**:

* Workfront per G Suite
* Workfront per Jira
* Workfront per Salesforce.

È consigliabile utilizzare l&#39;automazione e l&#39;integrazione di Workfront per le esigenze di integrazione dell&#39;organizzazione con Google Workspace.
Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del secondo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
