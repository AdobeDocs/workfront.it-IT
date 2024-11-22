---
title: Panoramica sulla versione del quarto trimestre 2024
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 8ad2ed8389fdc00649f0853e07d2e83d21ccb385
workflow-type: tm+mt
source-wordcount: '2178'
ht-degree: 0%

---

# Panoramica sulla versione del quarto trimestre 2024

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del quarto trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

<span class="preview">Le funzioni fuori ciclo (quelle rilasciate in produzione prima della data di rilascio del quarto trimestre 2024) sono evidenziate in giallo.</span>

>[!IMPORTANT]
>
>La versione 23.3 includeva l’opzione per spostare l’organizzazione alle versioni mensili. Pertanto, Workfront ha modificato lo schema di numerazione delle versioni per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l’anno e il secondo il mese del rilascio. Esempio: la versione di aprile 2024 è la 24.4.
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>24.8 (15 agosto 2024)</li><li>24.9 (12 settembre 2024)</li><li>24.10 (17 ottobre 2024)</li></ul> | <ul><li>24.10 (17 ottobre 2024)</li></ul> |
>
>Tieni presente che per la versione finale di ogni trimestre (le 24.10 di questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno la versione con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alla gestione dei documenti](#document-management-enhancements)
* [Miglioramenti Home](#home-enhancements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti delle bozze](#proofing-enhancements)
* [Miglioramenti di Report e Dashboard](#report-and-dashboard-enhancements)
* [Altri miglioramenti](#other-enhancements)
* [Funzionalità presto rimossa da Workfront](#functionality-soon-to-be-removed-from-workfront)

### Miglioramenti per gli amministratori

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Livello di accesso ora disponibile nella promozione dell'ambiente</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per espandere le funzionalità di promozione dell’ambiente, è stata aggiunta la possibilità di includere i livelli di accesso. Ora è possibile configurare un livello di accesso in un ambiente Sandbox e quindi promuovere tale livello di accesso all’ambiente di produzione.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 17 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
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
                            <p>Versione di anteprima: 1 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">L'opzione "Seleziona tutto" è ora disponibile nei modelli di layout</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per semplificare la visualizzazione e la visualizzazione dei campi con modelli di layout, è stata aggiunta una casella di controllo "Seleziona tutto" alle aree Panoramica e Finanza della visualizzazione Dettagli in un modello di layout. Questa opzione è disponibile se hai selezionato Progetto, Attività, Problema, Portfolio o Programma in "Personalizza ciò che viene visualizzato dagli utenti".</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 29 agosto 2024</p>
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
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per rendere la promozione dell’ambiente più flessibile e facile da utilizzare, è stata abilitata la funzionalità di rollback. Ora è possibile eseguire il rollback dei pacchetti entro 24 ore, consentendo di ripristinare più facilmente le configurazioni precedenti interessate da un pacchetto di promozione dell’ambiente.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 29 agosto 2024</p>
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
                            <p><s>Versione di anteprima: 12 agosto 2024</s></p>
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
>Le funzionalità elencate in **Miglioramenti alla gestione dei documenti** fanno parte di una versione graduale e sono disponibili solo per clienti specifici.

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Visualizzare lo stato delle decisioni del documento direttamente nell'elenco dei documenti</a></p>
                    <p>È ora possibile visualizzare lo stato delle decisioni di un documento direttamente nell'elenco dei documenti.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p><s>Versione di anteprima: 3 ottobre 2024</s></p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Aggiunta rapida di revisori e approvatori precedenti alle nuove versioni del documento</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>È ora possibile aggiungere rapidamente revisori e approvatori delle versioni precedenti del documento.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti Home

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Aggiornamenti al widget In attesa di approvazione nella nuova Home</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Abbiamo apportato le seguenti modifiche al widget In attesa di approvazione:</p>
                        <ul>
                            <li>Il widget è stato rinominato: il nome di questo widget è Ora Le mie approvazioni.</li>
                            <li>È stata aggiunta l’opzione Approvazioni inviate come filtro: ora puoi visualizzare le approvazioni inviate nella nuova Home con questo widget.</li>
                            <li>Scadenza: ora puoi vedere la scadenza della bozza, se ne è stata impostata una. Se non viene impostata una scadenza, per impostazione predefinita viene utilizzata la data di creazione.</li>
                        </ul>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 10 ottobre 2024</p>
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
                    [!BADGE In produzione ]{type=Informative}
                    <p>Priorities migliora l’attenzione e la produttività per aiutare i clienti a ottenere di più in meno tempo.</p>
                    <p>Con Priorities puoi usufruire di:</p>
                        <ul>
                            <li>Gestione e assegnazione di priorità alle attività quotidiane: organizza il tuo giorno o la tua settimana con una navigazione consolidata per una maggiore chiarezza.</li>
                            <li>Maggiore produttività: accedere al contesto del progetto ed eseguire le attività più rapidamente con meno clic.</li>
                            <li>Funzioni personalizzate: usufruisci di funzioni progettate in modo univoco per i proprietari delle attività.</li>
                        </ul>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Miglioramenti dell'esperienza di accesso all'integrazione di Outlook</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>L’esperienza di accesso per l’integrazione con Outlook è stata semplificata: tutti i clienti possono visualizzare lo stesso pulsante per accedere a Workfront, indipendentemente dal fatto che siano abilitati IMS. I passaggi di accesso successivi rimangono diversi per le istanze IMS e non IMS, ma la pagina iniziale è la stessa per tutti gli utenti.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 6 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 6 agosto 2024</span></p>
                        </li>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Altre assegnazioni rilevanti aggiunte al flusso di lavoro Nuova attività</a></p>
                    [!BADGE In produzione per rilascio rapido ]{type=Positive}
                    <p>È stata aggiunta la stessa funzionalità per assegnazioni intelligenti più rilevanti al campo Assegnazioni della casella Nuova attività quando si aggiunge un'attività a un progetto e in un elenco di attività di progetto.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 13 febbraio 2024</p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: da annunciare</p>
                        </li>
                    </ul>
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
                            <p>Versione di anteprima: 21 dicembre 2023</p>
                        </li>
                        <li>
                            <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: da annunciare</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti delle bozze

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correzione del problema copia/incolla per il visualizzatore di bozze per il desktop</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>È stato risolto un problema a causa del quale il contenuto viene incollato in modo errato nella sezione Aggiornamenti del Visualizzatore bozze desktop.</p>
                    <p>Nuova versione: 2.1.39</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 2 ottobre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 2 ottobre 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correzione a schermo vuoto per gli utenti Windows del Visualizzatore bozze desktop</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>È stato risolto un problema relativo alla nuova versione del Visualizzatore bozze desktop 2.1.36 a causa del quale alcuni utenti di Windows visualizzavano una schermata vuota dopo l’apertura del visualizzatore. </p>
                    <p>Nuova versione per utenti Windows: 2.1.37</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 30 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 30 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamento Chromium per il Visualizzatore bozze desktop</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Stiamo aggiornando il Visualizzatore bozze desktop per supportare Chromium 126.0.6478.127 che risolverà i problemi con gli elementi dell’interfaccia utente nelle bozze interattive.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: 29 agosto 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione per tutti i clienti: 29 agosto 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Miglioramenti di Report e Dashboard

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Connessione dati Workfront disponibile per nuovi piani</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Workfront Data Connect sarà disponibile per le organizzazioni in uno dei nuovi piani Workfront. Data Connect consente alle organizzazioni di accedere ai propri dati come data lake sicuro e scalabile, che può essere analizzato e visualizzato utilizzando strumenti di business intelligence o memorizzato esternamente. Inoltre, le organizzazioni possono utilizzare Data Connect per visualizzare analisi dei dati precedentemente non disponibili, ad esempio analisi delle tendenze basate sul tempo, mappatura delle variabili e analisi dei dati di sistema esterni in combinazione con i dati di Workfront.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                    <p><i>Disponibile solo per le organizzazioni che utilizzano uno dei nuovi piani di Adobe Workfront. Data Connect è incluso nel piano Ultimate o può essere acquistato come componente aggiuntivo ai piani Prime e Select.</i></p>
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
                            <p>Versione di anteprima: 3 ottobre 2024</p>
                        </li>
                        <li>
                            <p>Versione di produzione per tutti i clienti: con la versione 24.10 (17 ottobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Disponibilità generale di Adobe Workfront Planning</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Workfront Planning è disponibile per tutti i clienti che hanno acquistato una licenza Workfront Planning, oltre alla licenza Workfront. Per ulteriori informazioni su Workfront Planning, contattare il proprio rappresentante commerciale.</p>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Assistente di Adobe disponibile in Workfront</a></p>
                    [!BADGE In produzione ]{type=Informative}
                    <p>Per facilitare l’esecuzione del tuo lavoro, abbiamo aggiunto l’Assistente di intelligenza artificiale di Adobe a Workfront. L’Assistente AI può aiutarti:</p>
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
                            <p>Versione di anteprima: 28 agosto 2024</p>
                        </li>
                        <li>
                            <p class="preview">Versione di produzione: 28 agosto 2024</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante l’intervallo di tempo del quarto trimestre 2024</a></p>
                    <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati nell’arco temporale del quarto trimestre 2024. Consulta le singole note sulla versione per specifiche date di rilascio.</p>
                </td>
                <td><p><b>Disponibile in queste date:</b></p>
                    <ul>
                        <li>
                            <p>Versione di anteprima: nell’arco temporale di rilascio del quarto trimestre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versione di produzione: consulta le note sulla versione per date specifiche</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Funzionalità presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### Obsolescenza dell’esperienza Home legacy con 24.10

Con la versione 24.10, l’esperienza Home legacy diventerà ufficialmente obsoleta. Gli utenti sono invitati a iniziare a utilizzare la nuova Home, che continuerà a essere migliorata con funzioni aggiuntive prima che venga dichiarata obsoleta.

## Notifiche

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza che esula dalla pianificazione del rilascio del quarto trimestre del 2024. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzioni più recenti, vedere [Attività sulla versione del quarto trimestre 2024 di Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

A questo punto della versione, non ci sono aggiornamenti per Workfront Proof. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non ci sono aggiornamenti per gli Obiettivi di Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### API versione 19

Per API versione 19, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del quarto trimestre 2024, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina Tutorials di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
