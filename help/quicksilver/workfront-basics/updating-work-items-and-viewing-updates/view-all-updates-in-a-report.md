---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visualizzare tutti gli aggiornamenti in un report Nota
description: Per visualizzare tutti gli aggiornamenti inseriti da un utente per un oggetto, è possibile creare un report di note che visualizza tutti gli aggiornamenti.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Visualizzare tutti gli aggiornamenti in un report Nota

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Per impostazione predefinita, nell&#39;area Aggiornamenti di un oggetto viene visualizzato un numero massimo di 200 aggiornamenti. Per visualizzare tutti gli aggiornamenti inseriti da un utente per un oggetto, è possibile creare un report di note che visualizza tutti gli aggiornamenti.

>[!NOTE]
>
>È possibile creare un report per visualizzare gli aggiornamenti sugli oggetti in Anteprima con il report Voce diario. Per ulteriori informazioni, vedere [Report sull&#39;area Aggiornamenti con un report sulle voci diario](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di modifica con la possibilità di creare quanto segue:</p> 
    <ul> 
     <li> <p>Report, dashboard e calendari</p> </li> 
     <li> <p>Filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni sugli oggetti nel rapporto</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Creare un rapporto di nota

La creazione di un report per Notes per qualsiasi oggetto è identica, indipendentemente dall&#39;oggetto.

Ad esempio, per creare un rapporto Note per tutte le note di un progetto:

{{step1-to-reports}}

1. Nell&#39;angolo superiore sinistro della pagina fare clic su **Nuovo report**, quindi selezionare **Nota**.

1. (Facoltativo) Fai clic su **(Colonne) Visualizza**, quindi su **Aggiungi colonna** per aggiungere **Nome** del **Progetto** alla visualizzazione del report. 

1. (Facoltativo) Se esegui report su più progetti contemporaneamente, fai clic su **Raggruppamenti**, quindi su **Aggiungi raggruppamento** per raggruppare in base al **Nome** del **Progetto**. In questo modo le note vengono raggruppate in base ai rispettivi progetti, facilitando la lettura del rapporto. 

1. (Facoltativo) Fai clic su **Filtri**, quindi su **Aggiungi regola filtro**.
1. Aggiungi un filtro per **Nota** > **Testo nota** > **Non è vuoto**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Se un campo di progetto è stato aggiornato ma non è stata aggiunta alcuna nota al momento dell&#39;aggiornamento, il **Testo nota** dell&#39;aggiornamento verrà visualizzato come **(Nessun testo aggiunto da aggiornare)**.


1. (Facoltativo) Aggiungi un altro filtro per **Progetto** > **Nome** > **È uguale a** e aggiungi uno o più nomi di progetto per i quali vuoi visualizzare le note.
1. Fai clic su **Salva + Chiudi**. Tutti gli aggiornamenti immessi nel progetto da tutti gli utenti con autorizzazioni di visualizzazione del progetto vengono visualizzati nel rapporto.
