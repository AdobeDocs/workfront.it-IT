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
source-git-commit: a30e505aa2061240f92642fda274be66e4947bce
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# Creare e gestire le mansioni

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Con la versione 25.11, la valuta di sostituzione per le mansioni è stata rimossa in Produzione. (La rimozione è avvenuta il 30 ottobre nell’ambiente di anteprima). Invece di avere una valuta di base e di sostituire le valute, ora è disponibile una valuta per le mansioni e i costi e le tariffe di fatturazione sono definiti utilizzando tale valuta.

In qualità di amministratore [!DNL Adobe Workfront] o di utente con accesso amministrativo ai Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione. Per informazioni sull&#39;accesso amministrativo in [!DNL Workfront], vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>I ruoli sono parte integrante della gestione delle risorse. Per utilizzare gli strumenti di pianificazione delle risorse, le mansioni devono avere un costo e una tariffa di fatturazione associati. Per informazioni, vedere [Introduzione a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

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

   * **Valuta**: per impostazione predefinita viene visualizzata la valuta di base. L&#39;amministratore di Workfront aggiunge la valuta di base nell&#39;area Configura. È possibile modificare la selezione in un&#39;altra valuta disponibile e modificare la valuta in intervalli di tempo con data di validità.

     >[!TIP]
     >
     >In questo campo sono disponibili solo le valute disponibili nell&#39;area Tassi di cambio del sistema. Se è impostata una sola valuta, sarà disponibile solo quella.

     Per informazioni sull&#39;impostazione della valuta di base in Workfront, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Per informazioni sulla modifica della valuta di un progetto, vedere [Modificare la valuta del progetto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Tariffa di costo**: tariffa oraria della mansione. Questo valore calcola i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e in ultima analisi i costi pianificati ed effettivi dei progetti. Inserire il tasso utilizzando la valuta selezionata.

     Per le tariffe effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore del costo/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa non avrà una data di inizio e l&#39;ultima tariffa non avrà una data di fine.

     Alcune date vengono aggiunte automaticamente. Ad esempio, se il primo tasso di costo non ha una data di fine e si aggiunge un secondo tasso di costo con una data di inizio del 1° maggio 2025, al primo tasso di costo verrà aggiunta una data di fine del 30 aprile 2025, in modo che non esistano spazi vuoti.

     Per informazioni su come Workfront calcola i costi, vedere [Tracciare i costi](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Quando modifichi una mansione esistente, puoi ordinare l’elenco in modo da visualizzare la data di inizio più recente nella parte superiore dell’elenco dei tassi.

   * **Tariffa di fatturazione**: tariffa oraria di fatturazione della mansione. Questo valore calcola le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo e in ultima analisi le entrate pianificate ed effettive dei progetti. Inserire il tasso utilizzando la valuta selezionata.

     Per le tariffe di fatturazione effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore della fatturazione/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa di fatturazione non avrà una data di inizio e l’ultima tariffa di fatturazione non avrà una data di fine.

     Alcune date vengono aggiunte automaticamente. Ad esempio, se la prima tariffa di fatturazione non ha una data di fine e aggiungi una seconda con una data di inizio del 1° maggio 2025, alla prima tariffa di fatturazione viene aggiunta una data di fine del 30 aprile 2025 in modo che non esistano spazi vuoti.

     Per informazioni su come Workfront calcola i ricavi, vedere [Panoramica su fatturazione e ricavi](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Quando modifichi una mansione esistente, puoi ordinare l’elenco in modo da visualizzare la data di inizio più recente nella parte superiore dell’elenco dei tassi.

1. Fai clic su **[!UICONTROL Crea ruolo]**. Il ruolo è ora disponibile per essere assegnato ad attività, problemi, approvazioni oppure puoi condividere modelli di layout o altri oggetti con esso. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedere [Panoramica sulle mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Per informazioni sull&#39;eliminazione di una mansione, vedere [Elimina mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.


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



