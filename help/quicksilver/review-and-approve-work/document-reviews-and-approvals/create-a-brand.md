---
product-area: documents
navigation-topic: approvals
title: Configurare i brand per il revisore IA
description: Configurare i brand per il revisore IA
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
source-git-commit: 07b401c70dfd209d13c34cf62844f334f3260af1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 5%

---

# Configurare i brand per il revisore IA

>[!IMPORTANT]
>
>Questa funzione è attualmente in versione beta.

Il revisore IA utilizza le linee guida del brand per valutare i contenuti durante il processo di revisione. Puoi creare marchi in Workfront caricando file PDF che contengono le linee guida per i marchi o immettendo manualmente gli elementi del marchio.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di sistema.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni di Admin Console*</td> 
   <td> <p>Devi usare GenStudio Brand Manager.</p>
    <p>NOTA: per selezionare GenStudio Brand Manager, è necessario seguire i passaggi descritti in <a href="https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/intro/configure-brand-permissions">Assegnare autorizzazioni marchio</a>.</p>
   </td> 
  </tr> 
 </tbody> 
</table>





Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Prerequisiti

* La tua organizzazione deve aver eseguito la migrazione ad Adobe IMS (Identity Management System).
* L&#39;istanza di Workfront deve avere le approvazioni unificate abilitate.
* La tua organizzazione deve disporre di GenStudio Foundation.
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file.
Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Creare un brand utilizzando una PDF

{{step-1-to-setup}}

1. Nel pannello a sinistra, vai a **Revisione e approvazione** > **Marchi**.
1. Fai clic su **Aggiungi marchio** nell&#39;angolo in alto a destra dello schermo.
1. Assegna un nome al marchio.
1. Fai clic su Carica PDF per caricare i file del brand.
   ![carica pdf marchio](assets/upload-PDF.png)
1. Fai clic su **Continue** (Continua).
1. Carica uno o più file PDF contenenti le linee guida per il tuo marchio, quindi fai clic su **Aggiungi marchio**.
1. Una volta caricati i file, controlla gli elementi del brand estratti per assicurarti che siano conformi alle linee guida del brand.

   >[!IMPORTANT]
   >
   >Le linee guida vengono generate utilizzando i file e la tecnologia di intelligenza artificiale generativa e possono essere imprecise. Rivedi le linee guida estratte per individuare dettagli mancanti o errati e modificale prima di pubblicare questo marchio.

1. Al termine, fai clic su **Pubblica** per rendere il brand disponibile per il revisore di intelligenza artificiale.

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
        <td>loghi</td>
        <td>Includi i logo ufficiali associati al brand.</td>
    </tr>
    <tr>
        <td>Colori</td>
        <td>Specifica la palette di colori del brand.</td>
    </tr>
    </table>

   ![aggiungere manualmente elementi del brand](assets/brand-elements.png)


1. Al termine, fai clic su **Pubblica** per rendere il brand disponibile per il revisore di intelligenza artificiale.
