---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Disattivazione di un utente tramite API
description: Disattivazione di un utente tramite API
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Disattivazione di un utente tramite API

Quando un utente lascia l’organizzazione, puoi disattivare l’utente, rendere disponibile la propria licenza Adobe Workfront per un altro utente e impedire che venga loro assegnato inavvertitamente il lavoro. Disattivando un utente, è possibile conservare la cronologia del lavoro, incluse le assegnazioni di lavoro e la relativa associazione a note, ore e documenti.

Per ulteriori informazioni sulla disattivazione di un utente, consulta &quot; [Disattivare o riattivare un utente](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Per informazioni sull’utilizzo dell’API core, consulta [Nozioni di base sulle API](../../wf-api/general/api-basics.md).

Per disattivare un utente tramite l’API:

1. Genera una chiave API utilizzando la seguente richiesta API:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Individuare il GUID dell&#39;utente da disattivare.

   1. Utilizza la seguente richiesta API per recuperare il GUID per tutti gli utenti del sistema, tieni presente che **isActive** mostre dei campi **true** per gli utenti attualmente attivi e **false** per gli utenti disattivati:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Individuare il GUID per l&#39;utente da disattivare, utilizzare quanto segue **PUT** richiesta di modifica del **isActive** valore campo a **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La risposta mostrerà che il **isActive** il valore del campo è stato modificato da **true** a **false** indica che l’utente è stato disattivato:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
