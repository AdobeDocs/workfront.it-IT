---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Creare e gestire i ruoli
description: In qualità di amministratore  [!DNL Adobe Workfront]  o di utente con accesso amministrativo ai Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: d342df9949eb1434acbb53c29b7e329dd91c9b28
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Creare e gestire le mansioni

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Con la versione 25.11, la valuta di sostituzione per le mansioni diventerà obsoleta in Produzione. (La rimozione verrà effettuata il 30 ottobre nell’ambiente di anteprima). Invece di avere una valuta di base e di sostituire le valute, sarà disponibile una valuta per le mansioni e i costi e le tariffe di fatturazione saranno definiti utilizzando tale valuta.

In qualità di amministratore [!DNL Adobe Workfront] o di utente con accesso amministrativo ai Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione. Per informazioni sull&#39;accesso amministrativo in [!DNL Workfront], vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai Ruoli</td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una mansione

Per creare una mansione:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su&#x200B; **[!UICONTROL Ruoli].**
1. Fai clic su **[!UICONTROL Nuova mansione].**
1. Configura i campi seguenti:

   * **Nome**: indicare un nome per la mansione. Questo è il nome visualizzato ovunque in Workfront, dove viene visualizzato il campo Ruolo.

     >[!TIP]
     >
     >Il nome di una mansione può contenere fino a 255 caratteri. Tuttavia, i nomi più lunghi potrebbero essere troncati in alcune aree di Workfront.

   * **Descrizione**: immettere una descrizione per il ruolo che indichi l&#39;elemento univoco.
   * **È attivo**: selezionare **Sì** se si desidera che il ruolo sia attivo e disponibile ovunque in Workfront per essere associato a utenti, elementi di lavoro e così via. Selezionare **No** se si desidera che il ruolo sia disattivato e non disponibile per l&#39;assegnazione a utenti, elementi di lavoro e così via.

     Per informazioni sulla disattivazione dei ruoli, vedere [Disattivare i ruoli](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Valuta di base**: è la valuta di base impostata dall&#39;amministratore di Workfront nell&#39;area Configura. Per informazioni, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     >[!TIP]
     >
     >Impossibile modificare la valuta di base a livello di mansione. Questo campo è oscurato e funge da promemoria per ciò che la valuta di base è per il sistema.

   * **Tariffa di costo**: tariffa oraria della mansione. Questo valore calcola i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e in ultima analisi i costi pianificati ed effettivi dei progetti. Inserire il tasso utilizzando la divisa di base.

     Per le tariffe effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore del costo/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa non avrà una data di inizio e l&#39;ultima tariffa non avrà una data di fine.

     Alcune date vengono aggiunte automaticamente. Ad esempio, se il primo tasso di costo non ha una data di fine e si aggiunge un secondo tasso di costo con una data di inizio del 1° maggio 2025, al primo tasso di costo verrà aggiunta una data di fine del 30 aprile 2025, in modo che non esistano spazi vuoti.

     >[!TIP]
     >
     >Quando modifichi una mansione esistente, puoi selezionare **Ordina per data di inizio** per visualizzare la data di inizio più recente all&#39;inizio dell&#39;elenco dei tassi.

   * **Tariffa di fatturazione**: tariffa oraria di fatturazione della mansione. Questo valore calcola le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo e in ultima analisi le entrate pianificate ed effettive dei progetti. Inserire il tasso utilizzando la divisa di base.

     Per le tariffe di fatturazione effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore della fatturazione/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa di fatturazione non avrà una data di inizio e l’ultima tariffa di fatturazione non avrà una data di fine.

     Alcune date vengono aggiunte automaticamente. Ad esempio, se la prima tariffa di fatturazione non ha una data di fine e aggiungi una seconda con una data di inizio del 1° maggio 2025, alla prima tariffa di fatturazione viene aggiunta una data di fine del 30 aprile 2025 in modo che non esistano spazi vuoti.

     >[!TIP]
     >
     >Quando modifichi una mansione esistente, puoi selezionare **Ordina per data di inizio** per visualizzare la data di inizio più recente all&#39;inizio dell&#39;elenco dei tassi.

   * **Sovrascrivi valuta**: selezionare una valuta associata a questa mansione. Valuta utilizzata da Workfront per calcolare i costi e i ricavi associati a questa mansione.

     È diversa dalla valuta di base impostata dall’amministratore di Workfront nell’area Configura e può essere diversa dalla valuta associata a un progetto.

     >[!TIP]
     >
     >In questo campo sono disponibili solo le valute disponibili nell&#39;area Tassi di cambio del sistema. Se è impostata una sola valuta, questo campo non viene visualizzato.

     Per informazioni sull&#39;impostazione della valuta di base in Workfront, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Per informazioni sulla modifica della valuta di un progetto, vedere [Modificare la valuta del progetto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Sostituisci tasso costo valuta**: è il tasso del costo orario della mansione che utilizza la valuta di sostituzione selezionata. Workfront utilizza questo valore per calcolare i costi pianificati ed effettivi delle attività e dei problemi associati alla mansione.

     Inserire il tasso nella divisa di sostituzione sopra specificata. In questo modo viene aggiornato anche il tasso di costo per questa mansione quando si utilizza la valuta di base.

     Per informazioni su come Workfront calcola i costi, vedere [Tracciare i costi](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Quando si aggiorna una mansione esistente a cui è già associato un tasso di costo, Workfront calcola il tasso di cambio di sostituzione in base al tasso di conversione del sistema. Se si aggiorna l&#39;opzione Sostituisci tasso costo divisa, anche il tasso di costo della mansione viene aggiornato automaticamente.

   * **Sovrascrivi tariffa di fatturazione valuta**: tariffa oraria di fatturazione della mansione che utilizza la valuta di sostituzione selezionata. Workfront utilizza questo valore per calcolare i ricavi pianificati ed effettivi delle attività e dei problemi associati alla mansione.

     Inserire il tasso nella divisa di sostituzione sopra specificata. Questo aggiorna anche la tariffa di fatturazione per questa mansione quando si utilizza la valuta di base.

     Per informazioni su come Workfront calcola i ricavi, vedere [Panoramica su fatturazione e ricavi](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Quando si aggiorna una mansione esistente a cui è già associato un tasso di fatturazione, Workfront calcola il tasso di cambio di sostituzione in base al tasso di conversione del sistema. Se si aggiorna il tasso di fatturazione della divisa di sostituzione, anche il tasso di fatturazione della mansione viene aggiornato automaticamente.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

>[!TIP]
>
>I ruoli sono parte integrante della gestione delle risorse. Per utilizzare gli strumenti di pianificazione delle risorse, le mansioni devono avere un costo e una tariffa di fatturazione associati. Per informazioni, vedere [Introduzione a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Fai clic su **[!UICONTROL Crea ruolo]**. Il ruolo è ora disponibile per essere assegnato ad attività, problemi, approvazioni oppure puoi condividere modelli di layout o altri oggetti con esso. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedere [Panoramica sulle mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Per informazioni sull&#39;eliminazione di una mansione, vedere [Elimina mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
