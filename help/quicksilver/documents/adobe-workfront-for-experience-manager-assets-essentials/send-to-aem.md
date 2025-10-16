---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Inviare un documento a Experience Manager Assets o Assets Essentials
description: Puoi inviare documenti da Workfront a Experience Manager Assets o Assets Essentials. I documenti caricati e inviati da Workfront ad Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. I collegamenti Assets da Assets Essentials non vengono considerati ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Inviare un documento a Experience Manager Assets o Assets Essentials

Puoi inviare documenti da Workfront a Experience Manager Assets o Assets Essentials. I documenti caricati e inviati da Workfront ad Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. I collegamenti Assets da Assets Essentials non vengono considerati ai fini dello storage complessivo.

Assets inviato ad Experience Manager tramite questa integrazione ha un limite di dimensioni di **5 GB**.

Nell&#39;ambiente di anteprima, Assets inviato ad Experience Manager tramite questa integrazione ha un limite di dimensioni di **30 GB**.

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o Assets Essentials. Vengono inviati anche tutti i metadati configurati per la mappatura degli oggetti principali. Per ulteriori informazioni sulla configurazione del mapping dei metadati, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Esempio** Quando invii una risorsa associata a un&#39;attività, i metadati dell&#39;attività vengono mappati su Experience Manager Assets o Assets Essentials, nonché i metadati mappati da oggetti principali come un progetto, un portfolio e un programma.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Devi disporre di Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni Experience Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Invia un documento da Workfront

Quando un utente invia un documento da Workfront a Experience Manager Assets o Assets Essentials, i metadati mappati vengono trasferiti lungo il documento. Dopo l’invio del documento, le modifiche apportate ai metadati del documento in Workfront non vengono applicate in Assets o Assets Essentials. Se viene modificato un campo mappato in Workfront, devi inviare una nuova versione del documento con i metadati aggiornati ad Assets o Assets Essentials. Per impostare o modificare i metadati, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Per inviare un documento:

1. Vai all&#39;area **Documenti** in Workfront e seleziona il documento che desideri inviare.
1. Fai clic su **Invia a**, quindi scegli l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

   ![Invia a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Scegli dove vuoi spostare la risorsa, quindi fai clic su **Seleziona cartella**.
1. Quando trovi la destinazione desiderata, fai clic su **Salva**.

## Invia una nuova versione

È possibile aggiungere una nuova versione a un documento caricato in precedenza in Workfront. Per ulteriori informazioni, vedere [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md). Una volta caricata la versione più recente, puoi inviarla ad Assets Essentials. Se un campo mappato in Workfront è stato modificato, la nuova versione aggiorna i metadati in Assets Essentials quando invia.

>[!IMPORTANT]
>
>Prima di caricare una nuova versione in Workfront, è consigliabile rinominare il file. Se carichi una nuova versione con lo stesso nome di file di una versione precedente, è possibile scaricare da Workfront solo la versione più recente. Tutte le versioni possono essere scaricate da Experience Manager Assets o Assets Essentials indipendentemente dal nome del file.

Per inviare la versione più recente:

1. Vai all&#39;area **Documenti** in Workfront e individua il documento.
1. Seleziona **Invia a**, quindi scegli l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

   ![Invia a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Fai clic su **Salva**. La nuova versione viene salvata nella stessa posizione della versione precedente.

## Spostare un documento in una cartella collegata in Experience Manager Assets

>[!NOTE]
>
>Questa funzionalità è disponibile solo per Experience Manager Assets as a Cloud Service. Non è disponibile per Experience Manager Assets Essentials.

È possibile spostare un documento in una cartella collegata in Experience Manager Assets se sia il documento che la cartella collegata si trovano nello stesso elenco di documenti, ad esempio l&#39;area del documento di un progetto.

1. Individuare il documento da spostare.
1. Trascinare e rilasciare il documento nella cartella Experience Manager Assets collegata in cui si desidera spostarlo.

Le opzioni del documento non sono disponibili mentre è in corso lo spostamento del documento. Una volta spostato il documento in Experience Manager Assets, non sarà più visibile nell&#39;elenco dei documenti in Workfront.

>[!NOTE]
>
> Tutte le azioni o le modifiche apportate al documento durante lo spostamento non verranno visualizzate nel documento in Experience Manager Assets e andranno quindi perse.

