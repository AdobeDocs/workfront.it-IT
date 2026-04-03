---
title: Miglioramenti al reporting per il secondo trimestre 2026
description: Miglioramenti al reporting per il secondo trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 1a37ff7e4e4b60ac23b0edde6b60258ed508e90b
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 8%

---

# Miglioramenti al reporting per il secondo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del secondo trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili in questo momento nel ciclo di rilascio del secondo trimestre 2026, consulta [Panoramica sulla versione del secondo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## La Distribuzione Pianificata Dei Rapporti Ora Supporta Le E-Mail Basate Su Collegamenti

>[!NOTE]
>
>Anteprima: 3 aprile 2026
>Rilascio rapido in produzione: giovedì 15 aprile 2026
>Produzione per tutti: venerdì 16 aprile 2026

Workfront ora include un nuovo tipo di consegna Collegamento per i rapporti pianificati. Invece di generare e allegare un file, questa opzione invia un’e-mail contenente un collegamento diretto al rapporto in Workfront, consentendo ai destinatari di visualizzare i dati più recenti nell’applicazione.

L’opzione Collegamento è ora il tipo di consegna predefinito per le nuove regole di consegna dei rapporti pianificate, mentre rimangono disponibili i formati basati su file esistenti (HTML, PDF, Excel e TSV).

Con questa modifica, abbiamo anche aggiornato l’aspetto dell’e-mail di consegna del rapporto.

Per ulteriori informazioni, consulta [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Eseguire rapporti come utente specifico nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 2 aprile 2026
>Rilascio rapido in produzione: giovedì 15 aprile 2026
>Produzione per tutti: venerdì 16 aprile 2026
>
>Canvas Dashboards è attualmente in versione beta.

Ora puoi configurare i rapporti sulle dashboard di Canvas in modo che vengano eseguiti come utente specifico. Quando è abilitato, il rapporto mostra i dati in base all’accesso dell’utente selezionato, anziché alle autorizzazioni del visualizzatore.

Ciò garantisce dati più coerenti e affidabili tra i visualizzatori del dashboard, anche quando l’accesso alle aree di lavoro di Planning, ai tipi di record o alle impostazioni di autorizzazione è diverso.

Per ulteriori informazioni, vedere [Generare un report KPI in un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Creare un report grafico in un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) o [Creare un report tabella in un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## Nuove opzioni di autenticazione per la connessione dati

>[!NOTE]
>
>Anteprima: 12 marzo 2026
>Rilascio rapido in produzione: venerdì 12 marzo 2026
>Produzione per tutti: venerdì 16 aprile 2026

È ora possibile eseguire l&#39;autenticazione a Data Connect utilizzando le chiavi RSA o le connessioni PAT (Programmatic Access Tokens), aggiungendo alternative più sicure e flessibili alle credenziali tradizionali di nome utente/password.

Queste nuove opzioni consentono alle organizzazioni di mantenere connessioni stabili da Power BI, Tableau e altri strumenti di BI di terze parti senza affidarsi a metodi di accesso basati sugli utenti.

>[!IMPORTANT]
>
>A giugno 2026, le credenziali nome utente/password saranno necessarie per utilizzare l’autenticazione a più fattori (MFA). È consigliabile passare all’autenticazione basata su RSA o PAT per gli account utente dei servizi utilizzati per caricare i dati da Data Connect in strumenti di visualizzazione di terze parti, processori di dati e script che non funzionano con MFA nel processo di autenticazione.

## Etichette di campi personalizzati visualizzate durante la creazione dei rapporti

>[!NOTE]
>
>Anteprima: 26 febbraio 2026
>Rilascio rapido in produzione: venerdì 12 marzo 2026
>Produzione per tutti: venerdì 16 aprile 2026

L’etichetta del campo personalizzato viene ora visualizzata prima del nome del campo e dell’oggetto negli strumenti di creazione dei rapporti, facilitando l’individuazione dei campi. Le etichette dei campi vengono visualizzate anche quando si definiscono filtri, visualizzazioni e raggruppamenti negli elenchi.

L’etichetta del campo personalizzato è destinata all’interfaccia di sistema, mentre il nome del campo viene spesso utilizzato a scopo di archiviazione API e back-end e potrebbe non essere altrettanto utile quando si individua un campo.

Per ulteriori informazioni, vedere [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Cartelle report condivisibili

>[!NOTE]
>
>Anteprima: 26 febbraio 2026
>Rilascio rapido in produzione: venerdì 12 marzo 2026
>Produzione per tutti: venerdì 16 aprile 2026

Ora puoi organizzare e condividere i rapporti utilizzando cartelle di rapporti condivisibili. Questa nuova funzione consente ai team che gestiscono grandi volumi di rapporti di mantenere un controllo degli accessi scalabile e coerente:

* **Creare strutture di cartelle organizzate**: gli amministratori di sistema possono creare cartelle di primo livello e gli utenti con accesso di gestione possono creare sottocartelle fino a 4 livelli di profondità.
* **Controlli delle autorizzazioni granulari**: condividere cartelle con due livelli di autorizzazione:
   * Visualizza: gli utenti possono aprire rapporti e condividere cartelle
   * Gestisci: gli utenti possono modificare i dettagli della cartella, aggiungere/rimuovere elementi e ricevere automaticamente l’accesso di gestione a tutti i rapporti all’interno della cartella
* **Autorizzazioni ereditate**: le autorizzazioni si sovrappongono dalle cartelle principali a tutte le sottocartelle e ai report nella struttura delle cartelle
* **Esperienza elenco avanzata**: quando abiliti le cartelle condivisibili, avrai accesso all&#39;esperienza elenco avanzata. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Per ulteriori informazioni, vedere [Utilizzare cartelle condivisibili](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Sono state migliorate le etichette di data per i raggruppamenti di grafici nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 26 febbraio 2026
>Rilascio rapido in produzione: venerdì 12 marzo 2026
>Produzione per tutti: venerdì 16 aprile 2026

>[!NOTE]
>
>Canvas Dashboards è attualmente in versione beta.

I grafici che raggruppano i dati per data ora presentano etichette di data più chiare e leggibili. Con questo aggiornamento, le etichette delle date vengono regolate in modo dinamico in base all’opzione Raggruppa per selezionata, ad esempio giorno, settimana, mese o anno, semplificando la lettura e l’interpretazione dei grafici:

<table> <tbody> <tr> <td>Day</td> <td>Visualizza la data completa. Esempio: 3/12/2026</td> </tr> <tr> <td>Settimana</td> <td>Visualizza una data di inizio settimana formattata. Esempio, 8 marzo 2026</td> </tr> <tr> <td>Month</td> <td>Visualizza il mese e l'anno. Esempio Mar 2026</td> </tr> <tr> <td>Year</td> <td>Visualizza solo l'anno. Esempio: 2026</td> </tr> </tbody> </table>

In precedenza, i raggruppamenti di grafici mostravano sempre la data di inizio del periodo selezionato in formato numerico.
