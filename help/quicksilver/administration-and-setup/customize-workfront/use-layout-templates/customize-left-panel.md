---
title: Personalizzare il pannello sinistro utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In un modello di layout, puoi personalizzare ciò che gli utenti visualizzano nell’area del pannello sinistro in Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 1%

---

# Personalizzare il pannello sinistro utilizzando un modello di layout

{{preview-fast-release-general}}

<!--Audited: 10/2024-->

In un modello di layout è possibile personalizzare gli elementi visualizzati dagli utenti nell&#39;area del pannello sinistro in [!DNL Adobe Workfront].

Ad esempio, puoi determinare quali dei seguenti elementi vengono visualizzati dagli utenti nel pannello a sinistra durante la visualizzazione di un progetto:

![Pannello sinistro di un progetto](assets/left-panel-in-project.png)

>[!IMPORTANT]
>
>Le modifiche apportate all’ordine e alla visibilità vengono riportate nell’app mobile.

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare gli utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p>
       <p>L’aggiunta di applicazioni personalizzate al menu principale è disponibile solo per le organizzazioni con licenza per Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.</p>
        <p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare il pannello sinistro per un&#39;area in [!DNL Workfront]:

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fare clic sulla freccia giù ![freccia giù](assets/dropdown-arrow.png) in **[!UICONTROL Personalizza gli elementi visualizzati dagli utenti]**, quindi fare clic sul nome di un tipo di oggetto o di un&#39;area [!DNL Workfront] di cui si desidera personalizzare il pannello sinistro.

   I tipi di oggetto e le aree [!DNL Workfront] di cui è possibile personalizzare il pannello sinistro sono elencati nella tabella seguente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo di oggetto o area [!DNL Workfront]</th> 
      <th>Quando gli utenti fanno clic su quanto segue:</th> 
      <th>Sezioni nel pannello sinistro visualizzate dagli utenti dopo che sono state visualizzate nel modello di layout:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Progetto [!UICONTROL]</td> 
      <td>Nome di un progetto</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rates], [!UICONTROL Billing Records], [!UICONTROL Expenses], [!UICONTROL Hours], [!UICONTROL Bilanciatore dei carichi di lavoro], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics], [!UICONTROL Planning]*, [!UICONTROL Custom Application]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Attività]</td> 
      <td>Nome di un'attività</td> 
      <td> [!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Dettagli Attività], [!UICONTROL Sottoattività], [!UICONTROL Problemi], [!UICONTROL Ore], [!UICONTROL Approvazioni], [!UICONTROL Spese], [!UICONTROL Predecessori], [!UICONTROL Applicazione Personalizzata]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>Nome di un problema</td> 
      <td> [!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Dettagli problema], [!UICONTROL Ore], [!UICONTROL Approvazioni], [!UICONTROL Applicazione personalizzata]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Nome di un portfolio</td> 
      <td>[!UICONTROL Progetti], [!UICONTROL Programmi], [!UICONTROL Dettagli Portfolio], [!UICONTROL Portfolio] [!UICONTROL Ottimizzazione], [!UICONTROL Documenti], [!UICONTROL Aggiornamenti], [!UICONTROL Planning]*, [!UICONTROL Applicazione personalizzata]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nome di un programma</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Planning]*, [!UICONTROL Custom application]**</td> 
     </tr> 
     <tr> 
      <td>Modello [!UICONTROL]</td> 
      <td>Nome di un modello di progetto</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Gruppo]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Attività Modello]</td> 
      <td>Nome di un'attività modello</td> 
      <td>[!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Dettagli Attività Modello], [!UICONTROL Sottoattività], [!UICONTROL Spese], [!UICONTROL Approvazioni], [!UICONTROL Predecessori]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Fatturazione]</td> 
      <td>Nome di un record di fatturazione per un progetto</td> 
      <td>[!UICONTROL Dettagli record fatturazione], [!UICONTROL Ore fatturabili], [!UICONTROL Spese fatturabili], [!UICONTROL Retribuzioni fisse]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Progetti]</td> 
      <td>Progetta <img src="assets/projects-in-main-menu.png"> nel menu principale [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Progetti]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>Nome di una richiesta</td> 
      <td>[!UICONTROL Nuova Richiesta], [!UICONTROL Richieste Inviate], [!UICONTROL Tutte Le Richieste], [!UICONTROL Bozze]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Nome di un dashboard</td> 
      <td>[!UICONTROL I Miei Dashboard], [!UICONTROL Dashboard Condivisi], [!UICONTROL Tutti I Dashboard]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Team Scrum]</td> 
      <td>Nome di un team Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>NOTA:</strong> l'elemento <strong>[!UICONTROL Current iteration]</strong> viene visualizzato nel pannello sinistro solo quando nell'iterazione è presente almeno un'attività o un problema.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>Nome di un team Kanban</td> 
      <td>[!UICONTROL Bilanciatore dei carichi di lavoro], [!UICONTROL Kanban Board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Team Waterfall]</td> 
      <td>Nome di un team Waterfall</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Aggiornamenti], [!UICONTROL Richieste Team], [!UICONTROL Impostazioni Team]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iterazione]</td> 
      <td>Nome di un'iterazione</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   *La società deve acquistare una licenza aggiuntiva per Workfront Planning per poter aggiungere quest&#39;area al pannello sinistro di progetti, portfolio e programmi. Per ulteriori informazioni, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)

   **Le applicazioni personalizzate devono essere create separatamente prima di diventare disponibili come opzioni del menu principale. Per ulteriori informazioni, vedere [Creare un&#39;applicazione personalizzata per Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).


1. Nell&#39;elenco **[!UICONTROL Pannello sinistro]**, eseguire una delle operazioni seguenti per determinare gli elementi visualizzati dagli utenti nel pannello sinistro per l&#39;area [!DNL Workfront] o il tipo di oggetto selezionato:

   * Fai clic sulle icone **Mostra** ![Mostra icona](assets/add-secondary-nav-item.png) o **Nascondi** ![Nascondi icona](assets/delete-secondary-nav-item.png) per visualizzare o nascondere le sezioni nel pannello a sinistra. Non puoi nascondere elementi che non hanno un&#39;icona **Mostra** o **Nascondi**.

   * Trascina gli elementi ![Icona Sposta](assets/move-icon---dots.png) per modificarne l&#39;ordine nel pannello sinistro.

   >[!NOTE]
   >
   >I seguenti elementi nell&#39;elenco a discesa **[!UICONTROL Personalizza gli elementi visualizzati dagli utenti]** fanno riferimento ad aree diverse dal pannello sinistro:
   >* [!UICONTROL Elenchi]
   >* [!UICONTROL Pannello di riepilogo]
   >* [!UICONTROL Home]
   >* [!UICONTROL Marchio]
   > 
   >Per informazioni su come personalizzare le aree aggiuntive, vedere gli articoli seguenti:
   >
   >* [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Personalizza il [!UICONTROL pannello di riepilogo] utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Personalizza la Home usando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Brand Adobe [!DNL Workfront] utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Facoltativo) Se desideri aggiungere un elemento del pannello sinistro collegato a uno dei dashboard dell&#39;organizzazione, fai clic su **[!UICONTROL Aggiungi dashboard]**, digita il **[!UICONTROL Nome collegamento rapido]** per l&#39;elemento, quindi scegli il dashboard.

   È necessario creare il dashboard prima che venga visualizzato nell&#39;elenco.

   Gli elementi del dashboard vengono visualizzati nella parte inferiore del pannello sinistro.

   >[!NOTE]
   >
   >Gli utenti possono aggiungere elementi del dashboard personalizzati al proprio pannello sinistro. Quando si aggiungono elementi del dashboard personalizzati in un modello di layout, gli elementi vengono visualizzati in aggiunta a quelli aggiunti, senza sovrascriverli o reimpostarli. Ciò si verifica anche se si assegnano gli utenti a un nuovo modello di layout con elementi del dashboard personalizzati. Per informazioni su come personalizzare il pannello sinistro, vedere [Aggiungere un dashboard nel pannello sinistro di un oggetto o di un&#39;area di Workfront](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Per informazioni sulle dashboard, vedere [Dashboard](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. <span class="preview">Nell&#39;ambiente di anteprima: continuare a personalizzare il modello di layout. Puoi fare clic su **Applica** in qualsiasi momento per salvare i tuoi progressi.</span>

   <span class="preview">O</span>

   <span class="preview">Se hai completato la personalizzazione, fai clic su **Salva e chiudi**.</span>

1. Nell’ambiente di produzione: continua a personalizzare il modello di layout.

   Oppure

   Se hai completato la personalizzazione, fai clic su **Salva**.

   >[!TIP]
   >
   >Puoi fare clic su **Salva** in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
