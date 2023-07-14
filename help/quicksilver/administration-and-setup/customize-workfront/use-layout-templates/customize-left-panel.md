---
title: Personalizzare il pannello sinistro utilizzando un modello di layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In un modello di layout, puoi personalizzare ciò che gli utenti visualizzano nell’area del pannello sinistro in Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Personalizzare il pannello sinistro utilizzando un modello di layout

In un modello di layout, puoi personalizzare ciò che gli utenti visualizzano nell’area del pannello sinistro [!DNL Adobe Workfront].

Ad esempio, puoi determinare quali dei seguenti elementi vengono visualizzati dagli utenti nel pannello a sinistra quando visualizzano un’attività:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Le modifiche apportate all’ordine e alla visibilità vengono riportate nell’app mobile.

Per informazioni sulla creazione di modelli di layout, vedere [Creare e gestire modelli di layout](../use-layout-templates/create-and-manage-layout-templates.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Dopo aver configurato un modello di layout, è necessario assegnarlo agli utenti affinché le modifiche apportate siano visibili agli altri utenti. Per informazioni sull&#39;assegnazione di un modello di layout agli utenti, vedere [Assegnare utenti a un modello di layout](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> Per eseguire questi passaggi a livello di sistema, è necessario il livello di accesso [!UICONTROL System Administrator].<p>Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare il pannello sinistro di un’area in [!DNL Workfront]:

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Fare clic sulla freccia giù ![](assets/dropdown-arrow.png) in **[!UICONTROL Personalizzare gli elementi visualizzati dagli utenti]**, quindi fai clic sul pannello a sinistra che desideri personalizzare.

   >[!NOTE]
   >
   >Per informazioni su [!UICONTROL Home] in questo elenco a discesa, vedi [Personalizza [!UICONTROL Home] e [!UICONTROL Riepilogo] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Per informazioni sull&#39;opzione Elenchi, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. In **[!UICONTROL Pannello sinistro]** , eseguire una delle operazioni seguenti per determinare ciò che verrà visualizzato dagli utenti nel pannello sinistro per l&#39;opzione ([!DNL Workfront] o tipo di oggetto) selezionato:

   * Spettacolo ![](assets/add-secondary-nav-item.png) o nascondi ![](assets/delete-secondary-nav-item.png) elementi. Qualsiasi elemento senza ![](assets/add-secondary-nav-item.png) o ![](assets/delete-secondary-nav-item.png) non può essere nascosto.

   * Trascina elementi ![](assets/move-icon---dots.png) per modificarne l’ordine nel pannello a sinistra.
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Opzione</th> 
      <th>Quando gli utenti fanno clic su quanto segue:</th> 
      <th>Visualizzano gli elementi del pannello sinistro scelti tra i seguenti:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Progetto [!UICONTROL]</td> 
      <td>Nome di un progetto</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rates], [!UICONTROL Billing Records], [!UICONTROL Expenses], [!UICONTROL Hours],!UICONTROL Bilanciatore Dei Carichi Di Lavoro], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Attività]</td> 
      <td>Nome di un'attività</td> 
      <td> [!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Dettagli Attività], [!UICONTROL Sottoattività], [!UICONTROL Problemi], [!UICONTROL Ore], [!UICONTROL Approvazioni], [!UICONTROL Spese], [!UICONTROL Predecessori]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>Nome di un problema</td> 
      <td> [!UICONTROL Aggiornamenti], [!UICONTROL Documenti], [!UICONTROL Dettagli Problema], [!UICONTROL Ore], [!UICONTROL Approvazioni]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfoli]</td> 
      <td>Nome di un portfolio</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfoli Details], [!UICONTROL Portfoli] [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nome di un programma</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>Modello [!UICONTROL]</td> 
      <td>Nome di un modello di progetto</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Argomento Coda], [!UICONTROL Argomento]</td> 
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
      <td>Progetti <img src="assets/projects-in-main-menu.png"> nel menu principale [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
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
      <td>[!UICONTROL I Miei Dashboard], [!UICONTROL Dashboard Condivisi], [!UICONTROL Tutti I Dashboard]<p><b>NOTA</b>: se hai creato schede personalizzate per l’area [!UICONTROL Reports] utilizzando un modello di layout in [!DNL Adobe Workfront Classic], vengono visualizzati in fondo all'elenco. Per gli utenti, vengono visualizzate nella parte inferiore del pannello sinistro nell'area [!UICONTROL Dashboards].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Team Scrum]</td> 
      <td>Nome di un team Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>NOTA:</strong> Il <strong>[!UICONTROL Current iteration]</strong> item (elemento) viene visualizzato nel pannello a sinistra solo quando nell’iterazione è presente almeno un’attività o un problema.</p></td> 
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

   >[!NOTE]
   >
   >Gli ultimi 3 elementi in **[!UICONTROL Personalizzare gli elementi visualizzati dagli utenti]** elenco a discesa ([!UICONTROL Elenchi], [!UICONTROL Home e Riepilogo], e [!UICONTROL Marchio]) sono per la configurazione di aree diverse dal pannello sinistro. Per informazioni su di essi, consulta i seguenti articoli:
>   >   
* [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personalizza [!UICONTROL Home] e [!UICONTROL Riepilogo] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Adobe del brand [!DNL Workfront] utilizzo di un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Facoltativo) Se desideri aggiungere un elemento del pannello a sinistra collegato a una delle dashboard della tua organizzazione, fai clic su **[!UICONTROL Aggiungi sezione personalizzata]**, digitare a **[!UICONTROL Titolo sezione personalizzato]** per l’elemento, quindi aggiungi il dashboard.

   Gli elementi del dashboard vengono visualizzati nella parte inferiore del pannello sinistro. Gli utenti visualizzano il titolo della sezione Personalizzata digitato accanto all’elemento del dashboard quando passano il puntatore del mouse sul pannello sinistro.

   >[!NOTE]
   >
   Gli utenti possono aggiungere elementi del dashboard personalizzati al proprio pannello sinistro. Quando si aggiungono elementi del dashboard personalizzati in un modello di layout, gli elementi vengono uniti ai relativi senza sovrascriverli o reimpostarli. Ciò si verifica anche se si assegnano gli utenti a un nuovo modello di layout con elementi del dashboard personalizzati. Per informazioni su come gli utenti possono personalizzare il pannello sinistro, vedi [Creare schede o sezioni personalizzate](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Per informazioni sulle dashboard, consulta [Dashboard](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continuate a personalizzare il modello di layout.

   Oppure

   Se hai finito di personalizzare, fai clic su **[!UICONTROL Salva]**.

   >[!TIP]
   >
   Puoi fare clic su [!UICONTROL Salva] in qualsiasi momento per salvare l’avanzamento, quindi continua a modificare il modello in un secondo momento.
