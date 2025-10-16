---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials
description: Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials

Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o Assets Essentials. Se l&#39;amministratore di Workfront ha attivato la sincronizzazione dei metadati dell&#39;oggetto, i campi rimangono aggiornati se vengono modificati in una delle applicazioni.

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
