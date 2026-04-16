---
product-area: documents
navigation-topic: approvals
title: Creare e gestire i brand per il revisore dei contenuti
description: Creare e gestire i brand per il revisore dei contenuti
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 243aa2b0893e3034d37b959384a50b8a5e4a4bf0
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 7%

---

# Creare e gestire i brand per il revisore dei contenuti

Il revisore dei contenuti utilizza le linee guida del brand per valutare i contenuti durante il processo di revisione. Puoi creare marchi in Workfront caricando file PDF che contengono le linee guida per i marchi o immettendo manualmente gli elementi del marchio.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di sistema.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni di Admin Console*</td> 
   <td> <p>Devi essere un Brand Manager GenStudio.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisiti

* L&#39;istanza di Workfront deve avere le approvazioni unificate abilitate.

* La tua organizzazione deve disporre di GenStudio Foundation.
   * Il Visualizzatore contenuti di Workfront fornisce le funzionalità disponibili in GenStudio Foundation per i flussi di lavoro di revisione e approvazione delle risorse. Non è necessario accedere direttamente a GenStudio Foundation per completare il lavoro. L’accesso alle funzionalità di GenStudio Foundation tramite Content Reviewer rientra nei termini del contratto Workfront.
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file.
Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Prerequisiti

1. Prima di poter creare i brand, devi concedere l’accesso alle autorizzazioni del brand in Admin Console e nei livelli di accesso di Workfront. Per istruzioni, consulta [Concedere l&#39;accesso alle autorizzazioni del brand](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Creare un brand utilizzando una PDF

{{step-1-to-setup}}

1. Nel pannello a sinistra, vai a **Revisione e approvazione** > **Marchi**.
1. Fai clic su **Aggiungi marchio** nell&#39;angolo in alto a destra dello schermo.
1. Assegna un nome al marchio.
1. Fai clic su **Carica PDF** per caricare i file del marchio.
   ![carica pdf marchio](assets/upload-PDF.png)
1. Fai clic su **Continue** (Continua).
1. Carica uno o più file PDF contenenti le linee guida per il tuo marchio, quindi fai clic su **Aggiungi marchio**.
1. Una volta caricati i file, controlla gli elementi del brand estratti per assicurarti che siano conformi alle linee guida del brand.

   >[!IMPORTANT]
   >
   >Le linee guida vengono generate utilizzando i file e la tecnologia di intelligenza artificiale generativa e possono essere imprecise. Rivedi le linee guida estratte per individuare dettagli mancanti o errati e modificale prima di pubblicare questo marchio.

1. Al termine, fai clic su **Pubblica** per rendere il brand disponibile per il revisore dei contenuti.

## Creare manualmente un brand

{{step-1-to-setup}}

1. Nel pannello a sinistra, vai a **Revisione e approvazione** > **Marchi**.
1. Fai clic su **Aggiungi marchio** nell&#39;angolo in alto a destra dello schermo.
1. Assegna un nome al marchio.
1. Fai clic su **Aggiungi manualmente** per creare un marchio con singoli elementi.
1. Compila i dettagli del brand in base alle esigenze. Puoi aggiungere i seguenti elementi:

   <table>
    <tr>
        <td>Quando utilizzare</td>
        <td>Informa gli esperti di marketing quando utilizzare questo marchio.</td>
    </tr>
    <tr>
        <td>Linee guida vocali</td>
        <td>Fornisci indicazioni sul tono e sullo stile della voce del brand.</td>
    </tr>
    <tr>
        <td>Linee guida per le immagini</td>
        <td>Specifica i tipi di immagini che sono allineati con l’identità del brand.</td>
    </tr>
    <tr>
        <td>Linee guida per il canale</td>
        <td>Delineare i canali appropriati per la comunicazione del brand.</td>
    </tr>
    <tr>
        <td>Logo</td>
        <td>Includi i logo ufficiali associati al brand.</td>
    </tr>
    <tr>
        <td>Colori</td>
        <td>Specifica la palette di colori del brand.</td>
    </tr>
    </table>

   ![aggiungere manualmente elementi del brand](assets/brand-elements.png)


1. Al termine, fai clic su **Pubblica** per rendere il brand disponibile per il revisore dei contenuti.


## Best practice per la scrittura di linee guida per i marchi

*  Scrivi le linee guida del brand che descrivono i criteri misurabili. Il revisore dei contenuti valuta i contenuti letteralmente, quindi le regole oggettive producono punteggi più coerenti di quelli soggettivi.

* Cerca parole come &quot;evitare&quot;, &quot;mantenere&quot; o &quot;assicurarsi&quot; nelle linee guida. Questi segnali spesso indicano una regola che puoi stringere. Sostituisci l’istruzione vaga con un elenco specifico di parole, formati o limiti. Ad esempio, sostituisci &quot;evita i comuni luoghi comuni di sci&quot; con &quot;non utilizzare &#39;gnar&#39;, &#39;pow&#39; o &#39;shred&#39;&quot;.

* Se non è possibile rimuovere la soggettività, restringerla. Sostituire gli aggettivi ampi con vincoli specifici. Ad esempio, &quot;Diretto e orientato all&#39;azione&quot; diventa &quot;Diretto e orientato all&#39;azione; omettere parole di riempimento e linguaggio di copertura&quot;.