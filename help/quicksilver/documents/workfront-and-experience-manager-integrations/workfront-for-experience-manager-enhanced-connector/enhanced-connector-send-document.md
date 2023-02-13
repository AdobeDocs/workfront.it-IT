---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Invia un documento con il connettore avanzato
description: Puoi inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets continuano a essere considerati rispetto all’archiviazione dei documenti complessiva. Le risorse collegate da Experience Manager Assets non vengono conteggiate per lo storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Invia un documento con il connettore avanzato

Puoi inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets continuano a essere considerati rispetto all’archiviazione dei documenti complessiva. Le risorse collegate da Experience Manager Assets non vengono conteggiate per lo storage complessivo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
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
   <td> <p>Visualizza accesso o superiore su documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, devi

* Installa Workfront per un connettore avanzato Experience Manager.

## Invia un documento a Experience Manager Assets

Quando un utente invia un documento da Workfront a Experience Manager Assets, i metadati mappati vengono trasferiti lungo il documento. Se configurati, i metadati vengono sincronizzati continuamente ogni volta che viene apportata una modifica.

Per inviare un documento:

1. Vai a **Documenti** in Workfront e selezionare il documento che si desidera inviare.
1. Fai clic su **Invia a**, quindi scegli l’integrazione Experience Manager Assets configurata dall’amministratore.

   >[!NOTE]
   >
   >È possibile scegliere qualsiasi nome per questa integrazione, pertanto non può menzionare specificamente Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Scegli la posizione in cui desideri inserire la risorsa, quindi fai clic su **Seleziona cartella**.
1. Quando trovi la destinazione desiderata, fai clic su **Salva**.

## Inviare una nuova versione a Experience Manager Assets

È possibile aggiungere una nuova versione a un documento precedentemente caricato in Workfront. Per ulteriori informazioni, consulta [Caricare una nuova versione di un documento](../../../documents/managing-documents/upload-new-document-version.md). Dopo il caricamento dell’ultima versione, puoi inviarla a Experience Manager Assets. Se un campo mappato in Workfront è stato modificato, la nuova versione aggiorna i metadati in Experience Manager Assets quando invia.

Per inviare la versione più recente:

1. Vai a **Documenti** in Workfront e individuare il documento.
1. Fai clic su **Invia a**, quindi scegli l’integrazione Experience Manager Assets configurata dall’amministratore.

   >[!NOTE]
   >
   >È possibile scegliere qualsiasi nome per questa integrazione, pertanto non può menzionare specificamente Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Fai clic su **Salva**. La nuova versione viene salvata nella stessa posizione della versione precedente.
