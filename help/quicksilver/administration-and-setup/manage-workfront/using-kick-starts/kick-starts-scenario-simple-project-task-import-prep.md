---
user-type: administrator
product-area: system-administration;projects
keywords: kick-start, kick-start, kick-start, kick-start
navigation-topic: use-kick-starts
title: 'Scenario di avvio: preparazione semplice per l''importazione di un progetto e un''attività'
description: Descrive in dettaglio le impostazioni e i controlli disponibili per un'importazione di base di progetti e attività utilizzando il metodo Kick Start.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 9%

---

# Scenario di avvio: preparazione semplice per l’importazione di un progetto e un’attività

Descrive in dettaglio le impostazioni e i controlli disponibili per un&#39;importazione di base di progetti e attività utilizzando il metodo Kick Start.

## Scenario

Il team di implementazione preferisce importare le informazioni sui progetti e sulle attività per i progetti attivi anziché inserire manualmente tali dati nel sistema.

* [Progetti](#projects)
* [Elenco attività](#task-list)

### Progetti {#projects}

Nella tabella seguente vengono visualizzati quattro progetti e i relativi dettagli di base che devono essere mappati nei formati di file di avvio.

Questo scenario presuppone che gli utenti siano già importati in Adobe Workfront. Se gli utenti non sono già in Workfront, sostituisci nomi diversi o completa lo scenario di avvio con gli utenti prima di questo scenario.

1. Implementa Workfront.

   | Data di inizio pianificata | Oggi |
   |---|---|
   | Project Manager | Jennifer Campbell |
   | Sponsor del progetto | Marc Lewis |
   | Gruppo | Marketing |
   | Azienda | *La tua azienda* |

   {style="table-layout:auto"}

1. Implementare il sistema HR.

   | Data di inizio pianificata | 14 luglio 20XX |
   |---|---|
   | Project Manager | Pam Reynolds |
   | Sponsor del progetto | Marc Lewis |
   | Gruppo | Marketing |
   | Azienda | *La tua azienda* |

   {style="table-layout:auto"}

1. Implementare Document Management System.

   | Data di inizio pianificata | 22 agosto 20XX |
   |---|---|
   | Project Manager | Jennifer Campbell |
   | Sponsor del progetto | Ray Andrews |
   | Gruppo | IT |
   | Azienda | *La tua azienda* |

   {style="table-layout:auto"}

1. Implementare un nuovo sistema di calendario.

   | Data di inizio pianificata | 6 settembre 20XX |
   |---|---|
   | Project Manager | Pam Reynolds |
   | Sponsor del progetto | Ray Andrews |
   | Gruppo | IT |
   | Azienda | *La tua azienda* |

   {style="table-layout:auto"}

### Elenco attività {#task-list}

Nell&#39;elenco di attività seguente vengono visualizzati elenchi di attività eccessivamente semplificati per i progetti. L’unica differenza tra i progetti è rappresentata dalle date di inizio e dall’avanzamento di ciascun progetto.

Le attività padre ereditano la durata, il lavoro e la percentuale di completamento delle attività figlio. Non è necessario impostare tali valori per che diventeranno attività di riepilogo.

>[!NOTE]
>
>Le istruzioni fornite in questo scenario non sono così esplicite come le istruzioni dettagliate fornite in [Scenario di avvio: società, gruppo, ruolo e preparazione di avvio utente](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). Il presupposto è che tu abbia già imparato a cercare e copiare i valori dai fogli Azienda e Gruppo, quindi questi passaggi saranno menzionati, ma non descritti in modo specifico.

1. Configura.
1. Importa utenti.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività principale</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>1 ora</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>1 ora</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Documentazione: 100%</p> <p>Calendario: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Impostare le autorizzazioni.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività principale</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pred</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>1 ora</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>1 ora</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Documentazione: 100%</p> <p>Calendario: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Creare gruppi.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività principale</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pred</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>2 giorni</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>4 ore</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Documentazione: 100%</p> <p>Calendario: 25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Prepara l’addestramento.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>2 giorni</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>4 ore</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Documentazione: 50%</p> <p>Calendario: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Creare criteri di supporto continui.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>2 giorni</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>4 ore</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Documentazione: 50%</p> <p>Calendario: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Esegui il rollout.

   | Pred | 1, 6, 7 |
   |---|---|

   {style="table-layout:auto"}

1. Formazione degli utenti.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazione a</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività principale</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td>1 giorno</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoro</td> 
      <td>2 ore</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completata</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 0%</p> <p>Documenti: 0%</p> <p>Calendario: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Scarica modello

Vai alla pagina Kick-Start. Selezionare gli oggetti Company (Società), Group (Gruppo), Project (Progetto), Task (Attività) e User (Utente). Seleziona la casella di controllo Includi dati esistenti (questa operazione consente di fare rapidamente riferimento agli ID società, gruppo e utente). Fai clic sul pulsante Scarica.

## Immetti dettagli progetto

Apri il file Workfront.xlsx appena scaricato. Passare all&#39;elenco Progetto PROJ.

![](assets/im2.png)
A meno che tu non abbia già creato dei progetti in Workfront, questo campo deve essere vuoto.

![](assets/im10.png)

Impostare i valori per i seguenti campi del progetto:

* **Imposta colonna isNew**
Immettere TRUE nelle righe da 3 a 6 per la colonna isNew.
* **Impostare ID univoci**
Immettere un ID univoco in ogni riga per la colonna ID. In genere, i numeri interi a partire da 1 funzionano correttamente durante la creazione di nuovi record.
* **Imposta nomi progetto**
Immettere i nomi di ciascun progetto nella colonna setName.
* **Imposta pianificazione progetto**

  Immettere l&#39;ID della pianificazione che si desidera venga utilizzata dal progetto nel campo setScheduleID

* **Imposta la data di inizio pianificata del progetto**

  Immettere la data e l&#39;ora nella colonna setPlannedStartDate con l&#39;ora e la data di inizio desiderate per il progetto. Se lasciato vuoto, Workfront importa il progetto con la data del giorno corrente e una marca temporale della mezzanotte di quel giorno in base al fuso orario del browser.

* **Imposta numeri attività**
Immettere i valori nella colonna setTaskNumber per controllare l&#39;ordine di visualizzazione delle attività nel piano di progetto.
* **Fornisci le date del progetto.**
Immettere la Data inizio pianificata per ogni progetto nella colonna setPlannedStartDate.
* **Imposta altri dettagli necessari.**
Compila altri dettagli, ad esempio una descrizione o lo stato corrente, secondo necessità. Cercare gli ID gruppo per ciascun progetto nel foglio Gruppo di gruppi e inserirli nella colonna setGroupID per i rispettivi progetti. Cercare l&#39;ID società per i progetti nel foglio Società della società e inserirlo nella colonna setCompanyID. Cercare l&#39;ID utente per ogni proprietario del progetto nel foglio Utente e inserirlo nella colonna setOwnerID. Cercare l&#39;ID utente di ogni sponsor del progetto nel foglio Utente e inserirlo nella colonna setSponsorID.

![](assets/im9.png)

>[!NOTE]
>
>I valori accettabili per i campi Stato e Priorità possono essere individuati esaminando le preferenze di stato e priorità per ciascun oggetto nell&#39;area Configurazione flusso di lavoro di Workfront.

## Immetti dettagli attività

È possibile aggiungere informazioni sulle attività del progetto durante l&#39;importazione del progetto mediante l&#39;avvio.

Apri il file Workfront.xlsx appena scaricato. **Passare alla finestra Attività.**

Questo foglio deve essere vuoto, a meno che non siano già state create attività in Workfront.

![](assets/im8.png)

![](assets/im7.png)

![](assets/im6.png)

Il modo più semplice per mappare le attività è un progetto alla volta (in particolare quando le attività sono le stesse in ogni progetto). È quindi possibile copiare il piano attività per il primo progetto e apportare piccole modifiche al piano attività per i progetti successivi. Per i passaggi rimanenti si presuppone la creazione di attività solo per il progetto Implementa Workfront. In base allo scenario, importerai 9 attività per progetto, quindi inserisci TRUE nelle righe da 3 a 11 per la colonna isNew.

Impostare i valori per i campi delle attività seguenti:

* **Imposta ID**
Inserisci un ID univoco in ogni riga per la colonna ID.
* **Imposta nomi**
Immettere i nomi delle attività nella colonna setName.
* **Conferma ID Progetto**
Immettere l&#39;ID impostato per l&#39;implementazione del progetto Workfront; esaminare il foglio Progetto PROJ per assicurarsi che sia l&#39;ID corretto.
* **Imposta utenti**
Andare al foglio Utente per cercare l&#39;ID dell&#39;utente assegnato a ogni attività e immettere questi valori nelle rispettive celle della colonna setAssignedToID.
* **Identificare le relazioni tra le attività**
Per le attività da 2 a 5, immettere 1 nella colonna setParentID. Per l&#39;operazione 9, immettere 8 nella colonna setParentID. Nella colonna setPredecessorString immettere il numero di attività per ogni attività predecessore. Se un&#39;attività ha più predecessori, come l&#39;attività 8 in questo scenario, è necessario utilizzare una virgola per separare l&#39;ID di ogni attività predecessore. I Predecessori possono essere definiti con ritardi nelle relazioni non-Fine-Inizio utilizzando la scorciatoia descritta nell’articolo Creazione di relazioni dei Predecessori.
* **Imposta durata**
Impostare la durata di ogni attività immettendo il numero di ore, giorni, settimane o mesi per l&#39;attività nel campo setDuration. Immettere quindi l&#39;unità di durata nel campo setDurationUnit.

  |   | Valore accettabile |
  |---|---|
  | Minuti | M |
  | Ore | H |
  | Giorni | Dsbld |
  | Settimane | M |
  | Mesi | G |

  I minuti possono anche essere rappresentati come frazione di un&#39;ora (p. es., minuti = 5 ore)

* Impostare la quantità di lavoro per ogni attività nel campo setWorkRequired. Inserire quindi l&#39;unità di lavoro nel campo setWorkUnit. Se il valore Work Required è diverso dalla durata, sarà inoltre necessario immettere un valore A nel campo setDurationType.

  | Tipo di Durata | Valore accettabile |
  |---|---|
  | Incarico Calcolato | A |
  | Lavoro Calcolato | M |
  | Impegno Aggiuntivo | Dsbld |
  | Semplice | S |

* Immettere la rappresentazione numerica completa della percentuale di completamento nel campo setPercentComplete per ogni attività. Questo valore non deve includere il simbolo di percentuale (%).
* Includi una descrizione e altri dettagli per ogni attività che stai creando, secondo necessità.

  ![](assets/im5.png)

* Le colonne setPlannedStartDate e setTaskConstraint non vengono utilizzate per creare l&#39;indicatore cronologico di questo progetto perché si basano su relazioni predecessori. In alternativa, è possibile immettere una data per ogni attività. In questo caso, assicurarsi di specificare un vincolo di attività valido anche nella colonna setTaskConstraint. Per informazioni dettagliate sui valori validi per questo campo, consulta Vincolo attività e articoli correlati.

  In questo caso, il modo più semplice per creare le attività per gli altri progetti che si stanno importando consiste nel copiare le attività appena definite e incollarle di seguito, a partire dalla riga 12. In questo modo:

   1. Rinumera i valori nella colonna ID.
   1. Aggiornare la colonna setProjectID al valore impostato per il progetto successivo.
   1. Aggiornare i valori setParentID e setPredecessorString per riflettere i nuovi ID assegnati alle attività del progetto.
   1. Aggiorna assegnazioni attività e percentuale di completamento.
   1. Ripeti questi passaggi per le attività del progetto successivo.

* **Importa il file Excel**

  Seguire le istruzioni fornite in [Importare dati in Adobe Workfront utilizzando un modello di avvio](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
