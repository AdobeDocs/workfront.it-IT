---
title: Panoramica dell’Assistente di Adobe Workfront Planning AI
description: È possibile utilizzare l’assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina e alla struttura dei record correnti. I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 98ba6e1c1624639ba45ccf2cc3fd8e29bc716f89
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Panoramica dell’Assistente di Adobe Workfront Planning AI

<!-- update metadata above at GA-->

>[!IMPORTANT]
>
><span class="preview">L&#39;Assistente AI è stato temporaneamente rimosso e tornerà in un secondo momento.</span>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning e Workfront AI Assistant (beta), ovvero nuove offerte di Adobe Workfront.
>
>Attualmente, Workfront Planning è in una fase di accesso iniziale e Workfront AI Assistant è in una fase beta.
>
>Workfront Planning e l’Assistente IA (beta) sono aperti a un numero limitato di clienti.
>
>Per utilizzare queste funzionalità è necessario essere clienti di Workfront.
>
>Il rappresentante del tuo account ti informerà se partecipi a questa fase.
>
>Per ulteriori informazioni, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

È possibile utilizzare l&#39;Assistente AI per generare, aggiornare o rimuovere record in base al contesto della pagina corrente e alla struttura dei record.

I comandi dell’utente e l’esecuzione di tali comandi da parte dell’IA collaborano per garantire che le modifiche apportate dall’IA vengano riflesse accuratamente nell’ambiente.

## Considerazioni sull’Assistente AI

* Per impostazione predefinita, l’Assistente AI è disponibile per l’amministratore principale di Workfront. Per informazioni, vedere [Configurare le informazioni di base per il sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

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

## Accedere all’Assistente AI

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
