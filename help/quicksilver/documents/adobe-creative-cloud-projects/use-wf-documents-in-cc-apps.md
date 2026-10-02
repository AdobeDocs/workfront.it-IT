---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Utilizzare i documenti Workfront nelle app Creative Cloud
description: Apri, modifica e salva documenti Workfront da Photoshop, Illustrator e InDesign e richiedi le relative approvazioni.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: deeb63ceccc28b8f376713d4a6fb6c103ab4e06b
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 7%
---
# Utilizzare i documenti Workfront nelle app Creative Cloud

Quando un progetto Workfront è disponibile nel pannello Progetti Creative Cloud, potete utilizzarne i documenti direttamente da Photoshop, Illustrator o InDesign.

## Prerequisiti

* La tua organizzazione deve utilizzare una versione di Workfront che supporti l’archiviazione cloud di Adobe.
* Workfront e Photoshop, Illustrator o InDesign devono avere diritto nella stessa organizzazione Adobe Identity Management System (IMS).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versione Adobe Workfront</td> 
   <td>Flusso di lavoro di Ultimate, con l'archiviazione cloud Adobe abilitata</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td>
      <p>Accesso in visualizzazione a un progetto per visualizzarlo nel pannello Progetti Creative Cloud</p>
      <p>Modificare l’accesso a un progetto per aggiungerlo, modificarlo o eliminarlo</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedere a un progetto Workfront

La struttura di cartelle Documenti in un progetto Workfront si riflette nel pannello Progetti. Quando si apre un documento da una cartella di progetto, lo si modifica e lo si salva, le modifiche vengono visualizzate in Workfront.

>[!NOTE]
>
>I progetti di archiviazione Workfront precedenti non sono supportati nel pannello Progetti: solo progetti di archiviazione cloud Adobe.


Per accedere a un progetto Workfront in Photoshop, Illustrator o InDesign:

1. Apri Photoshop, Illustrator o InDesign.
1. Nel pannello **Progetti** sul lato sinistro dell&#39;app, seleziona il progetto Workfront che desideri aprire.

   ![Progetti Workfront elencati nel pannello Progetti](assets/cc-projects.png)

1. Aprire un documento nel progetto per modificarlo. Dopo aver salvato le modifiche, queste vengono automaticamente salvate nuovamente nel progetto Workfront.


>[!TIP]
>
>Per modificare un tipo di file che non può essere aperto da Photoshop, Illustrator o InDesign, ad esempio un documento Word o Excel, utilizza Adobe Cloud Drive. Per ulteriori informazioni, consulta [Panoramica di Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Richiedere un&#39;approvazione per un documento

È possibile aggiungere un’approvazione del documento in Workfront a qualsiasi documento caricato da Photoshop, Illustrator o InDesign, o da Adobe Cloud Drive, come qualsiasi altro documento. Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
need to verify
Creating an approval on a Creative Cloud document also creates a new version of the document. For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md#view-the-current-file-during-an-approval).
-->