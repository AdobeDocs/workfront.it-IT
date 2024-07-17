---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Archiviazione di campi in formato Rich Text nell’API
description: Se un oggetto come un progetto, un problema o un’attività contiene testo formattato, questo viene memorizzato e accessibile come valore di parametro tramite l’API Workfront.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Archiviazione di campi in formato Rich Text nell’API

Se un oggetto come un progetto, un problema o un’attività contiene testo formattato, questo viene memorizzato e accessibile come valore di parametro tramite l’API Workfront.

È possibile richiedere informazioni di testo da un oggetto di progetto che contiene testo RTF utilizzando il campo **parameterValues**.

Ad esempio, una semplice richiesta HTTP potrebbe essere simile alla seguente:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Se questo progetto di esempio contiene un modulo personalizzato con 3 campi personalizzati: campo di calcolo, testo di paragrafo e RTF 1. La richiesta precedente restituirebbe quindi una risposta simile alla seguente, in cui il campo &quot;rich 1&quot; è un campo con parametri Rich Text e il valore del testo è &quot;**Hello** *World!*&quot;:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Per informazioni più approfondite sulla memorizzazione e il recupero delle informazioni in formato Rich Text tramite l&#39;API Adobe Workfront, vedere [Campi Rich Text nell&#39;API Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
