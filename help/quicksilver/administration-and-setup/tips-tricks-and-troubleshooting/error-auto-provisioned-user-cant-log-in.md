---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Errore: L'utente con provisioning automatico non può effettuare l'accesso"
description: Se un utente con provisioning automatico tenta di accedere per la prima volta e riceve un errore che indica che il sistema non sta assegnando loro un livello di accesso, ciò potrebbe essere dovuto al fatto che il sistema non dispone dei livelli di accesso associati alla licenza di richiesta. Il provisioning automatico utilizza il tipo di licenza Request, per risolvere il problema creando un livello di accesso associato a una licenza Request.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Errore: L&#39;utente con provisioning automatico non può accedere

Quando un utente con provisioning automatico tenta di accedere per la prima volta, riceve il seguente errore:

## Problema

Il sistema non assegna un livello di accesso al nuovo utente.

Per impostazione predefinita, il provisioning automatico utilizza il tipo di licenza Request. Se non esistono livelli di accesso con una licenza di richiesta, il sistema non può assegnare all&#39;utente un livello di accesso.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

Crea un livello di accesso di base con una licenza di richiesta:

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Livelli di accesso]**.

1. Fai clic su **[!UICONTROL Nuovo livello di accesso]**.
1. Inserisci un **[!UICONTROL Nome]**.
1. In **[!UICONTROL Tipo di licenza]** dal menu a discesa, selezionare Richiesta.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

Dopo aver creato un livello di accesso con una licenza Request, chiedi all&#39;utente di accedere con le loro credenziali SSO.
