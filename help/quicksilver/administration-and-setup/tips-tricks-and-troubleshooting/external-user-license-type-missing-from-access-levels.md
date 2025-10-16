---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Tipo di licenza per utente esterno mancante dai livelli di accesso
description: Non è più possibile visualizzare il tipo di licenza per utente esterno in Livelli di accesso in Configurazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# Tipo di licenza utente esterno mancante dai livelli di accesso

## Problema

Non è più possibile visualizzare il tipo di licenza per utente esterno in Livelli di accesso in Configurazione.

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

1. Vai a **[!UICONTROL Configurazione]** > **[!UICONTROL Sistema]** > **[!UICONTROL Preferenze]**.

1. Nella sezione **[!UICONTROL Sicurezza]**, assicurati che sia abilitata l&#39;opzione **[!UICONTROL Collaborare con persone senza account Workfront utilizzando il loro indirizzo e-mail]**.

   Se questa opzione non è abilitata, l&#39;utente esterno non viene visualizzato in Configurazione del livello di accesso.
