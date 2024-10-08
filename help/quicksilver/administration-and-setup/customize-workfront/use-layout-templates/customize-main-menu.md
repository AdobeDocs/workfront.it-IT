---
title: Personalizzare il menu principale utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront o di un gruppo, puoi utilizzare un modello di layout per configurare le opzioni che gli utenti visualizzano all’apertura del menu principale in Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 3%

---

# Personalizzare il menu principale utilizzando un modello di layout

<!--Audited: 01/2024-->

In qualità di amministratore di Adobe Workfront o di un gruppo, puoi utilizzare un modello di layout per configurare le opzioni che gli utenti visualizzano all’apertura del menu principale in Workfront.

![Opzioni menu principale](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Le opzioni del menu principale visualizzate dagli utenti dipendono dal tipo di licenza e dalle impostazioni configurate nel livello di accesso. Alcuni utenti che utilizzeranno questo modello di layout potrebbero non visualizzare tutte le opzioni selezionate. Per ulteriori informazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) e [Accesso configurabile alle funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Workfront Unified Experience, nel menu principale potrebbero essere visualizzate opzioni diverse. Per informazioni, vedere [Esperienza unificata di Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront</strong></td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td><p>Corrente: Piano</p>
   Oppure
   <p>Nuovo: Standard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
    <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare il menu principale

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fare clic su **Imposta menu principale** nell&#39;angolo superiore destro del modello.

   Viene visualizzata la casella Main Menu (Menu principale) che consente di visualizzare le aree attualmente visualizzate nel Main Menu (Menu principale) del modello, nonché gli elementi disponibili per l&#39;aggiunta. Di seguito sono riportati tutti gli elementi che è possibile aggiungere:
   * Pagina Home

     >[!TIP]
     >
     >Per impostazione predefinita, l&#39;icona Home nel menu principale visualizza l&#39;area My Updates (I miei aggiornamenti) per gli utenti con licenza Revisione (nel piano di licenza corrente), a meno che non abbiano un modello di layout associato al loro profilo che include l&#39;area My Updates (I miei aggiornamenti) nel menu principale, oltre all&#39;area Home.

   * Portfolio
   * Programmi
   * Progetti
   * Report
   * Dashboard
   * Calendari
   * Gestione risorse
   * Scenari

     >[!NOTE]
     >
     >Scenario Planner richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   * Team
   * Utenti

     >[!NOTE]
     >
     >Solo gli utenti con una licenza Pianificazione (nel modello di licenza corrente) o gli utenti con una licenza Standard (nel nuovo modello di licenza) possono visualizzare l&#39;area Utenti ![](assets/users-icon-in-main-menu.png) nel menu principale.

   * Richieste
   * Schede orario
   * Documenti
   * Modelli
   * Analisi
   * Verifica
   * Obiettivi

     >[!NOTE]
     >
     >Gli obiettivi richiedono una licenza aggiuntiva. Per informazioni sugli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * I miei aggiornamenti
   * Bacheche
   * Blueprint
   * In Pianificazione

     >[!NOTE]
     >
     >Planning richiede una licenza aggiuntiva. Per informazioni su Workfront Planning, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)

1. Effettua una delle seguenti operazioni:

   * Nascondi ![](assets/remove-icon---x-in-circle.png) **elementi attivi** che non desideri visualizzare
   * Mostra ![](assets/add-icon-plus-in-circle.png) **Elementi disponibili** che si desidera visualizzare nel menu principale.
   * Trascina ![](assets/move-icon---dots.png) **elementi attivi** per modificarne l&#39;ordine di visualizzazione nel menu principale.

1. Fai clic su **Fine**.

   Puoi anche fare clic su **Annulla** in qualsiasi momento se desideri annullare le modifiche.

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l’avanzamento, quindi continuare a modificare il modello in un secondo momento.

Per ulteriori informazioni sui modelli di layout, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
