---
title: Creare un percorso milestone
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In qualità di amministratore di Adobe Workfront, puoi creare percorsi milestone che possono quindi essere applicati a qualsiasi progetto del sistema. Le modifiche apportate ai percorsi milestone in quest'area hanno effetto sull'intero sistema Workfront.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---

# Creare un percorso milestone

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Adobe Workfront, puoi creare percorsi milestone che possono quindi essere applicati a qualsiasi progetto del sistema. Le modifiche apportate ai percorsi milestone in quest&#39;area hanno effetto sull&#39;intero sistema Workfront.

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

## Milestone e percorsi milestone

È possibile associare le attività chiave di un progetto alle attività cardine predefinite. Questa funzione può fornire ai manager e ad altre parti interessate una panoramica di alto livello sullo stato di avanzamento di un progetto.

La somma di tutte le milestone predefinite è chiamata percorso milestone.

Il primo passo nella creazione di un percorso milestone consiste nell&#39;identificare le fasi cardine e nel definirne le tappe. Poiché è possibile associare un percorso milestone a più progetti, i passaggi milestone devono essere fasi generali o fasi di qualsiasi progetto.

Per ulteriori informazioni su come associare un percorso milestone a un progetto e un milestone a un&#39;attività, vedere [Associare i milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Creare un percorso milestone

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Processi** > **Percorsi milestone**.
1. Fai clic su **Nuovo percorso milestone.**
1. Specificare le informazioni seguenti nell&#39;area **Informazioni di base**:

   <table style="table-layout:auto">
    <tr>
      <td>Nome percorso milestone</td>
       <td>Immettere un nome per il percorso milestone.</td>
    </tr>
    <tr>
      <td>Descrizione</td>
      <td>Immettere una descrizione per definire il percorso della milestone.</td>
    </tr>
    <tr>
       <td>È attivo</td>
      <td>Selezionare questa casella di controllo se si desidera che il percorso milestone sia attivo. Altri utenti possono trovare questo percorso e allegarlo ai progetti durante la creazione o la modifica dei progetti. I percorsi delle milestone inattivi non possono essere associati ai progetti. Questa opzione è attivata per impostazione predefinita.</td>
    </tr>
    <tr>
      <td>Gruppi</td>
      <td>Seleziona i gruppi elencati per consentire agli utenti di questi gruppi di visualizzare e applicare questo percorso milestone ai loro progetti. Per impostazione predefinita, viene selezionato il gruppo predefinito dell'utente che immette il percorso milestone.</td>
    </tr>
   </table>

1. Specifica le seguenti informazioni nell&#39;area **Milestones**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Digita nomi descrittivi per ogni milestone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione per la fase cardine.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Colore</td> 
      <td> <p>Scegliere un colore da associare alla milestone. </p> <p>Se non scegliete un colore, il sistema sceglie l'ultimo colore utilizzato in un percorso milestone. È consigliabile scegliere un colore univoco per ogni fase cardine. Il colore viene utilizzato a scopo visivo e di reporting.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi milestone** e continua ad aggiungere le milestone necessarie fino al completamento del percorso.
1. Fai clic su **Crea percorso milestone** per salvare le modifiche.

   Il percorso milestone è pronto per essere associato a un progetto.

   Per ulteriori informazioni su come associare percorsi milestone a progetti e milestone ad attività, vedere [Associare milestone ad attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
