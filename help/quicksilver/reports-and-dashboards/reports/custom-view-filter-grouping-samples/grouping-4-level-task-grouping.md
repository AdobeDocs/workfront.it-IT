---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: Raggruppamento di attività a 4 livelli per proprietario Portfolio, proprietario del programma, proprietario del progetto e stato del progetto'
description: Questo raggruppamento di attività fornisce 4 livelli di raggruppamento. In questo caso, le attività sono raggruppate per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto. È possibile disporre di un massimo di 3 livelli di raggruppamento utilizzando l'interfaccia standard. Per aggiungere un quarto livello, è necessario utilizzare la modalità testo. Non è possibile raggruppare i rapporti in base a più di 4 criteri contemporaneamente.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Raggruppamento: raggruppamento di attività a 4 livelli per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto

<!--Audited: 10/2024-->

Questo raggruppamento di attività fornisce 4 livelli di raggruppamento. In questo caso, le attività sono raggruppate per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto. È possibile disporre di un massimo di 3 livelli di raggruppamento utilizzando l&#39;interfaccia standard. Per aggiungere un quarto livello, è necessario utilizzare la modalità testo. Non è possibile raggruppare i rapporti in base a più di 4 criteri contemporaneamente.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Creazione di un raggruppamento di attività a 4 livelli per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto

Per applicare questo raggruppamento:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Raggruppamento**, selezionare **Nuovo raggruppamento**.

1. Fare clic su **Passa alla modalità testo**.
1. Rimuovi il testo nell&#39;area **Raggruppa il report**.
1. Sostituire il testo nella casella visualizzata con il seguente codice:
   <pre>group.0.linkedname=project<br>group.0.name=Proprietario Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM .3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val<br><br><br><br></pre>

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.
