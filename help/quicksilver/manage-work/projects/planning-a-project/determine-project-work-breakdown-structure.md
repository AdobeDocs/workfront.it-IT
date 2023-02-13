---
product-area: projects
navigation-topic: plan-a-project
title: Determinare la struttura di suddivisione del lavoro in un progetto
description: La definizione di una struttura di suddivisione del lavoro (WBS, Work Breakdown Structure) per un progetto è un insieme di attività che in ultima analisi delineano il piano di progetto. Il WBS suddivide il risultato del progetto in elementi di lavoro gestibili, che possono essere utilizzati per definire le fasi cardine e organizzare le assegnazioni di lavoro.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 1%

---

# Determinare la struttura di suddivisione del lavoro in un progetto

La definizione di una struttura di suddivisione del lavoro (WBS, Work Breakdown Structure) per un progetto è un insieme di attività che in ultima analisi delineano il piano di progetto. Il WBS suddivide il risultato del progetto in elementi di lavoro gestibili, che possono essere utilizzati per definire le fasi cardine e organizzare le assegnazioni di lavoro.

Per creare la struttura di suddivisione del lavoro di un progetto, è necessario disporre di una licenza Piano con accesso Modifica a progetti. Potrebbe essere necessario un accesso aggiuntivo ad altre aree di Adobe Workfront, a seconda del numero di attività che esegui durante la creazione del WBS.

È consigliabile mantenere il progetto in uno stato di pianificazione mentre si apportano modifiche alla struttura di suddivisione del lavoro, per evitare notifiche di attivazione agli utenti del team di progetto.

## Definire i risultati finali del progetto

Lo scopo di un progetto è quello di fornire risultati tangibili alle parti interessate interne ed esterne. I risultati finali di un progetto sono i risultati che desideri raggiungere completando il progetto. I risultati sono quasi sempre associati ad almeno un risultato finale e tutti i risultati finali devono essere associati a un progetto.

I risultati finali del progetto possono essere beni di consumo, output intellettuale (ad esempio, rapporti) o servizi. Ad esempio, se l’ambito del progetto è quello di creare una casa, alcuni dei risultati finali possono includere:

* creazione di piani architettonici
* completamento dell&#39;impianto idraulico
* lavori elettrici
* versando la fondazione
* intelaiatura
* chiusura della vendita della casa.

A seconda delle dimensioni e dell’ambito, un progetto può essere costituito da più risultati finali.

Una volta identificati i risultati finali, puoi iniziare a suddividerli in attività. Le attività sono l’output ottenuto per fornire il risultato complessivo del progetto. Quando definisci le attività, prendi in considerazione i seguenti parametri:

* Quantità di tempo necessario per il completamento.
* Budget necessario per completare il lavoro.
* Risorse necessarie per completare il lavoro.
* Pianificazione delle risorse in base alla cronologia logica delle attività.

Quando definisci le attività, assicurati di non pianificare troppo lavoro per una singola attività. Se il lavoro richiesto per un&#39;attività è superiore a 40 ore (una settimana di lavoro tipica), potrebbe essere necessario suddividere tale quantità di lavoro nelle sottoattività. Il completamento di tutte le sottoattività completerà quindi l’attività principale.

Per definire i risultati WBS e i risultati finali in Workfront, si consiglia di eseguire le seguenti attività per creare una visualizzazione gerarchica delle attività del progetto:

