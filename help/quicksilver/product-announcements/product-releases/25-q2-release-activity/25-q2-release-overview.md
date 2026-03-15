---
title: Panoramica sul rilascio del secondo trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9b78a58e-7ced-4b13-8108-40bd36339667
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 18%

---

# Panoramica sul rilascio del secondo trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

<span class="preview">Le funzioni Off-cycle (quelle rilasciate alla produzione prima della data di rilascio del secondo trimestre 2025) sono evidenziate in giallo.</span>

## Pianificazione della versione

Le versioni Workfront sono numerate per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l’anno e il secondo il mese di rilascio. Esempio: la versione di aprile 2025 è numerata 25.4.

Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.

| Rilascio mensile | Rilascio trimestrale |
| ----------------- | ----------------- |
| <ul><li>25,2 (13 febbraio 2025)</li><li>25.3 (13 marzo 2025)</li><li>25.4 (10 aprile 2025)</li></ul> | <ul><li>25.4 (10 aprile 2025)</li></ul> |

>[!NOTE]
>
>Per la versione finale di ogni trimestre (25.4 questo trimestre), gli utenti che eseguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alla gestione dei documenti](#document-management-enhancements)
* [Miglioramenti per dispositivi mobili](#mobile-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti al reporting](#reporting-enhacements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Miglioramenti alla logica dei moduli personalizzati</a></p><p>[!BADGE In produzione &#x200B;]{type=Informative}</p>
            <p>Il generatore di logica dei moduli personalizzati dispone di un'interfaccia aggiornata che offre maggiore spazio per la creazione di regole logiche. Questo nuovo design può essere più facilmente adattato a tipi di logica aggiuntivi che potrebbero essere aggiunti in futuro.</p><p>Oltre alle opzioni di visualizzazione e salta logica correnti, è disponibile anche la logica di convalida.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 13 marzo 2025</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (aprile 2025)</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Espressioni aggiunte ai campi personalizzati calcolati</a></p>
            [!BADGE In Produzione &#x200B;]{type=Informative}
            <p>Le seguenti espressioni sono ora disponibili nei campi personalizzati calcolati da Workfront: ARRAY, FORMAT, SWITCH, SORTASCARRAY, SORTDESCARRAY, ARRAYLENGTH, ARRAYELEMENT e ADDHOUR. Le definizioni e gli esempi di ogni espressione sono disponibili nell'editor di calcolo e nell'Experience League.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: sabato 31 gennaio 2025</li>
                <span class="preview"><li>Rilascio per produzione per tutti i clienti: 31 gennaio 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti della gestione dei documenti

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<!--    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            New document approval decision buttons available in proofing viewer</a></p>
            <p>The new document approval decision buttons now appear in the proofing viewer. Now, when you create a simple proof and then add approvers and reviewers from the Document summary, they can make their decision directly inside the proofing viewer.</p>
        </td>
        <td>
            <p><b>Available on these dates:</b></p>
            <ul>
                <li>Preview release: April 9, 2025</li>
                <li>Production release for a limited set of customers: With the 25.4 release (April 2025)</li>
            </ul>
        </td>
    </tr>   -->                     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamento del visualizzatore di correzione del desktop </a></p>[!BADGE In Produzione &#x200B;]{type=Informative}
            <p>Il Visualizzatore correzione desktop è stato aggiornato alla versione 2.1.45. Questo aggiornamento consente al visualizzatore di utilizzare
            <ul><li>Electron versione 35</li><li>Chromium versione 134</li><ul></p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 20 marzo 2025</li>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 20 marzo 2025</li></span>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modificare più documenti contemporaneamente in un report di documenti </a></p>[!BADGE In Produzione &#x200B;]{type=Informative}
            <p>Ora puoi modificare più documenti contemporaneamente in un report documento. È possibile modificare le descrizioni e aggiornare i moduli personalizzati.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 6 febbraio 2025</li>
                <span class="preview"><li>Rilascio per produzione per tutti i clienti: 13 marzo 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti per dispositivi mobili

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Miglioramenti delle bozze nell’app per dispositivi mobili (solo iOS)</a><p>[!BADGE In Produzione &#x200B;]{type=Informative}</p></p>
            <p>Nell’app mobile Adobe Workfront sono disponibili diversi miglioramenti per la verifica della funzionalità:
            <ul>
            <li>Ora puoi aprire un file di prova dall’applicazione e-mail per dispositivi mobili, da un collegamento condiviso con te. In precedenza, i collegamenti dalle e-mail non erano supportati e dovevi accedere alle prove dall'app mobile Workfront.</li>
            <li>I file di bozza multimediali sono ora supportati nell’app mobile.</li>
            </ul>
            </p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Anteprima versione: N/D</li>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 12 marzo 2025</li> 
            </ul>
            <p><b>Disponibile in questi ambienti:</b></p>
            <ul>
                <li>App iOS per dispositivi mobili</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti ai progetti

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiungi un commento ai progetti quando li modifichi nella casella Modifica progetto</a><p>[!BADGE In produzione &#x200B;]{type=Informative}</p>
            <p>È ora possibile aggiungere un commento a un progetto mentre lo si modifica nella casella Modifica progetto. Puoi anche aggiungere un commento a più progetti contemporaneamente quando li modifichi in blocco. Prima di questo aggiornamento, questa funzionalità non esisteva durante la modifica dei progetti.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 13 febbraio 2025</li>
                <li>Produzione per rilascio rapido: con la versione 25.3 (marzo 2025)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (aprile 2025)</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti al reporting

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">
            I dati relativi all’approvazione dei documenti e alle decisioni sono ora disponibili in Data Connect</a><p>[!BADGE In produzione &#x200B;]{type=Informative}</p>
            <p>È ora possibile accedere ai dati per le approvazioni dei documenti e le decisioni in Data Connect. Questo set di dati collega le approvazioni dei documenti dalle funzionalità di verifica di Workfront e le approvazioni Frame.io che si verificano sui documenti di Workfront. Ora potrai illustrare la durata del ciclo, il numero di cicli e gli impatti della timeline per le approvazioni in ritardo tramite le visualizzazioni BI.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: mercoledì 25 marzo 2025</li>
                <li>Versione di produzione per tutti i clienti: 25 marzo 2025</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti al calendario di Workfront</a></p><p>[!BADGE In produzione &#x200B;]{type=Informative}</p>
            <p>Abbiamo aggiornato l’aspetto del Calendario di Workfront a un design moderno coerente con altre aree di Workfront. Esistono piccole differenze di funzionalità rispetto al calendario Workfront corrente, tra cui:
            <ul>
            <li>Come aggiungere elementi ad hoc al calendario</li>
            <li>Come creare e rinominare il calendario</li>
            <li>Le azioni del calendario sono state spostate in un menu Altro accanto al nome del calendario</li>
            <li>Un nuovo pannello laterale per la visualizzazione delle informazioni del calendario</li>
            <li>E altro ancora</li>
            <ul>        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 27 febbraio 2025</li>
                <li>Questa funzione verrà rilasciata in Produzione in tre fasi: a partire dalla versione 25.4 (10 aprile 2025) e fino al 17 aprile 2024</li>
            </ul>
        </td>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Effettua l’aggiornamento alla nuova versione dell’abbonamento agli eventi con gli endpoint di aggiornamento della versione</a></p>
            [!BADGE In produzione &#x200B;]{type=Informative}
            <p>Workfront ora dispone di versioni delle sottoscrizioni agli eventi. Questa nuova versione non cambia l’API Workfront, ma la funzionalità di sottoscrizione eventi. È possibile cambiare gli abbonamenti agli eventi alla nuova versione senza creare uno spazio vuoto nell’abbonamento agli eventi</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 6 marzo 2025</li></span>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Rappresenta le modifiche utente di Adobe Admin Console come "System" nel feed di aggiornamento di Workfront</a></p><p>[!BADGE In produzione &#x200B;]{type=Informative}</p><p>Ora, quando l’amministratore di Adobe Admin Console apporta una modifica alle informazioni utente di un utente Workfront, Workfront registra tale modifica nella scheda Attività di sistema dell’area Aggiornamenti dell’utente come appartenente al "Sistema". Si riferisce all’amministratore di Adobe Admin Console.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Rilascio in anteprima: venerdì 23 gennaio 2025</li>
                <li>Produzione per rilascio rapido: con la versione 25.2 (13 febbraio 2025)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (aprile 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamenti look-and-feel durante l’arco temporale del secondo trimestre 2025</a></p>
            <p>Aggiornamenti minori all’aspetto di varie aree dell’applicazione Adobe Workfront vengono effettuati nell’arco di tempo del secondo trimestre 2025. Esamina le singole note sulla versione per le date di rilascio specifiche.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: per tutto l’arco temporale della versione del secondo trimestre 2025</li>
                <span class="preview"><li>Rilascio per produzione: esamina le note sulla versione per date specifiche</li></span>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Funzionalità che verrà presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### Versione API 2-15 obsoleta

Poiché continuiamo a migliorare la piattaforma Workfront, è fondamentale mantenere aggiornate le API. Ciò garantisce prestazioni e sicurezza ottimali e supporta nuove funzionalità. Pertanto, le versioni 2-15 delle API di Workfront verranno dichiarate obsolete.

* **Settembre 2025**: le versioni API 2-14, che non sono attualmente supportate, diventeranno obsolete. Dopo questa data, queste versioni non saranno più accessibili.
* **Dicembre 2025**: la versione 15 dell&#39;API diventerà obsoleta.

#### Stiamo rimuovendo la vista Agile legacy in un progetto

La vista Agile legacy in un progetto verrà rimossa da Workfront con la versione 25.3 del 13 marzo 2025. Puoi comunque visualizzare le attività in una visualizzazione Agile in un progetto facendo clic sull’icona Bacheche. Gli strumenti Agile legacy esistenti sono ancora disponibili nell’area Teams.

L’immagine seguente mostra l’opzione Agile legacy che verrà rimossa:
![collegamento alla vista Agile legacy](assets/project-agile-board-view.png)


#### Obsolescenza avanzata di Analytics

A causa di un utilizzo basso e in calo, abbiamo deciso di rendere obsoleto il prodotto Analytics avanzato nella settimana del 25 maggio 2025.
Consigliamo di considerare il nostro prodotto Data Connect come un sostituto. Data Connect consente di creare visualizzazioni personalizzate simili utilizzando gli strumenti di business intelligence preferiti.
Per ulteriori informazioni su questa rimozione, consulta la [Guida all&#39;eliminazione di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).

## Annunci

### Modernizzazione dell’interfaccia

L’interfaccia di Adobe Workfront è in fase di aggiornamento per migliorare l’esperienza utente e per uniformarla alle altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione di rilascio standard. Per un elenco di queste modifiche, consulta [Modernizzazione dell’interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

### Miglioramenti di Workfront Fusion

>[!IMPORTANT]
>
>La documentazione di Workfront Fusion è stata spostata in una nuova posizione. Per informazioni, istruzioni e versioni di Fusion, visitare la [documentazione di Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home).
>
>Ogni articolo della documentazione di Fusion corrente contiene un collegamento all’articolo corrispondente nella nuova posizione. Aggiorna i segnalibri.
>
>L’attuale set di documentazione di Fusion non è più in fase di aggiornamento e verrà rimosso a breve.

Le nuove funzioni di Workfront Fusion sono disponibili nell’ambiente di Produzione con una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Pianificazione di Workfront

Nuove funzioni di Pianificazione di Workfront sono disponibili nell’ambiente di Produzione. Per ulteriori informazioni sulle funzioni più recenti, vedere [Attività sulla versione di Adobe Workfront Planning per il secondo trimestre 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q2.md).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

A questo punto della versione, non ci sono aggiornamenti per Workfront Proof. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non ci sono aggiornamenti per gli Obiettivi di Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Versione 19 dell’API

Nella versione 19 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 19 dell’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API attualmente supportate, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del secondo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/it/docs/workfront-known-issues/releases/current-updates).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home).
