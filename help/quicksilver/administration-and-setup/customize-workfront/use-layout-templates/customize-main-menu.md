---
title: Personalizzare il menu principale utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront o di amministratore di gruppo, puoi utilizzare un modello di layout per configurare le opzioni visualizzate dagli utenti all’apertura del menu principale in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# Personalizzare il menu principale utilizzando un modello di layout

In qualità di amministratore di Adobe Workfront o di amministratore di gruppo, puoi utilizzare un modello di layout per configurare le opzioni che gli utenti vedranno all’apertura del menu principale in Workfront:

![Opzioni menu principale](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Le opzioni del menu principale visualizzate dagli utenti dipendono dal tipo di licenza e dalle impostazioni configurate nel livello di accesso. Alcuni utenti che utilizzeranno questo modello di layout potrebbero non visualizzare tutte le opzioni selezionate qui. Per ulteriori informazioni consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) e [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

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
   <td role="rowheader"><strong>Licenza Adobe Workfront</strong></td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare il menu principale

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic su **Imposta menu principale** nell&#39;angolo in alto a destra.

   Nella casella Menu principale visualizzata, è possibile visualizzare gli elementi attualmente attivi nel menu principale per il modello, nonché gli elementi disponibili per l&#39;aggiunta. Di seguito sono riportati tutti gli elementi possibili che è possibile aggiungere:

   * Home

      >[!TIP]
      >
      >Per impostazione predefinita, Home viene visualizzato come Aggiornamenti personali per gli utenti con licenza di revisione, a meno che non dispongano di un modello di layout associato al profilo che include l&#39;area Aggiornamenti personali nel menu principale.

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
      >Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   * Team
   * Utenti

      >[!NOTE]
      >
      >Solo gli utenti con una licenza Plan possono visualizzare gli utenti ![](assets/users-icon-in-main-menu.png) nel menu principale.

   * Richieste
   * Schede orario
   * Documenti
   * Modelli
   * Analisi
   * Verifica
   * Obiettivi

      >[!NOTE]
      >
      >Questo richiede una licenza aggiuntiva. Per informazioni sugli obiettivi di Workfront, vedi [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * I miei aggiornamenti
   * Bacheche
   * Blueprint

1. Effettua una delle seguenti operazioni:

   * Nascondi ![](assets/remove-icon---x-in-circle.png) **Elementi attivi** che non si desidera visualizzare
   * Mostra ![](assets/add-icon-plus-in-circle.png) **Articoli disponibili** che si desidera visualizzare nel menu principale.
   * Trascina ![](assets/move-icon---dots.png) **Elementi attivi** per modificare l&#39;ordine di visualizzazione nel menu principale.

1. Fai clic su **Fine**.

   Puoi anche fare clic su **Annulla** in qualsiasi momento se desideri eliminare le modifiche.

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su Salva in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.

Per ulteriori informazioni sui modelli di layout, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
