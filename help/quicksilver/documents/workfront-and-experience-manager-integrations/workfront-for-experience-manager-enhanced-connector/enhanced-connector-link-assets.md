---
title: Collegare risorse e cartelle con il connettore avanzato
description: È possibile collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporti i documenti.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---


# Collegare risorse e cartelle con il connettore avanzato

È possibile collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporti i documenti. Assets inviato da Experience Manager Assets non viene conteggiato per l’archiviazione complessiva dei documenti in Workfront. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono conteggiati ai fini dell’archiviazione complessiva.


>[!NOTE]
>
>I file Excel collegati tramite il connettore avanzato non possono essere visualizzati in anteprima in Workfront. È necessario scaricare il file per accedervi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o superiore in un documento</p> </td> 
  </tr> 
 </tbody> 
</table>


Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario

* Installare il connettore avanzato di Workfront for Experience Manager

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

   ![Seleziona una risorsa](assets/select-an-asset.png)

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

   ![Seleziona una cartella](assets/select-a-folder.png)

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

   ![Seleziona una risorsa](assets/select-an-asset.png)

1. Fai clic su **Collegamento**.
