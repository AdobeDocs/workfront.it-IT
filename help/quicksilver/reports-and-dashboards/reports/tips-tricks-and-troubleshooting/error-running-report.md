---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Messaggio di errore durante l’esecuzione di un rapporto: "Al momento non hai effettuato l’accesso".'
description: Scopri il messaggio di errore "Non hai effettuato l’accesso".
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Vg-z-oXY25if70i5l2GBZad4iBj6hNRhu9LHE-6kCU8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 31%
---
# Messaggio di errore durante l’esecuzione di un rapporto: “Non hai effettuato l’accesso”.

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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

Quando si esegue un report o lo si visualizza in un dashboard, viene restituito il seguente errore:\
*Riproviamo. Non si è al momento connessi.*

Nessun risultato viene visualizzato nel rapporto.

## Causa

Il report è attualmente impostato per l&#39;esecuzione come utente disattivato.

## Soluzione

Per modificare le impostazioni del report è necessario disporre delle autorizzazioni di gestione.\
Per adeguare il rapporto e visualizzare i risultati:

1. Passa al report.
1. Fai clic su **Azioni report** > **Modifica** > **Impostazioni report**.

1. Specificare il nome di un utente attivo nel campo **Esegui report con diritti di accesso di:**.\
   Oppure\
   Lasciare vuoto il campo **Esegui report con diritti di accesso di:**.

1. Fai clic su **Fine**.
1. Fai clic su **Salva e Chiudi**.\
   L’errore non dovrebbe più essere visualizzato durante l’esecuzione del rapporto.
