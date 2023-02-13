---
title: Personalizzare il pannello a sinistra utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In un modello di layout, è possibile personalizzare ciò che gli utenti visualizzano nell’area del pannello a sinistra in Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Personalizzare il pannello a sinistra utilizzando un modello di layout

In un modello di layout, è possibile personalizzare gli elementi visualizzati dagli utenti nell’area del pannello a sinistra [!DNL Adobe Workfront].

Ad esempio, puoi determinare quale dei seguenti elementi viene visualizzato dagli utenti nel pannello a sinistra durante la visualizzazione di un’attività:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Le modifiche apportate all’ordine e alla visibilità si riflettono nell’app mobile.

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso [!UICONTROL System Administrator].<p>Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare il pannello a sinistra di un’area in [!DNL Workfront]:

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fai clic sulla freccia giù ![](assets/dropdown-arrow.png) sotto **[!UICONTROL Personalizzare ciò che gli utenti visualizzano]**, quindi fai clic sul pannello a sinistra da personalizzare.

   >[!NOTE]
   >
   >Per informazioni sulla [!UICONTROL Pagina principale] in questo elenco a discesa, vedi [Personalizza [!UICONTROL Pagina principale] e [!UICONTROL Riepilogo] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Per informazioni sull’opzione Elenchi, consulta [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. In **[!UICONTROL Pannello a sinistra]** effettua una delle seguenti operazioni per determinare cosa vedranno gli utenti nel pannello a sinistra per l’opzione ([!DNL Workfront] area o tipo di oggetto) selezionata:

   * Mostra ![](assets/add-secondary-nav-item.png) o nascondere ![](assets/delete-secondary-nav-item.png) oggetti. Qualsiasi elemento senza ![](assets/add-secondary-nav-item.png) o ![](assets/delete-secondary-nav-item.png) non può essere nascosto.

   * Trascinamento di elementi ![](assets/move-icon---dots.png) per modificare l’ordine nel pannello a sinistra.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Opzione</th> 
      <th>Quando gli utenti fanno clic su quanto segue...</th> 
      <th>Visualizzano gli elementi del pannello a sinistra scelti tra i seguenti:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>Nome di un progetto</td> 
      <td>Attività di [!UICONTROL], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rilling Rall Rates],], Record di fatturazione, [!UICONTROL Cost], [!UICONTROL Cost], [!UICONTROL Hours], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL CONTROL Gruppo di argomenti], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Nome di un'attività</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expensors], [!UICONTROL Predecessori]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>Nome di un problema</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues Details], [!UICONTROL Hours], [!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>Portfolio [!UICONTROL]</td> 
      <td>Nome di un portafoglio</td> 
      <td>Progetti, [!UICONTROL Programmi], [!UICONTROL Dettagli Portfolio], [!UICONTROL Portfolio], [!UICONTROL Optimization], [!UICONTROL Documenti], [!UICONTROL Aggiornamenti]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nome di un programma</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Nome di un modello di progetto</td> 
      <td>Attività dei modelli, [!UICONTROL Template Details], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], Dettagli coda,],],], [!UICONTROL Regole di routing], [!UICONTROL Argomento Coda], [!UICONTROL Gruppo di argomenti]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>Nome di un'attività modello</td> 
      <td>[!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Template Task Details], [!UICONTROL Sottoattività], [!UICONTROL Spese], [!UICONTROL Approvazioni], [!UICONTROL Predecessori]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Record di fatturazione]</td> 
      <td>Nome di un record di fatturazione per un progetto</td> 
      <td>[!UICONTROL Dettagli record fatturazione], [!UICONTROL Ore fatturabili], [!UICONTROL Spese fatturabili], [!UICONTROL Entrate fisse]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Progetti <img src="assets/projects-in-main-menu.png"> nel menu principale <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>Nome di una richiesta</td> 
      <td>[!UICONTROL Nuova richiesta], [!UICONTROL Richieste inviate], [!UICONTROL Tutte le richieste], [!UICONTROL Bozze]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Nome di un dashboard</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b>NOTA</b>: Se hai creato schede personalizzate per l’area Rapporti utilizzando un modello di layout in [!DNL Adobe Workfront Classic], vengono visualizzati in fondo a questo elenco. Per gli utenti, vengono visualizzati nella parte inferiore del pannello di sinistra nell’area delle dashboard di .</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Nome di un team Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>NOTA:</strong> La <strong>[!UICONTROL iterazione corrente]</strong> nel pannello di sinistra viene visualizzato solo quando è presente almeno un'attività o un problema nell'iterazione.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>Nome di un team Kanban</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Aggiornamenti], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>Nome di una squadra di cascata</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
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

   >[!NOTE]
   >
   >Gli ultimi 3 elementi nel **[!UICONTROL Personalizzare ciò che gli utenti visualizzano]** elenco a discesa ([!UICONTROL Elenchi], [!UICONTROL Home e Riepilogo]e [!UICONTROL Branding]) sono per le aree di configurazione diverse dal pannello a sinistra. Per informazioni su di essi, consulta questi articoli:
>   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personalizza [!UICONTROL Pagina principale] e [!UICONTROL Riepilogo] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Adobe del marchio [!DNL Workfront] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. (Facoltativo) Se desideri aggiungere un elemento del pannello sinistro che si collega a una delle dashboard della tua organizzazione, fai clic su **[!UICONTROL Aggiungi sezione personalizzata]**, digitare a **[!UICONTROL Titolo sezione personalizzato]** per l’elemento , quindi aggiungi il dashboard.

   Gli elementi del dashboard vengono visualizzati nella parte inferiore del pannello di sinistra. Gli utenti visualizzano il titolo della sezione Personalizzato digitato accanto all’elemento del dashboard quando passano il puntatore del mouse sul pannello di sinistra.

   >[!NOTE]
   Gli utenti possono aggiungere elementi personalizzati del dashboard al proprio pannello a sinistra. Quando si aggiungono elementi dashboard personalizzati in un modello di layout, gli elementi vengono uniti con i rispettivi senza sovrascriverli o reimpostarli. Questo vale anche se assegni gli utenti a un nuovo modello di layout con elementi dashboard personalizzati. Per informazioni su come gli utenti possono personalizzare il pannello di sinistra, vedi [Creare schede o sezioni personalizzate](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Per informazioni sulle dashboard, consulta [Dashboard](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continua a personalizzare il modello di layout.

   Oppure

   Al termine della personalizzazione, fai clic su **[!UICONTROL Salva]**.

   >[!TIP]
   Puoi fare clic su [!UICONTROL Salva] in qualsiasi momento per salvare l&#39;avanzamento, quindi continuare a modificare il modello in un secondo momento.
