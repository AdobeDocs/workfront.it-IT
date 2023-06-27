---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli SDL Managed Translation
description: In un [!DNL Adobe Workfront Fusion] è possibile collegare l'account SDL Managed Translation a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi collegare il tuo [!DNL SDL Managed Translation] account per più applicazioni e servizi di terze parti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Moduli

>[!NOTE]
>
>Timeout dell&#39;operazione per le chiamate a [!DNL SDL Managed Translation] è **120 secondi**.

### File

#### [!UICONTROL Scarica file tradotto]

Questo modulo recupera il contenuto di un singolo file tradotto, contenuto all’interno del progetto specificato. Se il file richiesto non è ancora nello stato Downland, è possibile che il contenuto del file non sia ancora stato tradotto completamente. Se il file è nello stato Download e lo hai recuperato correttamente, assicurati di contrassegnarlo come completato utilizzando `Cancel or Complete File` metodo.

#### [!UICONTROL Carica un file]

Questo modulo consente il caricamento di file da tradurre o includere in un progetto di traduzione come materiale di riferimento. I caricamenti devono essere inviati utilizzando dati multipart/form e possono contenere più file. È possibile specificare `ProjectOptionId` da utilizzare per valutare i file caricati. Questo determina se ogni file che carichi è un possibile candidato per la traduzione o deve essere gestito come materiale di riferimento. Nel caso degli archivi (`zip `, `rar`, `7z`, `tar` file) l’app esamina il contenuto dell’archivio e indica se l’archivio nel suo insieme può essere tradotto o se contiene una combinazione di file traducibili e non traducibili.

>[!NOTE]
>
>Il caricamento di più file alla volta non è consigliato, in quanto può aumentare l’impatto di eventuali errori.

#### [!UICONTROL Aggiungi un file di riferimento]

Questo modulo aggiunge un file di riferimento.

### Progetti

#### [!UICONTROL Crea un Progetto]

Questo modulo crea il progetto specificato.

#### Annullare o completare un progetto

Questo modulo annulla o completa il progetto specificato. Se il progetto è in attesa di essere scaricato, il progetto passa attraverso gli eventuali passaggi finali del flusso di lavoro e alla fine si sposta per essere completato. Se il progetto è in attesa di approvazione o la selezione del fornitore è annullata. Se il progetto si trova in un altro stato, la richiesta non riuscirà.

#### [!UICONTROL Scarica ZIP progetto]

Questo modulo ottiene il `zip` file di file tradotti per il progetto specificato.

#### [!UICONTROL Leggi un progetto]

Questo modulo ottiene il progetto specificato.

#### [!UICONTROL Ottieni progetti allo stato]

Questo modulo ottiene tutti i progetti disponibili nello stato specificato. Questo metodo consente di impaginare i risultati specificando `$top`, `$skip`, e `$orderby` parametri di query.

#### [!UICONTROL Ottieni elenco progetti]

Ottiene un semplice elenco di tutti i progetti, fornendo informazioni generali su ciascun progetto. Questo metodo consente di impostare i risultati come pagine, specificando `$top`, `$skip`, e `$orderby` parametri di query.

#### [!UICONTROL Cerca opzioni di creazione progetto]

Questo modulo ottiene le opzioni di creazione del progetto.

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo esegue una chiamata API autorizzata arbitraria.
