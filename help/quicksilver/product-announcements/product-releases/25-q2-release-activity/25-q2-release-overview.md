---
title: Panoramica sulla versione del secondo trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9b78a58e-7ced-4b13-8108-40bd36339667
source-git-commit: 993b066ecefb4b345c59289d6c6466ef0416d620
workflow-type: tm+mt
source-wordcount: '1640'
ht-degree: 0%

---

# Panoramica sulla versione del secondo trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del secondo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

<span class="preview">Le funzioni fuori ciclo (quelle rilasciate in produzione prima della data di rilascio del secondo trimestre 2025) sono evidenziate in giallo.</span>

## Pianificazione della versione

Le versioni Workfront sono numerate per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l’anno e il secondo il mese di rilascio. Esempio: la versione di aprile 2025 è numerata 25.4.

Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.

| Versione mensile | Versione trimestrale |
| ----------------- | ----------------- |
| <ul><li>25.2 (13 febbraio 2025)</li><li>25.3 (13 marzo 2025)</li><li>25.4 (10 aprile 2025)</li></ul> | <ul><li>25.4 (10 aprile 2025)</li></ul> |

>[!NOTE]
>
>Per la versione finale di ogni trimestre (25.4 questo trimestre), gli utenti che eseguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alla gestione dei documenti](#document-management-enhancements)
* [Miglioramenti per dispositivi mobili](#mobile-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
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
            Miglioramenti alla logica dei moduli personalizzati</a></p>
            <p>Il generatore di logica dei moduli personalizzati dispone di un’interfaccia aggiornata che offre più spazio per la creazione di regole logiche. Questo nuovo design può accogliere più facilmente ulteriori tipi di logica che potrebbero essere aggiunti in futuro.</p><p>Oltre alle opzioni di visualizzazione e salta logica correnti, è disponibile anche la logica di convalida.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 13 marzo 2025</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (aprile 2025)</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Espressioni aggiunte ai campi personalizzati calcolati</a></p>
            [!BADGE In produzione ]{type=Informative}
            <p>Nei campi personalizzati calcolati di Workfront sono ora disponibili le seguenti espressioni: ARRAY, FORMAT, SWITCH, SORTASCARRAY, SORTDESCARRAY, ARRAYLENGTH, ARRAYELEMENT e ADDHOUR. Le definizioni e gli esempi di ciascuna espressione sono disponibili nell’editor di calcolo e in Experience League.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 31 gennaio 2025</li>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 31 gennaio 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti alla gestione dei documenti

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
                <li>Preview release: March 27, 2025</li>
                <li>Production release for all customers: With the 25.4 release (April 2025)</li>
            </ul>
        </td>
    </tr>    -->                      
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamento visualizzatore bozze desktop </a></p>[!BADGE In produzione ]{type=Informative}
            <p>Il Visualizzatore bozze desktop è stato aggiornato alla versione 2.1.45. Questo aggiornamento consente di utilizzare
            <ul><li>Electron versione 35</li><li>Cromo versione 134</li><ul></p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 20 marzo 2025</li>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 20 marzo 2025</li></span>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modificare più documenti contemporaneamente in un report di documenti </a></p>[!BADGE In produzione ]{type=Informative}
            <p>È ora possibile modificare più documenti contemporaneamente in un rapporto di documento. Puoi modificare le descrizioni e aggiornare i moduli personalizzati.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 6 febbraio 2025</li>
                <span class="preview"><li>Versione di produzione per tutti i clienti: 13 marzo 2025</li></span>
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
            Miglioramenti alle bozze nell'app mobile (solo iOS)</a>[!BADGE In produzione ]{type=Informative}</p>
            <p>Sono disponibili diversi miglioramenti per la funzionalità di bozza nell’app mobile di Adobe Workfront:
            <ul>
            <li>Ora puoi aprire un file di bozza dalla tua app e-mail mobile, da un collegamento condiviso con te. In precedenza, i collegamenti dalle e-mail non erano supportati e si doveva accedere alle bozze dall’app mobile di Workfront.</li>
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
                <li>app mobile di iOS</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Miglioramenti al progetto

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiungi un commento ai progetti quando li modifichi nella casella Modifica progetto</a>[!BADGE In produzione per rilascio rapido]{type=Positive}</p>
            <p>È ora possibile aggiungere un commento a un progetto mentre lo si modifica nella casella Modifica progetto. Puoi anche aggiungere un commento a più progetti contemporaneamente quando li modifichi in blocco. Prima di questo aggiornamento, questa funzionalità non esisteva durante la modifica dei progetti.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 13 febbraio 2025</li>
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
            I dati relativi all'approvazione e alle decisioni dei documenti sono ora disponibili in Data Connect</a>[!BADGE In produzione ]{type=Informative}</p>
            <p>È ora possibile accedere ai dati per le approvazioni dei documenti e le decisioni in Data Connect. Questo set di dati collega le approvazioni dei documenti dalle funzionalità di verifica di Workfront e le approvazioni Frame.io che si verificano sui documenti di Workfront. Ora puoi illustrare l’impatto della durata del ciclo, del numero di cicli e della timeline per le approvazioni in ritardo tramite visualizzazioni di BI.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 25 marzo 2025</li>
                <li>Versione di produzione per tutti i clienti: 25 marzo 2025</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti al calendario di Workfront</a></p>
            <p>Abbiamo aggiornato l’aspetto del Calendario di Workfront a un design moderno coerente con altre aree di Workfront. Esistono piccole differenze di funzionalità rispetto al calendario Workfront corrente, tra cui:
            <ul>
            <li>Come aggiungere elementi ad hoc al calendario</li>
            <li>Creazione e ridenominazione del calendario</li>
            <li>Le azioni del calendario sono state spostate in un menu Altro accanto al nome del calendario</li>
            <li>Un nuovo pannello laterale per la visualizzazione delle informazioni del calendario</li>
            <li>E altro ancora</li>
            <ul>        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 27 febbraio 2025</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (10 aprile 2025)</li>
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
            [!BADGE In produzione ]{type=Informative}
            <p>Workfront ora dispone di versioni delle sottoscrizioni agli eventi. La nuova versione non è una modifica all’API Workfront, ma piuttosto una modifica alla funzionalità di abbonamento agli eventi. È possibile cambiare gli abbonamenti agli eventi alla nuova versione senza creare uno spazio vuoto nell’abbonamento agli eventi</p>
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
            Rappresenta le modifiche utente di Adobe Admin Console come "System" nel feed di aggiornamento di Workfront</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>Ora, quando l’amministratore di Adobe Admin Console apporta una modifica alle informazioni utente di un utente Workfront, Workfront registra tale modifica nella scheda Attività di sistema dell’area Aggiornamenti dell’utente come appartenente al "Sistema". Si riferisce all’amministratore di Adobe Admin Console.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 23 gennaio 2025</li>
                <li>Produzione per rilascio rapido: con la versione 25.2 (13 febbraio 2025)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.4 (aprile 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamenti look-and-feel durante l’arco temporale del secondo trimestre 2025</a></p>
            <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale del secondo trimestre 2025. Consulta le singole note sulla versione per specifiche date di rilascio.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: nell’arco temporale di rilascio del secondo trimestre 2025</li>
                <span class="preview"><li>Versione di produzione: consulta le note sulla versione per date specifiche</li></span>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Funzionalità presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### API versione 2-15 obsoleta

Continuando a migliorare la piattaforma Workfront, è fondamentale mantenere aggiornate le API. Questo garantisce prestazioni e sicurezza ottimali e supporta nuove funzionalità. Stiamo pertanto dichiarando obsolete le versioni 2-15 delle API di Workfront.

* **Settembre 2025**: le versioni 2-14 delle API, attualmente non supportate, diventeranno obsolete. Dopo questa data, queste versioni non saranno più accessibili.
* **Dicembre 2025**: la versione 15 dell&#39;API diventerà obsoleta.

#### Stiamo rimuovendo la vista Agile legacy in un progetto

La vista Agile legacy in un progetto verrà rimossa da Workfront con la versione 25.3 del 13 marzo 2025. Puoi comunque visualizzare le attività in una visualizzazione Agile in un progetto facendo clic sull’icona Bacheche. Gli strumenti agili legacy esistenti sono ancora disponibili nell’area Team.

L’immagine seguente mostra l’opzione agile legacy che verrà rimossa:
![collegamento visualizzazione agile legacy](assets/project-agile-board-view.png)


#### Obsolescenza avanzata di Analytics

A causa di un utilizzo basso e in calo, abbiamo deciso di rendere obsoleto il prodotto Analytics avanzato nella settimana del 25 maggio 2025.
Consigliamo di considerare il nostro prodotto Data Connect come un sostituto. Data Connect consente di creare visualizzazioni personalizzate simili utilizzando gli strumenti di business intelligence preferiti.
Per ulteriori informazioni su questa rimozione, consulta la [Guida all&#39;eliminazione di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).

## Notifiche

### Modernizzazione dell&#39;interfaccia

Stiamo aggiornando l’interfaccia in Adobe Workfront per migliorare l’esperienza utente e per coerenza con altre applicazioni Adobe. Queste modifiche vengono rilasciate al di fuori della pianificazione standard. Per un elenco di queste modifiche, vedere [Modernizzazione interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

### Miglioramenti apportati a Workfront Fusion

>[!IMPORTANT]
>
>La documentazione di Workfront Fusion è stata spostata in una nuova posizione. Per informazioni, istruzioni e versioni di Fusion, visitare la [documentazione di Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home).
>
>Ogni articolo della documentazione di Fusion corrente contiene un collegamento all’articolo corrispondente nella nuova posizione. Aggiorna i segnalibri.
>
>L’attuale set di documentazione di Fusion non è più in fase di aggiornamento e verrà rimosso a breve.

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione di rilascio standard. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività sulla versione di Adobe Workfront Planning Second Quarter 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q2.md).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

A questo punto della versione, non ci sono aggiornamenti per Workfront Proof. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non ci sono aggiornamenti per gli Obiettivi di Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### API versione 19

Per API versione 19, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API attualmente supportate, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del secondo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
