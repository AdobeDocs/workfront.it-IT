---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Disattivazione dei ruoli di lavoro
description: Come [!DNL Adobe Workfront] un amministratore o un utente con accesso amministrativo a Ruoli lavoro può disattivare i ruoli di lavoro che diventano obsoleti nel sistema. Quando si disattiva un ruolo di lavoro invece di eliminarlo, è possibile mantenere tutte le informazioni storiche associate ad esso.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Disattivazione dei ruoli di lavoro

Come [!DNL Adobe Workfront] un amministratore o un utente con accesso amministrativo a Ruoli lavoro può disattivare i ruoli di lavoro che diventano obsoleti nel sistema. Quando si disattiva un ruolo di lavoro invece di eliminarlo, è possibile mantenere tutte le informazioni storiche associate ad esso.

È inoltre possibile riattivare i ruoli di lavoro precedentemente disattivati.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai ruoli di lavoro</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Impatto della disattivazione dei ruoli di lavoro

Se si disattiva un ruolo di lavoro, questo non viene più visualizzato nelle aree seguenti:

* La [!UICONTROL Assegnazioni] campo typeahead (per attività, task modello, problemi, approvazioni e regole di routing)
* La [!UICONTROL Assegnazioni] campi negli elenchi e nei rapporti
* Profili utente

   >[!NOTE]
   >
   >Quando si aggiunge un nuovo ruolo a un utente, non viene visualizzato un ruolo di processo disattivato. Ma continua a essere visualizzato nel [!UICONTROL Ruolo principale] e [!UICONTROL Altri ruoli] se l&#39;utente è stato associato al ruolo del processo prima che questo sia stato disattivato.

* La [!UICONTROL Condivisione] finestra di dialogo per gli oggetti, inclusa l&#39;assegnazione del modello di layout
* Campi di tipo anticipo nei moduli personalizzati
* La [!UICONTROL Membri pool] campo [!UICONTROL Pool di risorse]
* La [!UICONTROL Ruolo] campo di un [!UICONTROL Tasso di fatturazione] modifica la schermata quando un utente sovrascrive i tassi di fatturazione per i progetti
* La [!UICONTROL Aggiungi assegnazione a bacheca kanban] finestra di dialogo in un progetto
* La [!UICONTROL Ruolo] campo di un piano o di un&#39;iniziativa quando qualcuno utilizza [!DNL Adobe Workfront Scenario Planner].

   La [!DNL Scenario Planner] è disponibile solo nel nuovo [!DNL Adobe Workfront] esperienza e richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi [La [!DNL Scenario Planner] panoramica](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>I ruoli disattivati vengono sempre visualizzati in filtri in elenchi, rapporti e altri strumenti come [!DNL Workload Balancer].

## Considerazioni prima di disattivare un ruolo di lavoro

È preferibile disattivare anziché eliminare i ruoli di lavoro che diventano obsoleti, in modo da poter conservare tutte le informazioni storiche associate ai ruoli eventualmente utilizzati in passato.

>[!NOTE]
>
>Qualsiasi lavoro assegnato al ruolo di lavoro prima della disattivazione rimane assegnato.

Prima di disattivare un ruolo di lavoro non utilizzato, è consigliabile effettuare le seguenti operazioni:

* Creare rapporti per tutti gli oggetti assegnati al ruolo che si intende disattivare e riassegnare a un ruolo attivo. Per informazioni sulla creazione dei rapporti, vedi [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >È possibile creare un rapporto per filtrare le attività o i problemi a cui è assegnato il ruolo disattivato. Quindi utilizzare il rapporto per riassegnare le attività o i problemi in sospeso a un ruolo attivo.

* Fare un inventario di tutti i processi di approvazione, i percorsi di approvazione correnti e le regole di routing o altri oggetti assegnati al ruolo di lavoro che si prevede di disattivare e riassegnare a un ruolo attivo.

   >[!TIP]
   >
   >Quando si utilizzano le code di richiesta, se si disattiva un ruolo di lavoro assegnato come assegnatario predefinito in una regola di routing, il ruolo rimane e le richieste vengono comunque indirizzate al ruolo disattivato. È consigliabile aggiornare le regole di routing con i ruoli attivi prima di disattivare il team.

   Per informazioni sulla creazione di processi di approvazione e regole di routing, vedere i seguenti articoli:

   * [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Disattivazione di un ruolo di lavoro

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su &#x200B; **[!UICONTROL Ruoli processo].**
1. (Facoltativo) In **[!UICONTROL Filtro]** menu a discesa, seleziona **[!UICONTROL Attivo]** per visualizzare solo i ruoli di lavoro attivi.
1. Fare clic sul nome del ruolo di processo che si desidera disattivare.
1. In **[!UICONTROL È attivo]** menu a discesa, seleziona **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Fai clic su **[!UICONTROL Salva modifiche]**.

   Il ruolo di processo è disattivato e non può più essere assegnato al lavoro, associato ai modelli di layout e così via. Per informazioni su tutti gli usi dei ruoli di lavoro in [!DNL Workfront], vedi [Panoramica sul ruolo del lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
