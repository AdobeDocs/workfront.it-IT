---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati personalizzati su un'attività o un problema spostato o copiato
description: Quando si sposta o si copia un'attività o un problema in un progetto diverso, alcuni stati dell'attività o del problema potrebbero essere aggiornati in modo da corrispondere agli stati utilizzati dal gruppo del progetto di destinazione.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
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