* Se non lo hai già fatto, crea un nuovo progetto.\
   Per informazioni sulla creazione di un progetto, consulta l’articolo [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

* Crea attività per tutti gli elementi di azione necessari per completare ogni risultato e risultato finale.\
   Per informazioni sulla creazione delle attività, consulta l’articolo [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* Dalle attività appena create, individua quali sono i principali risultati e associali alle fasi cardine.\
   Per informazioni sulla creazione di attività cardine, vedere gli articoli [Creare un percorso cardine](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associa milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Suddividere le attività con un ambito troppo grande in sottoattività. Associali all&#39;elemento padre che definisce il risultato finale .\
   Per informazioni sulla creazione delle sottoattività, consulta l’articolo [Creare sottoattività](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identificare le relazioni di dipendenza tra le sottoattività e tra le fasi cardine.\
   In una relazione di dipendenza, l&#39;inizio di un&#39;attività dipende dal completamento di un&#39;altra attività o gruppo di attività.\
   Per informazioni sulle dipendenze delle attività, vedere gli articoli [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) e [Creare una relazione predecessore nell&#39;elenco delle attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Determinare se in un qualsiasi momento della durata del progetto sono necessarie approvazioni e revisioni. Crea processi di approvazione per soddisfare questa esigenza.\
   Per informazioni sulle approvazioni, consulta l’articolo [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Stimare la pianificazione del lavoro e i vincoli di pianificazione

Una volta creata la fase cardine e la struttura delle attività di base del progetto, è possibile stimare il tempo necessario per completare il progetto complessivo definendo vincoli e durate delle attività.

Considera quanto segue:

* I vincoli task definiscono quando il lavoro su un&#39;attività deve iniziare o terminare.

   Per informazioni sulla definizione dei vincoli dell&#39;attività, vedere l&#39;articolo [Panoramica sul vincolo di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La durata di un&#39;attività corrisponde al periodo di tempo disponibile per il completamento di un&#39;attività. Quando si calcola la durata, è possibile inserire un valore che tenga conto della possibilità di un ritardo. Se in passato sono stati completati progetti simili, è possibile avere una buona idea su dove impostare questo valore.

   Poiché la durata è una stima, assicurarsi di impostare valori di tempo ottimistici per tenere conto di fattori che potrebbero influenzare il compito, come il tempo atmosferico, le interruzioni di corrente, le difficoltà del fornitore o altri eventi imprevisti. Inoltre, verificare se sono presenti attività predecessori o di dipendenza associate e come possono creare vincoli sul lavoro e influire sul completamento delle attività.

   A seconda del tipo di durata dell’attività, è possibile modificare la durata di un’attività durante la durata di un progetto, ma questo influisce anche sulla timeline del progetto. Per informazioni sulla durata di un&#39;attività, vedere l&#39;articolo [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Assegnare le attività

Dopo aver definito la durata e i vincoli di ogni attività, è possibile determinare chi dispone del tempo e delle competenze necessarie per eseguire il lavoro. In Workfront è possibile assegnare attività alle seguenti entità:

* Utenti\
   È possibile assegnare alle attività solo gli utenti con un livello di accesso Planner o Worker. Sebbene sia possibile assegnare le attività a Richiedenti e Revisori, questi non possono completarle. Per questo motivo, sconsigliamo di assegnare loro attività.

   Per informazioni sui livelli di accesso e su come definiscono le operazioni che gli utenti possono eseguire con gli oggetti Workfront, consultare [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Ruoli
* Team

Per informazioni sull&#39;assegnazione delle attività, vedere gli articoli nella sezione [Assegnare le attività](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) sezione .

## Gestione delle risorse

Gestione delle risorse in Workfront consente di determinare se il progetto dispone di personale adeguato. Quando gli utenti vengono aggiunti a un progetto, Workfront mostra l’utilizzo di ogni utente. I responsabili risorse possono vedere il numero totale di ore che la persona viene assegnata ad altri progetti durante l&#39;intervallo di tempo del progetto.

>[!NOTE]
>
>Se il progetto ha uno stato di Planning, le attività assegnate agli utenti non vengono visualizzate negli elenchi delle attività.

All&#39;inizio di un anno fiscale o di un trimestre, è possibile gestire le risorse a un livello più alto, in più progetti, senza conoscere una specifica struttura di suddivisione del lavoro.\
Per informazioni sulla pianificazione dell’utilizzo delle risorse a un livello più elevato, consulta l’articolo [Guida introduttiva alla pianificazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Quando gestisci le risorse nel contesto della creazione della struttura di suddivisione del lavoro di un progetto e assicurati che ogni attività sia assegnata alla risorsa corretta, puoi pianificare le risorse per il lavoro da eseguire.\
Per informazioni sulla pianificazione delle risorse, consulta gli articoli nella sezione [Pianificazione delle risorse](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md) sezione .

## Stimare le finanze del progetto

Workfront calcolerà i costi pianificati per ciascuna attività e i costi complessivi di un progetto. I costi pianificati per un&#39;attività includono tutte le spese dell&#39;attività più il costo del dipendente o del ruolo assegnato all&#39;attività. Le tariffe orarie per l&#39;attività, il ruolo e il dipendente vengono assegnati durante la creazione di attività, ruoli e utenti.

Per informazioni sulle finanze dei progetti, consulta la sezione [Finanziamento del progetto](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Determinare i punti di approvazione per il progetto

Creando i processi di approvazione in Workfront, è possibile stabilire punti di revisione per il progetto al fine di monitorare l&#39;avanzamento e le potenziali aree problematiche. Attraverso il processo di approvazione, i proprietari dei progetti possono individuare le attività in ritardo e in anticipo, visualizzare i percorsi di controllo in cui sono elencati gli utenti che hanno modificato lo stato di un&#39;attività e visualizzare le cronologie dei problemi, incluse le modalità di risoluzione dei problemi e la loro chiusura. Al momento della revisione di un progetto, i proprietari del progetto possono determinare quali passi intraprendere e aggiornare il piano di progetto, se necessario.

Per informazioni sulle approvazioni, consulta l’articolo [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Visualizza il tuo WBS

Per comprendere il WBS di un progetto, è necessario visualizzare i seguenti elementi dell&#39;attività:

* Sequenza e timeline delle attività (date di inizio e completamento pianificate e durata delle attività)
* Dipendenze predecessori
* Relazione figlio e padre
* Assegnazioni

Una volta completato il WBS, è possibile visualizzarlo in un elenco di attività a livello di progetto o in un rapporto.

* [Visualizzazione del WBS in un elenco di attività](#view-the-wbs-in-a-task-list)
* [Visualizzazione del WBS in un report attività](#view-the-wbs-in-a-task-report)

### Visualizzazione del WBS in un elenco di attività {#view-the-wbs-in-a-task-list}

È possibile visualizzare l&#39;elenco delle attività a livello di progetto.

1. Passa al progetto per il quale desideri visualizzare la Struttura di suddivisione del lavoro.
1. Seleziona la **Attività** scheda .
1. (Facoltativo) Seleziona **Niente** in **Raggruppamento** menu a discesa.

   La struttura di suddivisione del lavoro non visualizza il rientro delle attività nel WBS.

1. Da **Visualizza** dal menu a discesa e seleziona il **Suddivisione del lavoro** visualizza.

   La struttura Suddivisione lavoro viene visualizzata nella seconda colonna della vista selezionata.

   ![](assets/wbs-view-on-task-list-nwe-350x87.png)

### Visualizzazione del WBS in un report attività {#view-the-wbs-in-a-task-report}

È possibile creare un report attività e visualizzare il WBS delle attività eseguendo una delle operazioni seguenti:

* Applicare al rapporto la vista Struttura di suddivisione del lavoro esistente.
* Aggiungi la colonna Struttura di suddivisione del lavoro a qualsiasi rapporto personalizzato.

>[!TIP]
>
>È consigliabile aggiungere un raggruppamento di progetti per chiarire a quali progetti appartengono le attività. Il rientro delle attività non viene visualizzato in un rapporto delle attività.

Per informazioni sulla creazione dei rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Salvare come modello WBS di un progetto

Se si lavora su altri progetti che seguono programmi di lavoro simili a quelli creati in precedenza, è possibile salvare il progetto come modello. Un modello consente di risparmiare tempo e fatica nella creazione di progetti correlati futuri.

Se l&#39;azienda ha un fatturato ridotto, è consigliabile attendere che, dopo aver effettuato le assegnazioni, il modello venga salvato. A prescindere da quando un progetto viene salvato come modello, le assegnazioni utente o le attività specifiche possono essere rimosse durante l&#39;associazione del modello a un nuovo progetto.

I seguenti elementi di una struttura di suddivisione del lavoro possono essere salvati in un modello, per un utilizzo futuro con un altro progetto:

* Dipendenze predecessori
* Assegnazioni (inclusi Proprietario progetto, Sponsor e Gestione risorse)
* Processi di approvazione
* Vincoli attività
* Documenti
* Spese e altre informazioni finanziarie
* Obiettivi
* Tipi di Ora
* Struttura della coda richieste
* Notifiche promemoria
* Rischi
* Tariffe di fatturazione
* Condivisione delle informazioni
* Moduli personalizzati

Per informazioni sul salvataggio dei progetti come modelli, consulta l’articolo [Crea modello da progetto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
