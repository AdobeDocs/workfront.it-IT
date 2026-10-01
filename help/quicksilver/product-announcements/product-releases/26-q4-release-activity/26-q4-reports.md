---
title: Miglioramenti alla comunicazione del quarto trimestre 2026
description: Miglioramenti alla comunicazione del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 5%
---
# Miglioramenti alla comunicazione del quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del quarto trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Le dashboard di Canvas sono ora disponibili su Google Cloud Platform e Microsoft Azure

>[!NOTE]
>
>Anteprima: N/D
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Le istanze di Workfront su Google Cloud Platform (GCP) e Azure ora possono dare il consenso alla versione open beta delle dashboard di Canvas. Per ulteriori informazioni, vedere [Utilizzare i dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Registra un&#39;inserzione privata di Snowflake per Workfront Data Connect

>[!NOTE]
>
>Anteprima: N/D
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Ora puoi condividere i dati di Workfront Data Connect direttamente con l’account Snowflake della tua organizzazione registrando un’inserzione privata. Questo metodo di connessione utilizza la funzionalità di inserimento nell’elenco privato di Snowflake per condividere in modo sicuro i dati tra organizzazioni senza esporli pubblicamente e funziona tra aree geografiche e piattaforme di hosting.

Un’inserzione privata è utile quando desideri unire i dati di Workfront con altri dati nel data warehouse aziendale. Poiché i dati vengono memorizzati nel tuo account Snowflake, puoi eseguire query insieme agli altri dati.

Per ulteriori informazioni, vedere [Registrare un elenco privato per Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md).

## Sono ora disponibili gli strumenti MCP per la generazione di rapporti per i dashboard di Canvas

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Per semplificare l’utilizzo delle dashboard di Canvas, sono stati aggiunti degli strumenti a Workfront MCP. Ora puoi creare e gestire dashboard di Canvas tramite chat, e la dashboard e i widget vengono creati per te utilizzando i dati di Workfront. Questo funziona da client MCP come Claude e Cursor.

Sarà possibile, ad esempio:

* Crea rapporti facendo richiesta. Invece di creare manualmente un dashboard o un grafico, descrivilo nel linguaggio naturale.
* Modifica nella stessa posizione. Richiedi di rinominare un widget, modificare un filtro, cambiare un tipo di grafico o ridimensionarlo e le modifiche verranno applicate al dashboard attivo.
* Riutilizza quello che hai. Duplica un dashboard o un widget esistente come punto di partenza invece di ricompilarlo da zero.

### Funzioni supportate

**Dashboard**

* Crea un nuovo dashboard
* Elenca le tue dashboard (tue, condivise con te, tutte o preferite) e cerca per titolo
* Aprire o visualizzare la struttura di un dashboard
* Aggiorna titolo, descrizione, valuta, filtri e prompt
* Duplicare un dashboard (con o senza widget, prompt e filtri)
* Eliminare una dashboard

**Widget**

* KPI — un singolo numero aggregato (somma, media, conteggio, min, max, ecc.)
* Grafico - a barre, a colonne, a linee e a torta; supporta grafici semplici, a serie multiple e in pila
* Tabella — tabelle a più colonne con raggruppamento di righe
* Visualizzare la configurazione di un widget e aggiornarla, copiarla, ridimensionarla, riposizionarla o eliminarla

**Opzioni di reporting**

* Filtrare i dati con condizioni e gruppi AND/OR
* Raggruppa e aggrega per qualsiasi campo
* Espandere un indicatore KPI o un grafico nei record sottostanti
* Etichette di colonna personalizzate, formattazione di numero, data e valuta e stile di cella condizionale
* Richieste e filtri a livello di dashboard

Per ulteriori informazioni, vedere [Utilizzare i dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Copiare o spostare widget tra dashboard di Canvas

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Ora puoi copiare un widget nello stesso dashboard, in un altro dashboard a cui hai accesso in modifica o in un nuovo dashboard. Potete anche spostare un widget in un&#39;altra dashboard a cui potete accedere per la modifica o in una nuova dashboard.

Quando copiate un widget, ora viene visualizzata una finestra di dialogo in cui selezionate il dashboard di destinazione e se copiare o spostare il widget. In precedenza, Report Builder veniva aperto immediatamente.

## Filtrare le relazioni tra raccolte nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Quando si crea un filtro in un dashboard Area di lavoro, è ora possibile filtrare in base alle relazioni di raccolta, ovvero i campi che si collegano a un gruppo di record correlati anziché a un singolo record. Ad esempio, puoi filtrare in base allo stato delle attività appartenenti a un progetto per visualizzare un elenco di progetti con attività nello stato &quot;Nuovo&quot;.

In precedenza, per filtrare in base alle relazioni tra raccolte era necessaria la modalità testo.

Per ulteriori informazioni, vedere [Riferimento filtro report per dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

## Copiare dashboard in dashboard di Canvas

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile copiare un dashboard Canvas utilizzando la nuova azione **Copia dashboard**. Questa azione è disponibile per tutti gli utenti il cui livello di accesso consente di modificare o creare i diritti per i dashboard, anche se dispongono solo dell’accesso di visualizzazione al dashboard specifico da copiare. Gli utenti che non dispongono dei diritti di modifica o creazione per i dashboard non visualizzano questa azione.

Quando copiate un dashboard, potete rinominarlo, aggiornarne la descrizione e la valuta e scegliere quali widget, filtri del dashboard e prompt del dashboard trasferire nella copia.

Le configurazioni di Esegui come utente sui widget vengono mantenute solo se si è l&#39;utente designato o un amministratore di sistema. Le preferenze di condivisione non vengono copiate nel nuovo dashboard e, una volta completata la copia, viene visualizzato un messaggio di conferma con un collegamento al nuovo dashboard.

In precedenza, non era possibile copiare un dashboard: gli utenti dovevano ricreare i dashboard da zero per creare varianti specifiche per il pubblico.

## Campo Tipo di approvazione nei dashboard di Canvas

>[!NOTE]
>
>Produzione per tutti: 28 agosto 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

L&#39;entità Approvazione ora include un campo **Tipo di approvazione** che consente agli utenti di distinguere tra approvazioni di bozze, approvazioni di versioni di documenti, approvazioni di assunzioni e altri tipi di approvazione.

## Aggiornamento della terminologia di approvazione nei dashboard di Canvas

>[!NOTE]
>
>Produzione per tutti: 28 agosto 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

I seguenti nomi di campo utilizzati nei dashboard di Canvas per le approvazioni di documenti e lavori sono stati rinominati per maggiore chiarezza:

| Nome precedente | Nuovo nome |
| --- | --- |
| Approvazione documento | Approvazione |
| Fase di approvazione documento | Fase di approvazione |
| Partecipante alla fase di approvazione documento | Fase di approvazione del partecipante |
| Processo di approvazione | Processo di approvazione del lavoro |
| Fase di approvazione | Fase di approvazione lavoro |
| Stato approvatore | Stato approvatore lavoro |
| In attesa di approvazione | In attesa di approvazione del lavoro |

Questa modifica non influisce sul funzionamento dei rapporti correnti.

## Rapporti di tabella pivot nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 27 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Il nuovo tipo di rapporto per tabella pivot nei dashboard di Canvas aggrega i dati con aggregazioni dati precise e complete. Puoi creare metriche quali conteggi, somme e medie direttamente sul dashboard, quindi eseguire il drill-through nei record sottostanti dietro qualsiasi totale.

Per ulteriori informazioni, vedere [Creare un report di tabella pivot in un dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Applicazione delle date di fine per i rapporti pianificati

>[!NOTE]
>
>Anteprima: 13 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

I rapporti pianificati ora richiedono una data di fine per impedire la consegna indefinita. Le pianificazioni che superano la data di fine vengono disattivate automaticamente.

Le pianificazioni esistenti sono state aggiornate con le date di fine per migliorare l’affidabilità e ridurre l’utilizzo non necessario del sistema. Workfront offre inoltre visibilità e avvisi aggiuntivi per aiutarti a gestire i cicli di vita della pianificazione dei rapporti in vista della data di fine.

Per ulteriori informazioni, consulta [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## I campi di riferimento nativi sono disponibili per gli elenchi e i report

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile aggiungere campi di riferimento nativi a elenchi e rapporti in Workfront.

Un campo di riferimento nativo è un campo personalizzato. Quando il campo si trova in un modulo personalizzato allegato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, se il campo fa riferimento al campo Descrizione e si trova in un modulo personalizzato allegato a un progetto, estrae la descrizione del progetto. Il campo può mostrare “N/D” se non sono disponibili dati.

Per informazioni sulla creazione di campi di riferimento nativi, incluso l&#39;elenco dei campi nativi supportati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Per informazioni sull&#39;aggiunta di campi ai report, vedere [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordinamento coerente dei valori dei campi a selezione multipla negli elenchi e nei rapporti legacy

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Le opzioni selezionate per i campi personalizzati a selezione multipla vengono ora visualizzate in un ordine coerente e prevedibile negli elenchi e nei rapporti precedenti. L’ordine dei campi è determinato dalla disposizione dei campi nel modulo personalizzato.

![L&#39;ordine dei campi modulo personalizzato corrisponde all&#39;ordine dei valori selezionati in un elenco o report](assets/new-field-order-multi-select.png)

In precedenza, le opzioni selezionate venivano visualizzate nell’ordine in cui erano state scelte o in un ordine incoerente, rendendo più difficile la scansione e il confronto delle righe.

Nota: il nuovo ordinamento non è applicabile se il campo utilizza la modalità testo.
