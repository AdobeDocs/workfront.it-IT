---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica dello stato di avanzamento del progetto
description: Adobe Workfront determina lo stato di avanzamento di un progetto osservando l’avanzamento del progetto lungo la relativa sequenza temporale. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Ulteriori informazioni sullo stato di avanzamento del progetto in questo articolo .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
TQID: https://experienceleague.adobe.com/V9eyzkoYIREb4zUuDxmyDhnQa54YQaYTv2woNTOhq24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 375
ht-degree: 3%

---

# Panoramica sullo stato di avanzamento del progetto

<!--Audited: 12/2023-->

Adobe Workfront determina lo stato di avanzamento di un progetto osservando l’avanzamento del progetto lungo la relativa sequenza temporale. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Per ulteriori informazioni sulla configurazione della condizione del progetto, vedere l&#39;articolo [Panoramica della condizione e del tipo di condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Di seguito sono riportati gli stati di avanzamento dei progetti in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Nei Tempi</td> 
   <td> Lo stato di avanzamento di un progetto è <strong>Nei tempi</strong> se:<ul><li>Se le date di scadenza previste e quelle previste sono precedenti o uguali alla data di completamento pianificata del progetto <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>A Rischio</td> 
   <td> Lo stato di avanzamento di un progetto è <strong>A rischio</strong> se <strong>tutti</strong> dei seguenti valori sono true:<ul><li>Le date di completamento previste e quelle previste sono entrambe nel futuro</li><li> La data di scadenza stimata è successiva sia alla data di completamento pianificata che alla data di completamento prevista <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>Indietro</td> 
   <td> Lo stato di avanzamento di un progetto è <strong>Indietro</strong> se <strong>tutti</strong> dei seguenti valori sono true:<ul><li>Le date di completamento previste e quelle previste sono entrambe nel futuro</li><li> Le date di completamento previste e quelle previste sono successive alla data di completamento pianificata del progetto</li><li> La data di scadenza stimata non è successiva alla data di completamento prevista
   <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>In Ritardo</td> 
   <td> 
     Lo stato di avanzamento di un progetto è <strong>Late</strong> se <strong>any</strong> dei seguenti è true:<ul><li>Il progetto è completo e la data di completamento effettiva è successiva alla data di completamento pianificata <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Il progetto non è completo e la data di completamento pianificata è nel passato <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Considera i seguenti aspetti:

* La data di completamento prevista del progetto dipende dall&#39;attività nel percorso critico con la data di completamento prevista più recente.
* La Data di Scadenza Stimata del progetto dipende dall&#39;attività nel Percorso Critico con la Data di Scadenza Stimata più recente.

Per informazioni sul percorso critico del progetto, vedere [Panoramica del percorso critico del progetto](../../../manage-work/tasks/manage-tasks/critical-path.md).

Per informazioni sulle date di completamento previste, vedere [Panoramica sulla data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
