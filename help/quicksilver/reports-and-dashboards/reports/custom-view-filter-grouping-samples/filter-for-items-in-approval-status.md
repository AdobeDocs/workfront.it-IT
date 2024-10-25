---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizza solo gli elementi in stato di approvazione"
description: È possibile visualizzare solo gli elementi con un determinato stato attualmente in In attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Filtro: consente di visualizzare solo gli elementi con stato di approvazione

<!--Audited: 10/2024-->

È possibile visualizzare solo gli elementi con un determinato stato attualmente in In attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.

È possibile inserire i seguenti oggetti in uno stato di approvazione:

* Attività
* Problemi
* Progetti

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza solo gli elementi nello stato di approvazione

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.
1. Scegli di filtrare per **Progetto: Stato**, quindi seleziona dall&#39;elenco lo stato in base al quale desideri filtrare.

   In un report di progetti, ad esempio, aggiungere **Stato uguale a pianificazione** se si desidera visualizzare solo i progetti con stato **Pianificazione - In attesa di approvazione**.
1. Fare clic su **Modalità testo**.
1. Modificare la riga `status` aggiungendo **:A** alla chiave di tre lettere dello stato:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Fai clic su **Applica** > **Salva come nuovo**.

   Nell&#39;elenco vengono visualizzati solo i progetti con stato Pianificazione - In attesa di approvazione.
