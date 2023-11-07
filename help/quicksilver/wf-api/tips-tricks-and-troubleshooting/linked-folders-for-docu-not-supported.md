---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Le cartelle collegate non sono supportate per l'oggetto DOCU
description: Le cartelle collegate non sono supportate per l'oggetto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# L’utilizzo dell’API per aggiungere una cartella collegata non è supportato

L&#39;utilizzo dell&#39;API per aggiungere una cartella collegata all&#39;array di cartelle per un oggetto Document (DOCU) non è supportato. La richiesta avrà esito positivo, ma alcuni provider esterni potrebbero rimuovere il documento dal sistema. Questo perché il sistema esterno sarà usato come fonte finale di verità. Pertanto, se il documento viene rimosso dal provider esterno, viene considerato come non più esistente. Tutti i documenti non trovati nella cartella collegata (esterna) possono essere rimossi automaticamente da [!DNL Workfront] senza alcun modo per recuperarli.
