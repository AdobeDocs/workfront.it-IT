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
TQID: https://experienceleague.adobe.com/MPnQTGB88j8sZHuA6p6SVWI-1tDn7wi77GMsq0vX05c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 329
ht-degree: 20%

---

# Utilizzare la diagnostica per attivare processi automatizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

È possibile utilizzare Diagnostica per attivare manualmente processi automatizzati, ad esempio script basati sul tempo, ricalcoli o notifiche e-mail.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizzare la diagnostica per attivare i processi automatizzati

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic sull&#39;icona **Setup** ![Gear settings](assets/gear-icon-settings.png).

1. Espandere **Sistema**, quindi fare clic su **Diagnostica**.
1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Invia avvisi di ritardo</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatici per le attività e i problemi scaduti. </p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, vedere <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurazione dei promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia avvisi di scadenze</td> 
      <td> <p>Invia manualmente le notifiche di promemoria automatici per le attività e i problemi che si stanno avvicinando alle rispettive date di scadenza.</p> <p>Per ulteriori informazioni sulla configurazione dei promemoria automatici, vedere <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurazione dei promemoria automatici</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia avvisi di promemoria</td> 
      <td> <p>Invia manualmente notifiche promemoria. </p> <p>Per ulteriori informazioni sulla configurazione delle notifiche dei promemoria, vedere <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurare le notifiche dei promemoria</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Controlla tutti gli account POP</td> 
      <td>Cerca nuove e-mail inviate ad account POP collegati a Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calcola nuovamente le timeline</td> 
      <td> <p>Ricalcola la sequenza temporale per tutti i progetti in Workfront con stato Corrente. </p> <p>Per ulteriori informazioni sul calcolo automatico o manuale della sequenza temporale dei progetti, un progetto alla volta, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le sequenze temporali del progetto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ripristina i report dei clienti predefiniti</td> 
      <td>Ripristina i report predefiniti originariamente consegnati con Workfront, in modo che siano visibili a tutti gli utenti nella sezione <strong>Report</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genera schede orario</td> 
      <td>Genera schede orario per gli utenti in base ai loro profili di schede orario ricorrenti. Questa opzione deve essere eseguita solo se il profilo della scheda orario è stato modificato in modo significativo dopo che è stato assegnato agli utenti e solo dopo che tutte le schede orario correnti e future sono state eliminate.</td> 
     </tr> 
    </tbody> 
   </table>
