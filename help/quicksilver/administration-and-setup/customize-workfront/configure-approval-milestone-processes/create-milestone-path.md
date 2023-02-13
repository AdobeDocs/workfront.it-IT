---
title: Creare un percorso cardine
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In qualità di amministratore di Adobe Workfront, puoi creare percorsi cardine che possono essere applicati a qualsiasi progetto nel sistema. Le modifiche apportate ai percorsi cardine in quest’area influiscono sull’intero sistema Workfront.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---

# Creare un percorso cardine

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Adobe Workfront, puoi creare percorsi cardine che possono essere applicati a qualsiasi progetto nel sistema. Le modifiche apportate ai percorsi cardine in quest’area influiscono sull’intero sistema Workfront.

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Milestone e percorsi cardine

È possibile associare le attività chiave di un progetto a tappe predefinite. Questa funzione può fornire ai manager e agli altri soggetti interessati una panoramica di alto livello dei progressi di un progetto.

La somma di tutte le tappe predefinite è denominata percorso cardine.

Il primo passo per la creazione di un percorso cardine consiste nell&#39;identificare quali sono i passaggi cardine e stabilire le fasi cardine. Poiché è possibile associare un percorso cardine a più progetti, i passaggi cardine devono essere fasi generali o fasi di qualsiasi progetto.

Per ulteriori informazioni su come associare un percorso cardine a un progetto e un&#39;attività cardine a un&#39;attività, consulta [Associa milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Creare un percorso cardine

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Processi** > **Percorsi Milestone**.
1. Fai clic su **Nuovo percorso Milestone.**
1. Specifica le seguenti informazioni nella **Informazioni di base** area:

   <table style="table-layout:auto">
    <tr>
      <td>Nome percorso milestone</td>
       <td>Immettere un nome per il percorso cardine.</td>
    </tr>
    <tr>
      <td>Descrizione</td>
      <td>Immettere una descrizione per definire il percorso della cardine.</td>
    </tr>
    <tr>
       <td>È attivo</td>
      <td>Selezionare questa casella di controllo se si desidera che il percorso cardine sia attivo. Altri utenti possono trovare questo percorso e allegarlo ai progetti durante la creazione o la modifica di progetti. Non è possibile allegare ai progetti percorsi di cardine inattivi. Questa opzione è attivata per impostazione predefinita.</td>
    </tr>
    <tr>
      <td>Gruppi</td>
      <td>Seleziona i gruppi elencati per consentire agli utenti di questi gruppi di visualizzare e applicare questo percorso cardine ai loro progetti. Per impostazione predefinita, il gruppo home dell’utente che accede al percorso della cardine viene selezionato.</td>
    </tr>
   </table>

1. Specifica le seguenti informazioni nella **Milestone** area:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Digitare nomi descrittivi per ogni cardine.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione per la fase cardine.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clr icn</td> 
      <td> <p>Scegliere un colore da associare alla cardine. </p> <p>Se non si sceglie un colore, il sistema sceglie l'ultimo colore utilizzato in un percorso cardine. È consigliabile scegliere un colore univoco per ogni cardine. Il colore viene utilizzato a scopo visivo e di reporting.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi Milestone** e continua ad aggiungere le tappe necessarie fino al completamento del percorso.
1. Fai clic su **Crea percorso Milestone** per salvare le modifiche.

   Il percorso cardine è pronto per essere associato a un progetto.

   Per ulteriori informazioni su come associare percorsi cardine a progetti e fasi cardine alle attività, vedere [Associa milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
