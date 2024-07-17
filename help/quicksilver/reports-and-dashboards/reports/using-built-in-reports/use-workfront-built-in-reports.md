---
product-area: reporting
navigation-topic: using-built-in-reports
title: Utilizzare i rapporti incorporati di Adobe Workfront
description: Adobe Workfront dispone di un ampio elenco di rapporti incorporati pronti all’uso. Gli amministratori di Workfront possono nascondere i rapporti incorporati in modo che gli utenti non possano accedervi.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: f2b6f0fb8a24723fec60c6fc1a99e1b8f9cf39c7
workflow-type: tm+mt
source-wordcount: '2953'
ht-degree: 10%

---

# Utilizzare i rapporti incorporati di Adobe Workfront

<!--Audited: 07/2024-->

Adobe Workfront dispone di un ampio elenco di rapporti incorporati che puoi utilizzare.

Gli amministratori di Workfront possono nascondere i rapporti incorporati in modo che gli utenti non possano accedervi.

Per ulteriori informazioni su come nascondere i report incorporati, vedere [Nascondere i report incorporati](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>  
   <p>Corrente: richiesta o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Accesso di visualizzazione o superiore a report, dashboard, calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni di un report per aggiungere o modificare un filtro in un report</p> <p>Gestire le autorizzazioni per un filtro per modificarlo in un elenco</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Panoramica dei rapporti incorporati {#overview-of-built-in-reports}

Puoi personalizzare un rapporto incorporato e salvarlo come nuovo rapporto. Per ulteriori informazioni sulla personalizzazione dei report incorporati, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

I seguenti rapporti sono forniti con il pacchetto Workfront. I rapporti sono disponibili per tutti gli utenti che dispongono almeno dei diritti di visualizzazione per i rapporti incorporati nel proprio livello di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome report</strong> </th> 
   <th><strong>Descrizione report</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo Reale di Portfolio per Programma</td> 
   <td>Un report di progetti che visualizza il costo pianificato e il costo effettivo dei progetti. Il report è raggruppato per Nome programma, richiesto dal Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo Reale di Portfolio per Progetto</td> 
   <td>Un report di progetti che visualizza il costo pianificato e il costo effettivo dei progetti. Il report è raggruppato per Nome progetto, richiesto dal Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale di Portfolio per Programma</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report è raggruppato per Nome programma, richiesto dal Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale di Portfolio per Progetto</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report è raggruppato per Nome progetto, richiesto dal Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questa mostra il Reddito Reale per Azienda</td> 
   <td>Un report di progetti che visualizza la Retribuzione effettiva e la Società dei progetti. Il report è raggruppato per nome della società e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questa mostra il Reddito Reale per Gruppo</td> 
   <td>Un report di progetti che visualizza la Retribuzione effettiva e il Gruppo dei progetti. Il report è raggruppato per Nome gruppo e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Tutti i Timesheets Aperti</td> 
   <td>Un report di timesheet che visualizza i Timesheet aperti. Il rapporto visualizza i campi seguenti: Intervallo date, Nome proprietario, Ore totali, Straordinario, Nome approvatore e Stato delle schede orario.</td> 
  </tr> 
  <tr> 
   <td>Timesheets da Approvare(Suggeriti)</td> 
   <td>Un report di Timesheet che visualizza i Timesheet inviati o rifiutati con gli approvatori. Il rapporto visualizza i campi seguenti: Intervallo date, Proprietario, Ore totali, Straordinario, Nome approvatore e Stato delle schede orario. Il report viene richiesto da: Data inizio scheda orario, Data fine scheda orario, Nome approvatore scheda orario e Nome utente.</td> 
  </tr> 
  <tr> 
   <td>Progetti a Rischio</td> 
   <td>Un report di progetti che visualizza i progetti correnti e di pianificazione con una condizione A rischio o In difficoltà. Il rapporto visualizza i campi seguenti: Descrizione, Data di completamento pianificata, Data di completamento prevista, Percentuale di completamento, Stato e Priorità dei progetti. Il rapporto è raggruppato per nome Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per azienda</td> 
   <td>Un report di progetti che visualizza la Società e la Fatturazione retribuzione dei progetti. Il report è raggruppato per nome della società e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per gruppo</td> 
   <td>Un report di progetti che visualizza la Fatturazione retribuzione e il Gruppo dei progetti. Il report è raggruppato per Nome gruppo e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per mese</td> 
   <td>Un report di record fatturazione che visualizza il Nome progetto, il Ricavo fatturazione progetto e la Data fatturazione dei record fatturazione. Il rapporto è raggruppato per il mese della data di fatturazione dei record di fatturazione e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Issues Completate per Settimana</td> 
   <td>Un report di problemi che visualizza la Data di completamento effettiva dei problemi. Il rapporto è raggruppato per la settimana della Data di completamento effettiva dei problemi e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Issues Completate per Utente per Settimana</td> 
   <td>Un report di problemi che visualizza la Data di completamento effettiva e le assegnazioni dei problemi. Il rapporto è raggruppato per l’assegnatario principale e per la settimana della data di completamento effettiva dei problemi, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti Attuali</td> 
   <td>Un report di progetti che visualizza tutti i progetti correnti. Il rapporto visualizza i campi seguenti: Descrizione, Data di completamento pianificata, Data di completamento prevista, Percentuale di completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Costo orario per utente per mese</td> 
   <td>Un report di ore matrice che visualizza il numero di ore registrate e il relativo costo effettivo. Il rapporto è raggruppato per nome del proprietario e per il mese della data di immissione delle ore.</td> 
  </tr> 
  <tr> 
   <td>Ore per utente</td> 
   <td>Un report di ore che visualizza il numero di ore registrate. Il rapporto è raggruppato per nome del proprietario e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Ore per utente per settimana</td> 
   <td>Un report di ore matrice che visualizza il numero di ore registrate nelle ultime quattro settimane e la data di immissione delle ore. Il report viene richiesto in base alla Data di immissione delle ore ed è raggruppato per Nome proprietario e per il mese della Data di immissione delle ore.</td> 
  </tr> 
  <tr> 
   <td>Problemi per stato</td> 
   <td>Un report di problemi che visualizza lo Stato dei problemi. Il report è raggruppato per stato dei problemi e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Problemi per stato e progetto</td> 
   <td>Un report di problemi matrice che visualizza lo Stato dei problemi nei progetti correnti e il Nome del progetto. Il report è raggruppato per Nome progetto e Stato dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Costi Lavoro vs. Costi Spese per Portfolio</td> 
   <td>Un report di progetti che visualizza Costo manodopera pianificata, Costo effettivo manodopera, Costo spesa pianificata e Costo spesa effettivo dei progetti. Il report è raggruppato per nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Lavoro vs. Costi Spese per Programma</td> 
   <td>Un report di progetti che visualizza Costo manodopera pianificata, Costo effettivo manodopera, Costo spesa pianificata e Costo spesa effettivo dei progetti. Il report è raggruppato per nome Portfolio e nome programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo pianificato rispetto al costo effettivo portfolio mensile per Progetto</td> 
   <td>Un report di progetti (dati finanziari) matrice che visualizza la Data di allocazione, il Costo pianificato totale, il Costo effettivo totale e la Variazione costo totale dei progetti. Il report è raggruppato per Nome progetto, il trimestre e il mese della Data di allocazione.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione pianificata rispetto alla retribuzione effettiva portfolio mensile per Progetto</td> 
   <td>Un report di progetti (dati finanziari) matrice che visualizza la Data di allocazione, la Retribuzione pianificata totale, la Retribuzione effettiva totale e la Variazione retribuzione totale dei progetti. Il report è raggruppato per Nome progetto, il trimestre e il mese della Data di allocazione.</td> 
  </tr> 
  <tr> 
   <td>Costi pianificati del progetto mensili rispetto ai costi effettivi</td> 
   <td>Un report di progetti (dati finanziari) matrice che visualizza la Data di allocazione, il Costo pianificato totale, il Costo effettivo totale e la Variazione costo totale dei progetti. Il report è raggruppato per Nome progetto, il trimestre e il mese della Data di allocazione e viene richiesto da Nome progetto.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione pianificata rispetto alla retribuzione effettiva portfolio mensile</td> 
   <td>Un report di progetti (dati finanziari) matrice che visualizza la Data di allocazione, la Retribuzione pianificata totale, la Retribuzione effettiva totale e la Variazione retribuzione totale dei progetti. Il report è raggruppato per Nome progetto, il trimestre e il mese della Data di allocazione e viene richiesto da Nome progetto.</td> 
  </tr> 
  <tr> 
   <td>I Miei Documenti</td> 
   <td>Un report di documenti che visualizza i documenti caricati dall'utente connesso. Il report visualizza i campi seguenti: Nome proprietario, Data modifica, Dimensione, Conteggio versioni, Source e Tipo dei documenti.</td> 
  </tr> 
  <tr> 
   <td>I Miei Preferiti</td> 
   <td>Un report Preferiti che visualizza un elenco di oggetti contrassegnati come preferiti dall'utente connesso. Il report visualizza i campi seguenti: Tipo di oggetto e Nome dei preferiti.</td> 
  </tr> 
  <tr> 
   <td>I miei problemi</td> 
   <td>Un report di problemi che visualizza i problemi incompleti assegnati all'utente connesso. Il rapporto visualizza i campi seguenti: Nome Source, Tipo di problema, Assegnatario principale, Data immissione, Stato e Priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>I Miei Portfolio</td> 
   <td>Un report di Portfoli che visualizza i Portfoli attivi in cui l'utente connesso è il Manager Portfolio.</td> 
  </tr> 
  <tr> 
   <td>I Miei Programmi</td> 
   <td>Un report di programmi che visualizza i programmi e la relativa descrizione, dove l'utente connesso è il responsabile del programma.</td> 
  </tr> 
  <tr> 
   <td>Le Mie Issues Aperte nei Progetti</td> 
   <td>Un report di problemi che visualizza i problemi incompleti in progetti il cui Team di progetto include l'utente connesso. Il rapporto visualizza i campi seguenti: Nome Source, Tipo di problema, Assegnatario principale, Data immissione, Stato e Priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>I miei progetti</td> 
   <td>Un report di progetti che visualizza i progetti correnti il cui Team di progetto include l'utente connesso. Il rapporto visualizza i campi seguenti: Descrizione, Data di completamento pianificata, Data di completamento prevista, Percentuale di completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Problemi inviati</td> 
   <td>Un report di problemi che visualizza i problemi inviati dall'utente connesso che sono stati chiusi negli ultimi tre mesi o che sono attualmente aperti. Il rapporto visualizza i campi seguenti: Nome Source, Tipo di problema, Data inserimento, Stato e Priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Le mie attività</td> 
   <td>Un report di attività che visualizza le attività incomplete nei progetti correnti che sono assegnati all'utente connesso. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, Assegnatario principale, Inizio pianificato, Completamento pianificato, Percentuale completata e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>Le mie schede orario</td> 
   <td>Un report di timesheet che visualizza tutti i timesheet dell'utente connesso. Il rapporto visualizza i campi seguenti: Intervallo date, Nome proprietario, Ore totali, Straordinario, Nome approvatore e Stato delle schede orario.</td> 
  </tr> 
  <tr> 
   <td>Issues non Assegnate a Me</td> 
   <td>Un report di problemi che visualizza i problemi aperti assegnati a una qualsiasi mansione dell'utente connesso e non assegnati all'utente. Il rapporto visualizza i campi seguenti: Nome Source, Tipo di problema, Data inserimento, Stato e Priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Le Mie Attività non Assegnate</td> 
   <td>Un report di attività che visualizza le attività incomplete assegnate a una qualsiasi mansione dell'utente connesso e non assegnate all'utente. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, Assegnatario principale, Data inizio pianificata, Data completamento pianificata, Percentuale completamento e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>Le Mie prossime Attività</td> 
   <td>Un report di attività che visualizza le attività incomplete che dovrebbero iniziare nelle due settimane successive, sono nei progetti correnti e sono assegnate all'utente connesso. Il rapporto visualizza i campi seguenti: Nome progetto, Data completamento pianificata, Data completamento prevista, Percentuale completamento e Stato delle attività.</td> 
  </tr> 
  <tr> 
   <td>Apri i Timesheets(Suggeriti)</td> 
   <td>Un report di timesheet che visualizza i Timesheet aperti. Il rapporto visualizza i campi seguenti: Intervallo date, Proprietario, Ore totali, Straordinario, Nome approvatore, Stato delle schede orario. Il report viene richiesto da: Data inizio scheda orario, Data fine scheda orario, Nome approvatore scheda orario e Nome utente.</td> 
  </tr> 
  <tr> 
   <td>Progetti Fuori Budget per Portfolio</td> 
   <td>Un report di progetti che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto è raggruppato per nome Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Costo Pianifcato Portfolio per Programma</td> 
   <td>Un report di progetti che visualizza il costo pianificato e il costo effettivo dei progetti. Il report viene richiesto in base al nome del Portfolio, raggruppato in base al nome del programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo Pianificato Portfolio per Progetto</td> 
   <td>Un report di progetti che visualizza il costo pianificato e il costo effettivo dei progetti. Il report viene richiesto in base al nome del Portfolio, raggruppato in base al nome del progetto e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Pianificato Portfolio per Programma</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report viene richiesto in base al nome del Portfolio, raggruppato in base al nome del programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Pianificato Portfolio per Progetto</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report viene richiesto in base al nome del Portfolio, raggruppato in base al nome del progetto e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Reali vs. Costi Pianificati per Portfolio</td> 
   <td>Un report di progetti che visualizza il Costo pianificato e il Costo effettivo dei progetti per Portfolio. Il report è raggruppato per nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Reali vs. Costi Pianificati per Programma</td> 
   <td>Un report di progetti che visualizza il Costo pianificato e il Costo effettivo dei progetti in base al Programma. Il report è raggruppato per nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale vs. Reddito Pianificato per Portfolio</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report è raggruppato per nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale vs. Reddito Pianificato per Programma</td> 
   <td>Un report di progetti che visualizza la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il report è raggruppato per Nome programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi portfolio raggruppati per programma e mese</td> 
   <td>Un report di progetti matrice che visualizza il Costo pianificato, il Costo preventivato e il Costo effettivo dei progetti. Il rapporto è raggruppato per nome Portfolio, nome programma e mese della data di inizio pianificata dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Progetti di Portfolio divisi per Stato e Programma</td> 
   <td>Un report di progetti che visualizza lo Stato dei progetti. Il report è raggruppato per Nome programma e Stato progetto e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti di Portfolio divisi per condizione e Portfolio</td> 
   <td>Un report di progetti che visualizza il Nome Portfolio e lo Stato dei progetti. Il report è raggruppato per nome del Portfolio e stato dei progetti e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Il Reddito del Portfolio per Programma</td> 
   <td>Un report di progetti che visualizza il Nome Portfolio, il Nome programma, la Retribuzione pianificata e la Retribuzione effettiva dei progetti. Il rapporto è raggruppato per nome del Portfolio e per nome del programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Retribuzioni raggruppate per programma e mese</td> 
   <td>Un report di progetti matrice che visualizza la Retribuzione pianificata, la Retribuzione effettiva, il Nome Portfolio e il Nome programma. Il rapporto è raggruppato per nome del Portfolio, nome del programma e mese della data di inizio pianificata dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione e costi progetto per stato attività</td> 
   <td>Un report di attività matrice che visualizza il Costo pianificato, il Costo effettivo, la Retribuzione pianificata, la Retribuzione effettiva e il Nome progetto delle attività. Il report è raggruppato per Nome progetto e Stato delle attività.</td> 
  </tr> 
  <tr> 
   <td>Costi Progetto vs. Redditi per Portfolio</td> 
   <td>Un report di progetti che visualizza il Nome Portfolio, il Costo effettivo e la Retribuzione effettiva dei progetti. Il report è raggruppato per nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Spese progetto per mese e trimestre</td> 
   <td>Un report Spesa matrice che visualizza la Data di inserimento, l'Importo pianificato, l'Importo effettivo e il Progetto delle spese. Il report è raggruppato in base al Nome del progetto, al trimestre e al mese della Data di inserimento delle spese.</td> 
  </tr> 
  <tr> 
   <td>Costo orario progetto per tipo di ore per mese</td> 
   <td>Un report di ore matrice che visualizza i campi seguenti: Ore, Data immissione, Costo effettivo dei progetti, Tipo di ora, Nome progetto. Il report è raggruppato per Nome progetto, Mese della Data di immissione delle ore e Tipo di Ora.</td> 
  </tr> 
  <tr> 
   <td>Costo spese e manodopera progetto per mese e trimestre</td> 
   <td>Un report di progetti matrice che visualizza Costo manodopera pianificata, Costo effettivo manodopera, Costo spesa pianificata e Costo spesa effettivo dei progetti. Il report è raggruppato in base al Nome del progetto e al trimestre e al mese della Data di inizio effettiva dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Prestazioni progetto</td> 
   <td>Un report di progetti che visualizza i seguenti campi dei progetti correnti: Data di scadenza, IPC, IPP, CSI, Costo pianificato, Budget, CES e Spese dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Richieste Progetto</td> 
   <td>Un report di progetti che visualizza i progetti richiesti. Il rapporto visualizza i campi seguenti: Descrizione, Data di completamento pianificata, Data di completamento prevista, Percentuale di completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Condizione</td> 
   <td>Un report di progetti che visualizza la Condizione dei progetti. Il report è raggruppato per Condizione e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Condizione per Gruppo</td> 
   <td>Un report di progetti che visualizza lo Stato di avanzamento e il Gruppo dei progetti. Il report è raggruppato per Nome gruppo e Stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Priorità</td> 
   <td>Un report di progetti che visualizza la Priorità dei progetti. Il rapporto è raggruppato per priorità e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Grafico Progetti per Stato Avanzamento</td> 
   <td>Un report di progetti che visualizza lo Stato di avanzamento dei progetti. Il report è raggruppato in base allo stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Attività per stato di avanzamento</td> 
   <td>Un report di attività che visualizza lo Stato di avanzamento di tutte le attività nei progetti correnti. Il report è raggruppato per stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Attività per stato</td> 
   <td>Un report di attività che visualizza lo Stato di tutte le attività. Il report è raggruppato per Stato e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Timesheets da Revisionare</td> 
   <td>Un report di timesheet che visualizza i timesheet inviati e rifiutati il cui approvatore è l'utente connesso. Il rapporto visualizza i campi seguenti: Intervallo date, Proprietario, Ore totali, Straordinario, Nome approvatore e Stato delle schede orario.</td> 
  </tr> 
  <tr> 
   <td>Le attività in pericolo</td> 
   <td>Un report di attività che visualizza le attività incomplete con uno Stato di avanzamento di In ritardo o In ritardo, una Data di handoff precedente a domani e dove l'utente connesso fa parte del Team di progetto del progetto in cui si trovano le attività. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, Assegnatario principale, Inizio pianificato, Completamento pianificato, Percentuale completata e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>I Login Utente</td> 
   <td>Un report di utenti che visualizza i campi seguenti: l’ID univoco, il conteggio degli accessi (il numero di volte in cui l’utente ha effettuato l’accesso dall’avvio con Workfront), la data dell’ultimo accesso degli utenti. Il rapporto è raggruppato per il livello di accesso degli utenti.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Accedere ai rapporti incorporati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Fai clic su **Rapporti**.
1. Fare clic su **Tutti i report**.
1. Espandere il menu a discesa **Filtro** e selezionare **Nuovo filtro**.

1. Fai clic su **Aggiungi una regola filtro**.
1. Nel campo **Inizia a digitare il nome del campo**, inizia a digitare **ID globale**.

1. Sotto l&#39;oggetto **Report**, selezionare **ID globale**.

1. Nel menu a discesa del modificatore di filtro, seleziona **Non è vuoto**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Fai clic su **Salva filtro**.\
   L’elenco dei rapporti mostra solo i rapporti incorporati.\
   Per ulteriori informazioni sui report incorporati disponibili, vedere la sezione [Panoramica dei report incorporati](#overview-of-built-in-reports) in questo articolo.
