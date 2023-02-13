---
title: Collegare risorse e cartelle con il connettore avanzato
description: Puoi collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporta i documenti.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Collegare risorse e cartelle con il connettore avanzato

Puoi collegare una risorsa o una cartella da Experience Manager Assets a qualsiasi oggetto Workfront che supporta i documenti. Le risorse inviate da Experience Manager Assets non vengono conteggiate per l’archiviazione completa dei documenti in Workfront. I documenti caricati e inviati da Workfront a Experience Manager Assets contano per lo storage complessivo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza accesso o superiore a un documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, devi

* Installare Workfront per un connettore avanzato Experience Manager

## Collegamento di una risorsa da Experience Manager Assets

Puoi collegare una risorsa da Experience Manager Assets a Workfront. Una volta collegata la risorsa, puoi

* [Prova di una risorsa collegata per Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Caricare una nuova versione di un documento](../../../documents/managing-documents/upload-new-document-version.md)

Per collegare una risorsa a Experience Manager Assets:

1. Vai a **Documenti** in Workfront in cui si desidera aggiungere il documento.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l’integrazione Experience Manager Assets configurata dall’amministratore.

   >[!NOTE]
   >
   >È possibile scegliere qualsiasi nome per questa integrazione, pertanto non può menzionare specificamente Experience Manager Assets.

1. Seleziona le risorse desiderate.

   ![](assets/select-an-asset.png)

1. Fai clic su **Collegamento**.

## Collegamento di una cartella da Experience Manager Assets

Le autorizzazioni per visualizzare le singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets.

Per collegare una cartella a Experience Manager Assets:

1. Vai a **Documenti** in Workfront in cui si desidera aggiungere il documento.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l’integrazione Experience Manager Assets configurata dall’amministratore.

   >[!NOTE]
   >
   >È possibile scegliere qualsiasi nome per questa integrazione, pertanto non può menzionare specificamente Experience Manager Assets.

1. Selezionare le cartelle desiderate.

   ![](assets/select-a-folder.png)

1. Fai clic su **Collegamento**.

## Collegamento di una nuova versione da Experience Manager Assets

Puoi estrarre una nuova risorsa da Experience Manager Assets e aggiungerla a una risorsa esistente come nuova versione in Workfront. Se il documento è già collegato e viene aggiunta una nuova versione in Experience Manager Assets, la nuova versione viene visualizzata automaticamente in Workfront.

>[!TIP]
>
>Se passi a **Dettagli documento** > **Versioni**.

Per collegare una nuova versione da Experience Manager Assets:

1. Vai a **Documenti** in Workfront in cui si desidera aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non è possibile creare una nuova versione di una risorsa in una cartella collegata.
1. Fai clic su **Aggiungi nuovo**, quindi scegli l’integrazione Experience Manager Assets configurata dall’amministratore.

   >[!NOTE]
   >
   >È possibile scegliere qualsiasi nome per questa integrazione, pertanto non può menzionare specificamente Experience Manager Assets.

1. Seleziona la risorsa desiderata.

   ![](assets/select-an-asset.png)

1. Fai clic su **Collegamento**.
