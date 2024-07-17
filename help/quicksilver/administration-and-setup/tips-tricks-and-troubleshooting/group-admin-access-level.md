---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gli amministratori dei gruppi devono disporre di un accesso più elevato rispetto a quelli che gestiscono
description: Se un amministratore gruppo dispone di autorizzazioni nel proprio livello di accesso inferiori a quelle gestite, non potrà visualizzare, modificare o assegnare livelli di accesso inferiori.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Gli amministratori dei gruppi devono disporre di un accesso più elevato rispetto a quelli che gestiscono

Se un amministratore gruppo dispone di autorizzazioni nel proprio livello di accesso inferiori a quelle gestite, non potrà visualizzare, modificare o assegnare livelli di accesso inferiori.

## Problema

Se a un amministratore gruppo viene assegnato un livello di accesso Planner modificato con autorizzazioni di visualizzazione per i team, ma ad alcuni utenti viene assegnato un livello di accesso Worker con autorizzazioni di modifica per i team, l&#39;amministratore gruppo non potrà interagire con il livello di accesso Worker modificato.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Questa logica si applica anche al menu a discesa Ottimizza impostazioni. Entrambi i livelli di accesso possono disporre dell’accesso di modifica, ma le impostazioni nel menu a discesa Ottimizza impostazioni devono essere più alte per l’amministratore del gruppo.
> ![](assets/fine-tune-your-settings.png)

## Soluzione

Gli amministratori dei gruppi devono disporre di autorizzazioni più elevate in tutte le aree del livello di accesso rispetto a quelle che gestiscono.
