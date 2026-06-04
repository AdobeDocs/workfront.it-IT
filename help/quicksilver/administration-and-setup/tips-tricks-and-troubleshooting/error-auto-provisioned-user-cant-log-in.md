---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Errore: l''utente con provisioning automatico non può accedere'
description: Se un utente con provisioning automatico tenta di accedere per la prima volta e riceve un errore che indica che il sistema non sta assegnando loro un livello di accesso, è possibile che il sistema non disponga di livelli di accesso associati alla licenza Request.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 15%

---

# Errore: l&#39;utente con provisioning automatico non può accedere

Quando un utente con provisioning automatico tenta di accedere per la prima volta, riceve il seguente errore:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

Il sistema non sta assegnando al nuovo utente un livello di accesso.

Per impostazione predefinita, il provisioning automatico utilizza il tipo di licenza Richiesta. Se non esiste alcun livello di accesso con una licenza Request, il sistema non può assegnare all&#39;utente un livello di accesso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

Creare un livello di accesso di base con una licenza Request:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Livelli di accesso]**.

1. Fai clic su **[!UICONTROL Nuovo livello di accesso]**.
1. Immetti un **[!UICONTROL Nome]**.
1. Nel menu a discesa **[!UICONTROL License Type]**, selezionare Request.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

Dopo aver creato un livello di accesso con una licenza Request, chiedi all&#39;utente di accedere con le proprie credenziali SSO.


