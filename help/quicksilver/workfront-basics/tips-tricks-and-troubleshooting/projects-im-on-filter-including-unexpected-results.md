---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Il filtro Progetti in corso include risultati imprevisti
description: Leggi questo articolo per risolvere i problemi relativi al filtro Progetti in corso, inclusi i risultati imprevisti.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 23%

---

# Il filtro Progetti a cui partecipo include risultati imprevisti

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td>Qualsiasi</td>
  </tr>
  <tr>
   <td>Licenze Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Piano</p>
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

Il filtro [!UICONTROL **Progetti in corso**] include risultati non previsti, in quanto non sono assegnato o associato a tali progetti.

## Soluzione

Il filtro [!UICONTROL **Progetti in corso**] include progetti che contengono l&#39;utente in uno dei campi [!UICONTROL **Dettagli progetto**], inclusi campi facilmente mancanti o compilati automaticamente come [!UICONTROL **Inserito da**] o [!UICONTROL **ID sponsor**]. Per rimuovere i risultati indesiderati, esistono due soluzioni possibili:

1. Controlla [!UICONTROL **Dettagli progetto**] per ogni progetto imprevisto incluso dal filtro e rimuovi il tuo nome da tutti i campi.

   O

1. Prova a utilizzare un filtro simile, ad esempio [!UICONTROL **Progetti di cui sono Proprietario**], che include solo i progetti specificamente assegnati a te.

Per ulteriori informazioni sull&#39;utilizzo dei filtri in [!DNL Workfront], vedere [Panoramica dei filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
