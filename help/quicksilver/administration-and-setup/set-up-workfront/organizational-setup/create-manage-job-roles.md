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
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Creare e gestire le mansioni

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore [!DNL Adobe Workfront] o di utente con accesso amministrativo ai Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione. Per informazioni sull&#39;accesso amministrativo in [!DNL Workfront], vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

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

## Creare una mansione

Per creare una mansione:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su&#x200B; **[!UICONTROL Ruoli].**
1. Fai clic su **[!UICONTROL Nuova mansione].**
1. Configura quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicare un nome per la mansione. Questo nome viene visualizzato ovunque in [!DNL Workfront], dove viene visualizzato il campo [!UICONTROL Job Role] (Ruolo). </p> <p>Suggerimento: il nome di una mansione può contenere fino a 255 caratteri. Tuttavia, i nomi più lunghi potrebbero essere troncati in alcune aree di [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immettere una descrizione per il ruolo che indichi l'elemento univoco. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Attivo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Selezionare <b>[!UICONTROL Sì]</b> se si desidera che il ruolo sia attivo e disponibile ovunque in [!DNL Workfront] per essere associato a utenti, elementi di lavoro e così via. </p> </li> 
        <li> <p>Selezionare <b>[!UICONTROL No]</b> se si desidera che il ruolo sia disattivato e non disponibile per l'assegnazione a utenti, elementi di lavoro e così via. </p> </li> 
       </ul> <p><span>Per informazioni sulla disattivazione dei ruoli, vedere</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Disattivare i ruoli</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Valuta Di Base]</span> </td> 
      <td> <p><span>Questa è la [!UICONTROL Base Currency], impostata nell'area [!UICONTROL Setup] dall'amministratore di Workfront. Per informazioni, vedere</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Impostare i tassi di cambio</a>.</p> <p>Suggerimento: <span>Impossibile modificare [!UICONTROL Base Currency] a livello di mansione. Questo campo è oscurato e funge da promemoria per la valuta di base del sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Tariffa oraria della mansione. Questo valore calcola i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e in ultima analisi i costi pianificati ed effettivi dei progetti. Immettere il tasso utilizzando la [!UICONTROL Base Currency].</p> 
      <p>Per i tassi di costo effettivi per data, fare clic su <strong>[!UICONTROL Add Rate]</strong>. Immettere il valore del costo/ora per il periodo di tempo e assegnare una data di inizio  e una data di fine  in base alle esigenze. La prima tariffa non avrà una data di inizio e l'ultima tariffa non avrà una data di fine.</p> <p>Alcune date vengono aggiunte automaticamente. Ad esempio, se il primo tasso di costo non ha una data di fine e si aggiunge un secondo tasso di costo con una data di inizio del 1° maggio 2023, al primo tasso di costo verrà aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</p> <p>Suggerimento: quando si modifica una mansione esistente, è possibile selezionare <strong>Ordina per data di inizio</strong> per visualizzare la data di inizio più recente all'inizio dell'elenco dei tassi.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tariffa Di Fatturazione] </td> 
      <td><p>Tariffa oraria fatturazione della mansione. Questo valore calcola le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo e in ultima analisi le entrate pianificate ed effettive dei progetti. Immettere il tasso utilizzando la [!UICONTROL Base Currency].</p> <p>Per le tariffe di fatturazione effettive della data, fare clic su <strong>[!UICONTROL Add Rate]</strong>. Immetti il valore della fatturazione/ora per il periodo di tempo e assegna una data di inizio  e una data di fine  secondo necessità. La prima tariffa di fatturazione non avrà una data di inizio e l’ultima tariffa di fatturazione non avrà una data di fine.</p> <p>Alcune date vengono aggiunte automaticamente. Ad esempio, se la prima tariffa di fatturazione non ha una data di fine e ne aggiungi una seconda con una data di inizio del 1° maggio 2023, alla prima tariffa di fatturazione viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</p> <p>Suggerimento: quando si modifica una mansione esistente, è possibile selezionare <strong>Ordina per data di inizio</strong> per visualizzare la data di inizio più recente all'inizio dell'elenco dei tassi.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sovrascrivi Valuta]</span> </td> 
      <td>
        <p>Selezionare una valuta associata a questa mansione. Valuta utilizzata da [!DNL Workfront] per calcolare i costi e i ricavi associati a questa mansione. </p> 
        <p><span>La valuta di base è diversa da quella impostata dall'amministratore di [!DNL Workfront] nell'area [!UICONTROL Setup] e può essere diversa da quella associata a un progetto.</span> </p> 
        <p>Suggerimento: in questo campo sono disponibili solo le valute disponibili nell'area [!UICONTROL Exchange Rates] del sistema. Se è impostata una sola valuta, questo campo non viene visualizzato.</p> 
       <p><span>Per informazioni sulla configurazione della [!UICONTROL Base Currency] in [!DNL Workfront], vedere</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Impostare i tassi di cambio</a>.</p> <p><span>Per informazioni sulla modifica della valuta di un progetto, vedere</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modificare la valuta del progetto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sostituisci tasso costo valuta]</span> </td> 
      <td>
        <p>Tariffa oraria della mansione che utilizza la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare i costi pianificati ed effettivi delle attività e dei problemi associati alla mansione. </p> 
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. Questo aggiorna anche il tasso di costo per questa mansione quando si utilizza la [!UICONTROL Base Currency].</span> </p> 
        <p>Per informazioni sul calcolo dei costi da parte di [!DNL Workfront], vedere <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> 
       <p>Suggerimento: quando si aggiorna una mansione esistente a cui è già associato un tasso di costo, [!DNL Workfront] calcola il tasso di [!UICONTROL Override Currency] in base al tasso di conversione nel sistema. Se si aggiorna [!UICONTROL Sostituisci tasso costo valuta], anche il tasso di costo del ruolo viene aggiornato automaticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sostituisci tariffa di fatturazione valuta]</span> </td> 
      <td>
        <p>Tariffa oraria di fatturazione della mansione che utilizza la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare i ricavi pianificati ed effettivi delle attività e dei problemi associati alla mansione. </p>
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. Questa opzione aggiorna anche la tariffa di fatturazione per questa mansione quando si utilizza la [!UICONTROL Base Currency].</span> </p>
        <p>Per informazioni sul modo in cui [!DNL Workfront] calcola i ricavi, vedere <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>.</p>
        <p>Suggerimento: quando si aggiorna una mansione esistente a cui è già associata una tariffa di fatturazione, [!DNL Workfront] calcola il tasso della valuta di sostituzione in base al tasso di conversione nel sistema. Se si aggiorna il tasso di fatturazione della divisa di sostituzione, anche il tasso di fatturazione del ruolo viene aggiornato automaticamente. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

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
