---
title: Panoramica sul rilascio del secondo trimestre 2026
description: This page provides information about functionality that is included in the Second Quarter 2026 release. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 93c22854ccc405c442331ac392d919d63b8a8aa8
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 38%

---

# Panoramica sul rilascio del secondo trimestre 2026

This page provides information about functionality that is included in the Second Quarter 2026 release scheduled for April 2026.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. This page will be updated with additional enhancements as the Second Quarter 2026 release nears its planned Production release.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Rilascio mensile | Rilascio trimestrale |
>|----|----|
>| <ul><li>26,2 (12 febbraio 2026)</li><li>26,3 (12 marzo 2026)</li><li>26,4 (15 aprile 2026)</li></ul> | <ul><li>26.1 (16 aprile 2026)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (26.4 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo (15 aprile 2026).
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti al reporting](#reporting-enhancements)
* [Requesting enhancements](#requesting-enhancements)
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
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Custom Quarters removed from Project Preferences</a><p>È stata spostata l’area Trimestre personalizzato dalla sezione Preferenze progetto. È ora una sezione autonoma del programma di installazione.</p>
        </td>
        <td><p>venerdì 5 marzo 2026</p></td>
        <td><p>giovedì 15 aprile 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Comprimi sezione modulo personalizzata per impostazione predefinita</a><p>Per impostazione predefinita, tutte le sezioni di un modulo personalizzato vengono espanse quando il modulo stesso viene espanso. Una nuova opzione di Designer di moduli personalizzati consente di contrassegnare una sezione da comprimere per impostazione predefinita quando un utente apre il modulo. Questa opzione viene applicata a livello di sezione, non ai campi.</p>
        </td>
        <td><p>venerdì 26 febbraio 2026</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Il tipo di campo RTF è ora disponibile nei moduli personalizzati</a><p>The new <b>Rich text</b> field type in custom forms is a robust text editor, with formatting options such as superscript and subscript, headings, and tables, in addition to the traditional options of bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. The character limit remains 15,000.</p>
        </td>
        <td><p>venerdì 29 gennaio 2026</p></td>
        <td><p>venerdì 12 febbraio 2026</p>
            <p>This feature has been temporarily removed from the Production environment on February 13, 2026.</p></td>
        <td><p>Da definire</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Nuovi indirizzi IP per le notifiche e-mail Workfront</a><p></p>
            <p>Stiamo aggiornando gli indirizzi IP utilizzati per inviare le notifiche e-mail da Workfront. Se la tua organizzazione mantiene un elenco di indirizzi e-mail o firewall consentiti, <b>devi</b> aggiungere i nuovi indirizzi IP di seguito per garantire la continuità del recapito delle notifiche di Workfront.</p><p>Questi aggiornamenti si applicano a tutti i messaggi e-mail in uscita generati dall'applicazione Workfront, inclusi approvazioni, promemoria, notifiche di prova e altri messaggi di sistema.</p>
            <ul>
            <li>USA:
            <ul>
            <li>206 55 149 212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>UE: 
            <ul>
            <li>24.110.76.224</li>
            <li>24.110.76.223</li>
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

### Miglioramenti ai documenti

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Unified Review &amp; Approval powered by Workfront and Frame.io</a><p></p>
            <p>Siamo lieti di introdurre la funzione di revisione e approvazione unificata basata su Workfront e Frame.io, un'esperienza di revisione e approvazione semplificata che unisce pianificazione, verifica e collaborazione in un unico flusso di lavoro connesso.
 </p>
        </td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>giovedì 15 aprile 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Flussi di lavoro di approvazione in più fasi disponibili per le approvazioni unificate</a><p></p>
            <p>I flussi di lavoro di approvazione in più fasi sono ora disponibili nelle approvazioni unificate, consentendo alle organizzazioni di applicare processi di approvazione strutturati e ripetibili che riflettono il modo in cui il lavoro viene rivisto nel mondo reale. </p>
        </td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>giovedì 15 aprile 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Configurare e utilizzare modelli di flusso di lavoro di approvazione in più fasi</a><p></p>
            <p>È ora possibile configurare e riutilizzare i modelli di flusso di lavoro di approvazione in più fasi, semplificando l'applicazione di regole di governance coerenti in flussi di lavoro di approvazione ripetibili. </p>
        </td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>giovedì 15 aprile 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
             </tbody>
        </table>


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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">Updated experience when and single- or bulk-assigning template tasks </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> We have updated the Assignments section in the Edit Template Tasks box when editing single template tasks or editing them in bulk.  </p>
        </td>
        <td><p>venerdì 5 febbraio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
        <td><p>A partire dal 5 febbraio 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Esperienza aggiornata durante l'assegnazione singola o in blocco di attività </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> È stata aggiornata la sezione Assegnazioni nella casella Modifica attività quando si modificano singole attività o in blocco. </p>
        </td>
        <td><p>martedì 26 gennaio 2026</p></td>
        <td><p>Starting February 5, 2026</p></td>
        <td><p>Starting February 5, 2026</p></td>
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
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">New Authentication Options for Data Connect Connection</a><p></p>
            <p>You can now authenticate to Data Connect using RSA keys or Programmatic Access Tokens (PAT) connections, adding more secure and flexible alternatives to traditional username/password credentials. </p>
        </td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Etichette dei campi personalizzati visualizzate durante la compilazione dei report</a><p></p>
            <p>L’etichetta del campo personalizzato viene ora visualizzata prima del nome del campo e dell’oggetto negli strumenti di creazione del report, per facilitare l’individuazione dei campi. Le etichette dei campi vengono visualizzate anche quando si definiscono filtri, visualizzazioni e raggruppamenti negli elenchi.</p>
        </td>
        <td><p>venerdì 26 febbraio 2026</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Cartelle report condivisibili</a><p></p>
            <p>Ora puoi organizzare e condividere i rapporti utilizzando cartelle di rapporti condivisibili. Questa nuova funzione consente ai team che gestiscono grandi volumi di report di mantenere un controllo degli accessi scalabile e coerente.</p>
        </td>
        <td><p>venerdì 26 febbraio 2026</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Improved Date Labels for Chart Groupings in Canvas Dashboards</a><p></p>
            <p>I grafici che raggruppano i dati per data ora presentano etichette di data più chiare e leggibili. Con questo aggiornamento, le etichette delle date vengono regolate in modo dinamico in base all’opzione Raggruppa per selezionata, ad esempio giorno, settimana, mese o anno, semplificando la lettura e l’interpretazione immediata dei grafici.</p><p>Note: Canvas Dashboards is currently in beta.</p>
        </td>
        <td><p>venerdì 26 febbraio 2026</p></td>
        <td><p>venerdì 12 marzo 2026</p></td>
        <td><p>venerdì 16 aprile 2026</p></td>
    </tr>
             </tbody>
        </table>

### Requesting enhancements

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Esperienza di condivisione aggiornata per visualizzazioni avanzate</a><p></p>
            <p>Nell'area Nuove richieste, quando si condivide una visualizzazione avanzata con un utente e si assegnano le autorizzazioni di visualizzazione, l'utente può modificare gli elementi di visualizzazione e tali modifiche vengono salvate nelle preferenze personali dell'utente. È ora possibile salvare una copia della visualizzazione che include le modifiche o ripristinare le impostazioni originali della visualizzazione condivisa. Possono inoltre condividere la vista copiata con altri utenti. </p>
        </td>
           <td><p>venerdì 26 febbraio 2026</p></td>
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

### Workfront Planning Trial is now available

[!BADGE Off schedule]{type=Neutral}

>[!NOTE]
>
>* Anteprima e produzione per tutti: 2 marzo 2026
>* Prima di poter accedere all&#39;ambiente di prova di Planning, è necessario accettare il contratto di prova disponibile nell&#39;ambiente.
>* Non è necessario firmare il contratto Adobe AI Agent per utilizzare Planning Designer durante il periodo di prova.

La versione di prova di Workfront Planning è ora disponibile per tutti i clienti Workfront.

La versione di prova gratuita offre ai clienti Workfront un accesso di 60 giorni con licenza Prime a Workfront Planning, a partire dal 2 marzo 2026. Il periodo di prova termina il 1° maggio 2026.

La versione di prova gratuita di Workfront Planning offre le seguenti funzionalità:

* Un ambiente Planning curato e con più aree di lavoro
* Dati di esempio per darti un’idea su dove iniziare
* Formazione e guida interne al prodotto
* Indica chiaramente le milestone durante la configurazione, personalizzate per ruoli specifici.
* Planning Designer: un assistente basato sull&#39;intelligenza artificiale che consente di creare l&#39;ambiente desiderato

For more information, see [Get started with the Adobe Workfront Planning free trial](/help/quicksilver/planning/general/trial-workfront-planning.md).

### Versione 21 dell’API

La versione 21 dell’API di Workfront è stata rilasciata il 23 ottobre 2025. Nella versione 21 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

>[!IMPORTANT]
>
>Questa modifica alla versione API comporta delle interruzioni e potrebbe interessare le chiamate API esistenti. Ciò è dovuto al fatto che la versione 21 dell’API utilizza la versione 2 delle sottoscrizioni eventi.
>
> For multi-select fields, Event Subscriptions version 2 always sends as an array. La versione 1 inviava un array solo se venivano selezionati più valori. Se veniva selezionato un solo valore, veniva inviata una stringa.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 21 dell’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Altre transizioni all’integrazione di Workfront

Per garantire maggiore stabilità e scalabilità alle integrazioni, è stato adottato un approccio moderno e flessibile basato su Workfront Automation and Integration (Fusion). Nell’ambito di questo processo di transizione, le seguenti integrazioni non saranno disponibili dopo il **28 febbraio 2026**:

* Workfront per G Suite
* Workfront per Jira
* Workfront per Salesforce.

Per le esigenze di integrazione dell’organizzazione è consigliabile utilizzare Workfront Automation and Inegration con Google Workspace.
Per una panoramica di Workfront Automation and Integration consulta [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Aggiornamenti di manutenzione di Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del secondo trimestre 2026, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=it).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
