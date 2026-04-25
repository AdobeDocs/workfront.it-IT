---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Collegare risorse e cartelle da Experience Manager Assets Essentials
description: Puoi collegare una risorsa o una cartella da Experience Manager Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 0b93f6f6-cf4b-4077-a464-be7f19f7cd25
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 12%

---

# Collegare risorse e cartelle da Experience Manager Assets Essentials

Puoi collegare una risorsa o una cartella da Experience Manager Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti.

Per collegare risorse e cartelle da Experience Manager Assets utilizzando Contenuto verificato, vedere [Collegare risorse e cartelle con Contenuto verificato basato su Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

Se ti trovi nell&#39;archiviazione aziendale, consulta [Utilizzare Adobe Experience Manager con l&#39;integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

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
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
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
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare:

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l&#39;integrazione di Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Collegare una risorsa da Experience Manager Assets Essentials

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets Essentials.

1. Seleziona le risorse desiderate.

   ![Seleziona una risorsa](assets/select-an-asset.png)

1. Fai clic su **Seleziona**.

## Collega una nuova versione da Experience Manager Assets Essentials

Puoi richiamare una nuova risorsa da Experience Manager Assets Essentials e aggiungerla a una risorsa esistente come nuova versione. Se il documento è già collegato e viene aggiunta una nuova versione in Experience Manager Assets Essentials, la nuova versione viene visualizzata automaticamente in Workfront.

Per collegare una nuova versione:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non puoi creare una nuova versione di una risorsa in una cartella collegata.
1. Seleziona **Aggiungi nuovo** > **Versione**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets Essentials.

1. Seleziona la risorsa da collegare.

1. Fai clic su **Seleziona**.

## Collegare una cartella da Experience Manager Assets Essentials

Le autorizzazioni per visualizzare singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets Essentials.

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire la cartella.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets Essentials.

1. Selezionare le cartelle desiderate.

   ![Seleziona una cartella](assets/select-a-folder.png)

1. Fai clic su **Seleziona**.

## Considerazioni

* La funzionalità Contenuto verificato non è disponibile per Assets Essentials. Per collegare risorse e cartelle tramite Contenuto verificato, vedere [Collegare risorse e cartelle con Contenuto verificato basato su Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Assets inviato da Assets Essentials non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials vengono conteggiati ai fini dello storage complessivo.

* I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets Essentials. Se l&#39;amministratore di Workfront ha attivato la sincronizzazione dei metadati dell&#39;oggetto, i campi rimangono aggiornati se vengono modificati in una delle applicazioni.
