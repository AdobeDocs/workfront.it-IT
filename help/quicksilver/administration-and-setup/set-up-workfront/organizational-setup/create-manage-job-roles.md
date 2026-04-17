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
source-git-commit: d8a01839b8f1332741f87be766f3ccb7d08cef96
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 2%

---

# Creare e gestire le mansioni

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Con la versione 25.11, la valuta di sostituzione per le mansioni è stata rimossa in Produzione. (La rimozione è avvenuta il 30 ottobre nell’ambiente di anteprima). Invece di avere una valuta di base e di sostituire le valute, ora è disponibile una valuta per le mansioni e i costi e le tariffe di fatturazione sono definiti utilizzando tale valuta.

In qualità di amministratore [!DNL Adobe Workfront] o di utente Standard con accesso in modifica alle mansioni, puoi creare mansioni che possono essere assegnate agli utenti ed eliminare mansioni predefinite non rilevanti per la tua organizzazione. Per informazioni sull&#39;accesso amministrativo in [!DNL Workfront], vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>I ruoli sono parte integrante della gestione delle risorse. Per utilizzare gli strumenti di pianificazione delle risorse, le mansioni devono avere un costo e una tariffa di fatturazione associati. Per informazioni, vedere [Introduzione a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Per creare o modificare una mansione: qualsiasi pacchetto Workfront o Workflow</p>
   <p>Per applicare gli attributi della tariffa e aggiungere moduli personalizzati alla mansione: Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Piano]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a Ruoli</td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una mansione

