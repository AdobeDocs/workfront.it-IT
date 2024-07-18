---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Miglioramenti alla gestione dei progetti
description: Questa pagina descrive tutti i miglioramenti alla gestione dei progetti apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 20.3 Miglioramenti alla gestione dei progetti

Questa pagina descrive tutti i miglioramenti alla gestione dei progetti apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, consulta la [panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Formattazione campi personalizzati negli elenchi

>[!NOTE]
>
>Questa funzione è supportata solo nella nuova esperienza Adobe Workfront. È disponibile per alcuni elenchi in Adobe Workfront Classic, ma non è supportato in Adobe Workfront Classic.

Ora, quando l’amministratore di sistema crea campi per moduli personalizzati configurati per la formattazione, è possibile formattare il testo nei campi in cui si utilizza di più: negli elenchi di Workfront. Invece di passare all&#39;area Dettagli per formattare il testo nel modulo personalizzato, è possibile fare clic su un campo di un elenco e applicare Grassetto, Corsivo e Sottolineato al testo.

Questa funzionalità è disponibile solo negli elenchi aggiornati. Per ulteriori informazioni sugli elenchi aggiornati, vedere [Introduzione agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## È stato aggiornato l’aspetto di diverse intestazioni globali

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Le aree globali di Progetti, Portfoli, Programmi e Modelli dispongono ora di un’intestazione aggiornata che sfrutta al meglio lo spazio sullo schermo. Questo aggiornamento offre più spazio per le informazioni da utilizzare su cui è necessario concentrarsi.

Il collegamento Modelli dall’area Progetti è stato rimosso. È comunque possibile accedere all&#39;area Modelli dal menu principale.

## Casella Nuovo progetto di modifica

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

La finestra Modifica progetto è stata riprogettata allo scopo di aggiornare l&#39;aspetto della nuova esperienza Workfront. Puoi accedere alla nuova casella Modifica progetto da un singolo progetto o quando modifichi un singolo progetto da un elenco.

Oltre a un aspetto aggiornato, nella casella Modifica progetto sono disponibili i seguenti miglioramenti:

* Personalizzare il modello di layout una volta e riflettere tali personalizzazioni sia nella pagina Dettagli che nella casella Modifica oggetto.
* I singoli nomi dei moduli personalizzati sono ora disponibili nel pannello a sinistra all’interno della casella Modifica progetto e da lì è possibile accedere rapidamente a ogni modulo.
* La funzionalità di aggiunta di commenti viene rimossa dalla schermata di modifica del progetto per eliminare la ridondanza con la sezione Aggiornamenti.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Per informazioni sulla nuova casella Modifica progetto, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

## Nuovi miglioramenti al pannello Riepilogo e agli Aggiornamenti per l’elenco dei documenti

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Il nuovo pannello Riepilogo a destra dell’elenco dei documenti è ora disponibile con una progettazione migliorata nella nuova esperienza Workfront. Questo pannello fornisce le stesse azioni e informazioni disponibili nel pannello a destra quando si seleziona un documento in Workfront Classic, inclusi i dettagli del documento, gli aggiornamenti, il Forms personalizzato, le approvazioni e le versioni del documento.

Alcune azioni non sono attualmente disponibili, ma saranno aggiunte in una versione futura. Queste azioni includono il flusso di lavoro di verifica.

Per ulteriori informazioni, vedere [Riepilogo per panoramica documenti](../../../documents/managing-documents/summary-for-documents.md).

## Miglioramenti in Dettagli documento

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront

Nella pagina Dettagli documento, cerca i seguenti miglioramenti:

* Le opzioni della nuova versione sono state spostate in un menu a discesa accanto al pannello sinistro, per un accesso più semplice.
* L’icona Apri bozza è stata modificata in un’etichetta Apri bozza, per facilitarne la visualizzazione nella pagina.
* Miniatura di anteprima più grande, che consente di identificare facilmente il documento
* È stata aggiunta l’icona Modifica globale, che consente di modificare più campi contemporaneamente.

Per ulteriori informazioni, vedere [Panoramica dei dettagli del documento](../../../documents/managing-documents/document-details-overview.md).

## Per gli amministratori: imposta le preferenze del progetto a livello di gruppo

>[!NOTE]
>
>Questa funzionalità non è al momento disponibile per la maggior parte dei clienti nei cluster 1, 2, 3 e 5. Questa pagina verrà aggiornata quando la funzionalità verrà ripristinata per tutti i clienti.

Per dare maggiore autonomia agli amministratori del gruppo e consentire una maggiore personalizzazione dei flussi di lavoro a livello di gruppo, ora puoi definire le preferenze del progetto a livello di gruppo, per i gruppi che amministri. Quando create un progetto, le preferenze del gruppo avranno effetto prima di quelle del sistema.

Tutte le preferenze di progetto sono personalizzabili a livello di gruppo, ad eccezione di Calcoli sequenza temporale e Trimestri personalizzati.

Per ulteriori informazioni sulle preferenze di progetto del gruppo, vedere [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Novità per gli amministratori: creare campi modulo personalizzati in cui gli utenti possono formattare il testo

In un modulo personalizzato è ora possibile creare campi che includono pulsanti di formattazione del testo. Quando gli utenti digitano in questi campi, possono evidenziare e organizzare il testo in grassetto, corsivo e sottolineato. Il limite massimo di 15.000 caratteri consente di inserire testo e formattazione.

Per ulteriori informazioni, consulta Creare un modulo personalizzato nella nuova esperienza Workfront.

## Novità per gli amministratori: creare un nome interno e un’etichetta rivolta all’utente per un campo modulo personalizzato

Per offrire maggiore flessibilità nell&#39;etichettatura e rietichettatura dei campi del modulo personalizzato, è ora possibile creare un *name* interno per un campo, oltre all&#39;*label* rivolto all&#39;utente che si sta utilizzando. In questo modo è possibile modificare l&#39;etichetta del campo visualizzata dagli utenti senza modificare il nome del campo visualizzato dal sistema.

In passato, l’etichetta veniva visualizzata sopra il campo per gli utenti e utilizzata dal sistema per identificare il campo. Cambiando l&#39;etichetta per gli utenti si causava il malfunzionamento del campo ovunque venisse usato, perché il sistema non poteva più identificarlo.


