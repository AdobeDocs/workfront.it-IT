---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare le date nei rapporti in modalità testo
description: Le date possono essere configurate per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront. Per stabilire un formato data, è necessario modificare la riga formato valore del codice della modalità testo nella colonna.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/-8gB8XDwLQTBCUsrex-PIAyxcF-rSPsoM2Gvw2EhTaU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 9%
---
# Formattare le date nei rapporti in modalità testo

<!-- Audited: 1/2025 -->

Le date possono essere configurate per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront. Per stabilire un formato data, è necessario modificare la riga `valueformat` del codice in modalità testo nella colonna.

`valueformat= [new date format]` Ad esempio, se si desidera che la data di completamento prevista venga visualizzata come MM/GG/AA, il codice sarà simile al seguente:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Se desideri visualizzare la Data di completamento pianificata come *Mese, GG, Anno*, il codice sarà simile al seguente:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale nei report e negli elenchi di Workfront utilizzando la modalità testo, vedere [Utilizzare la formattazione condizionale in modalità testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

È possibile formattare le date utilizzando i seguenti `valueformat` valori in modalità testo:

| **Formato** | Esempio  | ***formato valore=*** |
|---|---|---|
| GG/MM/AA | 10/11/18 | `atDate` |
| DD/MM/YY | 10/11/18 12:00 pm | `longAtDate` |
| GG/MM/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 ottobre 2018 | `mediumAtDate` |
| DW, mese, giorno, anno | lunedì 11 ottobre 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Lun, 11 ottobre 2018 12:00 pm | `fullAtDate` |
