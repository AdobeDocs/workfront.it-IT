---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials
description: Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials

Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o Assets Essentials. Se l&#39;amministratore di Workfront ha attivato la sincronizzazione dei metadati dell&#39;oggetto, i campi rimangono aggiornati se vengono modificati in una delle applicazioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi disporre di Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni Experience Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Collegare una risorsa da Experience Manager Assets o Assets Essentials

Puoi collegare una risorsa da Experience Manager Assets o Assets Essentials a Workfront. Una volta collegata la risorsa, puoi

* [Verifica di una risorsa collegata per Experience Manager Assets o Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Carica una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Seleziona le risorse desiderate.

   ![Seleziona una risorsa](assets/select-an-asset.png)

1. Fai clic su **Seleziona**.

## Collegare una cartella da Experience Manager Assets o Assets Essentials

Le autorizzazioni per visualizzare singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets o Assets Essentials.

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire la cartella.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Selezionare le cartelle desiderate.

   ![Seleziona una cartella](assets/select-a-folder.png)

1. Fai clic su **Seleziona**.

## Collegare una nuova versione da Experience Manager Assets o Assets Essentials

Puoi richiamare una nuova risorsa da Assets Essentials e aggiungerla a una risorsa esistente come nuova versione. Se il documento è già collegato e viene aggiunta una nuova versione in Assets Essentials, la nuova versione viene visualizzata automaticamente in Workfront.

Per collegare una nuova versione da Assets Essentials:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non puoi creare una nuova versione di una risorsa in una cartella collegata.
1. Seleziona **Aggiungi nuovo** > **Versione**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Seleziona la risorsa desiderata.

   ![Seleziona una risorsa](assets/select-an-asset.png)

1. Fai clic su **Seleziona**.

>[!TIP]
>
>Puoi visualizzare tutte le versioni di una risorsa se vai a **Dettagli documento** > **Versioni**.
