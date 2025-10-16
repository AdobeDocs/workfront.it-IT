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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 3%

---

# Errore: l&#39;utente con provisioning automatico non può accedere

Quando un utente con provisioning automatico tenta di accedere per la prima volta, riceve il seguente errore:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

Il sistema non sta assegnando al nuovo utente un livello di accesso.

Per impostazione predefinita, il provisioning automatico utilizza il tipo di licenza Richiesta. Se non esiste alcun livello di accesso con una licenza Request, il sistema non può assegnare all&#39;utente un livello di accesso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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


