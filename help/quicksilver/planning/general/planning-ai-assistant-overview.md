---
title: Panoramica dell’Assistente di Adobe Workfront Planning AI
description: È possibile utilizzare l’assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina e alla struttura dei record correnti. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a5b7683bffa6c63d7feb45e5c38404185d3f2b44
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---


# Panoramica dell’Assistente di Adobe Workfront Planning AI

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


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

* Durante la creazione, l’aggiornamento o l’eliminazione di un oggetto tramite l’Assistente IA, l’Assistente AI visualizza le azioni previste e richiede una conferma. Puoi quindi confermare o annullare le azioni.

## Funzionalità attualmente disponibile per l’Assistente IA

Attualmente, l’Assistente AI è disponibile nell’area Planning di Workfront per le seguenti pagine:

* Pagina Workspace
* Pagina tipo di record
* Pagina record

In questo momento, puoi utilizzare l’Assistente IA per eseguire le seguenti azioni:

* Cercare i record. È possibile eseguire ricerche in base alle informazioni contenute in qualsiasi campo record.
* Creare record. Dopo la creazione del record viene visualizzato un ID con un collegamento al nuovo record. Puoi specificare i campi da aggiornare durante il processo di creazione, come date o descrizione.
* Crea record basati su un documento caricato. Workfront supporta i seguenti formati di documento per l’Assistente IA:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e la maggior parte dei formati immagine
* Aggiorna i campi per i record visualizzati sullo schermo
* Elimina record
* Ripristina i record appena eliminati


## Individuare l&#39;Assistente IA in Workfront Planning

È possibile individuare l&#39;Assistente AI nelle seguenti aree di Workfront Planning:

* La barra di navigazione principale, nell’angolo superiore destro dello schermo.
* All&#39;interno dell&#39;area dei dettagli di un record, dopo aver aperto il record nell&#39;anteprima o dopo aver aperto la pagina del record.

## Accedere all’Assistente AI nell’area Pianificazione

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Dots main menu](assets/dots-main-menu.png) nell&#39;angolo superiore destro dello schermo oppure sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile.

. Fare clic su **Pianificazione**. Verrà visualizzata l&#39;area Pianificazione.

1. Fai clic su una **scheda dell&#39;area di lavoro**.

1. (Facoltativo) Fai clic su una **scheda del tipo di record**.

1. (Facoltativo) Fai clic su un **record** per aprire la pagina **Dettagli** del record.

1. Fare clic sull&#39;icona **Assistente AI** nell&#39;angolo superiore destro dello schermo nella barra di navigazione globale o nell&#39;angolo superiore destro dell&#39;anteprima o della pagina del record.

   ![Icona Assistente IA](assets/ai-assistant-icon-highlighted.png)

1. Nello spazio disponibile, inizia a digitare i comandi per l’Assistente AI, quindi al termine fai clic su Invio.

   ![Pannello Assistente IA con casella di comando vuota](assets/ai-assistant-panel-with-empty-command-box.png)

   Ad esempio, è possibile digitare uno dei seguenti elementi:

   * Crea una campagna con data di inizio 4 luglio e data di fine 30 luglio
   * Aggiorna il campo Descrizione del record Campagna estiva con data da determinare
   * Elimina l&#39;ultimo record
   * Ripristina il record

   Viene visualizzato un indicatore visivo mentre l’Assistente AI elabora i comandi, impostando le aspettative per il tempo di risposta.

   Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti o osserva le modifiche a sinistra.