Per creare una mansione:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Ruoli]**.
1. Fai clic su **[!UICONTROL Nuovo ruolo] > Crea nuovo ruolo**.
1. Immettere le informazioni nei campi riportati di seguito.

   * **Nome**: indicare un nome per la mansione. Questo è il nome visualizzato ovunque in Workfront, dove viene visualizzato il campo Ruolo.

     >[!TIP]
     >
     >Il nome di una mansione può contenere fino a 255 caratteri. Tuttavia, i nomi più lunghi potrebbero essere troncati in alcune aree di Workfront.

   * **Descrizione**: immettere una descrizione per il ruolo che indichi l&#39;elemento univoco.
   * **È attivo**: selezionare **Sì** se si desidera che il ruolo sia attivo e disponibile ovunque in Workfront per essere associato a utenti, elementi di lavoro e così via. Selezionare **No** se si desidera che il ruolo sia disattivato e non disponibile per l&#39;assegnazione a utenti, elementi di lavoro e così via.

     Per informazioni sulla disattivazione dei ruoli, vedere [Disattivare i ruoli](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

1. Fai clic su **[!UICONTROL Crea ruolo]**. Il ruolo è ora disponibile per essere assegnato ad attività, problemi, approvazioni oppure puoi condividere modelli di layout o altri oggetti con esso. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedere [Panoramica sulle mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Per informazioni sull&#39;eliminazione di una mansione, vedere [Elimina mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

## Aggiungere tariffe e attributi a una mansione

La fatturazione e i tassi di costo di una mansione vengono utilizzati nei calcoli finanziari.

Gli attributi delle tariffe sono supportati nelle aree di Workfront in cui le tariffe esistono, ad esempio i ruoli e gli utenti. Quando gli attributi vengono applicati a una mansione, le relative assegnazioni vengono risolte automaticamente in base alle tariffe corrette.

Per ulteriori informazioni, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Ruoli]**.
1. Fare clic sul nome di una mansione esistente per modificarla.
1. Per aggiornare i dettagli della mansione, fai clic su **Dettagli** nel pannello a sinistra.
1. (Facoltativo) Per allegare un modulo personalizzato alla mansione, fare clic sul campo **Aggiungi modulo personalizzato** nell&#39;angolo superiore destro della pagina Dettagli e selezionare un modulo personalizzato dall&#39;elenco visualizzato.

   Per ulteriori informazioni su come allegare un modulo personalizzato, vedere [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Fai clic su [!UICONTROL **Tariffe**] nel pannello a sinistra.
1. Fai clic su [!UICONTROL **Fatturazione**] o [!UICONTROL **Costo**] per selezionare il tipo di tariffa.
1. Fare clic su [!UICONTROL **Aggiungi tariffe**] per aggiungere una nuova tariffa.

   Oppure

   Seleziona una tariffa esistente e fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png) per aggiornarla.

   >[!NOTE]
   >
   >Poiché ogni tasso è associato alla combinazione di ruolo e attributi per creare un tasso univoco, gli attributi non possono essere modificati quando si modifica un tasso.

1. Nella casella **Nuova tariffa** selezionare gli attributi della tariffa, ad esempio Agenzia, Ubicazione o Centro di costo.

   >[!NOTE]
   >
   >Questi attributi vengono definiti separatamente e possono influire sui calcoli dei ricavi e dei costi. Per ulteriori informazioni, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Selezionare **Valuta** per il tasso. L&#39;amministratore di Workfront aggiunge la valuta di base nell&#39;area Configura. È possibile modificare la selezione in un&#39;altra valuta disponibile e modificare la valuta in intervalli di tempo con data di validità.

   >[!TIP]
   >
   >In questo campo sono disponibili solo le valute disponibili nell&#39;area Tassi di cambio del sistema. Se è impostata una sola valuta, sarà disponibile solo quella.

   Per informazioni sull&#39;impostazione della valuta di base in Workfront, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Per informazioni sulla modifica della valuta di un progetto, vedere [Modificare la valuta del progetto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Condizionale) Per una tariffa di fatturazione, immettere **Tariffa di fatturazione** per questa mansione.

   Tariffa oraria fatturazione della mansione. Questo valore calcola le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo e in ultima analisi le entrate pianificate ed effettive dei progetti. Inserire il tasso utilizzando la valuta selezionata.

   Se si utilizzano gli attributi, gli attributi e la mansione si combinano per definire un tasso univoco. Ad esempio, un ruolo Designer a New York per l&#39;Agenzia A può avere una tariffa separata da un ruolo Designer a Parigi per l&#39;Agenzia B.

   Per le tariffe di fatturazione effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore della fatturazione/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa di fatturazione non avrà una data di inizio e l’ultima tariffa di fatturazione non avrà una data di fine.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   Workfront ti consente di lasciare degli spazi tra gli intervalli di date, ma riceverai un avviso per confermare che è intenzionale.

   Per informazioni su come Workfront calcola i ricavi, vedere [Panoramica su fatturazione e ricavi](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Quando modifichi una mansione esistente, puoi ordinare l’elenco in modo da visualizzare la data di inizio più recente nella parte superiore dell’elenco dei tassi.

1. (Condizionale) Per una tariffa, immettere la **Tariffa costo** per questa mansione.

   Tariffa oraria della mansione. Questo valore calcola i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e in ultima analisi i costi pianificati ed effettivi dei progetti. Inserire il tasso utilizzando la valuta selezionata.

   Se si utilizzano gli attributi, gli attributi e la mansione si combinano per definire un tasso univoco. Ad esempio, un ruolo Designer a New York per l&#39;Agenzia A può avere una tariffa separata da un ruolo Designer a Parigi per l&#39;Agenzia B.

   Per le tariffe effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore del costo/ora per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La prima tariffa non avrà una data di inizio e l&#39;ultima tariffa non avrà una data di fine.

   Alcune date vengono aggiunte automaticamente. Ad esempio, se il primo tasso di costo non ha una data di fine e si aggiunge un secondo tasso di costo con una data di inizio del 1° maggio, al primo tasso di costo viene aggiunta una data di fine del 30 aprile in modo che non esistano spazi vuoti.

   Per informazioni su come Workfront calcola i costi, vedere [Tracciare i costi](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Quando modifichi una mansione esistente, puoi ordinare l’elenco in modo da visualizzare la data di inizio più recente nella parte superiore dell’elenco dei tassi.

1. Fai clic su [!UICONTROL **Salva**].

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

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



