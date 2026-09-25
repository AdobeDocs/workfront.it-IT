---
product-area: documents
navigation-topic: approvals
title: Passa dalle approvazioni di documenti legacy alle approvazioni unificate
description: Informazioni sui flussi di lavoro di approvazione dei documenti esistenti quando l'organizzazione passa a una versione di Workfront che supporta le approvazioni unificate.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%
---
# Passa dalle approvazioni di documenti legacy alle approvazioni unificate

Il passaggio a una versione di Workfront che supporta l’archiviazione cloud di Adobe comporta anche lo spostamento dell’organizzazione dalle approvazioni di documenti legacy alle approvazioni unificate. Questo articolo fornisce informazioni sulle funzionalità che saranno disponibili in Approvazioni unificate e consigli per gli amministratori di Workfront che spostano gli utenti dalle approvazioni dei documenti legacy.


>[!IMPORTANT]
>
>Questa modifica si applica a livello di organizzazione non appena si passa a una versione di Workfront che supporta l’archiviazione cloud di Adobe. Non esiste alcun gruppo pilota o opzione di rollout graduale per il passaggio dalle approvazioni di documenti legacy alle approvazioni unificate.<br>
>Per informazioni dettagliate sulle modifiche apportate all&#39;archiviazione cloud Adobe, vedere [Sposta su Workfront nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Informazioni sulle modifiche da approvazioni di documenti legacy ad approvazioni unificate

|  | Approvazioni documenti legacy | Approvazioni unificate |
| --- | --- | --- |
| Approvatori e revisori | Approvazione solo da parte di singoli utenti | Approvazione o revisione da parte di singoli utenti o team |
| Scadenze e promemoria | Nessun promemoria automatico | Promemoria automatizzati 72 ore di uscita, 24 ore di uscita e alla data di scadenza |
| Fasi e percorsi di approvazione | Una fase di approvazione, nessun percorso parallelo | [Più fasi di approvazione e percorsi di revisione paralleli](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Modelli di approvazione | Ogni approvazione configurata da zero | [Modelli riutilizzabili](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponibili in Installazione di Workfront |
| Revisione e markup | Visualizzatore bozze | [Visualizzatore bozze](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) sugli oggetti di archiviazione Workfront legacy o [Visualizzatore Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) sugli oggetti di archiviazione cloud Adobe |
| Revisione assistita da IA | Non disponibile | Controlli automatici di conformità al brand con [IA Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Generazione dei rapporti | Reportistica legacy | Widget per KPI predefinito e [Dashboard canvas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### Cosa succederà alle approvazioni già in corso

Le approvazioni in-flight create nelle approvazioni di documenti legacy continueranno a funzionare come prima dell&#39;aggiornamento. Tuttavia, tutte le nuove approvazioni create dopo l’aggiornamento utilizzeranno le approvazioni unificate.


## Prepararsi per l’aggiornamento

* Condividi l&#39;articolo [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) con gli utenti finali.
* Esamina gli scenari di Workfront Fusion esistenti. Se utilizzi le approvazioni dei documenti legacy con la verifica, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) prima degli aggiornamenti dell&#39;organizzazione.
* Imposta una dashboard di revisione e approvazione nei dashboard di Canvas per sostituire eventuali rapporti di approvazione legacy. Per ulteriori dettagli, vedere [Creare un dashboard di revisione e approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).


### Articoli della Guida per gli utenti finali

* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Funzionalità disponibile per le approvazioni dei documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Revisione e approvazione con il visualizzatore Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Utilizzare insieme approvazioni unificate e bozze](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Panoramica sullo stato delle decisioni relative ai documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Guida introduttiva a Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)