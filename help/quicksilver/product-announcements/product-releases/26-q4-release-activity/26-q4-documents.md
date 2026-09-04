---
title: Miglioramenti ai documenti del quarto trimestre 2026
description: Miglioramenti ai documenti del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 5e13c944ac485a6999dd0a788cfbb0f5d5169742
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 2%

---

# Miglioramenti ai documenti del quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del quarto trimestre 2026. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## System Administrators full access to approval templates

>[!NOTE]
>
>Preview: September 4, 2026
>Production fast release: September 4, 2026
>Production for everyone: September 4, 2026
>[!BADGE Off schedule]{type=Neutral}

System Administrators can now view, edit, delete, and bulk-delete every approval template in the account, regardless of who created or shared it. Previously, System Administrators were subject to the same sharing rules as other users, and could only see or manage templates they created or that were shared with them.

For more information, see [Manage approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

-->

## Visibilità dei commenti dei frame in Workfront

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Quando si crea un flusso di lavoro di approvazione per un documento, gli utenti possono lasciare commenti e aggiungere annotazioni nel visualizzatore Frame.io. Questi commenti non vengono visualizzati nel pannello Commenti di Workfront, ma possono essere visualizzati nel visualizzatore Frame.io.

Ora il pannello Commenti di Workfront visualizza un messaggio che informa quando sono disponibili nuovi commenti in Frame.io.

Per ulteriori informazioni, vedere [Aggiungere un aggiornamento a un documento](/help/quicksilver/documents/managing-documents/add-update-documents.md).

## Accesso diretto alle bozze dai collegamenti e-mail per l’approvazione

>[!NOTE]
>
>Anteprima: N/D
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Quando a un documento è allegata una bozza, il collegamento &quot;Vai alla revisione&quot; nelle e-mail di approvazione ora apre direttamente il visualizzatore di bozze, in modo che i revisori e gli approvatori possano iniziare la revisione immediatamente. Se un documento non ha una bozza, il collegamento continua ad aprire la sezione Approvazioni del documento, come prima.

## Aggiungere team alle approvazioni per gli oggetti tramite l’archiviazione cloud di Adobe

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile aggiungere un team di Workfront come approvatore o revisore in un modello di approvazione o approvazione del documento, anziché aggiungere ogni persona singolarmente:

* Oggetti nell’archiviazione cloud di Adobe: Workfront aggiunge ogni membro del team attivo singolarmente, in modo che l’elenco degli approvatori rifletta sempre chi è attualmente nel team.
* Oggetti che utilizzano l’archiviazione legacy di Workfront: per impostazione predefinita, il team viene aggiunto come partecipante singolo, ma ora puoi scegliere di aggiungere ogni membro del team come partecipante singolo.
* Nei modelli di approvazione, Workfront memorizza un riferimento al team e lo espande in membri attivi quando si applica il modello a un documento, non quando si salva il modello.

Per ulteriori informazioni, consulta:

* [Creare un flusso di lavoro di approvazione nella nuova area Documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Creare un flusso di lavoro di approvazione nell’area documenti legacy](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Creare un modello di flusso di lavoro di approvazione per i documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

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

## Pannello Versioni riprogettato nella nuova area dei documenti

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, il pannello Versioni nella nuova area Documenti presenta un nuovo design:

* Le versioni sono etichettate V1, V2 e così via per coerenza con Frame.io.
* Ogni versione mostra il proprio stato di approvazione, ad esempio &quot;Approvato&quot; o &quot;Ritirato&quot;, direttamente nell’elenco.
* Il pannello ora elenca solo la cronologia delle versioni, non esiste più una voce separata &quot;file più recente&quot; nella parte superiore.

In precedenza, le versioni avevano una marca temporale invece che un numero.

Per ulteriori informazioni, consulta [Gestire le versioni dei documenti](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Pannello Approvazioni riprogettato nella nuova area dei documenti

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, il pannello Approvazioni nella nuova area Documenti mostra ora la cronologia delle approvazioni per le diverse versioni:

* Il pannello elenca il flusso di lavoro di approvazione per ogni versione che ne ha una, non solo per la versione corrente.
* I flussi di lavoro ritirati rimangono nell’elenco, quindi puoi ancora rivedere le loro decisioni precedenti.
* Espandi qualsiasi versione per visualizzarne le fasi, le decisioni dell’approvatore, la regola di decisione e le date di scadenza senza uscire dal pannello.

In precedenza, il pannello Approvazioni mostrava solo il flusso di lavoro della versione corrente.

Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

