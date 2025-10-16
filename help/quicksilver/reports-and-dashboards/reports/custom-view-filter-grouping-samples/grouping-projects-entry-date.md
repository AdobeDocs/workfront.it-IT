---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: Progetti per Data Inserimento'
description: In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per i relativi valori di Data di ingresso.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Raggruppamento: progetti per data di inserimento

<!--Audited: 10/2024-->

In questo raggruppamento di progetti personalizzato, puoi visualizzare i progetti raggruppati per i relativi valori di Data di ingresso.

Ogni raggruppamento mostra i progetti con una Data di ingresso in:

* Ultimi 30 giorni
* 30-60 giorni
* 60 giorni o più

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Fai clic su **Fine** > **Salva raggruppamento**.
1. (Facoltativo) Aggiorna il nome del raggruppamento, quindi fai clic su **Salva raggruppamento**.
