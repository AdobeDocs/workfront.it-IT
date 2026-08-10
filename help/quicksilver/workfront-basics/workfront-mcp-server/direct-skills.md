---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Abilità disponibili per l’installazione diretta
description: Workfront offre alcune competenze che è possibile installare direttamente nel proprio LLM.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Abilità disponibili per l’installazione diretta

Adobe Workfront offre alcune competenze che è possibile installare direttamente nel proprio LLM. Le abilità guidano l’utilizzo di questi strumenti per attività specifiche, con i passaggi giusti già integrati.

Puoi trovare queste abilità come file nell’archivio GitHub delle abilità di Adobe. Questo archivio contiene file per diversi prodotti Adobe. Quando scarichi questi file e li copia a Claude, Claude può quindi utilizzare le abilità descritte nei file.

Ad esempio, le competenze di architetto della soluzione Planning consentono a Claude di rispondere a domande ed eseguire alcune azioni in Workfront Planning.

Non è necessario chiamare o attivare queste abilità dopo che sono state copiate nell&#39;LLM. Invece, è possibile interagire con il LLM come al solito, ponendo domande nel linguaggio naturale, e il LLM utilizza le informazioni e le azioni descritte nell&#39;abilità che sono appropriate per la conversazione.

>[!NOTE]
>
>Attualmente, queste abilità sono disponibili solo per Claude.
>Per istruzioni su come configurare Claude con Adobe, consulta [Guida introduttiva](https://developer.adobe.com/adobe-for-creativity/getting-started/) nella documentazione di Adobe Developer.

## Installare un’abilità dall’archivio GitHub di Workfront in Claude

1. Vai all&#39;[archivio Adobe Workfront skills](https://github.com/adobe/skills/tree/main/plugins/workfront) su GitHub.
1. Scarica la cartella delle abilità che desideri utilizzare.
1. Copia la cartella nella libreria Claude Skills.

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` (macOS) o equivalente.
   * Codice Claude: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Competenze attualmente disponibili

| Abilità/Collegamento alla cartella | Descrizione abilità | Disponibile per |
|---|---|---|
| [Architetto della soluzione Planning](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Configurare un&#39;area di lavoro di Workfront Planning in base alle proprie esigenze e rispondere alle domande su Workfront Planning. | Claude |
