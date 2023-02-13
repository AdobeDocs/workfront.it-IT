---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Creare e gestire ruoli di lavoro
description: Come [!DNL Adobe Workfront] amministratore o utente con accesso amministrativo ai ruoli, è possibile creare ruoli di lavoro che possono essere assegnati agli utenti ed eliminare ruoli di lavoro predefiniti non rilevanti per la propria organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Creare e gestire ruoli di lavoro

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Come [!DNL Adobe Workfront] amministratore o utente con accesso amministrativo ai ruoli, è possibile creare ruoli di lavoro che possono essere assegnati agli utenti ed eliminare ruoli di lavoro predefiniti non rilevanti per la propria organizzazione. Per informazioni sull&#39;accesso amministrativo in [!DNL Workfront], vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai ruoli di lavoro</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare un ruolo di lavoro

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su &#x200B; **[!UICONTROL Ruoli processo].**
1. Fai clic su **[!UICONTROL Nuovo ruolo del lavoro].**
1. Configura quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicare un nome per il ruolo del processo. Questo è il nome che viene visualizzato ovunque [!DNL Workfront] dove viene visualizzato il campo [!UICONTROL Job Role] (Ruolo lavoro). </p> <p>Suggerimento: Il nome di un ruolo di lavoro può contenere fino a 255 caratteri. Tuttavia, i nomi più lunghi potrebbero essere troncati in alcune aree di [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL È Attivo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Seleziona <b>[!UICONTROL Sì]</b> se desideri che il ruolo sia attivo e disponibile ovunque in [!DNL Workfront] da associare a utenti, elementi di lavoro, ecc. </p> </li> 
        <li> <p>Seleziona <b>[!UICONTROL No]</b>, se desideri che il ruolo sia disattivato e non disponibile per l’assegnazione a utenti, elementi di lavoro, ecc. </p> </li> 
       </ul> <p><span>Per informazioni sulla disattivazione dei ruoli di lavoro, consulta</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Disattivazione dei ruoli di lavoro</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione del ruolo che indichi l’elemento univoco al riguardo. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Valuta di base]</span> </td> 
      <td> <p><span>Si tratta della [!UICONTROL Base Currency], impostata nell'area [!UICONTROL Setup] dal proprio amministratore Workfront. Per informazioni, consulta</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a> .</p> <p>Suggerimento: <span>Non è possibile modificare la [!UICONTROL Base Currency] a livello di ruolo del lavoro. Questo campo è oscurato e funge da promemoria della valuta di base del sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost/ Hr.]</td> 
      <td>Percentuale del costo per ora del ruolo di lavoro. Questo valore consente di calcolare i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo e, in ultima analisi, i costi pianificati ed effettivi dei progetti. <span>Immettere il tasso utilizzando la [!UICONTROL Base Currency].</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Bill/ Hr.] </td> 
      <td>Percentuale di fatturazione oraria del ruolo di lavoro. Questo valore consente di calcolare le entrate previste ed effettive delle attività e dei problemi associati al ruolo e, in ultima analisi, le entrate previste ed effettive dei progetti. Immettere il tasso utilizzando la [!UICONTROL Base Currency]. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td> 
       <div> 
        <p>Selezionare una valuta associata a questo ruolo di lavoro. Questa è la valuta che [!DNL Workfront] utilizza per calcolare i costi e i ricavi associati a questo ruolo di lavoro. </p> 
        <p><span>È diverso dalla [!UICONTROL Base Currency] impostata dal [!DNL Workfront] amministratore nell’area [!UICONTROL Setup] e può essere diverso dalla valuta associata a un progetto.</span> </p> 
        <p>Suggerimento: In questo campo sono disponibili solo le valute disponibili nell'area [!UICONTROL Exchange Rates] del sistema.</p> 
       </div> <p><span>Per informazioni sulla configurazione della [!UICONTROL Base Currency] in [!DNL Workfront], vedi</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a>.</p> <p><span>Per informazioni sulla modifica della valuta di un progetto, consulta</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modificare la valuta del progetto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Ignora costo valuta/ora]</span> </td> 
      <td> 
       <div> 
        <p>È il tasso di costo per ora del ruolo di lavoro utilizzando la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare i costi pianificati ed effettivi delle attività e dei problemi associati al ruolo del lavoro. </p> 
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. Questo aggiorna anche il tasso costo/ora per questo ruolo di lavoro quando si utilizza la [!UICONTROL Base Currency].</span> </p> 
        <p>Per informazioni su come [!DNL Workfront] calcola costo, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> 
       </div> <p>Suggerimento: Quando si aggiorna un ruolo di lavoro esistente a cui è già associato un tasso di costo/ora, [!DNL Workfront] calcola il tasso di sostituzione in base al tasso di conversione nel sistema. Se si aggiorna il [!UICONTROL Override Currency Cost/ Hour], anche il costo/ora del ruolo di lavoro viene aggiornato automaticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Ignora fatturazione/ora valuta</span> </td> 
      <td> 
       <div> 
        <p>Tasso di fatturazione per ora del ruolo di lavoro utilizzando la [!UICONTROL Override Currency] selezionata. [!DNL Workfront] utilizza questo valore per calcolare i ricavi pianificati ed effettivi delle attività e dei problemi associati al ruolo del lavoro. </p> 
        <p><span>Immettere il tasso nella [!UICONTROL Override Currency] specificata sopra. Questo aggiorna anche il tasso di fatturazione/ora per questo ruolo di lavoro quando si utilizza la [!UICONTROL Base Currency].</span> </p> 
        <p>Per informazioni su come [!DNL Workfront] calcola i ricavi, vedi <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a>.</p> 
       </div> <p>Suggerimento: Quando si aggiorna un ruolo di lavoro esistente a cui è già associato un tasso di fatturazione/ora, [!DNL Workfront] calcola il tasso di sostituzione della valuta in base al tasso di conversione nel sistema. Se si aggiorna la fatturazione/ora della divisa di sostituzione, anche la fatturazione/ora del ruolo di lavoro viene aggiornata automaticamente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >I ruoli di lavoro sono parte integrante della gestione delle risorse. Per utilizzare gli strumenti di pianificazione delle risorse, i ruoli di lavoro devono essere associati a un costo e a un tasso di fatturazione. Per informazioni, consulta [Guida introduttiva a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Fai clic su **[!UICONTROL Crea ruolo lavoro]**. È ora possibile assegnare il ruolo di lavoro a attività, problemi, approvazioni oppure condividere modelli di layout o altri oggetti con esso. Per informazioni su tutti gli usi dei ruoli di lavoro in [!DNL Workfront], vedi [Panoramica sul ruolo del lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Per informazioni sull&#39;eliminazione di un ruolo di lavoro, vedere [Eliminare i ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
