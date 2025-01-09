---
title: Panoramica sulla versione del primo trimestre 2025
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del primo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 11b25decc88146568aad615eb06ef3521f7aa761
workflow-type: tm+mt
source-wordcount: '2527'
ht-degree: 0%

---

# Panoramica sulla versione del primo trimestre 2025

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del primo trimestre 2025. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

<span class="preview">Le funzioni fuori ciclo (quelle rilasciate in produzione prima della data di rilascio del primo trimestre 2025) sono evidenziate in giallo.</span>

>[!IMPORTANT]
>
>La versione 23.3 includeva l’opzione per spostare l’organizzazione alle versioni mensili. Pertanto, Workfront ha modificato lo schema di numerazione delle versioni per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l’anno e il secondo il mese del rilascio. Esempio: la versione di aprile 2025 è la 25.4.
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>24.11 (14 novembre 2024)</li><li>24.12 (12 dicembre 2024)</li><li>25.1 (15 gennaio 2025)</li></ul> | <ul><li>25.1 (16 gennaio 2025)</li></ul> |
>
>Tieni presente che per il rilascio finale di ogni trimestre (25.1 questo trimestre), gli utenti che seguono la pianificazione del rilascio rapido riceveranno il rilascio con un giorno di anticipo.
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alle schede madri](#boards-enhancements)
* [Miglioramenti alla gestione dei documenti](#document-management-enhancements)
* [Miglioramenti delle priorità](#priorities-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti delle bozze](#proofing-enhancements)
* [Miglioramenti di Report e Dashboard](#report-and-dashboard-enhancements)
* [Miglioramenti al flusso di aggiornamento](#update-stream-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Confrontare gli oggetti tra ambienti diversi per la promozione dell’ambiente</a></p>
            <p>Per determinare più facilmente quale oggetto deve essere incluso in un pacchetto di promozione dell’ambiente, è stata aggiunta la possibilità di confrontare oggetti tra ambienti diversi. È quindi possibile aggiungere oggetti a un pacchetto direttamente da questo confronto.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 6 gennaio 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Altri oggetti disponibili per la promozione dell’ambiente</a></p>
            <p>Per espandere le funzionalità di promozione dell’ambiente, sono stati aggiunti altri oggetti.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 6 gennaio 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (gennaio 2025)</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Impedisci lo spostamento di attività quando sono presenti ore registrate</a></p>
            <p>Poiché lo spostamento di attività o problemi che hanno registrato ore può talvolta causare problemi di conformità o di controllo, nell’area Preferenze attività e problemi di Configura è stata aggiunta una preferenza che consente di impedire agli utenti di spostare attività e problemi se sono presenti ore registrate.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Preferenza per l'utilizzo della pianificazione del progetto o dell'utente per le attività a assegnazione singola</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>In qualità di amministratore di sistema o di gruppo, è ora disponibile una nuova preferenza per indicare se Workfront deve utilizzare la pianificazione del progetto o quella dell'utente per calcolare la sequenza temporale del progetto quando si assegna un utente a un'attività e sia il progetto che l'utente sono associati a una pianificazione.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 21 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Le regole business ora supportano i collegamenti ipertestuali</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>È ora possibile includere collegamenti ipertestuali nel messaggio di errore personalizzato di una regola business, per guidare l’utente nella modifica della propria azione all’interno del vincolo della regola. L’URL statico potrebbe contenere un collegamento alla documentazione o ad altre pagine utili per l’utente.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 21 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            È ora disponibile il filtro per i campi nativi typeahead</a></p>
            <p>Quando si aggiunge un riferimento a un campo nativo in un modulo personalizzato che fa riferimento a un campo typeahead, ad esempio Portfolio, Società o Proprietario, è ora disponibile un'opzione di filtro. Il filtro consente di limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. Questo filtro personalizzato funziona come un filtro in un campo typeahead personalizzato, utilizzando la modalità testo per definire il filtro.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 21 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Icona "Sposta in" aggiunta ai campi personalizzati</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>Quando un modulo personalizzato contiene più sezioni con molti campi, può essere difficile spostare un campo da una sezione all’altra trascinandolo. A ciascun campo è stata aggiunta l’icona "sposta in", che consente di selezionare la sezione in cui inserire il campo.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 29 ottobre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Miglioramenti alle schede madri

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Cambia il proprietario di una bacheca</a></p>
            <p>Per impostazione predefinita, il proprietario è il creatore di una bacheca. Il proprietario della bacheca è l’unica persona che può eliminarla o aggiornarne i filtri nel pannello Configura.</p>
            <p>È stata aggiunta la funzionalità per consentire agli amministratori di sistema di Workfront di cambiare il proprietario di una bacheca. L’attuale proprietario di una bacheca può anche cambiare il proprietario di quella specifica bacheca. Questa funzionalità è disponibile su schede di base, retrospettive e Kanban, ma non su schede dinamiche.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 18 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
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
    <tr>
        <td>
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modificare più documenti contemporaneamente</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>È ora possibile modificare più documenti contemporaneamente. Puoi modificare le descrizioni e aggiornare i moduli personalizzati.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 21 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nuovo stato Ritirato disponibile per le approvazioni delle versioni dei documenti</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>Quando si aggiunge una nuova versione a un documento con approvazioni in sospeso, l’approvazione per la versione precedente viene ora visualizzata come "Ritirata", a indicare che il processo di approvazione preventiva è stato chiuso a causa dell’aggiunta della nuova versione.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 7 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
            <p><i>Questa funzione fa parte di un rilascio graduale ed è disponibile solo per clienti specifici.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Miglioramenti delle priorità

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Utilizzare i filtri avanzati per trovare il lavoro in Priorità</a></p>
            <p>Utilizza il linguaggio naturale per filtrare rapidamente il lavoro nell’elenco Priorità. Puoi digitare: </p>
            <ul>
                <li>Mostra attività in ritardo</li>
                <li>Mostra attività in scadenza questa settimana</li>
                <li>Mostra priorità principali</li>
            </ul>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 9 gennaio 2025</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Recuperare il lavoro in Priorità</a></p>
            <p>Puoi utilizzare Recupera per contribuire a ridurre il tempo necessario per cercare informazioni sui progetti attivi.</p>
            <p>Con l’Assistente AI di Workfront, Catch me up riassume gli aggiornamenti, i documenti caricati e altre modifiche di rilievo sui progetti entro i seguenti intervalli di tempo: 24 ore, 3 giorni o 7 giorni.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 20 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Visualizza le modifiche in tempo reale nella pagina Dettagli in Priorità</a></p>
            <p>Ora puoi visualizzare gli aggiornamenti in tempo reale nella pagina Dettagli di un’attività o di un problema. Puoi anche verificare se altri utenti visualizzano la pagina contemporaneamente a te con gli indicatori di presenza in tempo reale.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Caricare e visualizzare documenti e bozze in Priorità</a></p>
            <p>È ora possibile interagire con i documenti e le bozze per le attività e i problemi nell’elenco lavori e nel calendario. Nella nuova scheda Documenti, è possibile:</p>
            <ul>
                <li>Caricare un documento</li>
                <li>Creare una bozza</li>
                <li>Avvia il visualizzatore di bozze</li>
                <li>E altro ancora</li>
            </ul>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            La vista Calendario è ora disponibile in Priorità</a></p>
            <p>Puoi tenere traccia del tuo lavoro con un calendario mensile chiaro e visivo. Con il calendario Priorità è possibile:</p>
            <ul>
                <li>Utilizzare i filtri per trovare il lavoro</li>
                <li>Applicare campi personalizzati come stato e livello di attivazione per identificare il lavoro ad alta priorità</li>
                <li>Applicazione dei colori per un'organizzazione rapida</li>
                <li>E altro ancora</li>
            </ul>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamenti all’elenco delle priorità</a></p>
            <p>Abbiamo aggiornato l’elenco delle priorità per migliorarne le funzionalità e allinearlo ad altre aree dell’applicazione.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 12 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Da Priorità accedi alla pagina Dettagli di un progetto</a></p>
            <p>Ora è possibile passare direttamente a un progetto in Workfront dall’elenco delle priorità.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 5 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Opzioni aggiornate nella colonna Il mio focus in Priorità</a></p>
            [!BADGE In produzione ]{type=Informative}
            <p>Sono state aggiornate le opzioni nella colonna Il mio focus per consentire di definire le priorità e ordinare il lavoro in modo più intuitivo. Le nuove etichette includono</p>
            <ul>
                <li>Urgente</li>
                <li>Alta</li>
                <li>Normal</li>
                <li>Basso</li>
            </ul>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 14 novembre 2024</li>
                <li><span class="preview">Versione di produzione per tutti i clienti: 14 novembre 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Visualizzare i dettagli del progetto in Priorità</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>È ora possibile visualizzare i dettagli e i commenti del progetto dall’elenco di lavoro in Priorità.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 6 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
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
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Assegnazioni più rilevanti rimosse da Anteprima e Produzione per ambienti a rilascio rapido</a></p>
            <p>È stata rimossa una funzionalità presente nell’ambiente di anteprima da dicembre 2023 e nell’ambiente di produzione a rilascio rapido da marzo 2024. Le funzioni hanno aggiunto suggerimenti di assegnazione intelligente più rilevanti durante l’assegnazione delle attività.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
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
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nuova estensione del browser per la revisione interattiva disponibile in versione beta</a></p>
            [!BADGE In produzione ]{type=Informative}
            <p>Stiamo introducendo una nuova estensione del browser, lo strumento di revisione Adobe Workfront, per sostituire l’estensione del browser legacy per la revisione di contenuti ZIP interattivi. Il nuovo strumento di revisione di Adobe Workfront supporta la revisione dei contenuti ZIP in tutti i browser più diffusi.</p>
            <p>L’estensione legacy del browser verrà rimossa il 28 febbraio 2025.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 7 novembre 2024</li>
                <li><span class="preview">Versione di produzione per tutti i clienti: 7 novembre 2024</span></li>
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
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Limite di 25 rapporti, pagine esterne o calendari nei dashboard</a></p>
            <p>Per mantenere le prestazioni della dashboard, è stato implementato un limite al numero totale di report, pagine esterne o calendari che è possibile inserire in una dashboard. Durante la creazione di un nuovo dashboard, è possibile aggiungere un massimo di 25 elementi.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 16 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Pulsante per la creazione del primo account lettore per Data Connect</a></p>
            [!BADGE In produzione ]{type=Informative}
            <p>Agli amministratori che accedono a Data Connect per la prima volta viene ora offerta l’opzione di creare un nuovo account lettore di Snowflake facendo clic su un singolo pulsante. Il completamento del processo richiede alcuni minuti, ma non richiede ulteriori azioni.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 14 novembre 2024</li>
                <li><span class="preview">Versione di produzione per tutti i clienti: 14 novembre 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Miglioramenti al flusso di aggiornamento

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funzionalità</span></p>
        </td>
        <td>
            <p><span class="bold">Date di rilascio</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Esperienza di commento aggiornata nel widget Menzioni in Home e My Updates (I miei aggiornamenti)</a></p>
            <p>Stiamo aggiornando l’esperienza di aggiunta di commenti nel widget Menzioni in Home e nella sezione Menzioni nell’area I miei aggiornamenti. Ora, la stessa esperienza nell’area Aggiornamenti della maggior parte degli oggetti Workfront è disponibile anche nel widget Menzioni e nella sezione Menzioni di My Updates.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 19 dicembre 2024</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamento della modalità di gestione delle risorse spostate o eliminate nelle cartelle collegate</a></p>
            [!BADGE In produzione ]{type=Informative}
            <p>Abbiamo modificato il modo in cui vengono gestite le risorse spostate ed eliminate quando si utilizza l’integrazione Adobe Workfront con Experience Manager Assets e gli Assets Essentials:</p>
            <ul>
                <li>Risorse eliminate: quando una risorsa viene eliminata all’interno di una cartella collegata in Assets o in Assets Essentials, la risorsa eliminata viene mantenuta nell’area Documenti progetto.</li>
                <li>Risorse spostate: quando una risorsa viene spostata all’esterno di una cartella collegata in Assets o Assets Essentials, la risorsa spostata viene mantenuta nell’area Documenti progetti.</li>
            </ul>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 21 novembre 2024</li>
                <li><span class="preview">Versione di produzione per tutti i clienti: 5 dicembre 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Le sezioni all’interno di un modulo personalizzato ora sono comprimibili ed espandibili</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>Quando un modulo personalizzato con più sezioni viene allegato a un oggetto, è ora possibile comprimere ed espandere tutte le sezioni, ad eccezione della sezione predefinita nella parte superiore del modulo. L’amministratore può visualizzare questa funzionalità anche durante l’anteprima del modulo nel progettista del modulo.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 11 novembre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            L’Assistente AI ora può lavorare con progetti, attività e problemi</a></p>
            [!BADGE In produzione per rilascio rapido ]{type=Positive}
            <p>Per semplificare la gestione degli elementi di lavoro in Workfront, abbiamo aggiornato l’Assistente IA per lavorare con progetti, attività e problemi. Ora l’Assistente AI può individuare progetti, attività e problemi in base ai criteri specificati.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: 31 ottobre 2024</li>
                <li>Produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024)</li>
                <li>Versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Aggiornamenti look-and-feel durante l’arco temporale del primo trimestre 2025</a></p>
            <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale del primo trimestre 2025. Consulta le singole note sulla versione per specifiche date di rilascio.</p>
        </td>
        <td>
            <p><b>Disponibile in queste date:</b></p>
            <ul>
                <li>Versione di anteprima: nell’arco temporale di rilascio del primo trimestre 2025</li>
                <li><span class="preview">Versione di produzione: consulta le note sulla versione per date specifiche</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Notifiche

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza che esula dalla pianificazione del rilascio del primo trimestre 2025. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Miglioramenti di Workfront Planning

Le nuove funzioni di Workfront Planning sono disponibili in Produzione. Per ulteriori informazioni sulle funzioni più recenti, vedere [Attività sulla versione di Adobe Workfront Planning First Quarter 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

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

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del primo trimestre 2025, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina Tutorials di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
