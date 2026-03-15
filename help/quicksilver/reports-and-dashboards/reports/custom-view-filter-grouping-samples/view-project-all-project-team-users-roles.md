---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: Progetto con tutti gli utenti e i ruoli del team di progetto'
description: Questa visualizzazione del progetto mostra un elenco di utenti e ruoli di lavoro assegnati al team del progetto.
author: Courtney
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 14%

---

# Visualizzazione: progetto con tutti gli utenti e i ruoli del team di progetto

<!--Audited: 11/2024-->

Questa visualizzazione del progetto mostra un elenco di utenti e ruoli di lavoro assegnati al team del progetto.

>[!NOTE]
>
>Se il ruolo del processo è elencato nella stessa riga di un utente, ciò non implica che l&#39;utente stia ricoprendo tale ruolo nel progetto, né che all&#39;utente sia assegnato tale ruolo nel proprio profilo.

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Visualizzare un progetto con tutti gli utenti e i ruoli del team di progetto

1. Vai a un elenco di progetti.
1. Dal menu a discesa **Visualizza**, seleziona **Nuova vista**.

1. Nell&#39;area **Anteprima colonna**, eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa alla modalità Testo** > **Modifica modalità Testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il codice seguente:




   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0 querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.plural<br>column.1.stretch=30&lbrace;valufield HTML<br>column.1.width=150<br>column.2.description=Team Ruoli<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10&lbrace;3<br><br><br><br><br><br><br></pre>

1. Fai clic su **Fine** > **Salva vista**.
