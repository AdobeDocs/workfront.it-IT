---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Messaggio di errore sul calendario: ''Questo calendario dispone dei diritti di visualizzazione di un utente disattivato.'''
description: Scopri di più sul messaggio di errore "Questo calendario dispone dei diritti di visualizzazione di un utente disattivato".
author: Courtney
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3yxFjvj--T8taJ2xrLTIia6YamTCwZeueTFSI-bMg4o
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
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 23%

---

# Messaggio di errore sul calendario: “Questo calendario dispone dei diritti di visualizzazione di un utente disattivato”.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
     <p>Standard</p>
     <p>Work o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un calendario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problema

Quando si accede a un calendario condiviso con l&#39;utente viene visualizzato il messaggio di errore seguente: 

*Questo calendario dispone dei diritti di visualizzazione di un utente disattivato. Richiedere a un amministratore di correggere i privilegi del calendario.*

## Causa

L&#39;utente che ha creato il calendario (proprietario originale) è un utente che è stato disattivato. 

## Soluzione

Puoi risolvere il problema nel modo seguente:

1. Copia il calendario originale. Quando si copia un calendario, l&#39;utente diventa il proprietario del calendario. Il calendario copiato deve mostrare tutte le informazioni del calendario originale.\
   Per ulteriori informazioni sulla copia di un calendario, vedere [Copiare un report del calendario](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Condividere il calendario copiato con gli stessi utenti del calendario originale. Tutti gli utenti devono visualizzare le stesse informazioni nel nuovo calendario.
1. (Facoltativo e condizionale) Se si dispone delle autorizzazioni per gestire il calendario originale, rimuovere tutti gli altri utenti con cui il calendario è condiviso dall&#39;area Condivisione calendario. In questo modo si evita di confondere gli utenti che tentano di visualizzare un calendario errato.
