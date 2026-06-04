---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gli amministratori di gruppi devono avere un accesso più elevato rispetto a quelli che gestiscono
description: Se un amministratore di gruppo dispone di autorizzazioni nel proprio livello di accesso inferiori a quelle gestite, non potrà visualizzare, modificare o assegnare livelli di accesso inferiori.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
ht-degree: 7%

---

# Gli amministratori dei gruppi devono disporre di un accesso superiore rispetto a quelli che gestiscono

Se un amministratore di gruppo dispone di autorizzazioni nel proprio livello di accesso inferiori a quelle gestite, non potrà visualizzare, modificare o assegnare livelli di accesso inferiori.

## Problema

Se a un amministratore gruppo viene assegnato un livello di accesso Planner modificato con autorizzazioni di visualizzazione per i team, ma ad alcuni utenti viene assegnato un livello di accesso Worker con autorizzazioni di modifica per i team, l&#39;amministratore gruppo non potrà interagire con il livello di accesso Worker modificato.

![Accesso modificato dall&#39;amministratore del gruppo](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Questa logica si applica anche al menu a discesa Ottimizza impostazioni. Entrambi i livelli di accesso possono disporre dell’accesso di modifica, ma le impostazioni nel menu a discesa Ottimizza impostazioni devono essere più alte per l’amministratore del gruppo.
> ![Ottimizza le impostazioni](assets/fine-tune-your-settings.png)

## Soluzione

Gli amministratori dei gruppi devono disporre di autorizzazioni più elevate in tutte le aree del livello di accesso rispetto a quelle che gestiscono.
