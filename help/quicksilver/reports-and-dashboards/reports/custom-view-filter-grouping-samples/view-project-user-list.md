---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: elenco di utenti progetto con mansioni'
description: È possibile applicare questa visualizzazione in un elenco di progetti o in un report per visualizzare un elenco di utenti associati al progetto e un elenco delle mansioni che eseguono sul progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Visualizza: elenco di utenti del progetto con mansioni

<!--Audited: 11/2024-->

È possibile applicare questa visualizzazione in un elenco di progetti o in un report per visualizzare un elenco di utenti associati al progetto e un elenco delle mansioni che eseguono sul progetto.

Le informazioni contenute in questo rapporto sono reperibili anche nell’area Persone del progetto.

>[!TIP]
>
>Se per gli utenti non è elencata alcuna mansione ma si sa che sono associati a mansioni nei loro profili utente, ciò potrebbe significare che sono assegnati ad attività e problemi, ma potrebbero non essere associati a una mansione per l&#39;attività o il problema, o che gli utenti elencati nel rapporto non sono gli assegnatari per le attività e i problemi, ma adempiono ad altri ruoli sul progetto (ad esempio, Proprietario o Sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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


## Visualizza un elenco di utenti del progetto con ruoli

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.
1. Nell&#39;area **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.
