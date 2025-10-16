---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Modificare le impostazioni dei rapporti
description: È possibile modificare le impostazioni di un report per definirne la modalità di visualizzazione per gli altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il report.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 7%

---

# Modificare le impostazioni dei rapporti

<!-- Audited: 11/2024 -->

È possibile modificare le impostazioni di un report per definirne la modalità di visualizzazione per gli altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il report.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
 <td> <p>Gestire le autorizzazioni per un rapporto</p></td>  
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Passaggi pratici

1. Inizia a creare un report accedendo al **menu principale** > **Report**, quindi seleziona l&#39;oggetto del report.

   Oppure

   Apri un report esistente, quindi fai clic su **Azioni report** > **Modifica**.

1. Fai clic su **Impostazioni report** nell&#39;angolo superiore destro del Report Builder.
1. Configura le seguenti impostazioni per i rapporti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Titolo report</td> 
      <td>Specifica un titolo per il rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Specifica un’istruzione che descriva lo scopo e gli utilizzi del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esegui questo report con i diritti di accesso di</td> 
      <td>Selezionare l'utente di cui si desidera utilizzare i diritti di accesso per la visualizzazione del report per altri utenti. Per ulteriori informazioni sull'esecuzione di un report con i diritti di accesso di un altro utente, vedere l'articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Eseguire e distribuire un report con i diritti di accesso di un altro utente</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando il report viene caricato, mostra</td> 
      <td>Seleziona la scheda predefinita che viene visualizzata per tutti gli utenti al caricamento del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando il rapporto viene caricato su un dashboard, mostra ... elementi</td> 
      <td>Specifica il numero di elementi visualizzati per tutti gli utenti quando il rapporto viene caricato su un dashboard. Il valore predefinito è 15 elementi e il numero massimo è 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra la visualizzazione Griglia risorse nella scheda Dettagli</td> 
      <td> <p>(Solo report utente) Selezionare questa opzione per visualizzare la griglia delle risorse nella scheda Dettagli del report.</p> <p>Nota: quando si applica la visualizzazione Tabella risorse a un report utente, il report mostra solo i progetti che si trovano nello stato Corrente. Se si desidera visualizzare i progetti in qualsiasi altro stato, è possibile utilizzare la scheda Utilizzo utente nell'area Persone della barra di navigazione globale e applicare la visualizzazione griglia risorse. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra una visualizzazione speciale nella scheda Dettagli</td> 
      <td>(Solo report di progetto) Specifica il tipo di visualizzazione che gli utenti visualizzeranno quando accedono a queste informazioni nella scheda Dettagli. Ad esempio, puoi selezionare una vista Milestone o Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra il report in un grafico di Gantt per impostazione predefinita</td> 
      <td>(Solo report di progetto e report di attività) Selezionare questa opzione per attivare automaticamente la visualizzazione Gantt quando gli utenti visualizzano la scheda Dettagli in questo report.<br>Per ulteriori informazioni sulla visualizzazione del diagramma di Gantt nei report di progetto e nei report di attività, vedere la sezione "Visualizzare le informazioni sulle attività nell'elenco dei progetti Diagramma di Gantt" nell'articolo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visualizzare le informazioni nel Diagramma di Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica della visualizzazione nel report</td> 
      <td>Selezionare questa opzione per consentire agli utenti di modificare la visualizzazione durante l'esecuzione del report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica del gruppo nel report</td> 
      <td>Selezionare questa opzione per consentire agli utenti di modificare il gruppo durante l'esecuzione del report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica del filtro nel report</td> 
      <td>Selezionare questa opzione per consentire agli utenti di modificare il filtro durante l'esecuzione del report.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Prompt dei rapporti** per impostare eventuali prompt per il rapporto.\
   Per ulteriori informazioni sull&#39;aggiunta di prompt a un report, vedere l&#39;articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Fai clic su **Fine,** quindi su **Salva + Chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Introduzione ai report](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Utilizzare i report incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
