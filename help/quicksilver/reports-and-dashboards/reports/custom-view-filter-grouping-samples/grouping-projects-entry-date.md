---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: progetti per data di ingresso"
description: In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per i relativi valori di Data di ingresso.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Raggruppamento: progetti per data di inserimento

In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per i relativi valori di Data di ingresso.

Ogni raggruppamento mostra i progetti con una Data di ingresso in:

* Ultimi 30 giorni
* 30-60 giorni
* 60 giorni o più

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

## Raggruppa progetti per data immissione

Per applicare questo raggruppamento:

1. Passare a un report di progetto esistente o creare un nuovo report di progetto.\
   Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Fai clic su **Azioni report** > **Modifica**.
1. Dalla scheda **Raggruppamento**, fai clic su **Aggiungi raggruppamento**.
1. Fare clic su **Passa alla modalità testo**.
1. Rimuovi il testo nell&#39;area **Raggruppa per**.
1. Sostituisci il testo con il seguente codice:

   group.0.linkedname=direct
group.0.name=Voce progetto
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;Ultimi 30 giorni&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;30-60 giorni&quot;,&quot;Più vecchi di 60 giorni&quot;))
group.0.valueformat=atDateAsMonthString
textmode=true

1. Fai clic su **Fine** > **Salva raggruppamento**.
1. (Facoltativo) Aggiorna il nome del raggruppamento, quindi fai clic su **Salva raggruppamento**.
