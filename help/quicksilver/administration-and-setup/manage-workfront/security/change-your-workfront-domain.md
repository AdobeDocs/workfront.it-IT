---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Cambia il dominio di Adobe Workfront
description: In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 51d0989bdbf4ecdc799658f30500c68bf5867e65
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 17%

---

# Modificare il dominio di Adobe Workfront

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in Admin Console. Poiché tutte le organizzazioni sono ora state caricate in Adobe Admin Console, **non è possibile modificare il dominio Workfront**.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>Questo articolo verrà rimosso a breve.

In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Richiedi modifica dominio

1. Inizia a creare un ticket di supporto su Experience League.
1. Nella casella **Descrizione** includere il nuovo dominio desiderato e l&#39;intervallo di tempo in cui si desidera che il nuovo dominio venga attivato.
1. Completare la compilazione delle caselle relative al caso di supporto, quindi fare clic su **Invia**.

È inoltre possibile chiamare il supporto tecnico Workfront per ottenere assistenza nella modifica del dominio.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
