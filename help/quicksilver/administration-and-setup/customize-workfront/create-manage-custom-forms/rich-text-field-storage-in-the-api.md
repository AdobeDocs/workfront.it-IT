---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Archiviazione di campi RTF nell’API
description: Se un oggetto come un progetto, un problema o un'attività contiene testo RTF, viene memorizzato e accessibile come valore di parametro tramite l'API Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Archiviazione di campi RTF nell’API

Se un oggetto come un progetto, un problema o un&#39;attività contiene testo RTF, viene memorizzato e accessibile come valore di parametro tramite l&#39;API Workfront.

È possibile richiedere informazioni testuali da un oggetto di progetto contenente testo RTF utilizzando il campo . **parameterValues**.

Ad esempio, una semplice richiesta HTTP potrebbe essere simile alla seguente:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Se questo progetto di esempio contiene un modulo personalizzato con 3 campi personalizzati: campo calc, testo paragrafo e rich 1. Quindi la richiesta di cui sopra restituirà una risposta che assomiglia al seguente, dove il campo &quot;rich 1&quot; è un campo di parametro di testo RTF e il valore di testo è &quot;**Ciao** *Mondo!*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
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
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

Per informazioni più approfondite sulla memorizzazione e sul recupero delle informazioni Rich Text tramite l’API di Adobe Workfront, consulta [Campi di testo RTF nell’API di Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
