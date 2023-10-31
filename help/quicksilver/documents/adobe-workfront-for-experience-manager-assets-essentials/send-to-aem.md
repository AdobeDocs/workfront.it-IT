---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Inviare un documento a Experience Manager Assets o ad Assets Essentials
description: È possibile inviare documenti da Workfront a Experience Manager Assets o ad Assets Essentials. I documenti caricati e inviati da Workfront agli Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. Le risorse collegate dagli Assets Essentials non vengono conteggiate per lo storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 24ffde1850a005428a3f619fc00842a8779bbc6d
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Inviare un documento a Experience Manager Assets o ad Assets Essentials

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente Sandbox di anteprima.</span>

È possibile inviare documenti da Workfront a Experience Manager Assets o ad Assets Essentials. I documenti caricati e inviati da Workfront agli Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. Le risorse collegate dagli Assets Essentials non vengono conteggiate per lo storage complessivo.

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o ad Assets Essentials. Vengono inviati anche tutti i metadati configurati per la mappatura degli oggetti principali. Per ulteriori informazioni sulla configurazione della mappatura dei metadati, consulta [Configurare l’integrazione di Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l’integrazione di Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Esempio** La prima volta che invii una risorsa associata a un’attività, i metadati dell’attività vengono mappati su Experience Manager Assets o su Assets Essentials, nonché i metadati mappati da oggetti principali come un progetto, un portfolio e un programma.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a>*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze legacy</a>*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi disporre di Experienci Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza l'accesso o versione successiva nei documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l’integrazione di Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l’integrazione di Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Invia un documento da Workfront

Quando un utente invia un documento da Workfront a Experience Manager Assets o ad Assets Essentials, i metadati mappati vengono trasferiti lungo il documento. Dopo l’invio del documento, le modifiche apportate ai metadati del documento in Workfront non vengono riportate in Assets o Assets Essentials. Se viene modificato un campo mappato in Workfront, è necessario inviare una nuova versione del documento con i metadati aggiornati ad Assets o Assets Essentials. Per impostare o modificare i metadati, consulta [Configurare l’integrazione di Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l’integrazione di Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Per inviare un documento:

1. Vai a **Documenti** in Workfront e selezionare il documento che si desidera inviare.
1. Clic **Invia a**, quindi scegli l’integrazione di Experience Manager configurata dall’amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare in modo specifico Risorse o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Scegli dove desideri spostare la risorsa, quindi fai clic su **Seleziona cartella**.
1. Quando trovi la destinazione desiderata, fai clic su **Salva**.

## Invia una nuova versione

È possibile aggiungere una nuova versione a un documento caricato in precedenza in Workfront. Per ulteriori informazioni, consulta [Carica una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md). Una volta caricata l’ultima versione, puoi inviarla agli Assets Essentials. Se un campo mappato in Workfront è stato modificato, la nuova versione aggiorna i metadati negli Assets Essentials quando invia.

>[!IMPORTANT]
>
>Prima di caricare una nuova versione in Workfront, è consigliabile rinominare il file. Se carichi una nuova versione con lo stesso nome di file di una versione precedente, è possibile scaricare da Workfront solo la versione più recente. Tutte le versioni possono essere scaricate da Experience Manager Assets o dagli Assets Essentials indipendentemente dal nome del file.

Per inviare la versione più recente:

1. Vai a **Documenti** in Workfront e individuare il documento.
1. Seleziona **Invia a**, quindi scegli l’integrazione di Experience Manager configurata dall’amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare in modo specifico risorse o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Fai clic su **Salva**. La nuova versione viene salvata nella stessa posizione della versione precedente.

## Spostare un documento in una cartella collegata in Experience Manager Assets

>[!NOTE]
>
>Questa funzionalità è disponibile solo per Experience Manager Assets as a Cloud Service. Non è disponibile per Experience Manager Assets Essentials.

È possibile spostare un documento in una cartella collegata in Experience Manager Assets se sia il documento che la cartella collegata si trovano nello stesso elenco di documenti, ad esempio l&#39;area del documento di un progetto.

1. Individuare il documento da spostare.
1. Trascinare e rilasciare il documento nella cartella Experience Manager Assets collegata in cui si desidera spostarlo.

<div class="preview">Le opzioni del documento non sono disponibili mentre è in corso lo spostamento del documento. Una volta spostato il documento in Experience Manager Assets, non sarà più visibile nell'elenco dei documenti in Workfront.

>[!NOTE]
>
> Tutte le azioni o le modifiche apportate al documento durante lo spostamento non verranno visualizzate nel documento in Experience Manager Assets e andranno quindi perse.
</div>
