---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Le cartelle collegate non sono supportate per l'oggetto DOCU
description: Le cartelle collegate non sono supportate per l'oggetto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 9%

---

# L’utilizzo dell’API per aggiungere una cartella collegata non è supportato

L&#39;utilizzo dell&#39;API per aggiungere una cartella collegata all&#39;array di cartelle per un oggetto Document (DOCU) non è supportato. La richiesta avrà esito positivo, ma alcuni provider esterni potrebbero rimuovere il documento dal sistema. Questo perché il sistema esterno sarà usato come fonte finale di verità. Pertanto, se il documento viene rimosso dal provider esterno, viene considerato come non più esistente. Tutti i documenti non trovati nella cartella collegata (esterna) possono essere rimossi automaticamente da [!DNL Workfront] senza alcun modo di recuperarli.
