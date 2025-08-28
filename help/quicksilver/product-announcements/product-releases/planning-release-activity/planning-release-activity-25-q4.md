---
content-type: release-notes
title: Attività della versione del quarto trimestre 2025 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il quarto trimestre del 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f7dcae5e6bcc8674ef37ef94282c50dc9ffe951d
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 0%

---

# Attività della versione del quarto trimestre 2025 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del quarto trimestre 2025.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nuovi limiti per i campi formula

>[!NOTE]
>
>* Anteprima: 28 agosto 2025
>* Versione rapida di produzione: 11 settembre 2025
>* Produzione per tutti i clienti: 16 ottobre 2025

Abbiamo inserito i seguenti limiti per i campi formula:

* È previsto un limite di 20 campi formula per tipo di record
* Per un&#39;espressione di formula è previsto un limite di 50.000 caratteri

Per ulteriori informazioni, vedere [Panoramica del campo Formula](/help/quicksilver/planning/fields/formula-fields.md).

## Mostra errore quando i valori della formula non possono essere risolti

>[!NOTE]
>
>* Anteprima: 28 agosto 2025
>* Versione rapida di produzione: 11 settembre 2025
>* Produzione per tutti i clienti: 16 ottobre 2025

Per indicare che si è verificato un problema durante la risoluzione di un campo formula, il campo verrà visualizzato come &quot;#ERROR!&quot; in uno dei seguenti casi:

* Quando un campo utilizzato in una formula viene eliminato.

* Quando un campo utilizzato in un campo di ricerca aggregato viene visualizzato come #ERROR!.

* Quando non è possibile visualizzare un valore di formula nel formato selezionato.

Per informazioni, vedere [Panoramica dei campi formula](/help/quicksilver/planning/fields/formula-fields.md).

## Nuove espressioni aggiunte ai campi formula in Planning

>[!NOTE]
>
>Anteprima: 7 agosto 2025
>>Produzione per tutti i clienti:August, 2025
>>[!BADGE Fuori programma]{type=Neutral}

Sono state aggiunte nuove espressioni con il seguente utilizzo ai campi formula in Workfront Planning e ai campi personalizzati calcolati in Workfront:

* **REMOVEACCENTS(string)**: rimuove i segni diacritici da tutti i caratteri accentati nella stringa di input.
* **REPLACEPATTERN (stringa, modello, stringa di sostituzione)**: sostituisce le corrispondenze del modello specificato con la stringa di sostituzione.
* **PASCAL(string)**: converte la stringa di input in PascalCase digitando la prima lettera di ogni parola e rimuovendo tutti gli spazi.

Per ulteriori informazioni, vedere [Panoramica delle espressioni di dati calcolati](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Aggiunta di pulsanti Ingrandisci e Riduci a icona alla finestra di creazione dei campi della formula

>[!NOTE]
>
>Anteprima: 31 luglio 2025
>>Produzione per tutti i clienti: 31 luglio 2025
>>[!BADGE Fuori programma]{type=Neutral}

È stato aggiunto un pulsante Ingrandisci per ingrandire il campo Formula durante la creazione o la modifica del campo in una visualizzazione della tabella record. Inoltre, nella nuova finestra ingrandita è stato aggiunto un pulsante Riduci a icona per ripristinare la casella di creazione del campo.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## La pagina Record collegati è ora disponibile nell&#39;area di anteprima di un record

>[!NOTE]
>
>* Anteprima: 31 luglio 2025
>* Versione rapida di produzione: 14 agosto 2025
>* Produzione per tutti i clienti: 16 ottobre 2025

Ora l’esperienza nella pagina dei record collegati nella casella di anteprima corrisponde a quella della pagina nella pagina intera dell’area Dettagli di un record.

Prima di questo miglioramento, era possibile visualizzare i record collegati in una pagina di record collegati solo nella pagina intera dell’area Dettagli di un record.

Per informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Creare record nella visualizzazione timeline

>[!NOTE]
>
>Anteprima: 24 luglio 2025
>>Versione rapida di produzione: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025

È ora possibile creare record nella visualizzazione timeline di un tipo di record facendo doppio clic in un punto qualsiasi della timeline.

È possibile selezionare l&#39;intervallo di date del record oppure aprire la pagina del record per modificarne tutti i dettagli.

Prima di questo miglioramento, era possibile aggiungere nuovi record solo utilizzando il pulsante Nuovo record o in linea nella vista tabella.

Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

## Opzione Aggiungi condivisione nel menu Altro di una scheda del tipo di record

>[!NOTE]
>
>Anteprima: 24 luglio 2025
>>Versione rapida di produzione: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025

È ora possibile condividere un tipo di record dal menu Altro della scheda del tipo di record nella pagina dell&#39;area di lavoro. Prima di questo miglioramento, l’opzione Condividi era disponibile solo all’interno della pagina del tipo di record.

Per informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).

## Visualizza tutte le visualizzazioni di Workfront Planning in modalità a schermo intero

>[!NOTE]
>
>Anteprima: 24 luglio 2025
>>Versione rapida di produzione: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025

È ora possibile visualizzare tutte le visualizzazioni di Workfront Planning (tabella, sequenza temporale e calendario) in modalità a schermo intero. La funzionalità di visualizzazione viene mantenuta ed è possibile modificare la visualizzazione anche a schermo intero.

Prima di questo miglioramento, questa funzionalità non esisteva.

Per informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

## Aggiungere team come approvatori nei moduli di richiesta Planning

>[!NOTE]
>
>Anteprima: 22 luglio 2025
>>Produzione per rilascio rapido: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025

Per rendere più flessibile il processo di approvazione, è stata aggiunta la possibilità di aggiungere team come approvatori nei moduli di richiesta Planning. Ora è possibile immettere e selezionare i nomi dei team quando si impostano gli approvatori. Qualsiasi membro del team può prendere una decisione, che conta come decisione di approvazione per l’intero team.

In precedenza, era possibile assegnare come approvatori solo singoli utenti.

Per ulteriori informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Nuovi campi per visualizzare le informazioni sull&#39;approvazione dei record

>[!NOTE]
>
>Anteprima: 17 luglio 2025
>>Produzione per rilascio rapido: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025

Stiamo introducendo i seguenti campi per acquisire informazioni sull’approvazione per i record creati inviando una richiesta con un’approvazione:

* Approvato da
* Data di approvazione

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Compila automaticamente i campi in base ai raggruppamenti applicati

>[!NOTE]
>
>Anteprima: 10 luglio 2025
>>Versione rapida di produzione: 14 agosto 2025
>>Produzione per tutti i clienti: 16 ottobre 2025


Ora, quando si applicano i raggruppamenti a una vista tabella, l&#39;aggiunta di un record alla tabella determina la compilazione automatica dei campi associati ai raggruppamenti a cui si aggiunge il record.

Se sono stati applicati più raggruppamenti, il sistema inserisce automaticamente i campi associati a tutti i raggruppamenti solo quando si aggiunge il record alla fine dell&#39;elenco nell&#39;ultimo criterio di raggruppamento.

Prima di questo miglioramento, era necessario aggiornare manualmente i campi associati ai raggruppamenti.

Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
