---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utilizzare Diagnostica per attivare i processi automatizzati
description: È possibile utilizzare Diagnostica per attivare manualmente i processi automatizzati, ad esempio script basati su tempo, ricalcolamenti o notifiche e-mail.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 6%

---

# Utilizzare Diagnostica per attivare i processi automatizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

È possibile utilizzare Diagnostica per attivare manualmente i processi automatizzati, ad esempio script basati su tempo, ricalcolamenti o notifiche e-mail.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze legacy</a> </td> 
   <td> <p>Piano </p>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Utilizzare la diagnostica per attivare i processi automatizzati

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandi **Sistema**, quindi fai clic su **Diagnostica**.
1. Seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Invia Avviso di Ritardo</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatiche per attività e problemi in ritardo. </p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, consulta <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Imposta promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia Avviso di Scadenze</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatiche per le attività e i problemi che si avvicinano alle rispettive date di scadenza.</p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, consulta <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Imposta promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia Avvisi di Promemoria</td> 
      <td> <p>Invia manualmente notifiche di promemoria. </p> <p>Per ulteriori informazioni sulla configurazione delle notifiche dei promemoria, vedi <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Impostare le notifiche dei promemoria</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Controlla Tutti POP Account</td> 
      <td> <p>Verifica la presenza di nuove e-mail inviate agli account POP collegati a Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricalcolare i Timeline</td> 
      <td> <p>Ricalcola la timeline per tutti i progetti in Workfront con stato Corrente. </p> <p>Per ulteriori informazioni sul calcolo automatico o manuale della timeline dei progetti, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le timeline dei progetti</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Repristina i Report Predefiniti</td> 
      <td>Ripristina i rapporti predefiniti originariamente forniti con Workfront, in modo che siano visibili nella <strong>Rapporti</strong> per tutti gli utenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genera Timesheets</td> 
      <td>Genera fogli presenze per gli utenti in base ai profili ricorrenti della scheda attività. Questa opzione deve essere eseguita solo se il profilo della scheda attività è stato modificato in modo significativo dopo essere stato assegnato agli utenti e solo dopo l'eliminazione di tutte le schede attività correnti e future.</td> 
     </tr> 
    </tbody> 
   </table>
