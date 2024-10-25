---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizza successori tra progetti incompleti"
description: Questo filtro attività restituisce successori tra progetti incompleti.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Filtro: visualizza successori tra progetti incompleti

Questo filtro attività restituisce successori tra progetti incompleti.

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

## Filtrare i successori tra progetti

Per applicare questo filtro:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Fare clic su **Modalità testo**.
1. Nell’area visualizzata, incolla il seguente codice:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>successorsMM:projectID=FIELD:projectID<br>successorsMM:projectID_Mod=ne</pre>

1. Fai clic su **Applica** > **Salva come nuovo**.
