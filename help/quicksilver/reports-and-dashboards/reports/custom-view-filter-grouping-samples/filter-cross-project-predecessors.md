---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizzare predecessori tra progetti incompleti"
description: Questo filtro attività restituisce predecessori tra progetti incompleti.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Filtro: visualizzazione di predecessori tra progetti incompleti

<!--Audited: 10/2024-->

Questo filtro attività restituisce predecessori tra progetti incompleti.

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

## Filtrare i predecessori di progetti incrociati

Per applicare questo filtro:

1. Consente di passare a un elenco di attività o a un report di attività.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. (Facoltativo) Fai clic su **Modalità testo** se hai effettuato l&#39;accesso al filtro da un elenco oppure su **Passa alla modalità testo** se hai effettuato l&#39;accesso al filtro da un report.
1. Nella nuova area, incolla il seguente codice:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Condizionale) Fai clic su **Salva filtro** se hai effettuato l&#39;accesso al filtro da un report oppure su **Applica**, quindi su **Salva come nuovo** se hai effettuato l&#39;accesso al filtro da un elenco di attività.
