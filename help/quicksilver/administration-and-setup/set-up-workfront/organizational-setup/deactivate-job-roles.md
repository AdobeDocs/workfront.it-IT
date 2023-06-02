---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Disattiva mansioni
description: Come un [!DNL Adobe Workfront] amministratore o un utente con accesso amministrativo ai Ruoli, puoi disattivare i Ruoli che diventano obsoleti nel sistema. Quando si disattiva una mansione invece di eliminarla, è possibile conservare tutte le informazioni storiche ad essa associate.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Disattiva mansioni

Come un [!DNL Adobe Workfront] amministratore o un utente con accesso amministrativo ai Ruoli, puoi disattivare i Ruoli che diventano obsoleti nel sistema. Quando si disattiva una mansione invece di eliminarla, è possibile conservare tutte le informazioni storiche ad essa associate.

È inoltre possibile riattivare i ruoli precedentemente disattivati.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo alle mansioni</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Impatto della disattivazione delle mansioni

Se si disattiva una mansione, questa non verrà più visualizzata nelle seguenti aree:

* Il [!UICONTROL Assegnazioni] campo typeahead (per attività, attività modello, problemi, approvazioni e regole di routing)
* Il [!UICONTROL Assegnazioni] campi in elenchi e report
* Profili utente

   >[!NOTE]
   >
   >Quando si aggiunge un nuovo ruolo a un utente, non viene visualizzato alcun ruolo disattivato. Ma continua a comparire nel [!UICONTROL Ruolo principale] e [!UICONTROL Altri Ruoli] se l’utente era associato alla mansione prima della disattivazione.

* Il [!UICONTROL Condivisione] finestra di dialogo per gli oggetti, inclusa l&#39;assegnazione del modello di layout
* Campi typeahead nei moduli personalizzati
* Il [!UICONTROL Membri del pool] campo in [!UICONTROL Gruppi di risorse]
* Il [!UICONTROL Ruolo] campo di un [!UICONTROL Tariffa di fatturazione] schermata di modifica quando un utente esegue l’override delle tariffe di fatturazione per i progetti
* Il [!UICONTROL Aggiungi assegnazione a bacheca Kanban] finestra di dialogo in un progetto
* Il [!UICONTROL Ruolo] di un piano o di un&#39;iniziativa quando qualcuno utilizza [!DNL Adobe Workfront Scenario Planner].

   Il [!DNL Scenario Planner] è disponibile solo nel nuovo [!DNL Adobe Workfront] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi [Il [!DNL Scenario Planner] panoramica](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>I ruoli disattivati vengono sempre visualizzati nei filtri di elenchi, report e altri strumenti come [!UICONTROL Bilanciatore dei carichi di lavoro].

## Considerazioni prima di disattivare una mansione

È meglio disattivare anziché eliminare le mansioni che diventano obsolete, in modo da poter conservare tutte le informazioni storiche associate alle mansioni che potresti aver utilizzato in passato.

>[!NOTE]
>
>Qualsiasi lavoro assegnato alla mansione prima della disattivazione rimane assegnato.

Prima di disattivare una mansione non utilizzata, è consigliabile effettuare le seguenti operazioni:

* Creare report per tutti gli oggetti assegnati al ruolo che si intende disattivare e riassegnare a un ruolo attivo. Per informazioni sulla creazione di rapporti, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >Puoi creare un rapporto per filtrare le attività o i problemi a cui è assegnato il ruolo disattivato. Utilizzare quindi il report per riassegnare le attività o i problemi in sospeso a un ruolo attivo.

* Inventario di tutti i processi di approvazione, dei percorsi di approvazione correnti e delle regole di instradamento o di altri oggetti assegnati al ruolo che si intende disattivare e riassegnare a un ruolo attivo.

   >[!TIP]
   >
   >Quando si utilizzano le code di richieste, se si disattiva una mansione assegnata come assegnatario predefinito in una regola di instradamento, la mansione rimane e le richieste vengono ancora instradate al ruolo disattivato. Prima di disattivare il team, è consigliabile aggiornare le regole di routing con i ruoli attivi.

   Per informazioni sulla creazione di processi di approvazione e regole di instradamento, vedere gli articoli seguenti:

   * [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Creare regole di instradamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Disattivare una mansione

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su&#x200B; **[!UICONTROL Mansioni].**
1. (Facoltativo) In **[!UICONTROL Filtro]** menu a discesa, seleziona **[!UICONTROL Attivo]** per visualizzare solo i ruoli attivi.
1. Fare clic sul nome della mansione che si desidera disattivare.
1. In **[!UICONTROL È attivo]** menu a discesa, seleziona **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Clic **[!UICONTROL Salva modifiche]**.

   Il ruolo è disattivato e non può più essere assegnato al lavoro, associato ai modelli di layout e così via. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedi [Panoramica sui ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
