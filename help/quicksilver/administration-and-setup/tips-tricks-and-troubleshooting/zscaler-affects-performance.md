---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Le impostazioni ZScaler possono causare una riduzione delle prestazioni
description: Dopo la creazione dell’utente, puoi modificarlo e abilitare "Only Allow SAML 2.0 Authentication" (Consenti solo autenticazione SAML 2.0) in modo che l’utente e la password siano controllati dal sistema SAML. Se questa opzione è abilitata, l’utente può accedere solo tramite SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: le impostazioni ZScaler possono causare una riduzione delle prestazioni

>[!NOTE]
>
>Si tratta di un problema relativo a ZScaler che non verrà risolto da Workfront.

Il servizio Web di ZScaler utilizza `http/1.1` per impostazione predefinita, che può causare una riduzione delle prestazioni in Workfront.

Per verificare e risolvere il problema, configurare il software ZScaler per l&#39;utilizzo di `http/2`. Questo non può essere configurato in Workfront.

Per informazioni su `http/2`, vedere la documentazione di ZScaler.
