---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: visualizzare solo gli elementi con stato di approvazione'
description: È possibile visualizzare solo gli elementi in un determinato stato attualmente in attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 22%

---

# Filtro: visualizzare solo gli elementi con stato di approvazione

<!--Audited: 10/2024-->

È possibile visualizzare solo gli elementi in un determinato stato attualmente in attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.

È possibile inserire i seguenti oggetti in uno stato di approvazione:

* Attività
* Problemi
* Progetti

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
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza solo gli articoli nello stato di approvazione

1. Vai a un elenco di progetti.
1. Dal menu a discesa **Filtro**, seleziona **Nuovo filtro**.
1. Scegliere di filtrare in base a **Progetto: Stato**, quindi selezionare lo stato in base al quale si desidera filtrare dall&#39;elenco.

   Ad esempio, in un report di progetto, aggiungere **Stato uguale pianificazione**, se si desidera visualizzare solo i progetti con stato **Pianificazione - In attesa di approvazione**.
1. Fai clic su **Modalità testo**.
1. Modifica la riga `status` aggiungendo **:A** alla chiave a 3 lettere dello stato:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Fai clic su **Applica** > **Salva come nuovo**.

   Nell&#39;elenco vengono visualizzati solo i progetti con stato Pianificazione - Approvazione in sospeso.
