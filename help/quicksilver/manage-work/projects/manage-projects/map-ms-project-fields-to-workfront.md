---
product-area: projects
navigation-topic: manage-projects
title: Mappare i campi del progetto Microsoft ai progetti Adobe Workfront
description: I progetti in Adobe Workfront e Microsoft Project sono per lo più compatibili. Questo articolo descrive come i campi di progetto più comuni delle due applicazioni vengono mappati tra loro.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# Mappare i campi del progetto Microsoft ai progetti Adobe Workfront

I progetti in Adobe Workfront e Microsoft Project sono per lo più compatibili. Utilizzando le due applicazioni, è possibile effettuare le seguenti operazioni:

* Esportare progetti da Microsoft Project e importarli in Workfront
* Esporta i progetti da Workfront e importali in Microsoft Project.

Per ulteriori informazioni sull&#39;importazione di progetti da Microsoft Project in Workfront, vedere [Importare un progetto da Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Per ulteriori informazioni sull&#39;esportazione di un progetto da Workfront per importarlo in Microsoft Project, vedere [Esportare un progetto in Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Durante l’esecuzione di tali importazioni di dati, è importante comprendere in che modo le informazioni si traducono da un’applicazione all’altra. Nella maggior parte dei casi, dopo aver completato l’importazione dovrai apportare alcune modifiche manuali al progetto.

## Panoramica della mappatura dei campi

>[!NOTE]
>
>Le date pianificate non corrispondono sempre tra i due sistemi. Le discrepanze possono essere contabilizzate in base alla pianificazione e alle differenze nelle preferenze di sistema tra Workfront e Microsoft Project. Queste discrepanze di date possono anche causare differenze in termini di sforzo, durata e percentuale di completamento.

| **Campo progetto Microsoft** | **Campo Workfront** |
|---|---|
| Titolo progetto | Nome progetto |
| Date di inizio e di fine | Date Pianificate di Inizio e Completamento |
| Nome attività | Nome attività |
| Durata attività | Durata attività pianificata |
| Lavoro attività | Ore pianificate attività |
| % completamento attività | % completamento attività (in base alla durata dell&#39;attività) |
| % completamento lavoro attività | % completamento attività (in base alle ore pianificate dell&#39;attività) |
| Inizio e fine pianificati | Date Pianificate di Inizio e Completamento |
| Inizio e fine effettivi | Date effettive di inizio e di completamento |
| Nome risorsa | Assegnazione attività |
| Unità assegnazione | Percentuale di allocazione assegnazione |
| Nota attività | Descrizione attività |
| Predecessore | Predecessore |

## Panoramica dei dati non inclusi

Alcuni campi del progetto non vengono importati o esportati da Workfront.

Questi campi includono, tra l’altro:

* Allegati documento
* Campi personalizzati (a livello di progetto o di attività)
* Note di Workfront
* Problemi
* Ritardo negativo nelle attività con una relazione predecessore Inizio/Fine (le attività vengono importate senza ritardo)
* Assegnazioni
* Vincoli attività

  >[!NOTE]
  >
  >Poiché i vincoli non vengono mappati tra Microsoft Project e Workfront, verificare che esistano relazioni predecessori tra le attività. In caso contrario, le date di inizio pianificate e di completamento pianificate delle attività potrebbero non essere corrette nel progetto importato.
