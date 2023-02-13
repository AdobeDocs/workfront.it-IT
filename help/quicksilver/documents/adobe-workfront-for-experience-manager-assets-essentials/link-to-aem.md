---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials
description: Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Le risorse inviate da Assets Essentials non vengono conteggiate per l’archiviazione completa dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials sono considerati come documenti di archiviazione generale.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Collegare risorse e cartelle da Experience Manager Assets o Assets Essentials

Puoi collegare una risorsa o una cartella da Experience Manager Assets o Assets Essentials a qualsiasi oggetto Adobe Workfront che supporta i documenti. Le risorse inviate da Assets Essentials non vengono conteggiate per l’archiviazione completa dei documenti in Workfront. I documenti caricati e inviati da Workfront ad Assets Essentials sono considerati come documenti di archiviazione generale.

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o Assets Essentials. Se l’amministratore di Workfront ha abilitato la sincronizzazione dei metadati degli oggetti, i campi rimangono aggiornati se vengono modificati in entrambe le applicazioni.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi disporre di un Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni di Experienci Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza accesso o superiore</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l’integrazione as a Cloud Service di Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l’integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Collegamento di una risorsa da Experience Manager Assets o Assets Essentials

Puoi collegare una risorsa da Experience Manager Assets o Assets Essentials a Workfront. Una volta collegata la risorsa, puoi

* [Prova di una risorsa collegata per Experience Manager Assets o Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vai a **Documenti** in Workfront in cui si desidera aggiungere il documento.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l’integrazione di Experience Manager configurata dall’amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Seleziona le risorse desiderate.

   ![](assets/select-an-asset.png)

1. Fai clic su **Seleziona**.

## Collegamento di una cartella da Experience Manager Assets o Assets Essentials

Le autorizzazioni per visualizzare le singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets o Assets Essentials.

1. Vai a **Documenti** in Workfront in cui si desidera inserire la cartella.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l’integrazione di Experience Manager configurata dall’amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Selezionare le cartelle desiderate.

   ![](assets/select-a-folder.png)

1. Fai clic su **Seleziona**.

## Collegamento di una nuova versione da Experience Manager Assets o Assets Essentials

Puoi estrarre una nuova risorsa da Assets Essentials e aggiungerla a una risorsa esistente come nuova versione. Se il documento è già collegato e viene aggiunta una nuova versione in Assets Essentials, la nuova versione viene visualizzata automaticamente in Workfront.

Per collegare una nuova versione da Assets Essentials:

1. Vai a **Documenti** in Workfront in cui si desidera aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non è possibile creare una nuova versione di una risorsa in una cartella collegata.
1. Seleziona **Aggiungi nuovo** > **Versione**, quindi seleziona l’integrazione di Experience Manager configurata dall’amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Assets o Assets Essentials.

1. Seleziona la risorsa desiderata.

   ![](assets/select-an-asset.png)

1. Fai clic su **Seleziona**.

>[!TIP]
>
>Se passi a **Dettagli documento** > **Versioni**.
