---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Errore: l’utente con provisioning automatico non può accedere"
description: Se un utente con provisioning automatico tenta di accedere per la prima volta e riceve un errore che indica che il sistema non sta assegnando loro un livello di accesso, è possibile che il sistema non disponga di livelli di accesso associati alla licenza Request. Il provisioning automatico utilizza il tipo di licenza Richiesta, pertanto puoi risolvere il problema creando un livello di accesso associato a una licenza Richiesta.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Errore: l&#39;utente con provisioning automatico non può accedere

Quando un utente con provisioning automatico tenta di accedere per la prima volta, riceve il seguente errore:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

Il sistema non sta assegnando al nuovo utente un livello di accesso.

Per impostazione predefinita, il provisioning automatico utilizza il tipo di licenza Richiesta. Se non esiste alcun livello di accesso con una licenza Request, il sistema non può assegnare all&#39;utente un livello di accesso.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

Creare un livello di accesso di base con una licenza Request:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Livelli di accesso]**.

1. Clic **[!UICONTROL Nuovo livello di accesso]**.
1. Immetti un **[!UICONTROL Nome]**.
1. In **[!UICONTROL Tipo di licenza]** dal menu a discesa, seleziona Request.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

Dopo aver creato un livello di accesso con una licenza Request, chiedi all&#39;utente di accedere con le proprie credenziali SSO.


