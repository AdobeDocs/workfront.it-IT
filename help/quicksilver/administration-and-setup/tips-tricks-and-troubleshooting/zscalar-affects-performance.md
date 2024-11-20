---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Le impostazioni ZScalar possono causare una riduzione delle prestazioni
description: Dopo la creazione dell’utente, puoi modificarlo e abilitare "Only Allow SAML 2.0 Authentication" (Consenti solo autenticazione SAML 2.0) in modo che l’utente e la password siano controllati dal sistema SAML. Se questa opzione è abilitata, l’utente può accedere solo tramite SAML.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: le impostazioni ZScalar possono causare una riduzione delle prestazioni

>[!NOTE]
>
>Questo è un problema relativo a ZScalar e non verrà risolto da Workfront.

Il servizio Web di ZScalar utilizza `http/1.1` per impostazione predefinita, che può causare una riduzione delle prestazioni in Workfront.

Per verificare e risolvere il problema, configurare il software ZScalar per l&#39;utilizzo di `http/2`. Questo non può essere configurato in Workfront.

Puoi trovare informazioni su `http/2` nella documentazione di ZScalar.
