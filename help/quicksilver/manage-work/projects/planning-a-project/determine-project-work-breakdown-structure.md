---
product-area: projects
navigation-topic: plan-a-project
title: Determinare la struttura funzionale di un progetto
description: La definizione di una WBS (Work Breakdown Structure) per un progetto è un insieme di attività che alla fine delinea il piano del progetto. Il WBS divide il risultato del progetto in elementi di lavoro gestibili, che possono essere utilizzati per definire le attività cardine e organizzare le assegnazioni di lavoro.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Determinare la struttura funzionale di un progetto

La definizione di una WBS (Work Breakdown Structure) per un progetto è un insieme di attività che alla fine delinea il piano del progetto. Il WBS divide il risultato del progetto in elementi di lavoro gestibili, che possono essere utilizzati per definire le attività cardine e organizzare le assegnazioni di lavoro.

Per creare la struttura funzionale di un progetto, è necessario disporre di una licenza Pianificazione con accesso Modifica ai progetti. Potrebbe essere necessario un accesso aggiuntivo ad altre aree di Adobe Workfront, a seconda del numero di attività eseguite durante la creazione di WBS.

È consigliabile mantenere il progetto nello stato Pianificazione mentre si apportano modifiche alla struttura funzionale del progetto, per evitare notifiche da attivare per gli utenti del team di progetto.

## Definire i risultati finali del progetto

Lo scopo di un progetto è quello di fornire risultati tangibili a soggetti interessati interni ed esterni. I risultati finali di un progetto sono i risultati che si desidera ottenere completando il progetto. I risultati sono quasi sempre associati ad almeno un risultato finale e tutti i risultati finali devono essere associati a un progetto.

I prodotti del progetto possono essere beni di consumo, produzione intellettuale (ad esempio report) o servizi. Ad esempio, se l’ambito del progetto è la costruzione di una casa, alcuni dei risultati finali possono includere:

* creazione di piani architetturali
* completamento dell&#39;impianto idraulico
* lavori elettrici
* versamento della fondazione
* lavoro di inquadratura
* chiudere la vendita della casa.

A seconda delle dimensioni e dell&#39;ambito, un progetto può essere costituito da più risultati finali.

Una volta identificati i risultati finali, puoi iniziare a suddividerli in attività. Le attività sono l’output ottenuto per fornire il risultato complessivo del progetto. Quando definisci le attività, prendi in considerazione i seguenti parametri:

* Quantità di tempo richiesta per il completamento.
* Budget necessario per il completamento del lavoro.
* Risorse necessarie per completare il lavoro.
* Pianificazione delle risorse in base alla sequenza temporale logica delle attività.

Quando si definiscono le attività, assicurarsi di non pianificare troppo lavoro per una singola attività. Se il lavoro necessario per un&#39;attività è superiore a 40 ore (una settimana di lavoro tipica), potrebbe essere necessario suddividere tale quantità di lavoro nelle sottoattività. Il completamento di tutte le sottoattività completerà quindi l&#39;attività principale.

Per definire i risultati e i risultati finali WBS in Workfront, è consigliabile eseguire le attività seguenti per creare una visualizzazione gerarchica delle attività di progetto:

