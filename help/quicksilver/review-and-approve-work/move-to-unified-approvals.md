---
product-area: documents
navigation-topic: approvals
title: Passa dalle approvazioni di documenti legacy alle approvazioni unificate
description: Informazioni sui flussi di lavoro di approvazione dei documenti esistenti quando l'organizzazione passa a una versione di Workfront che supporta le approvazioni unificate.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%
---
# Passa dalle approvazioni di documenti legacy alle approvazioni unificate

I progetti Adobe di archiviazione cloud utilizzano le approvazioni unificate per impostazione predefinita. Questo articolo descrive le funzionalità disponibili in Approvazioni unificate rispetto alle approvazioni di documenti legacy.


>[!NOTE]
>
>Approvazioni unificate è l’impostazione predefinita solo per i nuovi oggetti creati nell’archiviazione cloud di Adobe. Gli oggetti di storage Workfront legacy mantengono il servizio di approvazione corrente.<br>
>Per ulteriori informazioni, consulta [Passare a Workfront nell&#39;archivio cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Informazioni sulle modifiche da approvazioni di documenti legacy ad approvazioni unificate

|  | Approvazioni documenti legacy | Approvazioni unificate |
| --- | --- | --- |
| Approvatori e revisori | Approvazione solo da parte di singoli utenti | Approvazione o revisione da parte di singoli utenti o team |
| Scadenze e promemoria | Nessun promemoria automatico | Promemoria automatizzati 72 ore di uscita, 24 ore di uscita e alla data di scadenza |
| Fasi e percorsi di approvazione | Una fase di approvazione, nessun percorso parallelo | [Più fasi di approvazione e percorsi di revisione paralleli](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Modelli di approvazione | Ogni approvazione configurata da zero | [Modelli riutilizzabili](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponibili in Installazione di Workfront |
| Revisione e markup | Visualizzatore bozze | [Visualizzatore bozze](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) sugli oggetti di archiviazione Workfront legacy o [Visualizzatore Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) sugli oggetti di archiviazione cloud Adobe |
| Revisione assistita da IA | Non disponibile | Controlli automatici di conformità al brand con [Revisore contenuti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Generazione dei rapporti | Reportistica legacy | Widget per KPI predefinito e [Dashboard canvas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### Cosa succederà alle approvazioni già in corso

Le approvazioni in volo create nelle approvazioni di documenti legacy continuano a funzionare come in precedenza. Le nuove approvazioni sugli oggetti di archiviazione cloud di Adobe utilizzano le approvazioni unificate. Le nuove approvazioni su oggetti di archiviazione Workfront legacy mantengono il servizio di approvazione di tali oggetti già in uso.


## Prepararsi per lo spostamento

* Condividi l&#39;articolo [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) con gli utenti finali.
* Esamina gli scenari di Workfront Fusion esistenti. Se utilizzi le approvazioni dei documenti legacy con la verifica, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) prima di inserire i team nell&#39;archiviazione cloud Adobe.
* Imposta una dashboard di revisione e approvazione nei dashboard di Canvas per sostituire eventuali rapporti di approvazione legacy. Per ulteriori dettagli, vedere [Creare un dashboard di revisione e approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).


### Articoli della Guida per gli utenti finali

* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Funzionalità disponibile per le approvazioni dei documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Revisione e approvazione con il visualizzatore Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Utilizzare insieme approvazioni unificate e bozze](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Panoramica sullo stato delle decisioni relative ai documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Introduzione a Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
