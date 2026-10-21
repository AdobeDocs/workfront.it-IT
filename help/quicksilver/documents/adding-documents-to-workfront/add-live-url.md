---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Aggiungere un collegamento web come documento
description: Puoi aggiungere un sito web ad Adobe Workfront come collegamento web e richiederne l’approvazione.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 05f148f2c28555e37fb415f606e314a5df564047
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 8%
---
# Aggiungere un collegamento web come documento

Puoi aggiungere un sito web ad Adobe Workfront come collegamento web dalla nuova area Documenti. Dopo averlo aggiunto, puoi richiedere l’approvazione sulla pagina web live nello stesso modo in cui richiedi l’approvazione su un file caricato.

Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando l’archiviazione cloud Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Archiviazione Workfront legacy: modifica accesso ai documenti</p> 
   <p>Adobe Cloud Storage: l’accesso di modifica ai documenti è abilitato per impostazione predefinita e non può essere modificato</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere un collegamento web come documento

Puoi caricare una pagina web html in Workfront come collegamento web. Dopo averlo aggiunto, puoi richiedere l’approvazione sulla pagina web live nello stesso modo in cui richiedi l’approvazione su un file caricato. Per ulteriori informazioni sulla gestione dei collegamenti Web da parte di Frame.io, vedere [Revisione HTML per Frame.io](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links).


>[!IMPORTANT]
>
>* Gli URL sono supportati se il sito consente incorporamenti iFrame.
>* Gli URL web privati sono supportati, ma alcuni flussi di autenticazione potrebbero non funzionare a seconda della configurazione del server.
>* Gli URL di Youtube e Figma non sono attualmente supportati.<br>
>Per ulteriori informazioni, vedere [Revisione HTML per Frame.io](https://help.frame.io/en/articles/12893213-html-review-for-frame-io).


Per aggiungere un collegamento Web:

1. Vai al progetto, all&#39;attività o al problema in cui desideri aggiungere il sito Web, quindi seleziona **Documenti** nel pannello a sinistra.
1. Fai clic su **Nuovo**, quindi seleziona **Collegamento web**.
1. Immettere un nome nel campo **Nome documento**, quindi immettere l&#39;indirizzo del sito Web nel campo **URL**.
1. Fai clic su **Aggiungi**.
   ![Aggiungere un collegamento Web come documento](assets/web-url.png)

Per richiedere l&#39;approvazione sul collegamento Web, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Limitazioni note

* Si è verificato un problema temporaneo con i documenti di collegamento web creati in Frame.io. Se si crea un collegamento web in Frame.io e quindi si crea un&#39;approvazione in Workfront, il documento non si aprirà in Frame.io. I collegamenti web creati in Workfront non subiscono modifiche. Fino a quando questo problema non viene risolto, crea documenti di collegamento web in Workfront prima di avviare un’approvazione.
* Attualmente non è possibile creare nuove versioni dei documenti di collegamento Web in Frame.io. Se è necessario creare una nuova versione di un documento di collegamento Web, creare la nuova versione in Workfront.