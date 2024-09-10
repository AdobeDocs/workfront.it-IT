---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Disattiva Ruoli
description: In qualità di amministratore  [!DNL Adobe Workfront]  o di utente con accesso amministrativo ai Ruoli, puoi disattivare i Ruoli che diventano obsoleti nel tuo sistema. Quando si disattiva una mansione invece di eliminarla, è possibile conservare tutte le informazioni storiche ad essa associate.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 1%

---

# Disattiva mansioni

In qualità di amministratore [!DNL Adobe Workfront] o di utente con accesso amministrativo ai Ruoli, puoi disattivare i Ruoli che diventano obsoleti nel tuo sistema. Quando si disattiva una mansione invece di eliminarla, è possibile conservare tutte le informazioni storiche ad essa associate.

È inoltre possibile riattivare i ruoli precedentemente disattivati.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>
   <p>Nuovo: [!UICONTROL Standard]</p>
   <p>Oppure</p>
   <p>Corrente: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai Ruoli</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Impatto della disattivazione delle mansioni

Se si disattiva una mansione, questa non verrà più visualizzata nelle seguenti aree:

* Il campo di completamento automatico [!UICONTROL Assegnazioni] (per attività, attività modello, problemi, approvazioni e regole di routing)
* I campi [!UICONTROL Assegnazioni] negli elenchi e nei report
* Profili utente

  >[!NOTE]
  >
  >Quando si aggiunge un nuovo ruolo a un utente, non viene visualizzato alcun ruolo disattivato. Ma continua a essere visualizzato nei campi [!UICONTROL Ruolo principale] e [!UICONTROL Altri ruoli] se l&#39;utente era associato alla mansione prima che fosse disattivato.

* Finestra di dialogo [!UICONTROL Condivisione] per gli oggetti, inclusa l&#39;assegnazione del modello di layout
* Campi typeahead nei moduli personalizzati
* Il campo [!UICONTROL Membri del pool] in [!UICONTROL Pool di risorse]
* Il campo [!UICONTROL Mansione] di una schermata di modifica [!UICONTROL Tariffa di fatturazione] quando un utente sta sostituendo le tariffe di fatturazione per i progetti
* Finestra di dialogo [!UICONTROL Aggiungi assegnazione a bacheca Kanban] in un progetto
* Il campo [!UICONTROL Ruolo] di un piano o di un&#39;iniziativa quando qualcuno sta utilizzando [!DNL Adobe Workfront Scenario Planner].

  [!DNL Scenario Planner] è disponibile solo nella nuova esperienza [!DNL Adobe Workfront] e richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedere [The [!DNL Scenario Planner] overview](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>I ruoli disattivati vengono sempre visualizzati nei filtri di elenchi, report e altri strumenti come il [!UICONTROL Bilanciatore dei carichi di lavoro].

## Considerazioni prima di disattivare una mansione

È meglio disattivare anziché eliminare le mansioni che diventano obsolete, in modo da poter conservare tutte le informazioni storiche associate alle mansioni che potresti aver utilizzato in passato.

>[!NOTE]
>
>Qualsiasi lavoro assegnato alla mansione prima della disattivazione rimane assegnato.

Prima di disattivare una mansione non utilizzata, è consigliabile effettuare le seguenti operazioni:

* Creare report per tutti gli oggetti assegnati al ruolo che si intende disattivare e riassegnare a un ruolo attivo. Per informazioni sulla creazione di report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

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

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su&#x200B; **[!UICONTROL Ruoli].**
1. (Facoltativo) Nel menu a discesa **[!UICONTROL Filtro]**, seleziona **[!UICONTROL Attivo]** per visualizzare solo i ruoli attivi.
1. Fare clic sul nome della mansione che si desidera disattivare.
1. Nel menu a discesa **[!UICONTROL È attivo]**, selezionare **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Fai clic su **[!UICONTROL Salva modifiche]**.

   Il ruolo è disattivato e non può più essere assegnato al lavoro, associato ai modelli di layout e così via. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedere [Panoramica sulle mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
