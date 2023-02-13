---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Le cartelle collegate non sono supportate per l'oggetto DOCU
description: Le cartelle collegate non sono supportate per l'oggetto DOCU
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# L’utilizzo dell’API per aggiungere una cartella collegata non è supportato

L&#39;utilizzo dell&#39;API per aggiungere una cartella collegata all&#39;array delle cartelle per un oggetto Document (DOCU) non è supportato. La richiesta avrà esito positivo, ma il documento potrebbe essere rimosso dal sistema da alcuni provider esterni. Questo perché il sistema esterno sarà usato come fonte finale di verità. Pertanto, se il documento viene rimosso dal provider esterno, il documento viene considerato non più esistente. I documenti non trovati nella cartella collegata (esterna) possono essere rimossi automaticamente da [!DNL Workfront] senza alcun modo per recuperarle.
