---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati personalizzati per un'attività o un problema che viene spostato o copiato
description: Quando si sposta o si copia un'attività o un problema in un progetto diverso, alcuni stati dell'attività o del problema potrebbero essere aggiornati in modo da corrispondere agli stati utilizzati dal gruppo del progetto di destinazione.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: 'https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---
# Stati personalizzati su un&#39;attività o un problema spostato o copiato

Quando si sposta o si copia un&#39;attività o un problema in un progetto diverso, alcuni stati dell&#39;attività o del problema potrebbero essere aggiornati in modo da corrispondere agli stati utilizzati dal gruppo del progetto di destinazione. Ciò dipende dal fatto che nel gruppo siano presenti stati con la stessa chiave:

* Se uno stato sull’attività o sul problema ha la stessa chiave di uno stato utilizzato dal gruppo del progetto di destinazione, lo stato sull’attività o sul problema rimane lo stesso.

  Se l’etichetta di questi due stati non corrisponde, lo stato sull’attività o sul problema eredita l’etichetta dello stato utilizzata dal gruppo del progetto di destinazione.

* Se uno stato nell’attività o nel problema non ha la stessa chiave dello stato equivalente nel gruppo del progetto di destinazione, lo stato nell’attività o nel problema cambia allo stato predefinito equivalente nel gruppo del progetto di destinazione.

Per informazioni sulle chiavi di stato, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
