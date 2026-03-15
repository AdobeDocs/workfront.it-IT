---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: gruppo principale del proprietario del progetto in un elenco di ore'
description: È possibile visualizzare il nome del gruppo principale del proprietario del progetto in un elenco o in un report ore.
author: Courtney
feature: Reports and Dashboards
exl-id: 6491ab9b-c09e-4bdb-99c2-56bb44f66947
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 22%

---

# Raggruppamento: gruppo predefinito del proprietario del progetto in un elenco di ore

<!--Audited: 10/2024-->

È possibile visualizzare il nome del gruppo principale del proprietario del progetto in un elenco o in un report ore.

Il raggruppamento raggruppa inoltre i risultati in base al nome del proprietario del progetto e al nome del progetto.

![raggruppamento_per_progetto_proprietario_casa_gruppo.png](assets/grouping-for-project-owner-home-group-350x51.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Raggruppa per home Gruppo del proprietario del progetto in un elenco di ore

Per applicare questo raggruppamento:

1. Consente di passare a un elenco di ore.
1. Dal menu a discesa **Raggruppamento**, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Passa alla modalità testo**.
1. Rimuovi il testo nell&#39;area **Raggruppa per**.
1. Sostituisci il testo con il seguente codice:

```
group.0.displayname=Home Group of Project Owner
group.0.valuefield=project:owner:homeGroup:name
group.0.valueformat=HTML
group.1.displayname=Project Owner
group.1.linkedname=projectOwnerMM
group.1.namekey=view.relatedcolumn
group.1.namekeyargkey.0=projectOwnerMM
group.1.namekeyargkey.1=name
group.1.valuefield=projectOwnerMM:name
group.1.valueformat=string
group.2.displayname=Project Name
group.2.linkedname=project
group.2.namekey=view.relatedcolumn
group.2.namekeyargkey.0=project
group.2.namekeyargkey.1=name
group.2.valuefield=project:name
group.2.valueformat=string
textmode=true
```

1. Fai clic su **Fine** > **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.
