---
title: Panoramica dell’Assistente di Adobe Workfront Planning AI
description: È possibile utilizzare l’assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina e alla struttura dei record correnti. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---


# Panoramica dell’Assistente di Adobe Workfront Planning AI

{{planning-important-intro}}

È possibile utilizzare l&#39;Assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina corrente e alla struttura dei record.

I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.

## Considerazioni sull’Assistente AI

* L’Assistente AI deve essere abilitato per la tua organizzazione prima che sia disponibile per gli utenti della tua azienda. Per informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Dopo che Workfront ha abilitato l’Assistente AI per la tua organizzazione, questo sarà disponibile per l’amministratore Workfront principale. Per informazioni, vedere [Configurare le informazioni di base per il sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* L’amministratore di Workfront deve abilitare l’Assistente AI per tutti gli altri utenti. Per ulteriori informazioni, vedere [Attivare o disattivare l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’Assistente AI funziona nel contesto di ogni pagina. Le richieste inviate per l&#39;Assistente AI devono fare riferimento alla funzionalità disponibile nella pagina aperta.

* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Planning si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront. Per informazioni, vedere i seguenti articoli:

   * [Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dall&#39;Assistente AI per conto dell&#39;utente vengono tracciate nel pannello della cronologia del record.

* Puoi utilizzare i comandi per annullare le azioni. Ad esempio, puoi digitare &quot;Annulla ultima modifica&quot; per ripristinare la modifica.

## Funzionalità attualmente disponibile per l’Assistente IA

Attualmente, l’Assistente AI è disponibile nell’area Planning di Workfront per le seguenti pagine:

* Pagina Workspace
* Pagina tipo di record
* Pagina record

In questo momento, puoi utilizzare l’Assistente IA per eseguire le seguenti azioni:

* Cercare i record. È possibile eseguire ricerche in base alle informazioni contenute in qualsiasi campo record.
* Creare record. Dopo la creazione del record viene visualizzato un ID con un collegamento al nuovo record. Puoi specificare i campi da aggiornare durante il processo di creazione, come date o descrizione.
* Crea record basati su un documento caricato. Workfront supporta i seguenti formati di documento per l’Assistente IA:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt e la maggior parte dei formati immagine
* Aggiorna i campi per i record visualizzati sullo schermo
* Elimina record
* Ripristina i record appena eliminati

## Accedere all’Assistente AI nell’area Pianificazione

1. Accedi a Workfront, quindi vai all&#39;area **Planning**.

1. Fai clic su una **scheda dell&#39;area di lavoro**.

1. (Facoltativo) Fai clic su una **scheda del tipo di record**.

1. (Facoltativo) Fai clic su un **record** per aprire la pagina **Dettagli** del record.

1. Fare clic sull&#39;icona **Assistente AI** nell&#39;angolo superiore destro della schermata nella barra di navigazione globale.

   ![](assets/ai-assistant-icon-highlighted.png)

1. Nello spazio disponibile, inizia a digitare i comandi per l’Assistente AI, quindi al termine fai clic su Invio.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Ad esempio, è possibile digitare uno dei seguenti elementi:

   * Crea una campagna con data di inizio 4 luglio e data di fine 30 luglio
   * Aggiorna il campo Descrizione del record Campagna estiva con data da determinare
   * Elimina l&#39;ultimo record
   * Ripristina il record

   Viene visualizzato un indicatore visivo mentre l’Assistente AI elabora i comandi, impostando le aspettative per il tempo di risposta.

   Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti o osserva le modifiche a sinistra.
