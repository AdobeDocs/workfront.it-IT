---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gli amministratori dei gruppi devono avere un accesso più elevato rispetto a quelli che gestiscono
description: Se un amministratore di gruppo dispone di autorizzazioni nel livello di accesso inferiore a quelle gestite, non sarà in grado di visualizzare, modificare o assegnare livelli di accesso inferiori.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Gli amministratori dei gruppi devono avere un accesso più elevato rispetto a quelli che gestiscono

Se un amministratore di gruppo dispone di autorizzazioni nel livello di accesso inferiore a quelle gestite, non sarà in grado di visualizzare, modificare o assegnare livelli di accesso inferiori.

## Problema

Se a un amministratore del gruppo viene assegnato un livello di accesso modificato al planner con le autorizzazioni di visualizzazione per i team, ma ad alcuni utenti viene assegnato un livello di accesso di lavoro con le autorizzazioni di modifica per i team, l&#39;amministratore del gruppo non sarà in grado di interagire con il livello di accesso di Worker modificato.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Questa logica si applica anche al menu a discesa Ottimizza le impostazioni . Entrambi i livelli di accesso possono avere accesso a Modifica , ma le impostazioni nel menu a discesa Ottimizza le impostazioni devono essere più alte per l&#39;amministratore del gruppo.
> ![](assets/fine-tune-your-settings.png)

## Soluzione

Gli amministratori dei gruppi devono disporre di autorizzazioni più elevate in tutte le aree del livello di accesso rispetto a quelle gestite.