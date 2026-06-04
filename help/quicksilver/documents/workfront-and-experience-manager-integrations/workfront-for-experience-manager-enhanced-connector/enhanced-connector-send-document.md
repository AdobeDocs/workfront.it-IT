---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Inviare un documento con il connettore avanzato
description: È possibile inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono comunque conteggiati rispetto all’archiviazione complessiva dei documenti. Assets collegato da Experience Manager Assets non viene considerato ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
TQID: https://experienceleague.adobe.com/tu4blsoJGh2ilDeTIwqdx4xtmuC-1OOnZ2QySDNnQpI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 15%

---

# Inviare un documento con il connettore avanzato

È possibile inviare documenti da Workfront a Experience Manager Assets. I documenti caricati e inviati da Workfront a Experience Manager Assets vengono comunque conteggiati rispetto all’archiviazione complessiva dei documenti. Assets collegato da Experience Manager Assets non viene considerato ai fini dello storage complessivo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso in modifica ai documenti</p> s="MCXref xref"&gt;Crea o modifica livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizza l'accesso o versione successiva nei documenti</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

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
