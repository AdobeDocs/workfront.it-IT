---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utilizzare la diagnostica per attivare i processi automatizzati
description: È possibile utilizzare Diagnostica per attivare manualmente processi automatizzati, ad esempio script basati sul tempo, ricalcoli o notifiche e-mail.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 6%

---

# Utilizzare la diagnostica per attivare i processi automatizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

È possibile utilizzare Diagnostica per attivare manualmente processi automatizzati, ad esempio script basati sul tempo, ricalcoli o notifiche e-mail.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Piano Adobe Workfront</a> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica licenze</a> </td> 
   <td> <p>Piano </p>Devi essere un amministratore di Workfront. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Utilizzare la diagnostica per attivare i processi automatizzati

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandere **Sistema**, quindi fare clic su **Diagnostica**.
1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Invia Avviso di Ritardo</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatici per le attività e i problemi scaduti. </p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, vedere <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurazione dei promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia Avviso di Scadenze</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatici per le attività e i problemi che si stanno avvicinando alle rispettive date di scadenza.</p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, vedere <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurazione dei promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia Avvisi di Promemoria</td> 
      <td> <p>Invia manualmente notifiche promemoria. </p> <p>Per ulteriori informazioni sulla configurazione delle notifiche dei promemoria, vedere <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurare le notifiche dei promemoria</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Controlla Tutti POP Account</td> 
      <td> <p>Cerca nuove e-mail inviate ad account POP collegati a Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricalcolare i Timeline</td> 
      <td> <p>Ricalcola la sequenza temporale per tutti i progetti in Workfront con stato Corrente. </p> <p>Per ulteriori informazioni sul calcolo automatico o manuale della sequenza temporale dei progetti, un progetto alla volta, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le sequenze temporali del progetto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Repristina i Report Predefiniti</td> 
      <td>Ripristina i report predefiniti originariamente consegnati con Workfront, in modo che siano visibili a tutti gli utenti nella sezione <strong>Report</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genera Timesheets</td> 
      <td>Genera schede orario per gli utenti in base ai loro profili di schede orario ricorrenti. Questa opzione deve essere eseguita solo se il profilo della scheda orario è stato modificato in modo significativo dopo che è stato assegnato agli utenti e solo dopo che tutte le schede orario correnti e future sono state eliminate.</td> 
     </tr> 
    </tbody> 
   </table>
