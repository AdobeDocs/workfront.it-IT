---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Passare a Workfront sull’archiviazione cloud Adobe
description: Pianifica il passaggio a Workfront sull’archiviazione cloud Adobe. Scopri cosa accade quando l’organizzazione è abilitata, cosa c’è di diverso sugli oggetti di archiviazione cloud di Adobe e come eseguirne il rollout secondo i tempi.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Passare a Workfront sull’archiviazione cloud Adobe

Workfront sull’archiviazione cloud Adobe offre l’esperienza completa di revisione e approvazione unificata: recensioni nel visualizzatore Frame.io, potenti flussi di lavoro di approvazione, visibilità delle risorse tra i prodotti e altro ancora.

Questo articolo è il punto di partenza per gli amministratori di Workfront che passano all’archiviazione cloud Adobe. Spiega cosa accade quando abiliti l’archiviazione cloud di Adobe, ti rimanda ai dettagli delle differenze e ai collegamenti agli articoli che ti aiutano a pianificare e implementare la modifica.

## Decidi quando Adobe Cloud Storage si attiva

Nessuna modifica dell&#39;ambiente Workfront finché un amministratore di Workfront non abilita l&#39;archiviazione cloud Adobe come opzione di archiviazione predefinita in **Configurazione** > **Sistema** > **Preferenze**. Fino ad allora, i progetti esistenti ed eventuali nuovi progetti creati rimangono sullo storage Workfront legacy e mantengono il servizio di approvazione utilizzato oggi.

Quando un amministratore abilita l’archiviazione cloud di Adobe come opzione di archiviazione predefinita:

* I nuovi progetti utilizzano l’archiviazione cloud di Adobe
* Frame.io è il visualizzatore predefinito
* Le approvazioni unificate sono il servizio di approvazione predefinito

I progetti esistenti non cambiano.

Poiché controlli la tempistica, puoi testare l’esperienza, aggiornare gli scenari di Workfront Fusion e pianificare le modifiche da apportare ai rapporti prima che qualcuno vi lavori. Per istruzioni dettagliate, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

## Funzionamento delle approvazioni sull’archiviazione cloud di Adobe

I progetti Adobe di archiviazione cloud utilizzano le approvazioni unificate per impostazione predefinita, con revisione e approvazione nel visualizzatore Frame.io. Gli oggetti che rimangono sullo storage Workfront legacy mantengono qualsiasi servizio di approvazione già utilizzato: approvazioni di documenti legacy o approvazioni unificate.

>[!NOTE]
>
>Se si imposta Adobe Cloud Storage come predefinito, il servizio di approvazione già in uso sugli oggetti di archiviazione Workfront legacy non viene modificato. Approvazioni unificate è l’impostazione predefinita solo per i nuovi oggetti creati nell’archiviazione cloud di Adobe.

Prima di implementare l’archiviazione cloud di Adobe, assicurati che gli utenti che gestiscono le approvazioni sappiano cosa aspettarsi. Per ulteriori informazioni, vedere [Passare dalle approvazioni dei documenti legacy alle approvazioni unificate](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md).

## Pianifica lo spostamento

Elabora questi articoli in modo da preparare:

* [Differenze nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md): le principali differenze negli oggetti di archiviazione cloud Adobe, dalla nuova area Documenti e dal visualizzatore Frame.io alle regole di denominazione, alla quota di archiviazione e a Fusion.
* [Pianifica il rollout dell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md): scegli una configurazione di rollout, esegui il test pilota con un singolo gruppo e metti in sequenza il lavoro in modo che non vi siano sorprese per i tuoi utenti.
* [Abilita l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md): i passaggi per impostare l&#39;opzione di archiviazione predefinita per l&#39;intera organizzazione o per gruppi specifici.
* [Converti oggetti legacy in Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md): i tre casi in cui puoi convertire un oggetto legacy in Adobe Cloud Storage e ciò che si sposta durante ogni conversione.


## Articoli correlati

* [Panoramica dell’archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [L’area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Autorizzazioni di oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
