---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Richiedi un documento
description: You can request a document on any object that supports Documents.
author: Courtney
feature: Digital Content and Documents
exl-id: 228b53ba-4a87-4edd-b478-501b216c4a1d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 10%

---

# Request a document

You can request a document on any object that supports Documents.

>[!NOTE]
>
>Questa funzionalità non è disponibile nell&#39;area nuovi documenti.<br>
>Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> 
   <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Request a document

1. Go to the area where you want the document you are requesting to reside.
1. Click the **Documents** tab. 
1. Click the **Add New** drop-down menu.

1. Click **Request a Document**.

   The Request a Document dialog box is displayed.

   ![document_request.png](assets/document-request-350x242.png)

1. Begin typing the name of the user who you are requesting the document from, then select it when it appears in the drop-down list. Only licensed Adobe Workfront users appear as options in the drop-down list.

   >[!NOTE]
   >
   >If you have the [Legacy licenses overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) enabled on your account, you can send a request to any email address. There is a setting in the [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) that determines whether or not these external email users need to create a password before interacting with Workfront. 

1. Describe the reason you are requesting the document.
1. Click **Send Request**.

   When you make a request to a user, a placeholder is added in the documents area. You can remind the user or cancel the request from this placeholder. The user receives a Workfront notification and an email about the request.

   The user receives an email notification if this preference is enabled, as well as an in-app notification. For more information on email notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   You can click the link found in the email notification, and then upload the document. Or you can click the in-app notification. Each option routes you to the user profile page where you can upload the requested document.

1. After you upload the document, the person who requested it can access the document in their personal **Documents** area.

   You can access your personal **Documents** area by clicking your user profile picture in the upper-right corner of any Workfront page, clicking your name, then clicking the **Documents** tab.
