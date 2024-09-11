---
title: Collegare risorse e cartelle con il connettore avanzato
description: È possibile collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporti i documenti.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: dd8718b00a310bee6caa13db7644b86174b476f4
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---


# Collegare risorse e cartelle con il connettore avanzato

È possibile collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporti i documenti. Assets inviato da Experience Manager Assets non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono conteggiati ai fini dell’archiviazione complessiva.


>[!NOTE]
>
>I file Excel collegati tramite il connettore avanzato non possono essere visualizzati in anteprima in Workfront. È necessario scaricare il file per accedervi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Corrente: richiesta o successiva</p> 
   oppure
   <p>Nuovo: Collaboratore o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o superiore in un documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.
+++

## Prerequisiti

Prima di iniziare, è necessario

* Installare Workfront, ad Experience Manager il connettore avanzato

## Collegare una risorsa da Experience Manager Assets

Puoi collegare una risorsa da Experience Manager Assets a Workfront. Una volta collegata la risorsa, puoi

* [Verifica di una risorsa collegata per Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Carica una nuova versione di un documento](../../../documents/managing-documents/upload-new-document-version.md)

Per collegare una risorsa a Experience Manager Assets:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l&#39;integrazione Experience Manager Assets configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >Qualsiasi nome può essere scelto per questa integrazione, quindi potrebbe non menzionare specificamente Experience Manager Assets.

1. Seleziona le risorse desiderate.

   ![](assets/select-an-asset.png)

1. Fai clic su **Collegamento**.

## Collegare una cartella da Experience Manager Assets

Le autorizzazioni per visualizzare singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets.

Per collegare una cartella a Experience Manager Assets:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l&#39;integrazione Experience Manager Assets configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >Qualsiasi nome può essere scelto per questa integrazione, quindi potrebbe non menzionare specificamente Experience Manager Assets.

1. Selezionare le cartelle desiderate.

   ![](assets/select-a-folder.png)

1. Fai clic su **Collegamento**.

## Collega una nuova versione da Experience Manager Assets

Puoi richiamare una nuova risorsa da Experience Manager Assets e aggiungerla a una risorsa esistente come nuova versione in Workfront. Se il documento è già collegato e viene aggiunta una nuova versione in Experience Manager Assets, la nuova versione viene visualizzata automaticamente in Workfront.

>[!TIP]
>
>Puoi visualizzare tutte le versioni di una risorsa se vai a **Dettagli documento** > **Versioni**.

Per collegare una nuova versione da Experience Manager Assets:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non puoi creare una nuova versione di una risorsa in una cartella collegata.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l&#39;integrazione Experience Manager Assets configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >Qualsiasi nome può essere scelto per questa integrazione, quindi potrebbe non menzionare specificamente Experience Manager Assets.

1. Seleziona la risorsa desiderata.

   ![](assets/select-an-asset.png)

1. Fai clic su **Collegamento**.
