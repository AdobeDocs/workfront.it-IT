---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: L’area Documenti
description: Nell’area Documenti puoi organizzare, gestire e visualizzare i metadati dei documenti caricati in Adobe Workfront. Puoi anche vedere la decisione relativa alla bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ed7944fe4934ac5ab52b1eed3e144309de9781c4
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 1%

---

# L’area Documenti

Nell’area Documenti puoi organizzare, gestire e visualizzare i metadati dei documenti caricati in Adobe Workfront. Puoi anche vedere la decisione relativa alla bozza.

In Workfront sono attualmente disponibili due versioni dell&#39;area Documenti: l&#39;area documenti legacy e l&#39;area nuovi documenti. La versione utilizzata dall&#39;organizzazione dipende dal fatto che l&#39;organizzazione si basi su sistemi di storage Workfront o aziendali legacy. Per ulteriori informazioni su questi tipi di archiviazione, vedere [Panoramica sullo storage aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Area documenti legacy

Sono disponibili due tipi di aree Documenti. Funzionalità e funzionalità identiche per:

* **Area Documenti in un programma, portfolio, progetto, attività o problema:** Elenca tutti i documenti a cui si ha accesso per un particolare progetto, attività o problema. Per accedere a questa area, fai clic su **Documenti** ![Icona Documenti](assets/document-icon-12x14.png) nel pannello a sinistra durante la visualizzazione di un progetto, un&#39;attività o un problema.

* **Area documenti globali:** Elenca tutti i documenti a cui si ha accesso in Workfront. Per accedere a quest&#39;area, fare clic su **Documenti** ![Icona Documenti](assets/document-icon.png) nel menu principale ![Icona Menu principale](assets/main-menu-icon.png).

Per informazioni sul caricamento di documenti in Workfront, consulta [Aggiungere documenti ad Adobe Workfront dal file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


Nell&#39;area documenti viene registrato il conteggio dei seguenti elementi:

* Cartelle di Workfront
* File caricati dal file system
* File aggiunti a Workfront da integrazioni
* Experience Manager Assets collegato

### Pannello di Riepilogo

Quando si seleziona un documento nell&#39;area documenti, è possibile utilizzare il Riepilogo a destra per visualizzare i dettagli del documento, gestire gli aggiornamenti e le approvazioni del documento, visualizzare le versioni del documento e aggiungere e modificare il Forms personalizzato per il documento.

Se per il documento è impostata la verifica, la sezione Dettagli include informazioni quali la data di scadenza della verifica e l&#39;avanzamento corrente della verifica.

È possibile fare clic sull&#39;intestazione Dettagli per passare all&#39;area Dettagli documento completa quando sono necessarie tutte le informazioni relative a un documento.

![Area documenti](assets/documents-area-v2-350x199.png)

Per informazioni sul Riepilogo, vedere [Riepilogo per la panoramica dei documenti](../../documents/managing-documents/summary-for-documents.md).

### Decisione bozza

Una volta presa la decisione relativa alla bozza, questa viene visualizzata nell&#39;elenco Documento.

![Decisione bozza nell&#39;elenco documenti](assets/proof-decision---doc-list-350x168.png)

### Cartelle

In un progetto, un&#39;attività o un problema in cui vengono caricati documenti, è possibile impostare cartelle per organizzare i documenti. Per ulteriori informazioni, vedere [Creare cartelle di documenti](../../documents/organizing-documents/create-documents-folder.md).

Nell&#39;area Documenti globale è possibile impostare due tipi di cartelle per organizzare i documenti a cui si ha accesso:

* **Cartelle avanzate:** visualizza solo i documenti che si desidera visualizzare. Per ulteriori informazioni, vedere [Creare e gestire cartelle avanzate](../../documents/organizing-documents/create-manage-smart-folders.md).

* **Cartelle personali:** Organizzare i documenti nel modo desiderato. Per ulteriori informazioni, vedere [Creare cartelle di documenti](../../documents/organizing-documents/create-documents-folder.md).

### Dettagli documento espanso

La pagina Dettagli documento fornisce una versione in scala più completa dei Dettagli documento nel Riepilogo a destra.

## Nuova area documento

La nuova area documenti è disponibile solo per le organizzazioni che utilizzano lo storage aziendale. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Utilizzare il pannello di riepilogo

Quando si seleziona un documento nell&#39;area documenti, è possibile utilizzare il pannello Riepilogo a destra per visualizzare i dettagli sul documento, aggiungere e modificare moduli personalizzati allegati, creare e gestire flussi di lavoro di approvazione, visualizzare le versioni del documento e altro ancora.

#### Revisione e approvazione con Frame.io

È possibile esaminare e approvare i documenti nell&#39;area nuovi documenti utilizzando il visualizzatore Frame.io.

Per ulteriori informazioni, vedere [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Gestione versioni

È possibile caricare nuove versioni di un documento nell&#39;area nuovi documenti. Quando carichi una nuova versione, questa viene mantenuta e vi si può accedere dal pannello Riepilogo. Le versioni vengono automaticamente denominate con la data e l’ora del caricamento, ma possono essere rinominate in base alle esigenze.

È inoltre possibile avviare un nuovo flusso di lavoro di approvazione per una versione specifica di un documento.

#### Visualizza cronologia documenti

È possibile visualizzare la cronologia di un documento nell&#39;area nuovi documenti. La cronologia include i seguenti tipi di informazioni:

* Quando il documento è stato caricato
* Quando sono state caricate nuove versioni
* Quando sono stati avviati i flussi di lavoro di approvazione per il documento
* E altro ancora

### Cartelle a livello di sistema per le autorizzazioni dei documenti

Workfront crea automaticamente una cartella a livello di sistema quando il primo documento viene caricato su un’attività o un problema. Queste cartelle ereditano le autorizzazioni dall’attività o dal problema e sono visibili nell’area documenti a livello di progetto. Tutti i documenti caricati su tale attività o problema sono memorizzati in tale cartella e da essa ereditano le autorizzazioni. Questo è il modo principale in cui le autorizzazioni vengono gestite per i documenti nell&#39;area nuovi documenti. Per ulteriori informazioni, vedere [Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di storage aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Considerazioni

* La nuova area dei documenti è ottimizzata per schermi di larghezza pari o superiore a 1024 pixel. Se si dispone di una schermata più piccola, è possibile che si verifichino problemi di accesso al pannello Riepilogo.

* L’area documenti globali non è disponibile nella nuova esperienza dell’area documenti. È possibile accedere ai documenti solo da programmi, portafogli, progetti, attività o problemi.
