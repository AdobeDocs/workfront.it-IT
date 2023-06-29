---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Creare e gestire le mansioni
description: Come un [!DNL Adobe Workfront] amministratore o un utente con accesso amministrativo a Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---

# Creare e gestire le mansioni

{{highlighted-preview}}

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Come un [!DNL Adobe Workfront] amministratore o un utente con accesso amministrativo a Ruoli, puoi creare Ruoli che possono essere assegnati agli utenti ed eliminare Ruoli predefiniti che non sono rilevanti per la tua organizzazione. Per informazioni sull’accesso amministrativo in [!DNL Workfront], vedi [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo alle mansioni</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Creare una mansione

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su&#x200B; **[!UICONTROL Mansioni].**
1. Clic **[!UICONTROL Crea Ruolo].**
1. Configura quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicare un nome per la mansione. Questo è il nome che compare ovunque in [!DNL Workfront] dove viene visualizzato il campo [!UICONTROL Ruolo]. </p> <p>Suggerimento: il nome di una mansione può contenere fino a 255 caratteri. Tuttavia, i nomi più lunghi potrebbero essere troncati in alcune aree di [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL È Attivo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri che il ruolo sia attivo e disponibile ovunque in [!DNL Workfront] da associare a utenti, elementi di lavoro, ecc. </p> </li> 
        <li> <p>Seleziona <b>[!UICONTROL No]</b>, se desideri che il ruolo sia disattivato e non disponibile per l’assegnazione a utenti, elementi di lavoro, ecc. </p> </li> 
       </ul> <p><span>Per informazioni sulla disattivazione delle mansioni, vedi</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Disattiva mansioni</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immettere una descrizione per il ruolo che indichi l'elemento univoco. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Valuta Di Base]</span> </td> 
      <td> <p><span>Questa è la [!UICONTROL Base Currency], impostata nell'area [!UICONTROL Setup] dall'amministratore di Workfront. Per informazioni, consulta</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta tassi di cambio</a> .</p> <p>Suggerimento <span>Non è possibile modificare la [!UICONTROL Base Currency] a livello di ruolo. Questo campo è oscurato e funge da promemoria per ciò che la valuta di base è per il sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Costo/Ora.]</td> 
      <td><p>Tariffa oraria della mansione. Questo valore calcola i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e in ultima analisi i costi pianificati ed effettivi dei progetti. Immettere il tasso utilizzando la [!UICONTROL Base Currency].</p> 
      <p><span class="preview">Per le tariffe effettive per data, fare clic su <strong>[!UICONTROL Add Rate]</strong>. Immettere il valore del costo/ora per il periodo di tempo e assegnare una data di inizio [!UICONTROL] e una data di fine [!UICONTROL] in base alle esigenze. La prima tariffa non avrà una data di inizio e l'ultima tariffa non avrà una data di fine.</span></p> <p><span class="preview">Alcune date vengono aggiunte automaticamente. Ad esempio, se il primo tasso di costo non ha una data di fine e si aggiunge un secondo tasso di costo con una data di inizio del 1° maggio 2023, al primo tasso di costo verrà aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fatturazione/ Ora.] </td> 
      <td><p>Tariffa oraria fatturazione della mansione. Questo valore calcola le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo e in ultima analisi le entrate pianificate ed effettive dei progetti. Immettere il tasso utilizzando la [!UICONTROL Base Currency].</p> <p><span class="preview">Per le tariffe di fatturazione effettive della data, fai clic su <strong>[!UICONTROL Add Rate]</strong>. Immetti il valore della fatturazione/ora per il periodo di tempo e assegna una data di inizio [!UICONTROL] e una data di fine [!UICONTROL] secondo necessità. La prima tariffa di fatturazione non avrà una data di inizio e l’ultima tariffa di fatturazione non avrà una data di fine.</span></p> <p><span class="preview">Alcune date vengono aggiunte automaticamente. Ad esempio, se la prima tariffa di fatturazione non ha una data di fine e ne aggiungi una seconda con una data di inizio del 1° maggio 2023, alla prima tariffa di fatturazione viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</span></p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sovrascrivi valuta]</span> </td> 
      <td> 
       <div> 
        <p>Selezionare una valuta associata a questa mansione. Questa è la valuta che [!DNL Workfront] utilizza per calcolare i costi e i ricavi associati a questa mansione. </p> 
        <p><span>È diverso dalla [!UICONTROL Base Currency] impostata dal [!DNL Workfront] nell'area [!UICONTROL Setup] e può essere diversa dalla valuta associata a un progetto.</span> </p> 
        <p>Suggerimento: in questo campo sono disponibili solo le valute disponibili nell'area [!UICONTROL Exchange Rates] del sistema.</p> 
       </div> <p><span>Per informazioni sulla configurazione della [!UICONTROL Base Currency] in [!DNL Workfront], vedi</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta tassi di cambio</a>.</p> <p><span>Per informazioni sulla modifica della valuta di un progetto, consulta</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modificare la valuta del progetto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sostituisci Costo valuta/Ora]</span> </td> 
      <td> 
       <div> 
        <p>Tariffa oraria della mansione che utilizza la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare i costi pianificati ed effettivi delle attività e dei problemi associati alla mansione. </p> 
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. In questo modo viene aggiornato anche il tasso Costo/Ora per questa mansione quando si utilizza la [!UICONTROL Base Currency].</span> </p> 
        <p>Per informazioni su come [!DNL Workfront] calcola il costo, vedere <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> 
       </div> <p>Suggerimento: quando si aggiorna una mansione esistente a cui è già associata una tariffa Costo/Ora, [!DNL Workfront] calcola il tasso di [!UICONTROL Override Currency] in base al tasso di conversione nel sistema. Se si aggiorna [!UICONTROL Sostituisci valuta costo/ora], anche il costo/ora della mansione viene aggiornato automaticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Sostituisci valuta fatturazione/ora]</span> </td> 
      <td> 
       <div> 
        <p>Tariffa oraria di fatturazione della mansione che utilizza la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare le entrate pianificate ed effettive delle attività e dei problemi associati al ruolo. </p> 
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. Questo aggiorna anche la tariffa di fatturazione/ora per questa mansione quando si utilizza la [!UICONTROL Base Currency].</span> </p> 
        <p>Per informazioni su come [!DNL Workfront] calcola i ricavi, vedere <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>.</p> 
       </div> <p>Suggerimento: quando si aggiorna una mansione esistente a cui è già associata una tariffa di fatturazione/ora, [!DNL Workfront] calcola il tasso della valuta di sostituzione in base al tasso di conversione nel sistema. Se aggiorni la valuta di sostituzione fatturazione/ora, anche la fatturazione/ora del ruolo viene aggiornata automaticamente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >I ruoli sono parte integrante della gestione delle risorse. Per utilizzare gli strumenti di pianificazione delle risorse, le mansioni devono avere un costo e una tariffa di fatturazione associati. Per informazioni, consulta [Introduzione alla gestione delle risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Clic **[!UICONTROL Crea Ruolo]**. Il ruolo è ora disponibile per essere assegnato ad attività, problemi, approvazioni oppure puoi condividere modelli di layout o altri oggetti con esso. Per informazioni su tutti gli utilizzi delle mansioni in [!DNL Workfront], vedi [Panoramica sui ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Per informazioni sull&#39;eliminazione di una mansione, vedere [Elimina mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
