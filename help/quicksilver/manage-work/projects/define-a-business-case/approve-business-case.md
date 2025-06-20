---
navigation-topic: business-case-and-scorecards
title: Approvare un caso di business
description: Dopo aver completato e sottomesso il Business Case per una richiesta di progetto, il Business Case deve essere approvato. Questo dipende dal flusso di lavoro dell’organizzazione. Un progetto può iniziare senza che sia necessario approvare il Business Case, ma l’amministratore di Adobe Workfront e i proprietari del progetto potrebbero non considerarlo ideale.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Approvare un caso di business

<!--Audit: 6/2025-->

Dopo aver completato e sottomesso il Business Case per una richiesta di progetto, il Business Case deve essere approvato. Questo dipende dal flusso di lavoro dell’organizzazione. Un progetto può iniziare senza che sia necessario approvare il Business Case, ma l’amministratore di Adobe Workfront e i proprietari del progetto potrebbero non considerarlo ideale.

Per ulteriori informazioni sul completamento e l&#39;invio di un Business Case, vedere l&#39;articolo [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
   <p>Corrente: Prime o versione successiva</p>
   <p>oppure</p>
   <p>Legacy: aziendale o superiore</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
   <p>Corrente: Standard </p> 
   <p>Legacy: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Visualizza o autorizzazioni superiori per un portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica sull&#39;approvazione del Business Case

Quando si approva un caso di business di un progetto, considera quanto segue:

* Per approvare il Business Case relativo a un progetto, è necessario disporre delle autorizzazioni di gestione.
* Non potrai vedere i progetti in attesa dell&#39;approvazione del Business Case nel widget Approvazioni personali della Home.
* Per verificare che i progetti siano in attesa di approvazione, è necessario passare manualmente ai singoli progetti che richiedono l&#39;approvazione del Business Case. Non esiste un meccanismo di notifica Workfront che avvisa gli utenti che devono approvare il Business Case di un progetto.
* È possibile trovare i progetti in attesa dell&#39;approvazione del Business Case creando un report di progetto o accedendo al portfolio a cui sono associati.

  Per ulteriori informazioni sui portafogli, vedere l&#39;articolo [Panoramica di Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Approvare il Business Case creando un report di progetto

È possibile generare un report per i progetti per vedere quali progetti richiedono l&#39;approvazione del relativo Business Case.

Per creare un report per i progetti in attesa di approvazione dei relativi casi aziendali:

1. Crea un rapporto per i progetti.

   Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleziona la scheda **Visualizza** del report, quindi fai clic su **Aggiungi colonna**.

1. Inizia a digitare &quot;Status&quot; nel campo **Mostra in questa colonna** e seleziona questo campo quando viene visualizzato nell&#39;elenco.

   In questa colonna verrà visualizzato lo stato dei progetti.

1. Seleziona la scheda **Filtri** del rapporto, quindi fai clic su **Aggiungi una regola filtro**.

1. Inizia a digitare &quot;Status&quot; in **Mostra solo i progetti in cui il campo ...** e selezionalo quando viene visualizzato nell&#39;elenco.
1. Seleziona **Uguale** per il modificatore di filtro.
1. Inizia a digitare &quot;Richiesto&quot; nel campo disponibile.

   In questo modo, il rapporto include solo i progetti nello stato Richiesto.

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Facoltativo) Fai clic su **Aggiungi un&#39;altra regola filtro**.

   Puoi aggiungere altri filtri per mostrare solo i progetti di cui sei il proprietario del progetto, lo sponsor del progetto o il proprietario di Portfolio.

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

   per visualizzare la posizione in cui si è designati come Portfolio Manager.

1. Fai clic su **Salva+Chiudi**.

   Tutti i progetti nel report sono in stato **Richiesto**.

1. Fare clic sul nome di un progetto nel report per aprirlo.
1. Fai clic su **Business Case** nel pannello a sinistra.
1. Fare clic su **Approva** o **Rifiuta** nell&#39;area Riepilogo caso di business per approvare o rifiutare il caso di business.

   ![Caso di studio](assets/business-case-summary-with-rp-information--1-.png)

   Lo stato del progetto viene modificato in **Approvato** se il Business Case viene approvato.

   Lo stato del progetto viene modificato in **Rifiutato** se il caso aziendale viene rifiutato.

   >[!NOTE]
   >
   >Non vi sono notifiche che avvisano l’utente che ha inviato l’approvazione del business case se la richiesta di progetto è stata approvata o rifiutata.

## Approvare il Business Case accedendo ai progetti richiesti in un portfolio

Per ulteriori informazioni sulla revisione dei progetti richiesti, vedere l&#39;articolo [Revisione dei progetti richiesti](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
