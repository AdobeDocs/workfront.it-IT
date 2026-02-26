---
title: Panoramica sul rilascio del secondo trimestre 2026
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2026. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 860bd4bef75a90f4e1c5a21f38de95962804c00c
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 51%

---

# Panoramica sul rilascio del secondo trimestre 2026

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2026 pianificata per aprile 2026.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che la versione del secondo trimestre 2026 si avvicina alla versione di produzione pianificata.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Rilascio mensile | Rilascio trimestrale |
>|----|----|
>| <ul><li>26.2 (12 febbraio 2026)</li><li>26.3 (12 marzo 2026)</li><li>26.4 (15 aprile 2026)</li></ul> | <ul><li>26.1 (16 aprile 2026)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (26.4 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo (15 aprile 2026).
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti ai documenti](#document-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti al reporting](#reporting-enhancements)
* [Richiesta di miglioramenti](#requesting-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Comprimi sezione modulo personalizzato per impostazione predefinita</a><p>Per impostazione predefinita, tutte le sezioni di un modulo personalizzato vengono espanse quando il modulo stesso viene espanso. Una nuova opzione di Designer di moduli personalizzati consente di contrassegnare una sezione da comprimere per impostazione predefinita quando un utente apre il modulo. Questa opzione viene applicata a livello di sezione, non ai campi.</p>
        </td>
        <td><p>giovedì 26 febbraio 2025</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Il tipo di campo Rich Text è ora disponibile nei moduli personalizzati</a><p>Il nuovo tipo di campo <b>Rich text</b> nei moduli personalizzati è un editor di testo affidabile, con opzioni di formattazione quali apice e pedice, intestazioni e tabelle, oltre alle opzioni tradizionali di grassetto, corsivo, sottolineatura, punti elenco, numerazione, collegamenti ipertestuali e virgolette. Il limite di caratteri rimane 15.000.</p>
        </td>
        <td><p>venerdì 29 gennaio 2026</p></td>
        <td><p>venerdì 12 febbraio 2026</p>
            <p>Questa funzione è stata temporaneamente rimossa dall’ambiente di produzione il 13 febbraio 2026.</p></td>
        <td><p>Da definire</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Nuovi indirizzi IP per le notifiche e-mail di Workfront</a><p></p>
            <p>Stiamo aggiornando gli indirizzi IP utilizzati per inviare notifiche e-mail da Workfront. Se l'organizzazione mantiene un inserisco nell'elenco Consentiti di posta elettronica o di firewall, <b>devi</b> aggiungere i nuovi indirizzi IP di seguito per garantire la continuità della consegna delle notifiche di Workfront.</p><p>Questi aggiornamenti si applicano a tutte le e-mail in uscita generate dall’applicazione Workfront, incluse approvazioni, promemoria, notifiche di bozze e altri messaggi di sistema.</p>
            <ul>
            <li>USA:
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>UE: 
            <ul>
            <li>24 110 76 224</li>
            <li>24 110 76 223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>venerdì 15 gennaio 2026</p></td>
        <td><p>venerdì 15 gennaio 2026</p></td>
        <td><p>15 gennaio 2026</p></td>
    <tr>
            </tbody>
        </table>

<!--

### Document enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Multi‑stage approval workflows available for unified approvals</a><p></p>
            <p>Multi‑stage approval workflows are now available in unified approvals, helping organizations enforce structured, repeatable approval processes that reflect how work is reviewed in the real world. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Set up and use multi-stage approval workflow templates</a><p></p>
            <p>You can now configure and reuse multi-stage approval workflow templates, making it easier to apply consistent governance across repeatable approval workflows. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
             </tbody>
        </table>   

-->

### Miglioramenti ai progetti

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">Esperienza aggiornata con l'assegnazione singola o in blocco delle attività modello </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> È stata aggiornata la sezione Assegnazioni nella casella Modifica attività modello quando si modificano attività modello singole o in blocco.  </p>
        </td>
        <td><p>venerdì 5 febbraio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Esperienza aggiornata con l'assegnazione singola o in blocco delle attività </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> È stata aggiornata la sezione Assegnazioni nella casella Modifica attività quando si modificano singole attività o in blocco. </p>
        </td>
        <td><p>martedì 26 gennaio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
    </tr>
            </tbody>
        </table>

### Miglioramenti al reporting

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Etichette campi personalizzati visualizzate durante la creazione dei report</a><p></p>
            <p>L’etichetta del campo personalizzato viene ora visualizzata prima del nome del campo e dell’oggetto negli strumenti di creazione dei rapporti, facilitando l’individuazione dei campi. Le etichette dei campi vengono visualizzate anche quando si definiscono filtri, visualizzazioni e raggruppamenti negli elenchi.</p>
        </td>
        <td><p>giovedì 26 febbraio 2025</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
<!--    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Shareable Report Folders</a><p></p>
            <p>You can now organize and share reports using shareable report folders. This new feature helps teams that manage large volumes of reports maintain scalable and consistent access control.</p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>-->
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Improved Date Labels for Chart Groupings in Canvas Dashboards</a><p></p>
            <p>Charts that group data by date now display clearer, more readable date labels. With this update, date labels dynamically adjust based on the selected Group by option—such as day, week, month, or year—making charts easier to read and interpret at a glance.</p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>-->
             </tbody>
        </table>

### Richiesta di miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Trimestrale</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Esperienza di condivisione aggiornata per le visualizzazioni avanzate</a><p></p>
            <p>Nell’area Nuove richieste, quando condividi una vista avanzata con un utente e concedi le autorizzazioni di visualizzazione, l’utente può modificare gli elementi della vista e tali modifiche vengono salvate nelle preferenze personali dell’utente. È ora possibile salvare una copia della visualizzazione che includa le modifiche apportate o ripristinare le impostazioni originali della visualizzazione condivisa. Possono inoltre condividere la vista copiata con altri utenti. </p>
        </td>
           <td><p>giovedì 26 febbraio 2025</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
 </tr>
            </tbody>
        </table>

### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funzione</strong>
        </td>
        <td><strong>Anteprima</strong></td>
        <td><strong>Rilascio rapido</strong></td>
        <td><strong>Ogni trimestre</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ora disponibile per altre organizzazioni Workfront</a><p></p>
            <p>Per consentire alle organizzazioni di accedere ai vantaggi di Adobe Unified Experience, la disponibilità è stata estesa per i clienti esistenti di Workfront.</p>
        </td>
        <td><p>venerdì 11 dicembre 2025</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
        <td><p>giovedì 11 febbraio 2026</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## Note sulla versione per altre aree

### Miglioramenti di Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili nell’ambiente di Produzione con una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Pianificazione di Workfront

Nuove funzioni di Pianificazione di Workfront sono disponibili nell’ambiente di Produzione. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività sulla versione del secondo trimestre 2026 per Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md).

Al momento, in questa versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenari
* Bozza
* Obiettivi

## Aggiornamenti del visualizzatore di bozza desktop

### Versione 2.1.54

**Rilascio in produzione per tutti i clienti: 11 dicembre 2025**

Il Visualizzatore di bozza per desktop è stato aggiornato dalla versione 2.1.52 alla 2.1.54 e ha incluso aggiornamenti interni relativi agli strumenti, senza interessare le funzionalità dell’utente finale.

Anche la versione 2.1.53 ha incluso modifiche interne agli strumenti.

Questo aggiornamento è valido sia per Mac che per Windows.

## Annunci

### Versione 21 dell’API

La versione 21 dell’API di Workfront è stata rilasciata il 23 ottobre 2025. Nella versione 21 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

>[!IMPORTANT]
>
>Questa modifica alla versione API comporta delle interruzioni e potrebbe interessare le chiamate API esistenti. Ciò è dovuto al fatto che la versione 21 dell’API utilizza la versione 2 delle sottoscrizioni eventi.
>
> Per i campi a selezione multipla, la versione 2 di Sottoscrizioni eventi invia sempre come array. La versione 1 inviava un array solo se venivano selezionati più valori. Se veniva selezionato un solo valore, veniva inviata una stringa.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 21 dell’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Altre transizioni all’integrazione di Workfront

Per garantire maggiore stabilità e scalabilità alle integrazioni, è stato adottato un approccio moderno e flessibile basato su Workfront Automation and Integration (Fusion). Nell’ambito di questo processo di transizione, le seguenti integrazioni non saranno disponibili dopo il **28 febbraio 2026**:

* Workfront per G Suite
* Workfront per Jira
* Workfront per Salesforce.

Per le esigenze di integrazione dell’organizzazione è consigliabile utilizzare Workfront Automation and Inegration con Google Workspace.
Per una panoramica di Workfront Automation and Integration consulta [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del secondo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=it).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
