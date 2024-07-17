---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Disattivare un utente tramite l’API
description: Disattivare un utente tramite l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Disattivare un utente tramite l’API

Quando un utente lascia l’organizzazione, puoi disattivarlo, rendendo la licenza Adobe Workfront disponibile per un altro utente ed evitando che venga inavvertitamente assegnato loro un lavoro. La disattivazione di un utente consente di conservarne la cronologia di lavoro, incluse le assegnazioni di lavoro e l&#39;associazione con note, ore e documenti.

Per ulteriori informazioni sulla disattivazione di un utente, vedere &quot; [Disattivare o riattivare un utente](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Per informazioni sull&#39;utilizzo dell&#39;API core, vedere [Nozioni di base sull&#39;API](../../wf-api/general/api-basics.md).

Per disattivare un utente tramite l’API:

1. Genera una chiave API utilizzando la seguente richiesta API:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Individuare il GUID per l&#39;utente che si desidera disattivare.

   1. Utilizza la seguente richiesta API per recuperare il GUID per tutti gli utenti nel tuo sistema. Il campo **isActive** mostra **true** per gli utenti attualmente attivi e **false** per gli utenti che sono stati disattivati:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Individua il GUID per l&#39;utente che desideri disattivare. Utilizza la seguente richiesta di **PUT** per modificare il valore del campo **isActive** dell&#39;utente in **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La risposta mostrerà che il valore del campo **isActive** è cambiato da **true** a **false** indicando che l&#39;utente è stato disattivato:

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
