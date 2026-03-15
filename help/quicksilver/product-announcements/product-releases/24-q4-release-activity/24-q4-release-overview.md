---
title: Panoramica sul rilascio del quarto trimestre 2024
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 14%

---

# Panoramica sul rilascio del quarto trimestre 2024

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

<span class="preview">Le funzioni fuori ciclo (quelle rilasciate in produzione prima della data di rilascio del quarto trimestre 2024) sono evidenziate in giallo.</span>

>[!IMPORTANT]
>
>La versione 23.3 includeva l’opzione per spostare l’organizzazione alle versioni mensili. Pertanto, Workfront ha modificato lo schema di numerazione delle versioni per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l&#39;anno, mentre il secondo indica il mese dell&#39;aggiornamento. Esempio: la versione di aprile 2024 è 24.4.
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Rilascio mensile | Rilascio trimestrale |
>|----|----|
>| <ul><li>24,8 (15 agosto 2024)</li><li>24,9 (12 settembre 2024)</li><li>24,10 (17 ottobre 2024)</li></ul> | <ul><li>24,10 (17 ottobre 2024)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (le 24.10 di questo trimestre), gli utenti che hanno pianificato il rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti della gestione dei documenti](#document-management-enhancements)
* [Miglioramenti alla Home](#home-enhancements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
* [Miglioramenti ai progetti](#project-enhancements)
* [Miglioramenti della correzione](#proofing-enhancements)
* [Miglioramenti a report e dashboard](#report-and-dashboard-enhancements)
* [Altri miglioramenti](#other-enhancements)
* [Funzionalità che verrà presto rimossa da Workfront](#functionality-soon-to-be-removed-from-workfront)

### Miglioramenti per gli amministratori

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Livello di accesso ora disponibile nella promozione dell'ambiente</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per espandere le funzionalità di promozione dell’ambiente, è stata aggiunta la possibilità di includere i livelli di accesso. Ora è possibile configurare un livello di accesso in un ambiente Sandbox e quindi promuovere tale livello di accesso all’ambiente di produzione.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 17 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Un contatore nei moduli personalizzati mostra il numero di campi</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>I moduli personalizzati sono limitati a 500 campi. In un modulo lungo può essere difficile sapere quanti campi sono presenti nel modulo e se ci si avvicina al limite. Un contatore è stato aggiunto ai moduli personalizzati in basso a sinistra. Il contatore indica il numero di campi utilizzati nel modulo ed è sempre visibile durante lo scorrimento all'interno del progettista del modulo.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: mercoledì 1 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Un'opzione "Seleziona tutto" è ora disponibile nei modelli di layout</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per semplificare la visualizzazione e la visualizzazione dei campi con modelli di layout, è stata aggiunta una casella di controllo "Seleziona tutto" alle aree Panoramica e Finanza della visualizzazione Dettagli in un modello di layout. Questa opzione è disponibile se hai selezionato Progetto, Attività, Problema, Portfolio o Programma in "Personalizza ciò che viene visualizzato dagli utenti".</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 29 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 29 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Ripristino dei pacchetti di promozione dell'ambiente</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Per rendere la promozione dell'ambiente più flessibile e facile da usare, abbiamo attivato la funzionalità di rollback. Ora è possibile ripristinare i pacchetti entro 24 ore, in modo da ripristinare più facilmente le configurazioni precedenti interessate da un pacchetto di promozione dell'ambiente.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 29 agosto 2024</p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: con la versione 24.9 (12 settembre 2024)</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Il pulsante Layout di Progettazione moduli personalizzati consente due o tre colonne</a></p>
                    <p>Un pulsante "Layout" nella finestra di progettazione del modulo personalizzato consente di scegliere un'area di lavoro a due o tre colonne. Il progettista del modulo originale utilizza tre colonne e le impostazioni dei campi vengono visualizzate nella colonna a destra. Se si selezionano due colonne, le impostazioni dei campi vengono visualizzate accanto alla raccolta campi nella colonna all'estrema sinistra.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p><s>Rilascio in anteprima: martedì 12 agosto 2024</s></p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: N/D</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: N/D</p>
                        </li>
                    </ul>
                    <p><i>Questa funzione è stata rimossa dall’anteprima e non verrà rilasciata con alcuna versione futura.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti alla gestione dei documenti

>[!IMPORTANT]
>
>Le funzionalità elencate in **Miglioramenti della gestione dei documenti** fanno parte di una versione per fasi e sono disponibili solo per clienti specifici.

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Visualizzare lo stato della decisione del documento direttamente nell'elenco dei documenti</a></p>
                    <p>Ora puoi visualizzare lo stato decisionale di un documento direttamente nell'elenco dei documenti.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p><s>Rilascio in anteprima: venerdì 3 ottobre 2024</s></p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Aggiungere rapidamente revisori e approvatori precedenti alle nuove versioni del documento</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Ora è possibile aggiungere rapidamente revisori e approvatori di versioni di documenti precedenti.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti alla Home

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Aggiornamenti al widget In attesa della mia approvazione nella nuova pagina principale</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Sono state apportate le seguenti modifiche al widget In attesa di approvazione:</p>
                        <ul>
                            <li>Rinominato widget: il nome di questo widget è ora Approvazioni personali.</li>
                            <li>Approvazioni aggiunte Inviate come opzione filtro: ora con questo widget puoi visualizzare le approvazioni inviate nella nuova pagina Home.</li>
                            <li>Scadenza: ora puoi vedere la scadenza della bozza, se ne è stata impostata una. Se non viene impostata una scadenza, per impostazione predefinita viene utilizzata la data di creazione.</li>
                        </ul>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 10 ottobre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 10 ottobre 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Introduzione alle priorità: un'esperienza Workfront più semplice, semplice e intuitiva per i proprietari delle attività</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Le priorità migliorano l'attenzione e la produttività per consentire ai clienti di ottenere di più in meno tempo.</p>
                    <p>Con Priorità, puoi godere di:</p>
                        <ul>
                            <li>Gestione e assegnazione di priorità alle attività quotidiane: organizzazione del giorno o della settimana con la navigazione consolidata per una maggiore chiarezza.</li>
                            <li>Maggiore produttività: accesso al contesto del progetto ed esecuzione più rapida delle attività con un numero inferiore di clic.</li>
                            <li>Funzioni personalizzate: caratteristiche progettate appositamente per i proprietari delle attività.</li>
                        </ul>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti dell’integrazione

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Miglioramenti dell'esperienza di accesso all'integrazione di Outlook</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>L’esperienza di accesso per l’integrazione con Outlook è stata semplificata: tutti i clienti possono visualizzare lo stesso pulsante per accedere a Workfront, indipendentemente dal fatto che siano abilitati IMS. I passaggi di accesso successivi rimangono diversi per le istanze IMS e non IMS, ma la pagina iniziale è la stessa per tutti gli utenti.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: mercoledì 6 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Rilascio per produzione per tutti i clienti: 6 agosto 2024</span></p>
                        </li>
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
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Altre assegnazioni rilevanti aggiunte al flusso di lavoro Nuova attività</a></p>
                    [!BADGE In produzione per rilascio rapido ]{type=Positive}
                    <p>È stata aggiunta la stessa funzionalità per assegnazioni intelligenti più rilevanti al campo Assegnazioni della casella Nuova attività quando si aggiunge un'attività a un progetto e in un elenco di attività di progetto.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: mercoledì 13 febbraio 2024</p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                        </li>
                    </ul>
                <p><i>Questa funzione è stata rimossa dall’anteprima e dalla produzione con rilascio rapido.</i></p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Altre assegnazioni avanzate rilevanti</a></p>
                    [!BADGE In produzione per rilascio rapido ]{type=Positive}
                    <p>È stato modificato l’algoritmo utilizzato da Workfront per calcolare e suggerire assegnazioni intelligenti per le attività. Il nuovo algoritmo si applica nelle seguenti aree di Workfront in cui si assegna un’attività: elenchi di attività, area Assegnazioni nell’intestazione dell’attività, Home e il pannello Riepilogo.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 21 dicembre 2023</p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                        </li>
                    </ul>
                <p><i>Questa funzione è stata rimossa dall’Anteprima e dalla Produzione con rilascio rapido.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti della correzione

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correzione dei problemi di copia/incolla per il visualizzatore di correzione del desktop</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>È stato risolto un problema a causa del quale il contenuto veniva incollato in modo errato nella sezione Aggiornamenti del Visualizzatore correzione desktop.</p>
                    <p>Nuova versione: 2.1.39</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: giovedì 2 ottobre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Rilascio per produzione per tutti i clienti: 2 ottobre 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correzione schermo vuoto per gli utenti di Windows che usano il visualizzatore di correzione del desktop</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>È stato risolto un problema relativo alla nuova versione 2.1.36 del Visualizzatore correzione desktop, a causa del quale alcuni utenti di Windows visualizzavano una schermata vuota dopo l’apertura del visualizzatore. </p>
                    <p>Nuova versione per gli utenti Windows: 2.1.37</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: sabato 30 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Rilascio per produzione per tutti i clienti: 30 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamento di Chromium per il visualizzatore di correzione per il desktop</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Stiamo aggiornando Desktop Proofing Viewer per supportare Chromium 126.0.6478.127 che risolverà i problemi con gli elementi dell'interfaccia utente nelle prove interattive.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 29 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Rilascio per produzione per tutti i clienti: 29 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti a report e dashboard

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Funzione</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Date di rilascio</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect disponibile per nuovi piani</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Workfront Data Connect sarà disponibile per le organizzazioni che dispongono di uno dei nuovi piani Workfront. Data Connect consente alle aziende di accedere ai dati come data lake sicuro e scalabile, che può essere analizzato e visualizzato utilizzando strumenti di business intelligence o archiviato esternamente. Inoltre, le organizzazioni possono utilizzare Data Connect per visualizzare le analisi dei dati precedentemente non disponibili, ad esempio l'analisi delle tendenze basata sul tempo, la mappatura delle variabili e l'analisi dei dati di sistema esterni in combinazione con i dati di Workfront.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                    <p><i>Disponibile solo per le organizzazioni con uno dei nuovi piani Adobe Workfront. Data Connect è incluso nel piano Ultimate e sarà disponibile per l’acquisto come componente aggiuntivo ai piani Prime e Select nella prima metà del 2025.</i></p>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Riepiloga progetti o aggiornamenti con un clic</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per visualizzare più facilmente le aree di rilievo di un progetto o di un flusso di aggiornamento, sono stati aggiunti i pulsanti Riepiloga in tali aree di Workfront. Ora puoi fare clic sul pulsante per generare un riepilogo nell’Assistente AI.</p><p>In precedenza, gli utenti potevano aprire l’Assistente IA e digitare un messaggio per richiedere di creare un riepilogo del progetto o del flusso di aggiornamento.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: venerdì 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Rilascio per produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Disponibilità generale di Adobe Workfront Planning</a></p>
                    [!BADGE In Produzione ]{type=Informative}
                    <p>Workfront Planning è disponibile per tutti i clienti che hanno acquistato una licenza Workfront Planning, oltre alla licenza Workfront. Per ulteriori informazioni su Workfront Planning, contattare il rappresentante dell'account.</p>
                    <p>Per informazioni aggiornate sulla versione di Workfront Planning ogni trimestre, vedere la sezione <a href="#workfront-planning-enhancements">Miglioramenti di Workfront Planning</a> di seguito.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 28 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Assistente Adobe AI disponibile in Workfront</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per facilitare l’esecuzione del tuo lavoro, abbiamo aggiunto l’Assistente di intelligenza artificiale di Adobe a Workfront. L'Assistente all'intelligenza artificiale consente di:</p>
                    <ul>
                        <li>Riepilogando elementi di lavoro e documenti, è possibile acquisire rapidamente una conoscenza generale di attività, progetti e risorse.</li>
                        <li>Fornire informazioni dalla documentazione di Experience League, portare istruzioni e materiale di riferimento in Workfront e collegarsi a una documentazione più dettagliata.</li>
                        <li>Creazione e ottimizzazione di formule per campi modulo personalizzati calcolati, generazione di formule dai prompt di testo o individuazione di errori nelle formule esistenti.</li>
                        </ul>
                        <p>L’amministratore di Workfront può abilitare o disabilitare l’Assistente IA per la tua organizzazione. L’Assistente AI è disponibile per le istanze con piani Select, Prime e Ultimate.</p>
                    </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Rilascio in anteprima: giovedì 28 agosto 2024</p>
                        </li>
                        <li>
                            <p class="preview">Rilascio per produzione: 28 agosto 2024</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti diretti durante l’arco temporale del quarto trimestre 2024</a></p>
                    <p>Aggiornamenti minori all’aspetto di varie aree dell’applicazione Adobe Workfront vengono eseguiti nell’arco di tempo del quarto trimestre 2024. Esamina le singole note sulla versione per le date di rilascio specifiche.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: per tutto il periodo di tempo della versione di quarto trimestre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Rilascio per produzione: esamina le note sulla versione per date specifiche</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Funzionalità che verrà presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### Obsolescenza dell’esperienza Home legacy con 24.10

Con la versione 24.10, l’esperienza Home legacy diventerà ufficialmente obsoleta. Gli utenti sono invitati a iniziare a utilizzare la nuova Home, che continuerà a essere migliorata con funzioni aggiuntive prima che venga dichiarata obsoleta.

## Annunci

### Miglioramenti di Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza che esula dalla pianificazione del rilascio del quarto trimestre del 2024. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Pianificazione di Workfront

Nuove funzioni di Pianificazione di Workfront sono disponibili nell’ambiente di Produzione. Per ulteriori informazioni sulle funzioni più recenti, vedere [Attività sulla versione del quarto trimestre 2024 di Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione non sono presenti aggiornamenti di Pianificazione scenari. Quest&#39;area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

Al momento non sono presenti aggiornamenti per Workfront Proof nella versione. Quest&#39;area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non sono disponibili aggiornamenti per gli obiettivi Workfront. Quest&#39;area verrà aggiornata quando saranno disponibili aggiornamenti.

### Versione 19 dell’API

Nella versione 19 dell’API sono state modificate alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 19 dell’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API, consulta [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione apportati durante il quarto trimestre 2024, vedere [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/it/docs/workfront-known-issues/releases/current-updates).

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home).
