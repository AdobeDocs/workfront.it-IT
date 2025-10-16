---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: Mostra attività padre fino a 4 livelli di profondità'
description: Questa visualizzazione delle attività mostra il nome dell'attività nella prima colonna e (se esistono) fino a 4 attività padre in colonne separate nello stesso elenco.
author: Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Visualizza: mostra le attività padre fino a 4 livelli di profondità

<!--Audited: 11/2024-->

Questa visualizzazione delle attività mostra il nome dell&#39;attività nella prima colonna e (se esistono) fino a 4 attività padre in colonne separate nello stesso elenco.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Mostra attività padre fino a 4 livelli

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.
1. Nell&#39;area **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modalità testo** e sostituirlo con il seguente codice:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=parent
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=parent:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=parent:objCode
   column.1.link.valueformat=val
   column.1.linkedname=parent
   column.1.listsort=nested(parent).string(name)
   column.1.namekey=parent
   column.1.querysort=parent:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=parent:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Parent
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=parent:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=parent:parent:objCode
   column.2.link.valueformat=val
   column.2.linkedname=parent
   column.2.listsort=nested(parent:parent).string(name)
   column.2.name=Parent Parent
   column.2.querysort=parent:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=parent:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Parent Parent Parent
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=parent:parent:parent:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=parent:parent:parent:objCode
   column.3.link.valueformat=val
   column.3.linkedname=parent
   column.3.listsort=nested(parent:parent:parent).string(name)
   column.3.name=Parent Parent Parent
   column.3.querysort=parent:parent:parent:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=parent:parent:parent:name
   column.3.valueformat=HTML
   column.3.width=150
   column.4.description=Parent Parent Parent Parent
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=parent:parent:parent:parent:ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.valuefield=parent:parent:parent:parent:objCode
   column.4.link.valueformat=val
   column.4.linkedname=parent
   column.4.listsort=nested(parent:parent:parent:parent).string(name)
   column.4.name=Parent Parent Parent Parent
   column.4.querysort=parent:parent:parent:parent:name
   column.4.shortview=false
   column.4.stretch=100
   column.4.valuefield=parent:parent:parent:parent:name
   column.4.valueformat=HTML
   column.4.width=150
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.

   Il nome dell&#39;attività viene visualizzato nella prima colonna e, se l&#39;attività ha padri, nelle colonne rimanenti vengono visualizzati fino a 4 padri.
