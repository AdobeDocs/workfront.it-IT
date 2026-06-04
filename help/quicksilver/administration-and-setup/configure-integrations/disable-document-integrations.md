---
title: Disabilita integrazioni documenti
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: In qualità di amministratore  [!DNL anAdobe] [!DNL Workfront], puoi disabilitare la connessione tra Workfront e qualsiasi provider di documenti di terze parti.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
TQID: https://experienceleague.adobe.com/3tfxxth82eJEjEmdVD3AJFxl6B1m3EVKMQP9Gy4LC24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 13%

---

# Disabilitare le integrazioni di documenti

In qualità di amministratore [!DNL Adobe] [!DNL Workfront], puoi disabilitare la connessione tra [!DNL Workfront] e qualsiasi provider di documenti di terze parti.

Quando si disattiva la connessione tra [!DNL Workfront] e un provider di documenti, i collegamenti ai documenti scompaiono da [!DNL Workfront]. Gli utenti non possono più visualizzare i documenti collegati, non possono apportare modifiche ai documenti tramite i collegamenti [!DNL Workfront] e non possono aggiungere altri documenti a tale provider.

## Requisiti di accesso

+++Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Flusso di lavoro Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licenze Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Piano</p>
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Disabilita integrazioni provider cloud

Per disabilitare le integrazioni dei documenti per [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Accedere a [!DNL Workfront] come amministratore [!DNL Workfront].

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider cloud]**.

1. Deselezionare uno dei provider cloud da cui si desidera disconnettersi da [!DNL Workfront].
1. Fai clic su **[!UICONTROL Salva]**.

   Gli utenti non possono connettersi al provider cloud specifico disabilitato e non possono più collegare i documenti da tale provider cloud a Workfront.

## Disattiva l&#39;integrazione di [!DNL SharePoint]

1. Accedere a [!DNL Workfront] come amministratore [!DNL Workfront].

{{step-1-to-setup}}

1. Espandere **[!UICONTROL Documenti]**, quindi fare clic su **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Selezionare l&#39;integrazione di [!DNL SharePoint] da disabilitare.
1. Fare clic su **[!UICONTROL Disattiva]**.\
   Gli utenti non possono connettersi al sito [!DNL SharePoint] disabilitato e non possono più collegare documenti da [!DNL SharePoint] a [!DNL Workfront].

## Disattiva integrazioni personalizzate

1. Accedere a [!DNL Workfront] come amministratore.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata]**.
1. Seleziona l’integrazione personalizzata da disabilitare.
1. Fare clic su **[!UICONTROL Disattiva]**.

   Gli utenti non possono connettersi al provider di documenti di terze parti disabilitato e non possono più collegare i documenti da tale provider di cloud a [!DNL Workfront].
