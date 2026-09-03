---
title: Miglioramenti ai documenti del quarto trimestre 2026
description: Miglioramenti ai documenti del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---

# Miglioramenti ai documenti del quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del quarto trimestre 2026. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## Accesso diretto alle bozze dai collegamenti e-mail per l’approvazione

>[!NOTE]
>
>Anteprima: N/D
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Quando a un documento è allegata una bozza, il collegamento &quot;Vai alla revisione&quot; nelle e-mail di approvazione ora apre direttamente il visualizzatore di bozze, in modo che i revisori e gli approvatori possano iniziare la revisione immediatamente. Se un documento non ha una bozza, il collegamento continua ad aprire la sezione Approvazioni del documento, come prima.

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## Impostare un workspace Frame.io sui modelli di progetto

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Se la tua organizzazione utilizza l’archiviazione cloud Adobe e disponi di una licenza Enterprise Frame.io, ora puoi scegliere un’area di lavoro Frame.io nel modello Dettagli progetto. I progetti creati dal modello utilizzano automaticamente l&#39;area di lavoro impostata sul modello, in modo che vengano instradati all&#39;area di lavoro Frame.io desiderata senza che sia necessaria alcuna azione aggiuntiva durante la creazione del progetto.

Nel nuovo campo sono elencate le aree di lavoro Frame.io per le quali si dispone dell&#39;autorizzazione di assegnazione dei progetti. Il campo rimane modificabile sul modello in qualsiasi momento; le modifiche si applicano solo ai progetti creati dopo l’aggiornamento, in modo che i progetti esistenti mantengano la loro area di lavoro originale.

Una volta creato un progetto dal modello, il relativo campo di lavoro Frame.io è di sola lettura e si collega al workspace in Frame.io.

Se non disponi di una licenza Enterprise per Frame.io, i progetti continuano ad andare all’area di lavoro predefinita per Workfront.

Per ulteriori informazioni, vedere [Modificare i modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) e [Gestire le informazioni nell&#39;area Panoramica progetto](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## Messaggio personalizzato nella riga dell’oggetto dell’e-mail

>[!NOTE]
>
>Anteprima: N/D
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Quando si imposta un messaggio personalizzato per l&#39;approvazione di un documento, tale messaggio viene ora visualizzato anche nella riga dell&#39;oggetto del messaggio di posta elettronica di richiesta di approvazione, guidato dalla data di scadenza impostata. In questo modo i revisori possono vedere cosa richiede attenzione e quando direttamente dalla casella in entrata, senza aprire l’e-mail.

Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## Allegare immagini ai commenti sugli oggetti di archiviazione cloud Adobe

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 30 luglio 2026
>Produzione per tutti: 30 luglio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

Le organizzazioni che utilizzano l’archiviazione cloud di Adobe come parte della revisione e dell’approvazione unificate possono ora allegare i file di immagine direttamente ai commenti, mantenendo insieme feedback, contesto e visualizzazioni di supporto in un unico thread di commenti tracciabile. Questo consente di colmare un vuoto precedente, in cui solo le organizzazioni che utilizzano sistemi di storage Workfront legacy possono allegare immagini ai commenti.

Tutti i formati di immagine dei tipi di media sono ora supportati per le organizzazioni di archiviazione cloud Adobe. I commenti degli oggetti legacy continuano a supportare solo i file con estensione jpg, gif e png. I file non di immagine non sono supportati nei commenti per gli oggetti di archiviazione cloud legacy o Adobe.

Per ulteriori informazioni, vedere [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Collegare le risorse da Experience Manager Assets con l’archiviazione cloud Adobe

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Se la tua organizzazione utilizza l’archiviazione cloud di Adobe, puoi collegare singole risorse da Experience Manager Assets a qualsiasi oggetto Workfront che supporti i documenti. Il contenuto collegato rimane sincronizzato automaticamente: le modifiche apportate in Experience Manager Assets vengono visualizzate in Workfront e puoi richiamare le nuove versioni delle risorse senza uscire da Workfront.

Il collegamento è basato su Contenuto verificato, in modo da ottenere anche Ricerche IA, suggerimenti avanzati, analisi di riepilogo della campagna e altro ancora durante la selezione del contenuto.

Per ulteriori informazioni, consulta [Collegare il contenuto da Experience Manager Assets con l&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).
