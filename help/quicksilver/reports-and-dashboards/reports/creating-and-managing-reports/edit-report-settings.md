---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Modificare le impostazioni dei rapporti
description: È possibile modificare le impostazioni di un rapporto per definirne la visualizzazione per altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 9%

---

# Modificare le impostazioni dei rapporti

È possibile modificare le impostazioni di un rapporto per definirne la visualizzazione per altri utenti o il tipo di informazioni che gli utenti possono richiedere prima di eseguire il rapporto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Procedura dettagliata

1. Inizia a creare un rapporto andando al **Menu principale** > **Rapporti**, quindi seleziona l’oggetto del rapporto.

   Oppure

   Apri un rapporto esistente, quindi fai clic su **Azioni dei rapporti** > **Modifica**.

1. Fai clic su **Impostazioni dei rapporti** nell’angolo in alto a destra del generatore di report.
1. Configura le seguenti impostazioni del rapporto:

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
      <td>Specificare un'istruzione che descriva lo scopo e gli utilizzi del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esegui il report con i diritti di accesso di</td> 
      <td>Selezionare l'utente di cui si desidera utilizzare i diritti di accesso durante la visualizzazione per altri utenti durante la visualizzazione del rapporto. Per ulteriori informazioni sull’esecuzione di un rapporto con i diritti di accesso di un altro utente, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando il report viene caricato, mostra</td> 
      <td>Seleziona la scheda predefinita visualizzata per tutti gli utenti al caricamento del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando il rapporto viene caricato su un dashboard, mostra gli elementi ...</td> 
      <td>Specifica il numero di elementi visualizzati per tutti gli utenti quando il rapporto viene caricato su un dashboard. Il valore predefinito è 15 elementi e il numero massimo è 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza la vista Griglia risorse nella scheda Dettagli</td> 
      <td> <p>Selezionare questa opzione per visualizzare la griglia delle risorse nella scheda Dettagli del rapporto.</p> <p>Nota: Quando si applica la visualizzazione Griglia risorse a un rapporto utente, il rapporto mostra solo i progetti che si trovano nello stato Corrente. Se si desidera visualizzare i progetti in qualsiasi altro stato, è possibile utilizzare la scheda Utilizzo utente nell'area Persone della barra di navigazione globale e applicare la visualizzazione Griglia risorse. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra una visualizzazione speciale nella scheda Dettagli</td> 
      <td>(Solo per report progetto) Specifica il tipo di visualizzazione che gli utenti vedranno quando accederanno a queste informazioni nella scheda Dettagli. Ad esempio, è possibile selezionare una visualizzazione Milestone o Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra il report in un grafico di Gantt per impostazione predefinita</td> 
      <td>(Solo rapporto progetto e rapporto attività) Selezionare questa opzione per attivare automaticamente la visualizzazione Gantt quando gli utenti visualizzano la scheda Dettagli in questo rapporto.<br>Per ulteriori informazioni sulla visualizzazione del diagramma di Gantt nei rapporti sui progetti e nei rapporti sulle attività, vedere la sezione "Visualizza informazioni sulle attività nell'elenco dei progetti Diagramma di Gantt" nell'articolo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visualizzazione delle informazioni nel diagramma di Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica della visualizzazione nel report</td> 
      <td>Selezionare questa opzione per consentire agli utenti di modificare la visualizzazione durante l'esecuzione del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica del gruppo nel report</td> 
      <td>Selezionare questa opzione per consentire agli utenti di modificare il Gruppo durante l’esecuzione del rapporto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la modifica del filtro nel report</td> 
      <td>Seleziona questa opzione per consentire agli utenti di modificare il Filtro durante l’esecuzione del rapporto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Richieste di rapporto** per impostare eventuali prompt per il rapporto.\
   Per ulteriori informazioni sull’aggiunta di prompt a un rapporto, consulta l’articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Fai clic su **Fatto,** quindi fai clic su **Salva e chiudi**.

## Informazioni aggiuntive

Vedi anche:

* [Programma di creazione di report di base per la nuova esperienza Workfront](https://one.workfront.com/s/basic-report-creation-program)
* [Guida introduttiva ai rapporti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Utilizzare i report incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
