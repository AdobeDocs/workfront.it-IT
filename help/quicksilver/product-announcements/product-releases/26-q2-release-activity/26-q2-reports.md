---
title: Miglioramenti al reporting per il secondo trimestre 2026
description: Miglioramenti al reporting per il secondo trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
source-git-commit: aceb9f7bd6c62036838b15d74ee2a9b7843e5c11
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 9%

---

# Miglioramenti al reporting per il secondo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del secondo trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili in questo momento nel ciclo di rilascio del secondo trimestre 2026, consulta [Panoramica sulla versione del secondo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

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
