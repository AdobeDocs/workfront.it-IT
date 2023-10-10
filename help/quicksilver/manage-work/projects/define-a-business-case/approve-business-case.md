---
navigation-topic: business-case-and-scorecards
title: Approvare un caso di business
description: Dopo aver completato e sottomesso il Business Case per una richiesta di progetto, il Business Case deve essere approvato. Questo dipende dal flusso di lavoro dell’organizzazione. Un progetto può iniziare senza che sia necessario approvare il Business Case, ma l’amministratore di Adobe Workfront e i proprietari del progetto potrebbero non considerarlo ideale.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Approvare un caso di business

Dopo aver completato e sottomesso il Business Case per una richiesta di progetto, il Business Case deve essere approvato. Questo dipende dal flusso di lavoro dell’organizzazione. Un progetto può iniziare senza che sia necessario approvare il Business Case, ma l’amministratore di Adobe Workfront e i proprietari del progetto potrebbero non considerarlo ideale. 

Per ulteriori informazioni sul completamento e l&#39;invio di un Business Case, vedere l&#39;articolo [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Panoramica sull&#39;approvazione del Business Case

Quando si approva un caso di business di un progetto, considera quanto segue:

* Per approvare il Business Case relativo a un progetto, è necessario disporre delle autorizzazioni di gestione. 
* Non potrai vedere i progetti che sono in attesa dell&#39;approvazione del Business Case con la tua approvazione nell&#39;area Home.
* Per verificare che i progetti siano in attesa di approvazione, è necessario passare manualmente ai singoli progetti che richiedono l&#39;approvazione del Business Case. Non esiste un meccanismo di notifica Workfront che avvisa gli utenti che devono approvare il Business Case di un progetto.
* È possibile trovare i progetti in attesa dell&#39;approvazione del Business Case creando un report di progetto o accedendo al portfolio a cui sono associati. 

  Per ulteriori informazioni sui Portfoli, consulta l’articolo [Panoramica del Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Approvare il Business Case creando un report di progetto

È possibile generare un report per i progetti per vedere quali progetti richiedono l&#39;approvazione del relativo Business Case. 

Per creare un report per i progetti in attesa di approvazione dei relativi casi aziendali:

1. Crea un rapporto per i progetti.

   Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleziona la **Visualizza** del rapporto, quindi fai clic su **Aggiungi colonna**.

1. Inizia a digitare &quot;Status&quot; nel **Mostra in questa colonna** e selezionare questo campo quando viene visualizzato nell&#39;elenco.

    In questa colonna verrà visualizzato lo stato dei progetti.

1. Seleziona la **Filtri** del rapporto, quindi fai clic su **Aggiungere una regola di filtro**.

1. Inizia a digitare &quot;Status&quot; nel **Mostra solo progetti in cui...** e selezionarlo quando viene visualizzato nell&#39;elenco.
1. Seleziona **Uguale** per il modificatore di filtro.
1. Inizia a digitare &quot;Richiesto&quot; nel campo disponibile. 

   In questo modo, il rapporto include solo i progetti nello stato Richiesto.

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Facoltativo) Fai clic su **Aggiungi un&#39;altra regola filtro**.

   Puoi aggiungere altri filtri per mostrare solo i progetti di cui sei il proprietario del progetto, lo sponsor del progetto o il proprietario del Portfolio.

   Ad esempio, puoi utilizzare le seguenti istruzioni di filtro: 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   per visualizzare i progetti in cui sei designato come sponsor del progetto

   ```
   Project Owner ID Equals $$USER.ID
   ```

   per visualizzare i progetti per i quali si è designati come proprietario del progetto

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   per visualizzare il punto in cui si è designati come manager del Portfolio. 

1. Clic **Salva+Chiudi**.

   Tutti i progetti nel report sono nello stato **Richiesto**.

1. Fare clic sul nome di un progetto nel report per aprirlo.
1. Clic **Business Case** nel pannello a sinistra.
1. Clic **Approva** o **Rifiuta** nell&#39;area Riepilogo caso di business per approvare o rifiutare il caso di business.

   ![](assets/business-case-summary-with-rp-information--1-.png)

   Lo stato del progetto viene modificato in **Approvato** se il Business Case viene approvato.

   Lo stato del progetto viene modificato in **Rifiutato** se il Business Case viene rifiutato.

   >[!NOTE]
   >
   >Non vi sono notifiche che avvisano l’utente che ha inviato l’approvazione del business case se la richiesta di progetto è stata approvata o rifiutata.

## Approvare il Business Case accedendo ai progetti richiesti in un portfolio

Per ulteriori informazioni sulla revisione dei progetti richiesti, consulta l’articolo [Esamina progetti richiesti](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
