---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 'Miglioramenti alla gestione delle risorse 2020.2: il Bilanciatore dei carichi di lavoro'
description: Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 2020.2 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# Miglioramenti alla gestione delle risorse 2020.2: il Bilanciatore dei carichi di lavoro

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 2020.2 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.2, consulta [Panoramica sulla versione 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Le persone sono una risorsa di livello 1. Con il Bilanciatore dei carichi di lavoro, puoi proteggerli dall’esaurimento e metterli in grado di svolgere al meglio il loro lavoro, allineandoli al contempo alle strategie aziendali chiave. Presentazione di un&#39;esperienza di pianificazione riprogettata che consente di visualizzare e gestire i carichi di lavoro e le richieste delle persone nella stessa visualizzazione. L’interfaccia utente fornisce una chiara mappatura visiva di sovrautilizzo e sottoutilizzo ed è trasparente per tutte le parti interessate. I responsabili delle persone possono utilizzare tali informazioni come input e dalla stessa schermata ribilanciare lo sforzo attraverso la timeline, che si riflette poi nel resto della piattaforma Workfront.

>[!NOTE]
>
>Il Bilanciatore dei carichi di lavoro ha iniziato a essere rilasciato come versione beta con la versione 2019.4. Tutti i miglioramenti al Bilanciatore dei carichi di lavoro sono generalmente disponibili con la versione 2020.2. I miglioramenti descritti in questa pagina sono stati aggiunti con la versione 2020.2 di. Per una panoramica del Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Regolare l’allocazione giornaliera e settimanale nel Bilanciatore dei carichi di lavoro

Per evitare il burnout delle risorse, ora puoi regolare l’allocazione giornaliera e settimanale degli utenti in modo che funzioni utilizzando il Bilanciatore dei carichi di lavoro.

Prima di questo miglioramento, questo era possibile solo utilizzando gli strumenti di pianificazione delle risorse.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Filtri del Bilanciatore dei carichi di lavoro

Per rendere rilevanti le informazioni nel Bilanciatore dei carichi di lavoro, ora puoi creare filtri sia per l’area Lavoro non assegnato che per l’area Lavoro assegnato del Bilanciatore dei carichi di lavoro e salvarli per utilizzi futuri. Puoi quindi modificare la versione salvata per apportarvi piccole modifiche, anziché iniziare da zero con un nuovo filtro.

Per informazioni sul filtro nel Bilanciatore dei carichi di lavoro, vedi [Gestire i filtri nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Mostra le ore rimanenti nel Bilanciatore dei carichi di lavoro

Per facilitare le decisioni corrette in merito alle assegnazioni, una nuova impostazione consente ora di visualizzare la differenza di ore tra le ore che un utente è disponibile a lavorare in base alla propria pianificazione e le ore che è già stato assegnato al lavoro (le ore rimanenti). La nuova impostazione è ora disponibile nel Bilanciatore dei carichi di lavoro.

Per informazioni sulla visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro, vedi [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o se utilizzi Adobe Workfront Classic, vedi [Navigare nel Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront

## Mostra le ore pianificate giornaliere per attività e progetti nell’area Lavoro non assegnato del Bilanciatore dei carichi di lavoro

Per comprendere in che modo le attività influiranno sul carico di lavoro degli utenti prima di assegnarli, l’impostazione &quot;Show allocations&quot; (Mostra allocazioni) ora gestisce le informazioni visualizzate nell’area Unassigned Work (Lavoro non assegnato) del bilanciatore dei carichi di lavoro. Quando questa impostazione è abilitata, le ore pianificate sia per le attività che per i progetti vengono visualizzate nell’area Lavoro non assegnato del Bilanciatore dei carichi di lavoro.

Prima di questa modifica, questa impostazione aggiornava solo le informazioni nell’area Lavoro assegnato del Bilanciatore.

Per informazioni sull&#39;esplorazione del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Navigare nel Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront (precedentemente disponibile solo per le attività)

## Nuova casella Impostazioni per il Bilanciatore dei carichi di lavoro

Per semplificare l’esperienza, ora è disponibile una casella Impostazioni che mostra strumenti aggiuntivi per aggiornare la visualizzazione nel Bilanciatore dei carichi di lavoro. Questa casella include le impostazioni seguenti:

* Gruppo per progetto
* Visualizza le ore allocate o le ore rimanenti per le attività e i progetti.

Per informazioni sulla visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro, vedi [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (o se utilizzi Adobe Workfront Classic, vedi [Navigare nel Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home).).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Condividere il Bilanciatore dei carichi di lavoro con un collegamento

Ora puoi condividere il carico di lavoro delle tue persone con dirigenti in modo che possano contestualizzare le tue esigenze di personale. Per questo, ora puoi condividere il Bilanciatore dei carichi di lavoro condividendo un URL univoco con chiunque altro.

Per informazioni sull&#39;esplorazione del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Navigare nel Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Modificare l’intervallo di date nel Bilanciatore dei carichi di lavoro

Per personalizzare ulteriormente la durata della timeline del Bilanciatore dei carichi di lavoro in base alle tue esigenze, ora puoi selezionare un periodo personalizzato di 2, 4 o 6 settimane da visualizzare contemporaneamente.

Prima di questo miglioramento, il Bilanciatore dei carichi di lavoro visualizzava sempre le informazioni a partire dalla settimana corrente.

Per informazioni sull&#39;esplorazione del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Navigare nel Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront (precedentemente disponibile)

## Lo spostamento e la copia delle attività in un altro progetto mantengono il vincolo attività quando le attività possono rientrare nella sequenza temporale del progetto

È stato migliorato il modo in cui Workfront gestisce il vincolo attività specifico per data di un&#39;attività quando questa viene copiata o spostata in un altro progetto. Esempi di vincoli attività specifici per data sono Deve iniziare il, Deve finire il, Date fisse, Inizia non dopo il e così via.

Quando ad esempio si sposta o si copia un&#39;attività con un vincolo Deve iniziare il in un altro progetto la cui Data inizio pianificata è precedente alla Data inizio dell&#39;attività, l&#39;attività mantiene il vincolo dopo che è stata copiata o spostata. Quando si sposta o si copia un&#39;attività con un vincolo Deve iniziare il in un progetto la cui Data inizio pianificata è successiva alla Data inizio dell&#39;attività, il vincolo attività viene impostato su Il più presto possibile.

Prima di questa modifica, il vincolo dell’attività diventa sempre Appena possibile.

Per informazioni sullo spostamento delle attività, vedi [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md) (o se utilizzi Adobe Workfront Classic, vedi [Spostamento delle attività](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

Per informazioni sulla copia delle attività, vedere [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Copiare e duplicare le attività](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

Per una panoramica di tutti i vincoli di attività, vedere [Panoramica dei vincoli di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (o se si utilizza Adobe Workfront Classic, vedere [Panoramica dei vincoli di attività](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Impedire la perdita di dati durante l&#39;esecuzione di modifiche nella scheda Dettagli o in un elenco di attività

Per evitare la perdita di dati durante l&#39;aggiornamento manuale delle informazioni nella pagina Dettagli di un oggetto o di attività in un elenco di attività a livello di progetto, quando si salvano le modifiche viene visualizzato un messaggio di avvertenza per segnalare che sono presenti modifiche non salvate prima di tentare di modificare le informazioni nell&#39;intestazione. Le uniche azioni consentite prima di salvare le modifiche sono la sottoscrizione o l&#39;aggiunta dell&#39;oggetto ai preferiti.

Per informazioni sulla modifica delle attività in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront

## Creare processi di approvazione per gruppi utilizzando stati personalizzati

Per facilitare la gestione dei propri flussi di lavoro univoci da parte dei gruppi, è ora possibile utilizzare gli stati personalizzati specifici dei gruppi nei processi di approvazione.

In precedenza, un gruppo non poteva utilizzare i propri stati personalizzati con i propri processi di approvazione specifici per gruppo. Erano disponibili solo gli stati a livello di sistema, che non sempre rientravano nei processi di approvazione di gruppo.

Gli stati personalizzati possono essere utilizzati ora nei processi di approvazione a uso singolo e a livello di sistema:

* Crea un processo di approvazione a utente singolo per un oggetto (progetto, attività o problema) e basalo sugli stati associati al gruppo che lavora su tale oggetto. Questo include eventuali stati personalizzati associati al gruppo.
* Crea un processo di approvazione globale e rendilo disponibile solo per il gruppo o per tutti gli utenti del sistema.

Per gli utenti con accesso amministrativo ai processi di approvazione, le informazioni sulla configurazione dei processi di approvazione sono disponibili in [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (o se si utilizza Adobe Workfront Classic, vedere [Creazione di processi di approvazione](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

Per gli utenti, le informazioni sull&#39;associazione dei processi di approvazione agli elementi di lavoro sono disponibili in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (oppure se si utilizza Adobe Workfront Classic, vedere [Associazione di un processo di approvazione nuovo o esistente al lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/home)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Un modo più pratico per aggiornare le allocazioni nel Bilanciatore dei carichi di lavoro

Per semplificare la gestione delle allocazioni di un utente a un elemento di lavoro nel Bilanciatore dei carichi di lavoro, è ora possibile fare doppio clic sull’elemento di lavoro. È inoltre possibile utilizzare l&#39;opzione di menu Modifica allocazioni esistente. Inoltre, non è più necessario abilitare la visualizzazione delle allocazioni per poterle aggiornare.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Aggiornare le ore pianificate per l’attività nel Bilanciatore dei carichi di lavoro

>[!NOTE]
>
>Questo miglioramento sarà disponibile in produzione subito dopo la versione 2020.2.

Una nuova opzione nell’area Gestione risorse del livello di accesso ora consente agli utenti con questo livello di accesso di modificare le Ore pianificate dal Bilanciatore dei carichi di lavoro. Quando si modificano le allocazioni nel Bilanciatore dei carichi di lavoro, il totale delle allocazioni giornaliere non deve necessariamente corrispondere al numero di ore pianificate delle attività. Una volta salvate le allocazioni, il totale delle ore di allocazione diventerà le ore pianificate dell&#39;attività. Ciò è possibile solo per le attività con un tipo di durata semplice.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Per informazioni sulla concessione dell&#39;accesso a Gestione risorse, vedere [Concedere l&#39;accesso a Gestione risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Rimozione dell’etichetta &quot;beta&quot; dal bilanciatore dei carichi di lavoro

Con la versione 2020.2, il Bilanciatore dei carichi di lavoro non sarà più in uno stato beta e potrai utilizzare il Bilanciatore delle risorse per rivedere e gestire le assegnazioni e le allocazioni delle risorse. L’etichetta &quot;beta&quot; è stata rimossa nell’ambiente di anteprima. La stessa modifica verrà apportata con la versione di produzione 20.2. Per informazioni sul Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
