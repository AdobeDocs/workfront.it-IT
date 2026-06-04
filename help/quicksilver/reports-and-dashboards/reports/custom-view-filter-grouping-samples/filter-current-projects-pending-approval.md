---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: visualizzare i progetti correnti in attesa di approvazione'
description: Il seguente filtro di progetto mostra i progetti nello stato Corrente - In attesa di approvazione, dove l’utente connesso è lo sponsor del progetto o Portfolio Manager.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sPLW4-QHP5aXEd--UZVsS1WjY5-bJeyoOZ8mzYe7sww
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 28%

---

# Filtro: visualizzare i progetti correnti in attesa di approvazione

<!--Audited: 10/2024-->

Il seguente filtro di progetto mostra i progetti nello stato Corrente - In attesa di approvazione, dove l’utente connesso è lo sponsor del progetto o Portfolio Manager.

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
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtra progetti correnti in attesa di approvazione

Per applicare questo filtro:

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Fare clic su **Modalità testo**.
1. Nell’area visualizzata, copia e incolla il seguente codice:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Fai clic su **Applica** > **Salva come nuovo**.
