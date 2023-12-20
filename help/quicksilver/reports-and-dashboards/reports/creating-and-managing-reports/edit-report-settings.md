---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Modificare le impostazioni dei rapporti
description: È possibile modificare le impostazioni di un report per definirne la modalità di visualizzazione per gli altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il report.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 6%

---

# Modificare le impostazioni dei rapporti

È possibile modificare le impostazioni di un report per definirne la modalità di visualizzazione per gli altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il report.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Passaggi pratici

1. Per iniziare a creare un rapporto, vai al **Menu principale** > **Rapporti**, quindi seleziona l’oggetto del rapporto.

   Oppure

   Apri un rapporto esistente, quindi fai clic su **Azioni report** > **Modifica**.

1. Clic **Impostazioni dei rapporti** nell’angolo superiore destro del report builder.
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
      <td>Selezionare l'utente di cui si desidera utilizzare i diritti di accesso per la visualizzazione del report per altri utenti. Per ulteriori informazioni sull’esecuzione di un rapporto con i diritti di accesso di un altro utente, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Eseguire e consegnare un report con i diritti di accesso di un altro utente</a>.</td> 
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
      <td>(Solo report di progetto e report di attività) Selezionare questa opzione per attivare automaticamente la visualizzazione Gantt quando gli utenti visualizzano la scheda Dettagli in questo report.<br>Per ulteriori informazioni sulla visualizzazione del diagramma di Gantt nei report del progetto e nei report delle attività, vedere la sezione "Visualizzare le informazioni sulle attività nell'elenco dei progetti Diagramma di Gantt" nell'articolo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visualizzare le informazioni nel diagramma di Gantt </a>.</td> 
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

1. Clic **Prompt dei report** per impostare eventuali richieste per il report.\
   Per ulteriori informazioni sull&#39;aggiunta di prompt a un report, vedere l&#39;articolo [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Clic **Fine,** quindi fai clic su **Salva e chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Introduzione ai rapporti](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Utilizzare i rapporti incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
