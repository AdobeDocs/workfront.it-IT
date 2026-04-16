---
product-area: documents
navigation-topic: approvals
title: Introduzione a Workfront Content Reviewer
description: Utilizza Workfront Content Reviewer AI Collaborator per valutare i contenuti rispetto alle linee guida del brand durante i flussi di lavoro di revisione e approvazione.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Introduzione a Workfront Content Reviewer

Il revisore dei contenuti è un collaboratore AI, un tipo di agente AI che può essere aggiunto ai tuoi progetti, attività e documenti. I collaboratori IA possono essere configurati nell’area Configurazione e assegnati proprio come gli utenti.

In Workfront, Content Reviewer aiuta ad accelerare i contenuti e a migliorare la conformità al brand durante il processo di revisione e approvazione. Puoi aggiungere i revisori del contenuto ai modelli di approvazione o includerli in singole richieste di revisione e approvazione.

## Requisiti di accesso

Per impostare i revisori dei contenuti in Workfront, devi essere un amministratore di sistema.

Qualsiasi utente può aggiungere il revisore dei contenuti a una richiesta di revisione e approvazione.

## Requisiti

* L&#39;istanza di Workfront deve avere le approvazioni unificate abilitate.
* La tua organizzazione deve disporre di GenStudio Foundation.
   * Il Visualizzatore contenuti di Workfront fornisce le funzionalità disponibili in GenStudio Foundation per i flussi di lavoro di revisione e approvazione delle risorse. Non è necessario accedere direttamente a GenStudio Foundation per completare il lavoro. L’accesso alle funzionalità di GenStudio Foundation tramite Content Reviewer rientra nei termini del contratto Workfront.
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file.
Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Tipi di file supportati {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Tipo di file non supportato"
>abstract="Questo revisore contenuto non supporta il tipo di file selezionato. Carica un tipo di file supportato o rimuovi il revisore dei contenuti per inviare la richiesta."

Il revisore dei contenuti può esaminare i seguenti tipi di file:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF non animato (.gif)
* PDF (.pdf)
* PPT (ppt, pptx)
* DOC (.doc, .docx)

Se carichi un tipo di file non supportato, l’opzione Revisore contenuto non sarà disponibile durante la creazione di un flusso di lavoro di approvazione.

## Impostare le linee guida per il marchio

Il revisore dei contenuti di Workfront utilizza le linee guida del brand durante la revisione dei contenuti. Gli amministratori di Workfront possono impostare le linee guida per il marchio nell’area Configurazione di Workfront. I brand creati in GenStudio Foundation sono disponibili anche in Workfront.

Per impostare le linee guida per il marchio, gli amministratori di sistema devono:

1. [Concedere l’accesso alle autorizzazioni del brand](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Crea e gestisci i brand per il revisore dei contenuti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Crea revisori contenuto

Una volta configurato almeno un marchio, gli amministratori di Workfront possono iniziare a creare i revisori dei contenuti nell’area Configurazione. Puoi creare più revisori dei contenuti incentrati su linee guida diverse:

* **Immagine**: questo revisore dei contenuti esaminerà la risorsa in base alle linee guida per il marchio delle immagini impostate in Workfront. [!BADGE Beta]{type=Positive tooltip="Questa funzione è attualmente in versione beta."}
   * Per abilitare questa funzione, gli amministratori di sistema devono firmare il contratto beta.
* **Voce marchio**: il revisore dei contenuti esaminerà la risorsa in base alle linee guida per la voce marchio impostate in Workfront.

I revisori dei contenuti possono quindi essere assegnati a modelli di approvazione e a singole richieste di revisione e approvazione.

Per ulteriori informazioni, vedere [Configurare i collaboratori IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Aggiungi revisori di contenuti per rivedere e approvare le richieste

Gli utenti possono aggiungere i revisori del contenuto ai modelli di approvazione esistenti o a singole richieste di revisione e approvazione.

### Modelli di approvazione

Se nell&#39;organizzazione vengono spesso aggiunte le stesse persone alle richieste di revisione e approvazione, gli utenti con licenza Standard possono creare modelli di approvazione nell&#39;area Configurazione di Workfront.

Gli utenti possono aggiungere i revisori dei contenuti ai modelli di approvazione per verificare automaticamente la conformità del brand quando un modello viene utilizzato per creare una richiesta.

Una volta creati, i modelli di approvazione possono essere applicati alle risorse nell’area Documenti di un progetto, un’attività o un problema.

Per ulteriori informazioni, vedere [Creare un modello di workflow di approvazione per i documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![elenco di modelli che mostra i revisori AI](assets/ai-review-templates.png)

### Richiesta di revisione e approvazione individuale

Quando gli utenti creano richieste di revisione e approvazione individuali, possono aggiungere un revisore dei contenuti in con altri partecipanti oppure possono creare una singola richiesta con solo il revisore dei contenuti per verificare la conformità del brand.

Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Revisore contenuto aggiunto alla richiesta di approvazione individuale](assets/new-stage.png)

## Visualizzare il punteggio e il feedback del revisore dei contenuti

Pochi secondi dopo l&#39;invio della richiesta di revisione e approvazione con un revisore dei contenuti, il punteggio e il feedback del revisore dei contenuti sono disponibili nel pannello Riepilogo documento, anche se altri partecipanti stanno ancora esaminando e prendendo decisioni.

Anche i proprietari delle approvazioni ricevono un’e-mail di notifica del completamento di una revisione della risorsa. Nell&#39;e-mail, fai clic su **Vai a revisione** e visualizza il punteggio e il feedback in Workfront.

Il revisore dei contenuti non è progettato per essere un responsabile delle decisioni nel flusso di lavoro di revisione e approvazione. Fornisce solo un punteggio e consigli per allineare la risorsa ai requisiti del brand specificati.

Se la risorsa non soddisfa le linee guida del marchio, il creativo può caricare una nuova versione e il proprietario dell’approvazione può creare una seconda richiesta di revisione e approvazione con il revisore dei contenuti.

Per ulteriori informazioni sulla visualizzazione di punteggi e feedback, consulta [Visualizza punteggio e feedback del revisore dei contenuti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

