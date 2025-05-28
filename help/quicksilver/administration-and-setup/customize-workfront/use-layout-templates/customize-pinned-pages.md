---
title: Personalizzare le pagine bloccate utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In un modello di layout, puoi fissare le pagine che dovranno essere sempre disponibili per gli utenti nella parte superiore di Adobe Workfront. È possibile accedere a queste pagine tramite il menu principale o le dashboard.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 76797ce2afb6a6a929531f02ed3a3b3f75240602
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 4%

---

# Personalizzare le pagine bloccate utilizzando un modello di layout

In un modello di layout, puoi fissare le pagine che dovranno essere sempre disponibili per gli utenti nella parte superiore di Adobe Workfront. È possibile accedere a queste pagine tramite l&#39;icona del menu principale ![Main menu icon](assets/main-menu-icon.png) o l&#39;icona del menu principale ![Main menu](assets/main-menu-icon.png), se disponibile, oppure tramite le dashboard.

I pin aggiunti autonomamente dagli utenti vengono visualizzati a destra dei pin aggiunti nel modello di layout.

Per ulteriori informazioni sul blocco delle pagine, vedere [Fissa pagine per personalizzare l&#39;area di lavoro](../../../workfront-basics/the-new-workfront-experience/pin-pages.md).

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fissa pagine utilizzando un modello di layout

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. In **Area di navigazione superiore**, fai clic su **Aggiungi nuovo pin**.

1. Nel menu a discesa visualizzato, effettuare una delle seguenti operazioni:

   * Seleziona tra le seguenti aree:

      * Calendari
      * Dashboard
      * Documenti
      * Obiettivi
      * Pagina Home
      * I miei aggiornamenti
      * Portfolio
      * Programmi
      * Progetti
      * Rapporti
      * Richieste
      * Gestione risorse
      * Scenari
      * Team
      * Modelli
      * Schede orario
      * Utenti
      * Blueprint
      * In Pianificazione

     >[!IMPORTANT]
     >
     >Per visualizzare le aree Obiettivi, Scenari e Pianificazione sono necessarie licenze aggiuntive.
     >
     >* Per informazioni sugli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).
     >
     >* Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).
     >
     >* Per informazioni su Workfront Planning, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Fai clic su **Aggiungi dashboard**
      * Digita un nome descrittivo nel campo <!--**Quick link name**-->**Nome personalizzato**
      * Seleziona un dashboard nel **Aggiungi un dashboard** campo <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now -->
      * Fare clic su **Aggiungi**.

1. Ripeti il passaggio precedente per fissare qualsiasi altra pagina.

1. (Facoltativo) Per spostare un pin, passa il cursore del mouse sul pin e fai clic sull&#39;icona del menu Altro ![Icona Altro](assets/more-icon.png) accanto al nome del pin, quindi fai clic su **Sposta a sinistra** o **Sposta a destra** per spostare il pin nella direzione scelta oppure fai clic su **Sposta in primo piano** per spostare il pin nella posizione più a sinistra.

1. (Facoltativo) Per rinominare un pin, passa il puntatore del mouse sul pin e fai clic sull&#39;icona del menu Altro ![Icona Altro](assets/more-icon.png) accanto al nome del pin, quindi fai clic su **Rinomina pin**. Immetti un nuovo nome, quindi fai clic su **Salva**.

1. (Facoltativo) Per eliminare un pin, passa il puntatore sul pin e fai clic sull&#39;icona del menu Altro ![Icona Altro](assets/more-icon.png) accanto al nome del pin, quindi fai clic su **Rimuovi pin**.

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su **Salva** in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
