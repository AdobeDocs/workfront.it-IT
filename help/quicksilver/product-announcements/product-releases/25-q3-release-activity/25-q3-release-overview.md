---
title: Panoramica sulla versione del terzo trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del terzo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9342f393-a404-44b4-aad6-2c4cf634dfd5
source-git-commit: 2629598989726e1beaf03092dcd1a4b93a23a9aa
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 3%

---

# Panoramica sulla versione del terzo trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nel rilascio del terzo trimestre 2025 pianificato per luglio 2025.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che il rilascio del terzo trimestre 2025 si avvicina al rilascio pianificato in produzione.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>25.5 (maggio 2025)</li><li>26.6 (giugno 2025)</li><li>25.7 (luglio 2025)</li></ul> | <ul><li>25.7 (luglio 2025)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (25.7 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).



## Miglioramenti di Adobe Workfront

* [Miglioramenti alla gestione dei documenti](#document-management-enhancements)
* [Miglioramenti al reporting](#reporting-enhancements)
* [Miglioramenti per gli aggiornamenti e le notifiche](#update-and-notification-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti alla gestione dei documenti

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funzionalità</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamento visualizzatore bozze desktop</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Questo aggiornamento è una correzione di un problema per mantenere il Visualizzatore desktop compatibile con i sistemi operativi Mac. L'Electron fu declassato a 34.4.0 e il Chromium a 132.</p>
        </td>
        <td>giovedì 7 maggio 2025</td>
        <td>giovedì 7 maggio 2025</td>
        <td>giovedì 7 maggio 2025</td>
    </tr> 
      <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Assets in una cartella Google collegata deve essere aggiunto singolarmente per essere visualizzato in Workfront</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Google sta <a href="https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps">migliorando i controlli di sicurezza</a>
            per le applicazioni di terze parti che accedono a Google Drive, che richiedono l'adozione di un modello di consenso per utente. Di conseguenza, per essere visibili in Workfront, le singole risorse devono essere collegate una alla volta. Consulta <a href="/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md">Configurare le integrazioni dei documenti</a>
             per ulteriori informazioni. </p>
        </td>
        <td>25 maggio 2023</td>
        <td>25 maggio 2023</td>
        <td>25 maggio 2023</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuovi pulsanti di decisione per l'approvazione dei documenti disponibili nel visualizzatore di bozze</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>I nuovi pulsanti di decisione per l'approvazione del documento vengono ora visualizzati nel visualizzatore di bozze. Ora, quando si crea una semplice bozza e si aggiungono approvatori e revisori dal riepilogo del documento, questi possono prendere la decisione direttamente all’interno del visualizzatore di bozze.</p>
        </td>
        <td>venerdì 10 aprile 2025</td>
        <td>venerdì 17 aprile 2025</td>
        <td>venerdì 17 aprile 2025</td>
    </tr>     
  </tbody>
</table>

### Miglioramenti al reporting

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funzionalità</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">I caratteri jolly dell'utente non restituiscono più risultati con un valore null quando si filtra </a><p></p>
            <p>Il comportamento dei caratteri jolly utente è stato aggiornato per escludere il valore null durante il filtraggio di un report. Questa modifica consente al filtro di produrre risultati più precisi, anziché restituire risultati che non hanno un utente configurato correttamente (un risultato nullo). </p>
        </td>
        <td>giovedì 30 aprile 2025</td>
        <td>venerdì 15 maggio 2025</td>
        <td>venerdì 17 luglio 2025</td>
    </tr>     
  </tbody>
</table>

### Miglioramenti per gli aggiornamenti e le notifiche

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funzionalità</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-update-and-notification-enhancements.md" class="MCXref xref" xrefformat="{para}">Esperienza modificata durante l'aggiunta di persone ai commenti</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Per migliorare le prestazioni, è stata introdotta un’esperienza modificata per l’aggiunta di persone ai commenti. Ora, il collegamento "Assegna tag a persone o team" rimane persistente nella casella Commento, dopo aver iniziato ad aggiungere utenti o team al commento. </p>
        </td>
        <td>giovedì 30 aprile 2025</td>
        <td>(Rollout graduale): 8 maggio - 15 maggio 2025</td>
        <td>(Rollout graduale): 8 maggio - 15 maggio 2025</td>
    </tr>     
  </tbody>
</table>

### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante l’intervallo di tempo di rilascio del terzo trimestre 2025</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale di rilascio del terzo trimestre 2025. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale di rilascio del terzo trimestre 2025<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: almeno 2 settimane dopo il rilascio in anteprima (se non diversamente specificato)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernizzazione dell&#39;interfaccia

Stiamo aggiornando l’interfaccia in Adobe Workfront per migliorare l’esperienza utente e per coerenza con altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione standard. Per un elenco di queste modifiche, vedere [Modernizzazione interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Note sulla versione per altre aree

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzioni più recenti, vedere [Attività sulla versione del terzo trimestre 2025 di Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q3.md).

A questo punto della versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenario
* Bozza
* Obiettivi

### API versione 20

La versione 20 dell’API di Workfront è stata rilasciata il 4 maggio 2024. Per API versione 20, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 20](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del primo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).



<!-- HTML you might need

New table

### add product area name

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    </tr>
    <tr>
        <td>
            <p>Title</p>
            <p>Body</p>
        </td>
        <td>Date</td>
        <td>Date</td>
        <td>Date</td>
    </tr>     
  </tbody>
</table> 

New row for table 

<tr>
    <td>
        <p>Title</p>
        <p>Body</p>
    </td>
        <td>Date</td>
        <td>Date</td>
        <td>Date</td>
    </tr>   



-->
