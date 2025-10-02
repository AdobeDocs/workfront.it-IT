---
title: Creare un percorso milestone
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In qualità di amministratore di Adobe Workfront, puoi creare percorsi milestone che possono quindi essere applicati a qualsiasi progetto del sistema. Le modifiche apportate ai percorsi milestone in quest'area hanno effetto sull'intero sistema Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 3%

---

# Creare un percorso milestone

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<div class="preview">

Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Le stesse funzioni saranno disponibili anche nell’ambiente di produzione per tutti i clienti a partire da una settimana dalla versione di anteprima.

Per ulteriori informazioni, vedere [Modernizzazione interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

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
   <td><p>Standard</p>
   <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Milestone e percorsi milestone

È possibile associare le attività chiave di un progetto alle attività cardine predefinite. Questa funzione può fornire ai manager e ad altre parti interessate una panoramica di alto livello sullo stato di avanzamento di un progetto.

La somma di tutte le milestone predefinite è chiamata percorso milestone.

Il primo passo nella creazione di un percorso milestone consiste nell&#39;identificare le fasi cardine e nel definirne le tappe. Poiché è possibile associare un percorso milestone a più progetti, i passaggi milestone devono essere fasi generali o fasi di qualsiasi progetto.

Per ulteriori informazioni su come associare un percorso milestone a un progetto e un milestone a un&#39;attività, vedere [Associare i milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Creare un percorso milestone

{{step-1-to-setup}}

1. Fai clic su **Processi** > **Percorsi milestone**.
1. Fai clic su **Nuovo percorso milestone.**

   <div class="preview">

   Viene visualizzata la casella Nuovo percorso milestone (New Milestone Path).

   ![Nuova casella percorso milestone](assets/new-milestone-path-box.png)

   </div>

1. Fai clic su **Informazioni di base** nel pannello a sinistra.

   Aggiorna le seguenti informazioni:

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

1. Fai clic su **Milestones** nel pannello a sinistra.

1. Nell&#39;ambiente di produzione, fare clic su **Aggiungi milestone** per aggiungere le milestone al percorso.
   <span class="preview">Nell&#39;ambiente di anteprima, fare clic su **Nuova riga** per aggiungere le milestone al percorso.</span>
1. Aggiorna le seguenti informazioni:

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

1. (Facoltativo) Trascina e rilascia ciascuna milestone per riordinarle.
1. Fai clic su **Crea percorso milestone** per salvare le modifiche.

   Il percorso milestone è pronto per essere associato a un progetto.

   Per ulteriori informazioni su come associare percorsi milestone a progetti e milestone ad attività, vedere [Associare milestone ad attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

1. (Facoltativo) Dall&#39;elenco Percorsi milestone, selezionare una milestone, quindi fare clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png) per aprire il percorso milestone e modificarne le informazioni.
1. (Facoltativo) Fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export-icon.png), quindi seleziona uno dei seguenti formati per esportare l&#39;elenco dei percorsi delle milestone in un file:

   * PDF
   * Excel
   * Excel (xlsx)
   * Delimitato in tabella

1. (Facoltativo) Seleziona una o più milestone nell&#39;elenco, quindi fai clic sull&#39;icona **Elimina** ![Elimina icona](assets/delete-icon.png) per eliminarla.
1. Fai clic su **Sì, elimina**.

   La milestone viene eliminata e non può essere recuperata. Il percorso milestone viene rimosso da qualsiasi progetto precedentemente associato a esso e tutte le milestone vengono rimosse dalle attività associate.

   Non è possibile recuperare le milestone eliminate.


## Visualizzare i dettagli del percorso milestone in un rapporto del progetto

Puoi visualizzare i dettagli di un percorso milestone in un rapporto di progetto.

È necessario associare un percorso milestone a un progetto prima di visualizzarne i dettagli in un report di progetto.

Per informazioni sull&#39;associazione dei percorsi milestone ai progetti, vedere [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

{{step1-to-reports}}

1. Fai clic su **Nuovo report**, quindi fai clic su **Progetto**.
1. Fai clic su **Aggiungi colonna**.
1. Nell&#39;area **Mostra in questa colonna**, inizia a digitare **Percorso milestone**, quindi fai clic su **Nome percorso milestone**.
1. (Facoltativo) Fai clic su **Filtri** e aggiungi il seguente filtro al rapporto: **L&#39;ID percorso milestone del progetto non è vuoto**.

   Il filtro assicura che nel rapporto vengano visualizzati solo i progetti associati a un percorso milestone.

1. Fai clic su **Salva e Chiudi**.
1. Aggiungi un nome per il report, quindi fai clic su **Applica**.

   Viene visualizzato il report del progetto. I percorsi milestone associati a ciascun progetto vengono visualizzati nell’ultima colonna del rapporto.
1. Fare clic sul nome di un percorso milestone nell&#39;ultima colonna del report.

   Vengono visualizzati i dettagli del percorso milestone.

   ![Dettagli del percorso milestone dal report del progetto](assets/milestone-details-from-project-report.png)

   Nella pagina dei dettagli del percorso della milestone vengono visualizzate le seguenti informazioni:

   * Nome, ID e descrizione del percorso di Milestone
   * Gruppi di percorsi milestone
   * Nomi milestone, descrizioni, colori e icone colore

1. (Facoltativo) Fai clic su **Indietro** per tornare al report del progetto.



