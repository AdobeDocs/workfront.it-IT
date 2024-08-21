---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utilizzare la diagnostica per attivare processi automatizzati
description: È possibile utilizzare Diagnostica per attivare manualmente processi automatizzati, ad esempio script basati sul tempo, ricalcoli o notifiche e-mail.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 9%

---

# Utilizzare la diagnostica per attivare processi automatizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

È possibile utilizzare Diagnostica per attivare manualmente processi automatizzati, ad esempio script basati sul tempo, ricalcoli o notifiche e-mail.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

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
