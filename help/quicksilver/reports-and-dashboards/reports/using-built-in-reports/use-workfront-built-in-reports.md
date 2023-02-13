---
product-area: reporting
navigation-topic: using-built-in-reports
title: Utilizzare i report incorporati di Adobe Workfront
description: Adobe Workfront dispone di un elenco completo dei rapporti incorporati che puoi utilizzare.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2997'
ht-degree: 11%

---

# Utilizzare i report incorporati di Adobe Workfront

Adobe Workfront dispone di un elenco completo dei rapporti incorporati che puoi utilizzare.

Gli amministratori di Workfront possono nascondere i rapporti incorporati in modo che gli utenti non abbiano accesso a tali rapporti.\
Per ulteriori informazioni su come nascondere i rapporti incorporati, consulta [Nascondere i rapporti incorporati](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

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
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Visualizzazione o accesso successivo a Report, Dashboard, Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per aggiungere o modificare un filtro a un report</p> <p>Gestire le autorizzazioni di un filtro per modificarlo in un elenco</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Panoramica dei report incorporati {#overview-of-built-in-reports}

Puoi personalizzare un rapporto incorporato e salvarlo come nuovo. Per ulteriori informazioni sulla personalizzazione dei rapporti incorporati, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

I seguenti rapporti sono forniti con il pacchetto Workfront. I rapporti sono disponibili per tutti gli utenti che dispongono almeno dei diritti di visualizzazione per i rapporti incorporati nel loro livello di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome Report</strong> </th> 
   <th><strong>Descrizione del rapporto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo Reale di Portfolio per Programma</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome programma, richiesto per Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo Reale di Portfolio per Progetto</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome progetto, richiesto per Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale di Portfolio per Programma</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto è raggruppato per Nome programma, richiesto per Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale di Portfolio per Progetto</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto è raggruppato per Nome progetto, richiesto per Nome Portfolio, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questa mostra il Reddito Reale per Azienda</td> 
   <td>Rapporto Progetto che visualizza le entrate effettive e la società dei progetti. Il rapporto è raggruppato per Nome società e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questa mostra il Reddito Reale per Gruppo</td> 
   <td>Rapporto Progetto che visualizza le entrate effettive e il gruppo dei progetti. Il rapporto è raggruppato per Nome gruppo e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Tutti i Timesheets Aperti</td> 
   <td>Rapporto Scheda attività contenente fogli presenze aperti. Il rapporto visualizza i campi seguenti: Intervallo date, nome proprietario, ore totali, ore straordinarie, nome approvatore e stato dei fogli ore.</td> 
  </tr> 
  <tr> 
   <td>Timesheets da Approvare(Suggeriti)</td> 
   <td>Rapporto Scheda attività che visualizza schede attività inviate o rifiutate con approvatori. Il rapporto visualizza i campi seguenti: intervallo di date, proprietario, ore totali, ore straordinarie, nome dell'approvatore e stato dei fogli ore. Il rapporto è richiesto da: Data inizio foglio presenze, Data fine foglio presenze, Nome approvatore scheda attività e Nome utente.</td> 
  </tr> 
  <tr> 
   <td>Progetti a Rischio</td> 
   <td>Rapporto di progetto che visualizza i progetti correnti e di pianificazione che presentano una condizione di rischio o in difficoltà. Il rapporto visualizza i campi seguenti: Descrizione, Data completamento pianificato, Data completamento previsto, Percentuale completamento, Stato e Priorità dei progetti. Il rapporto è raggruppato per Nome Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per azienda</td> 
   <td>Rapporto Progetto che visualizza i ricavi aziendali e di fatturazione dei progetti. Il rapporto è raggruppato per Nome società e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per gruppo</td> 
   <td>Rapporto Progetto che visualizza i ricavi di fatturazione e il gruppo dei progetti. Il rapporto è raggruppato per Nome gruppo e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Questo mostra il reddito fatturato per mese</td> 
   <td>Rapporto Record di fatturazione che visualizza il nome del progetto, i ricavi di fatturazione del progetto e la data di fatturazione dei record di fatturazione. Il rapporto è raggruppato in base al mese della data di fatturazione dei record di fatturazione e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Issues Completate per Settimana</td> 
   <td>Rapporto di problema che visualizza la data di completamento effettivo dei problemi. Il rapporto è raggruppato per la settimana della data di completamento effettivo dei problemi e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Issues Completate per Utente per Settimana</td> 
   <td>Rapporto di problema che visualizza la data di completamento effettivo e le assegnazioni dei problemi. Il rapporto è raggruppato per l'assegnatario principale e per la settimana della data di completamento effettivo dei problemi e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti Attuali</td> 
   <td>Rapporto Progetto che visualizza tutti i progetti correnti. Il rapporto visualizza i campi seguenti: Descrizione, Data completamento pianificato, Data completamento previsto, Percentuale completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Costo orario per utente per mese</td> 
   <td>Rapporto Ora matrice che visualizza il numero di ore registrate e il relativo costo effettivo. Il rapporto è raggruppato per Nome proprietario e per il mese della Data di immissione delle ore.</td> 
  </tr> 
  <tr> 
   <td>Ore per utente</td> 
   <td>Rapporto Ora che visualizza il numero di ore registrate. Il rapporto è raggruppato per Nome proprietario e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Ore per utente per settimana</td> 
   <td>Report dell'ora della matrice che visualizza il numero di ore registrate nelle ultime quattro settimane e la data di ingresso delle ore. Il rapporto viene richiesto dalla data di ingresso delle ore e viene raggruppato per Nome proprietario e per il mese della data di ingresso delle ore.</td> 
  </tr> 
  <tr> 
   <td>Problemi per stato</td> 
   <td>Un report di problema che visualizza lo stato dei problemi. Il rapporto è raggruppato in base allo stato dei problemi e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Problemi per stato e progetto</td> 
   <td>Report di problema della matrice che visualizza lo stato dei problemi nei progetti correnti e il nome del progetto. Il rapporto è raggruppato per Nome progetto e Stato dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Costi Lavoro vs. Costi Spese per Portfolio</td> 
   <td>Rapporto Progetto che visualizza il costo del lavoro pianificato, il costo del lavoro effettivo, il costo della spesa pianificata e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Lavoro vs. Costi Spese per Programma</td> 
   <td>Rapporto Progetto che visualizza il costo del lavoro pianificato, il costo del lavoro effettivo, il costo della spesa pianificata e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome Portfolio e Nome programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo pianificato rispetto al costo effettivo portfolio mensile per Progetto</td> 
   <td>Rapporto Progetto a matrice (dati finanziari) che visualizza la data di allocazione, il costo totale pianificato, il costo effettivo totale e lo scostamento del costo totale dei progetti. Il rapporto è raggruppato per Nome progetto, trimestre e mese della data di allocazione.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione pianificata rispetto alla retribuzione effettiva portfolio mensile per Progetto</td> 
   <td>Rapporto Progetto a matrice (dati finanziari) che visualizza la data di allocazione, i ricavi totali pianificati, i ricavi effettivi totali e la varianza dei ricavi totali dei progetti. Il rapporto è raggruppato per Nome progetto, trimestre e mese della data di allocazione.</td> 
  </tr> 
  <tr> 
   <td>Costi pianificati del progetto mensili rispetto ai costi effettivi</td> 
   <td>Rapporto Progetto a matrice (dati finanziari) che visualizza la data di allocazione, il costo totale pianificato, il costo effettivo totale e lo scostamento del costo totale dei progetti. Il rapporto è raggruppato per Nome progetto, il trimestre e il mese della data di allocazione ed è richiesto per Nome progetto.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione pianificata rispetto alla retribuzione effettiva portfolio mensile</td> 
   <td>Rapporto Progetto a matrice (dati finanziari) che visualizza la data di allocazione, i ricavi totali pianificati, i ricavi effettivi totali e la varianza dei ricavi totali dei progetti. Il rapporto è raggruppato per Nome progetto, il trimestre e il mese della data di allocazione ed è richiesto per Nome progetto.</td> 
  </tr> 
  <tr> 
   <td>I Miei Documenti</td> 
   <td>Rapporto Documento che visualizza i documenti caricati dall'utente connesso. Il rapporto visualizza i campi seguenti: Nome proprietario, Data modifica, Dimensioni, Conteggio versioni, Origine e Tipo dei documenti.</td> 
  </tr> 
  <tr> 
   <td>I Miei Preferiti</td> 
   <td>Un rapporto Preferiti che visualizza un elenco di oggetti contrassegnati come preferiti dall'utente connesso. Il rapporto visualizza i campi seguenti: Tipo di oggetto e Nome dei preferiti.</td> 
  </tr> 
  <tr> 
   <td>I miei problemi</td> 
   <td>Un report di problema che visualizza i problemi incompleti assegnati all'utente che ha effettuato l'accesso. Il rapporto visualizza i campi seguenti: Nome origine, tipo di emissione, assegnatario principale, data di ingresso, stato e priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>I Miei Portfolio</td> 
   <td>Rapporto di Portfolio che visualizza i Portfoli attivi in cui l'utente connesso è il manager di Portfolio.</td> 
  </tr> 
  <tr> 
   <td>I Miei Programmi</td> 
   <td>Rapporto Programma che visualizza i programmi e la relativa descrizione, in cui l’utente connesso è il Program Manager.</td> 
  </tr> 
  <tr> 
   <td>Le Mie Issues Aperte nei Progetti</td> 
   <td>Report di problema che visualizza problemi incompleti nei progetti il cui team di progetto include l'utente connesso. Il rapporto visualizza i campi seguenti: Nome origine, tipo di emissione, assegnatario principale, data di ingresso, stato e priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>I miei progetti</td> 
   <td>Un report di progetti che visualizza i progetti correnti il cui Team di progetto include l'utente connesso. Il rapporto visualizza i campi seguenti: Descrizione, Data completamento pianificato, Data completamento previsto, Percentuale completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Le Issues che ho inviato</td> 
   <td>Un report di problema che visualizza i problemi inviati dall'utente connesso che sono stati chiusi negli ultimi tre mesi o sono attualmente aperti. Il rapporto visualizza i campi seguenti: Nome origine, tipo di emissione, data di ingresso, stato e priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Le mie attività</td> 
   <td>Report attività che visualizza le attività incomplete in Progetti correnti assegnate all'utente connesso. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, assegnatario principale, Inizio pianificato, Completamento pianificato, Percentuale completata e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>Le mie schede orario</td> 
   <td>Un report di Timesheet che visualizza tutti i timesheet dell'utente connesso. Il rapporto visualizza i campi seguenti: Intervallo date, nome proprietario, ore totali, ore straordinarie, nome approvatore e stato dei fogli ore.</td> 
  </tr> 
  <tr> 
   <td>Issues non Assegnate a Me</td> 
   <td>Un rapporto di problema che visualizza i problemi aperti assegnati a uno qualsiasi dei ruoli di lavoro dell’utente connesso e che non sono assegnati all’utente. Il rapporto visualizza i campi seguenti: Nome origine, tipo di emissione, data di ingresso, stato e priorità dei problemi.</td> 
  </tr> 
  <tr> 
   <td>Le Mie Attività non Assegnate</td> 
   <td>Report attività che visualizza le attività incomplete assegnate a uno qualsiasi dei ruoli di lavoro dell'utente connesso e non assegnate all'utente. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, assegnatario principale, Data inizio pianificata, Data completamento pianificato, Percentuale completamento e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>Le Mie prossime Attività</td> 
   <td>Un rapporto di attività che visualizza le attività incomplete che dovrebbero iniziare nelle due settimane successive, si trova su progetti correnti e viene assegnato all’utente connesso. Il rapporto visualizza i campi seguenti: Nome progetto, Data completamento pianificato, Data completamento previsto, Percentuale completamento e Stato delle attività.</td> 
  </tr> 
  <tr> 
   <td>Apri i Timesheets(Suggeriti)</td> 
   <td>Rapporto Scheda attività contenente fogli presenze aperti. Il rapporto visualizza i campi seguenti: intervallo di date, proprietario, ore totali, ore straordinarie, nome dell'approvatore, stato dei fogli presenze. Il rapporto è richiesto da: Data inizio foglio presenze, Data fine foglio presenze, Nome approvatore scheda attività e Nome utente.</td> 
  </tr> 
  <tr> 
   <td>Progetti Fuori Budget per Portfolio</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Costo Pianifcato Portfolio per Programma</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto viene richiesto in Nome Portfolio, raggruppato per Nome programma, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costo Pianificato Portfolio per Progetto</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti. Il rapporto viene richiesto in Nome Portfolio, raggruppato per Nome progetto, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Pianificato Portfolio per Programma</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto viene richiesto in Nome Portfolio, raggruppato per Nome programma, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Pianificato Portfolio per Progetto</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto viene richiesto in Nome Portfolio, raggruppato per Nome progetto, e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Reali vs. Costi Pianificati per Portfolio</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti per Portfolio. Il rapporto è raggruppato per Nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi Reali vs. Costi Pianificati per Programma</td> 
   <td>Rapporto Progetto che visualizza il costo pianificato e il costo effettivo dei progetti in base al programma. Il rapporto è raggruppato per Nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale vs. Reddito Pianificato per Portfolio</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto è raggruppato per Nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Reddito Reale vs. Reddito Pianificato per Programma</td> 
   <td>Rapporto Progetto che visualizza i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto è raggruppato per Nome programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Costi portfolio raggruppati per programma e mese</td> 
   <td>Rapporto Progetto a matrice che visualizza il costo pianificato, il costo preventivato e il costo effettivo dei progetti. Il rapporto è raggruppato per Nome Portfolio, Nome programma e il mese della Data di inizio pianificata dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Progetti di Portfolio divisi per Stato e Programma</td> 
   <td>Rapporto Progetto che visualizza lo stato dei progetti. Il rapporto è raggruppato per Nome programma e Stato progetto e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti di Portfolio divisi per condizione e Portfolio</td> 
   <td>Rapporto Progetto che visualizza il Nome Portfolio e lo Stato dei progetti. Il rapporto è raggruppato in base al nome del Portfolio e allo stato dei progetti e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Il Reddito del Portfolio per Programma</td> 
   <td>Rapporto Progetto che visualizza il nome Portfolio, il nome del programma, i ricavi pianificati e i ricavi effettivi dei progetti. Il rapporto è raggruppato in base al nome del Portfolio e al nome del programma e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Retribuzioni raggruppate per programma e mese</td> 
   <td>Rapporto Progetto a matrice che visualizza Ricavo pianificato, Ricavo effettivo, Nome Portfolio e Nome programma. Il rapporto è raggruppato in base al nome del Portfolio, al nome del programma e al mese della data di inizio prevista dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Retribuzione e costi progetto per stato attività</td> 
   <td>Report task a matrice che visualizza il costo pianificato, il costo effettivo, i ricavi pianificati, i ricavi effettivi e il nome del progetto delle attività. Il rapporto è raggruppato per Nome progetto e Stato delle attività.</td> 
  </tr> 
  <tr> 
   <td>Costi Progetto vs. Redditi per Portfolio</td> 
   <td>Rapporto Progetto che visualizza il nome Portfolio, il costo effettivo e i ricavi effettivi dei progetti. Il rapporto è raggruppato per Nome Portfolio e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Spese progetto per mese e trimestre</td> 
   <td>Una nota spese matrice che visualizza la data di immissione, l'importo pianificato, l'importo effettivo e il progetto delle spese. Il rapporto è raggruppato in base al Nome del progetto, al trimestre e al mese della Data di ingresso delle spese.</td> 
  </tr> 
  <tr> 
   <td>Costo orario progetto per tipo di ore per mese</td> 
   <td>Rapporto Ora matrice che visualizza i campi seguenti: Ore, Data di entrata, Costo effettivo dei progetti, Tipo ora, Nome del progetto. Il rapporto è raggruppato per Nome progetto, mese della data di ingresso delle ore e tipo di ora.</td> 
  </tr> 
  <tr> 
   <td>Costo spese e manodopera progetto per mese e trimestre</td> 
   <td>Rapporto Progetto a matrice che visualizza il costo del lavoro pianificato, il costo del lavoro effettivo, il costo della spesa pianificata e il costo effettivo dei progetti. Il rapporto è raggruppato in base al Nome progetto e al trimestre e al mese della Data di inizio effettiva dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Performance del Progetto</td> 
   <td>Rapporto Progetto che visualizza i campi seguenti dei progetti correnti: Data di scadenza, CPI, SPI, CSI, Costo pianificato, Budget, EAC e Spese dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Richieste Progetto</td> 
   <td>Rapporto Progetto che visualizza i progetti richiesti. Il rapporto visualizza i campi seguenti: Descrizione, Data completamento pianificato, Data completamento previsto, Percentuale completamento, Stato e Priorità dei progetti.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Condizione</td> 
   <td>Rapporto Progetto che visualizza la condizione dei progetti. Il rapporto è raggruppato per Condizione e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Condizione per Gruppo</td> 
   <td>Rapporto Progetto che visualizza lo stato di avanzamento e il gruppo dei progetti. Il rapporto è raggruppato per Nome gruppo e Stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Progetti per Priorità</td> 
   <td>Rapporto Progetto che mostra la Priorità dei progetti. Il rapporto è raggruppato per Priorità e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Grafico Progetti per Stato Avanzamento</td> 
   <td>Rapporto Progetto che visualizza lo stato di avanzamento dei progetti. Il rapporto è raggruppato in base allo stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Attività per stato di avanzamento</td> 
   <td>Rapporto attività che visualizza lo stato di avanzamento di tutte le attività nei progetti correnti. Il rapporto è raggruppato per Stato di avanzamento e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Attività per stato</td> 
   <td>Un report di attività che visualizza lo Stato di tutte le attività. Il rapporto è raggruppato per Stato e include un grafico.</td> 
  </tr> 
  <tr> 
   <td>Timesheets da Revisionare</td> 
   <td>Report Scheda attività che visualizza i fogli presenze inviati e rifiutati il cui approvatore è l'utente connesso. Il rapporto visualizza i campi seguenti: intervallo di date, proprietario, ore totali, ore straordinarie, nome dell'approvatore e stato dei fogli ore.</td> 
  </tr> 
  <tr> 
   <td>Le attività in pericolo</td> 
   <td>Report attività che visualizza le attività incomplete con stato di avanzamento in ritardo o in ritardo, una data di consegna precedente a domani e in cui l'utente connesso fa parte del team di progetto del progetto in cui si trovano le attività. Il rapporto visualizza i campi seguenti: Durata pianificata, Nome progetto, assegnatario principale, Inizio pianificato, Completamento pianificato, Percentuale completamento e Priorità delle attività.</td> 
  </tr> 
  <tr> 
   <td>I Login Utente</td> 
   <td>Un rapporto utente che visualizza i campi seguenti: l’ID univoco, Conteggio accessi (il numero di volte in cui l’utente ha effettuato l’accesso a partire da Workfront), Data ultimo accesso degli utenti. Il rapporto è raggruppato in base al livello di accesso degli utenti.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Accesso ai report incorporati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.
1. Fai clic su **Rapporti**.
1. Fai clic su **Tutti i report**.
1. Espandi la **Filtro** menu a discesa e seleziona **Nuovo filtro**.

1. Fai clic su **Aggiungere una regola filtro**.
1. In **Inizia a digitare il nome del campo** campo, inizia a digitare **ID globale**.

1. Sotto la **Rapporto** oggetto, selezionare **ID globale**.

1. Nel menu a discesa del modificatore del filtro, seleziona **Non vuoto**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Fai clic su **Salva filtro**.\
   Nell’elenco dei rapporti sono visualizzati solo i rapporti incorporati.\
   Per ulteriori informazioni sui rapporti incorporati disponibili, vedi [Panoramica dei report incorporati](#overview-of-built-in-reports).
