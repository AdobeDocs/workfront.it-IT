---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Miglioramenti a Project Management
description: Questa pagina descrive tutti i miglioramenti apportati alla gestione dei progetti con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 20.3 Miglioramenti a Project Management

Questa pagina descrive tutti i miglioramenti apportati alla gestione dei progetti con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, vedi [Panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Formattazione dei campi personalizzata negli elenchi

>[!NOTE]
>
>Questa funzione è supportata solo nella nuova esperienza Adobe Workfront. È disponibile per alcuni elenchi in Adobe Workfront Classic, ma non è supportato in Adobe Workfront Classic.

Ora, quando l’amministratore di sistema crea campi di moduli personalizzati configurati per la formattazione, è possibile formattare il testo nei campi in cui sono più utilizzati: negli elenchi in Workfront. Invece di passare all’area Dettagli per formattare il testo nel modulo personalizzato, è possibile fare clic su un campo in un elenco e applicare Grassetto, Corsivo e Sottolineato al testo.

Questa funzionalità è disponibile solo negli elenchi aggiornati. Per ulteriori informazioni sugli elenchi aggiornati, consulta [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Per informazioni sulla creazione di campi di testo con formattazione da parte di un amministratore Workfront, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Aspetto aggiornato di diverse intestazioni globali

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Nelle aree globali di Progetti, Portfoli, Programmi e Modelli è ora disponibile un’intestazione aggiornata che consente di sfruttare al meglio lo spazio disponibile sullo schermo. Questo aggiornamento fornisce più spazio per le informazioni su cui lavorare.

Il collegamento Modelli dall’area Progetti è stato rimosso. È comunque possibile accedere all&#39;area Modelli dal menu principale.

## Nuova casella di controllo Modifica progetto

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Per aggiornare l’aspetto della nuova esperienza Workfront, abbiamo riprogettato la casella Modifica progetto . È possibile accedere alla nuova casella Modifica progetto da un singolo progetto o quando si modifica un singolo progetto da un elenco.

Oltre a un aspetto e a un aspetto aggiornati, nella casella Modifica progetto sono disponibili i seguenti miglioramenti:

* Personalizzare il modello di layout una volta e riflettere le personalizzazioni nella pagina Dettagli e nella casella Modifica oggetto.
* Nel pannello a sinistra della casella Modifica progetto sono ora disponibili singoli nomi di moduli personalizzati ed è possibile accedere rapidamente a ciascun modulo.
* La funzionalità di commento viene rimossa dalla schermata di modifica del progetto per eliminare la ridondanza con la sezione Aggiornamenti .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Per informazioni sulla nuova casella Modifica progetto, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

## Nuovo pannello Riepilogo e miglioramenti dell&#39;elenco dei documenti

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Il nuovo pannello Riepilogo a destra dell’elenco dei documenti è ora disponibile con una progettazione avanzata nella nuova esperienza Workfront. Questo pannello fornisce le stesse azioni e informazioni disponibili nel pannello a destra quando si seleziona un documento in Workfront Classic, inclusi dettagli del documento, aggiornamenti, Forms personalizzato, approvazioni e versioni del documento.

Alcune azioni non sono al momento disponibili, ma verranno aggiunte in una versione futura. Queste azioni includono il flusso di lavoro di correzione.

Per ulteriori informazioni, consulta [Panoramica del riepilogo dei documenti](../../../documents/managing-documents/summary-for-documents.md).

## Miglioramenti nei dettagli dei documenti

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Nella pagina Dettagli documento sono disponibili i seguenti miglioramenti:

* Le nuove opzioni di versione sono state spostate in un menu a discesa vicino al pannello a sinistra, per un accesso più semplice.
* L’icona a forma di bozza aperta è stata modificata in un’etichetta a prova aperta, facilitando la visualizzazione sulla pagina.
* Miniatura di anteprima più grande, che consente di identificare facilmente il documento
* È stata aggiunta l’icona Modifica globale , che consente di modificare più campi contemporaneamente.

Per ulteriori informazioni, consulta [Panoramica dei dettagli del documento](../../../documents/managing-documents/document-details-overview.md).

## Per gli amministratori: imposta le preferenze del progetto a livello di gruppo

>[!NOTE]
>
>Questa funzionalità non è temporaneamente disponibile per la maggior parte dei clienti nei cluster 1, 2, 3 e 5. Questa pagina verrà aggiornata quando la funzionalità verrà ripristinata per tutti i clienti.

Per dare agli amministratori del gruppo maggiore autonomia e consentire una personalizzazione a livello di gruppo dei flussi di lavoro, ora puoi definire le preferenze di progetto a livello di gruppo per i gruppi amministrati. Quando crei un progetto, le preferenze del gruppo avranno effetto prima di quelle del sistema.

Tutte le preferenze del progetto sono personalizzabili a livello di gruppo, ad eccezione dei calcoli Timeline e dei trimestri personalizzati.

Per ulteriori informazioni sulle preferenze per i progetti di gruppo, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Novità per gli amministratori: Creazione di campi modulo personalizzati in cui gli utenti possono formattare il testo

In un modulo personalizzato è ora possibile creare campi che includono pulsanti di formattazione del testo. Quando l’utente digita i campi, può evidenziare e organizzare il testo in grassetto, corsivo e sottolineato. L&#39;elevato limite di caratteri di 15.000 consente un&#39;ampia quantità di testo e formattazione.

Per ulteriori informazioni, consulta Creare un modulo personalizzato nella nuova esperienza Workfront .

## Novità per gli amministratori: Creare un nome interno e un’etichetta rivolta all’utente per un campo Modulo personalizzato

Per garantire una maggiore flessibilità nell’etichettatura e nella rietichettatura dei campi modulo personalizzati, è ora possibile creare un *name* per un campo oltre a quello rivolto all’utente *etichetta* tu hai usato. In questo modo è possibile modificare l’etichetta del campo visualizzata dagli utenti senza modificare il nome del campo visualizzato dal sistema.

In passato, l’etichetta veniva visualizzata sia sopra il campo per gli utenti sia utilizzata dal sistema per identificare il campo. Pertanto, la modifica dell’etichetta per gli utenti ha causato il malfunzionamento del campo dovunque sia stato utilizzato, perché il sistema non era più in grado di identificarlo.

Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