* Se non lo hai già fatto, crea un nuovo progetto.\
  Per informazioni sulla creazione di un progetto, consulta l’articolo [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

* Crea attività per tutte le azioni necessarie per completare ogni risultato finale e risultato finale.\
  Per informazioni sulla creazione di attività, vedere l&#39;articolo [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* Dalle attività appena create, identificare i risultati principali e associarli alle attività cardine.\
  Per informazioni sulla creazione di attività cardine, vedere gli articoli [Creare un percorso milestone](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associa attività cardine ad attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Suddividere le attività con un ambito troppo grande in sottoattività. Associale all&#39;elemento padre che definisce il risultato finale.\
  Per informazioni sulla creazione di sottoattività, vedere l&#39;articolo [Crea sottoattività](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identificare le relazioni di dipendenza tra le sottoattività e tra le attività cardine.\
  In una relazione di dipendenza, l&#39;inizio di un&#39;attività dipende dal completamento di un&#39;altra attività o gruppo di attività.\
  Per informazioni sulle relazioni tra attività, vedere gli articoli [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) e [Creare una relazione predecessore nell&#39;elenco delle attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Determina se, in qualsiasi momento della durata del progetto, sono necessarie approvazioni e revisioni. Crea processi di approvazione per soddisfare questa esigenza.\
  Per informazioni sulle approvazioni, consulta l’articolo [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Stima vincoli programmazione lavoro e programmazione

Dopo aver creato l&#39;attività cardine e la struttura delle attività di base del progetto, è possibile stimare il tempo necessario per completare il progetto complessivo definendo vincoli e durate delle attività.

Considera quanto segue:

* I vincoli di attività definiscono quando il lavoro su un&#39;attività deve iniziare o terminare.

  Per informazioni sulla definizione dei vincoli delle attività, vedere l&#39;articolo [Panoramica sui vincoli delle attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La Durata di un&#39;attività è l&#39;intervallo di tempo disponibile per completare un&#39;attività. Durante la stima della durata, è possibile immettere un valore che tenga conto della possibilità di un ritardo. Se progetti simili sono stati completati in passato, potresti avere una buona idea su dove impostare questo valore.

  Poiché la durata è una stima, assicurarsi di impostare valori di tempo ottimistici per tenere conto di fattori che potrebbero influenzare l&#39;attività, come condizioni meteorologiche, interruzioni dell&#39;alimentazione, difficoltà del fornitore o altri eventi imprevisti. Inoltre, assicurarsi di considerare se esistono attività predecessore o di relazione associate e come queste possano creare vincoli sul lavoro e influire sul completamento dell&#39;attività.

  A seconda del Tipo di durata dell&#39;attività, è possibile modificare la durata di un&#39;attività durante il ciclo di vita di un progetto, ma questo influirà anche sulla sequenza temporale del progetto. Per informazioni sulla durata di un&#39;attività, vedere l&#39;articolo [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Assegna attività

Dopo aver definito la durata e i vincoli di ogni attività, è possibile determinare chi dispone del tempo e delle competenze necessarie per eseguire il lavoro. In Workfront è possibile assegnare attività alle seguenti entità:

* Utenti\
  Solo gli utenti con un livello di accesso Planner o Worker possono essere assegnati alle attività. Sebbene sia possibile assegnare le attività a richiedenti e revisori, questi non possono completarle. Per questo motivo, si sconsiglia di assegnare loro le attività.

  Per informazioni sui livelli di accesso e sulla definizione delle operazioni che gli utenti possono eseguire con gli oggetti di Workfront, vedere [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Ruoli
* Team

Per informazioni sull&#39;assegnazione delle attività, vedere gli articoli della [Assegna attività](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) sezione.

## Gestire le risorse

La gestione delle risorse in Workfront consente di determinare se è disponibile personale adeguato per completare il progetto. Quando gli utenti vengono aggiunti a un progetto, Workfront mostra l’utilizzo di ciascun utente. I responsabili delle risorse possono visualizzare il numero totale di ore assegnate dalla persona ad altri progetti durante l’intervallo di tempo del progetto.

>[!NOTE]
>
>Se lo stato del progetto è Pianificazione, i task assegnati agli utenti non vengono visualizzati nei relativi elenchi di task.

All’inizio di un anno fiscale o di un trimestre, potrebbe essere utile gestire le risorse a un livello più alto, su più progetti, senza conoscere una specifica struttura funzionale.\
Per informazioni sulla pianificazione dell’utilizzo delle risorse a un livello più alto, consulta l’articolo [Introduzione alla pianificazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Quando si gestiscono le risorse nel contesto della creazione della struttura funzionale di un progetto e si assicura che ogni attività sia assegnata alla risorsa corretta, è possibile programmare le risorse per il lavoro da eseguire.\
Per informazioni sulla pianificazione delle risorse, consulta gli articoli nella sezione [L’indice del Bilanciatore dei carichi di lavoro: articolo](../../../resource-mgmt/workload-balancer/workload-balancer.md) sezione.

## Stima i dati finanziari del progetto

Workfront calcolerà i costi pianificati per ogni attività e i costi complessivi per un progetto. I costi pianificati per un task includono tutte le spese del task più il costo del dipendente o del ruolo assegnato al task. Le tariffe orarie per il task, il ruolo e il dipendente vengono assegnate durante la creazione del task, del ruolo e dell&#39;utente.

Per informazioni sui dati finanziari del progetto, vedere la sezione [Finanze del progetto](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Determinare i punti di approvazione per il progetto

Creando i processi di approvazione in Workfront, è possibile stabilire punti di revisione per il progetto al fine di monitorare lo stato di avanzamento e le potenziali aree problematiche. Attraverso il processo di approvazione, i proprietari del progetto possono individuare le attività in ritardo e in anticipo, visualizzare audit trail in cui sono elencati gli utenti che hanno modificato lo stato di un’attività e visualizzare la cronologia dei problemi, tra cui il modo in cui sono stati risolti e quando sono stati chiusi. Dopo aver esaminato un progetto, i proprietari del progetto possono determinare quali passi intraprendere e aggiornare il piano del progetto, se necessario.

Per informazioni sulle approvazioni, consulta l’articolo [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Visualizza WBS

Per comprendere la struttura WBS di un progetto, è necessario visualizzare i seguenti elementi dell&#39;attività:

* Sequenza attività e sequenza temporale (date di inizio e completamento pianificate e durata attività)
* Dipendenze dei predecessori
* Relazione padre e figlio
* Assegnazioni

Una volta completato il WBS, è possibile visualizzarlo in un elenco di attività a livello di progetto o in un report.

* [Visualizzare il file WBS in un elenco di attività](#view-the-wbs-in-a-task-list)
* [Visualizzare WBS in un report attività](#view-the-wbs-in-a-task-report)

### Visualizzare il file WBS in un elenco di attività {#view-the-wbs-in-a-task-list}

È possibile visualizzare l&#39;elenco delle attività a livello di progetto.

1. Passare al progetto per il quale si desidera visualizzare la struttura funzionale.
1. Seleziona la **Attività** scheda.
1. (Facoltativo) Seleziona **Niente** nel **Raggruppamento** menu a discesa.

   Nella struttura Work Breakdown Structure (Suddivisione lavoro) non viene visualizzato il rientro delle attività nel WBS.

1. Dalla sezione **Visualizza** e selezionare il menu a discesa **Work Breakdown** visualizzazione.

   La struttura Work Breakdown (Suddivisione lavoro) viene visualizzata nella seconda colonna della vista selezionata.

   ![Work Breakdown Structure (Struttura di suddivisione del lavoro) in un elenco di attività](assets/work-breakdown-structure.png)

### Visualizzare WBS in un report attività {#view-the-wbs-in-a-task-report}

È possibile creare un report di attività e visualizzare il WBS delle attività eseguendo una delle operazioni seguenti:

* Applica al report la vista Work Breakdown Structure esistente.
* Aggiungi la colonna Work Breakdown Structure (Struttura di suddivisione del lavoro) a qualsiasi rapporto personalizzato.

>[!TIP]
>
>È consigliabile aggiungere un raggruppamento di progetti per chiarire a quali progetti appartengono le attività. Il rientro delle attività non viene visualizzato in un report attività.

Per informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Salvare il file WBS di un progetto come modello

Se si lavora su altri progetti che seguono pianificazioni di lavoro simili a quelle appena create, è possibile salvare il progetto come modello. Un modello consente di risparmiare tempo e fatica nella creazione di progetti correlati futuri.

Se l&#39;organizzazione ha poco fatturato, è consigliabile attendere fino a quando non vengono effettuate le assegnazioni utente per salvare il modello. Indipendentemente da quando un progetto viene salvato come modello, le assegnazioni utente o le attività specifiche possono essere rimosse durante l’associazione del modello a un nuovo progetto.

I seguenti elementi di una struttura funzionale di un progetto possono essere salvati in un modello per utilizzi futuri con un altro progetto:

* Dipendenze predecessore
* Assegnazioni (inclusi Proprietario progetto, Sponsor e Responsabile risorse)
* Processi di approvazione
* Vincoli attività
* Documenti
* Spese e altre informazioni finanziarie
* Obiettivi
* Tipi di Ora
* Struttura coda richieste
* Notifiche promemoria
* Rischi
* Tariffe di fatturazione
* Condivisione delle informazioni
* Moduli personalizzati

Per informazioni sul salvataggio dei progetti come modelli, consulta l’articolo [Crea modello da progetto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
