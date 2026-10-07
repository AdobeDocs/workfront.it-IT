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
source-git-commit: db6d682b43caf1d28779599495b931da5c80d126
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 3%
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

## Salvare un nuovo documento in Workfront da un&#39;app Creative Cloud

È possibile salvare un nuovo file in Workfront oppure una nuova copia di un file esistente in Workfront da Photoshop, Illustrator o InDesign.

Per salvare un nuovo documento in Workfront:

1. Apri Photoshop, Illustrator o InDesign e crea un nuovo file.
1. Se salvi un nuovo file, fai clic su **Salva** nel menu principale.
Oppure
Se salvi una nuova copia di un file esistente, fai clic su **Salva con nome** nel menu principale.
1. Nella finestra di dialogo **Salva con nome**, seleziona **Salva in documenti cloud**, quindi scegli il progetto Workfront necessario.

   >[!NOTE]
   >
   >Quando si salva un documento già nel progetto Workfront, la finestra di dialogo Salva con nome non si apre. Puoi selezionare un progetto Workfront, salvarlo in un’altra cartella o scegliere un altro progetto Workfront.


   ![salva nuovo documento in workfront](assets/save-new-to-wf.png)

1. Scegli una cartella documenti, quindi fai clic su **Salva**. Se non si sceglie una cartella, il documento viene salvato nella cartella principale del progetto.

   ![scegli la cartella in cui salvare il nuovo documento](assets/save-to-folder.png)

## Richiedere un&#39;approvazione per un documento

È possibile aggiungere un’approvazione del documento in Workfront a qualsiasi documento caricato da Photoshop, Illustrator o InDesign, o da Adobe Cloud Drive, come qualsiasi altro documento. Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).



## Gestire le versioni di un documento in Workfront da un’app Creative Cloud

Quando si salva un documento da Photoshop, Illustrator o InDesign a Workfront, le modifiche salvate vengono visualizzate nel file Corrente della scheda Versioni e contrassegnate con il contrassegno &quot;Nuove modifiche&quot;.

È possibile richiedere un&#39;approvazione sul file corrente anziché caricare una nuova versione del documento. Per ulteriori informazioni, vedere [Richiedere un&#39;approvazione per il file corrente](#request-approval-on-the-current-file).

![file corrente con nuovo badge modifiche](assets/current-file.png)

### Richiedi approvazione sul file corrente

Per richiedere l&#39;approvazione del file corrente di un documento in Workfront:

1. Vai al progetto in Workfront che contiene il documento su cui desideri richiedere l’approvazione.
1. Apri il documento e passa alla scheda **Versioni**.
1. Nel file corrente, fai clic sul menu **Altro**, quindi fai clic su **Richiedi approvazione**.
1. Nella finestra di dialogo **Richiedi approvazione**, segui i passaggi descritti in [Crea un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) per creare l&#39;approvazione.

   ![richiede l&#39;approvazione per il file corrente](assets/request-update-on-current-file.png)

