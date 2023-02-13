---
product-area: projects
navigation-topic: manage-projects
title: Mappatura dei campi del progetto Microsoft su progetti Adobe Workfront
description: I progetti in Adobe Workfront e Microsoft Project sono per lo più compatibili. In questo articolo viene descritto come i campi di progetto più comuni delle due applicazioni vengono mappati tra loro.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Mappatura dei campi del progetto Microsoft su progetti Adobe Workfront

I progetti in Adobe Workfront e Microsoft Project sono per lo più compatibili. Utilizzando le due applicazioni, puoi effettuare le seguenti operazioni:

* Esportare progetti da Microsoft Project e importarli in Workfront
* Esporta progetti da Workfront e importali in Microsoft Project. 

Per ulteriori informazioni sull’importazione di progetti da Microsoft Project in Workfront, consulta [Importare un progetto da un progetto Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Per ulteriori informazioni sull’esportazione di un progetto da Workfront per importarlo in un progetto Microsoft, consulta [Esportare un progetto in un progetto Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Quando si eseguono tali importazioni di dati, è importante comprendere in che modo le informazioni si traducono da un&#39;applicazione all&#39;altra. Nella maggior parte dei casi, dopo aver completato l’importazione, sarà necessario apportare alcune modifiche manuali al progetto. 

## Panoramica della mappatura dei campi

>[!NOTE]
>
>Le date pianificate non corrispondono sempre tra i due sistemi. Le discrepanze possono essere prese in considerazione attraverso la pianificazione e le differenze nelle preferenze di sistema tra Workfront e Microsoft Project. Queste discrepanze di date possono anche causare differenze di sforzo, durata e percentuale di completamento.

| **Campo progetto Microsoft** | **Campo Workfront** |
|---|---|
| Titolo del progetto | Nome progetto |
| Date di inizio e di fine | Date di inizio e di completamento pianificate |
| Nome attività | Nome attività |
| Durata attività | Durata pianificata attività |
| Lavoro | Orario pianificato attività |
| Attività % completata | % attività completata (in base alla durata dell&#39;attività) |
| % lavoro attività completata | % attività completata (in base all&#39;ora pianificata dell&#39;attività) |
| Inizio e fine pianificati | Date di inizio e di completamento pianificate |
| Inizio effettivo e Fine | Date di inizio e di completamento effettive |
| Nome risorsa | Assegnazione di Attività |
| Unità di assegnazione | Percentuale di allocazione assegnazione |
| Nota attività | Descrizione attività |
| Predecessore | Predecessore |

## Panoramica dei dati non inclusi

Esistono diversi campi di progetto che non vengono importati o esportati da Workfront.

Questi campi includono ma non sono limitati ai seguenti:

* Allegati documento
* Campi personalizzati (a livello di progetto o di attività)
* Note Workfront
* Problemi
* Ritardo negativo nelle attività con una relazione predecessore Inizio/Fine (le attività vengono importate senza ritardo)
* Assegnazioni
* Vincoli attività

   >[!NOTE]
   Poiché i vincoli non vengono mappati tra Microsoft Project e Workfront, assicurati che ci siano relazioni predecessori tra le attività. In caso contrario, le date di inizio e di completamento pianificati delle attività potrebbero non essere corrette nel progetto importato. 
