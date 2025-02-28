---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Inviare un documento con il connettore avanzato
description: È possibile inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono comunque conteggiati rispetto all’archiviazione complessiva dei documenti. Assets collegato da Experience Manager Assets non viene considerato ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# Inviare un documento con il connettore avanzato

È possibile inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono comunque conteggiati rispetto all’archiviazione complessiva dei documenti. Assets collegato da Experience Manager Assets non viene considerato ai fini dello storage complessivo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
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
   <td> <p>Visualizza l'accesso o versione successiva nei documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Prima di iniziare, è necessario

* Installa il connettore avanzato Workfront for Experience Manager.

## Inviare un documento a Experience Manager Assets

Quando un utente invia un documento da Workfront a Experience Manager Assets, i metadati mappati vengono trasferiti lungo il documento. Se configurati, i metadati vengono sincronizzati continuamente ogni volta che viene apportata una modifica.

Per inviare un documento:

1. Vai all&#39;area **Documenti** in Workfront e seleziona il documento che desideri inviare.
1. Fai clic su **Invia a**, quindi scegli l&#39;integrazione Experience Manager Assets configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >Qualsiasi nome può essere scelto per questa integrazione, quindi potrebbe non menzionare specificamente Experience Manager Assets.

   ![Invia a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Scegli dove vuoi spostare la risorsa, quindi fai clic su **Seleziona cartella**.
1. Quando trovi la destinazione desiderata, fai clic su **Salva**.

## Invia una nuova versione a Experience Manager Assets

È possibile aggiungere una nuova versione a un documento caricato in precedenza in Workfront. Per ulteriori informazioni, vedere [Caricare una nuova versione di un documento](../../../documents/managing-documents/upload-new-document-version.md). Una volta caricata l’ultima versione, puoi inviarla a Experience Manager Assets. Se un campo mappato in Workfront è stato modificato, la nuova versione aggiorna i metadati in Experience Manager Assets al momento dell’invio.

Per inviare la versione più recente:

1. Vai all&#39;area **Documenti** in Workfront e individua il documento.
1. Fai clic su **Invia a**, quindi scegli l&#39;integrazione Experience Manager Assets configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >Qualsiasi nome può essere scelto per questa integrazione, quindi potrebbe non menzionare specificamente Experience Manager Assets.

   ![Invia a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Fai clic su **Salva**. La nuova versione viene salvata nella stessa posizione della versione precedente.
