---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: visualizzare la relazione padre-figlio in un''attività applicando un rientro alle attività'
description: È possibile mantenere la distinzione tra relazioni padre-figlio in un elenco di attività esportato aggiungendo una visualizzazione personalizzata all'elenco di attività e verificando che questa visualizzazione sia selezionata prima di esportare l'elenco.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Visualizza: visualizzare la relazione padre-figlio in un&#39;attività applicando un rientro alle attività

È possibile mantenere la distinzione tra relazioni padre-figlio in un elenco di attività esportato aggiungendo una visualizzazione personalizzata all&#39;elenco di attività e verificando che questa visualizzazione sia selezionata prima di esportare l&#39;elenco.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Passa al progetto con l’elenco delle attività da esportare.
1. Fai clic sul pulsante **Visualizza** menu a discesa e seleziona **Nuova vista**.

1. Denomina il filtro nell&#39;angolo in alto a sinistra dello schermo.
1. Fai clic in **Nome attività** intestazione di colonna.

1. Seleziona **Passa alla modalità testo** nell&#39;angolo in alto a destra.
1. Fare clic in un punto qualsiasi della casella di testo per modificare il testo e rimuovere tutto il testo esistente.
1. Incolla il testo seguente:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Fai clic su **Salva**.
1. Fai clic su **Salva visualizzazione**.
