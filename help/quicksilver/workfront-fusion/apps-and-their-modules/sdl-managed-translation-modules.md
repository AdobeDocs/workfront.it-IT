---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di traduzione gestiti da SDL
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile collegare l'account SDL Managed Translation a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] moduli

In un [!DNL Adobe Workfront Fusion] in uno scenario, è possibile collegare [!DNL SDL Managed Translation] account a più applicazioni e servizi di terze parti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Moduli

>[!NOTE]
>
>Timeout dell’operazione per le chiamate a [!DNL SDL Managed Translation] è **120 secondi**.

### File

#### [!UICONTROL Scarica file tradotto]

Questo modulo recupera il contenuto di un singolo file tradotto contenuto nel progetto specificato. Se il file richiesto non è ancora nello stato Downland, il contenuto del file potrebbe non essere ancora tradotto completamente. Se il file è nello stato Download e lo hai recuperato correttamente, assicurati di contrassegnare il file come completo utilizzando il `Cancel or Complete File` metodo .

#### [!UICONTROL Caricare un file]

Questo modulo consente il caricamento di file da tradurre o da includere in un progetto di traduzione come materiale di riferimento. I caricamenti devono essere inviati utilizzando dati multiparte/modulo e possono contenere più di un file. Specifica la `ProjectOptionId` da utilizzare per valutare i file caricati. Questo determina se ogni file caricato è un possibile candidato per la traduzione o deve essere gestito come materiale di riferimento. Per gli archivi (`zip `, `rar`, `7z`, `tar` file) l&#39;app esamina il contenuto dell&#39;archivio e indica se l&#39;archivio nel suo complesso può essere tradotto, o se contiene una miscela di file traducibili e non traducibili.

>[!NOTE]
>
>Il caricamento di più file alla volta non è consigliato, in quanto può aumentare l’impatto di eventuali errori.

#### [!UICONTROL Aggiungi un file di riferimento]

Questo modulo aggiunge un file di riferimento.

### Progetti

#### [!UICONTROL Crea un Progetto]

Questo modulo crea il progetto specificato.

#### Annullare o completare un progetto

Questo modulo annulla o completa il progetto specificato. Se il progetto è in attesa di download, il progetto passa attraverso tutti i passaggi finali nel flusso di lavoro e alla fine passa al completamento. Se il progetto è in attesa di approvazione o la selezione del fornitore viene annullata. Se il progetto si trova in un altro stato, la richiesta avrà esito negativo.

#### [!UICONTROL Scarica ZIP progetto]

Questo modulo ottiene il `zip` file di file convertiti per il progetto specificato.

#### [!UICONTROL Leggi un progetto]

Questo modulo ottiene il progetto specificato.

#### [!UICONTROL Ottieni progetti allo stato]

Questo modulo ottiene tutti i progetti disponibili nello stato specificato. Questo metodo consente di impaginare i risultati specificando `$top`, `$skip`e `$orderby` parametri di query.

#### [!UICONTROL Ottieni elenco progetti]

Ottiene un elenco semplice di tutti i progetti, fornendo informazioni generali su ciascun progetto. Questo metodo consente di ottenere risultati sotto forma di pagine, specificando `$top`, `$skip`e `$orderby` parametri di query.

#### [!UICONTROL Opzioni di creazione di progetti di ricerca]

Questo modulo ottiene le opzioni di creazione del progetto.

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo esegue una chiamata API arbitraria autorizzata.
