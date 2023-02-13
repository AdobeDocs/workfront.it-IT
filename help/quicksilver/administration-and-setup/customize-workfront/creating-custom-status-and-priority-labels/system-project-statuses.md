---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Stato del progetto di sistema
description: Workfront dispone di 9 stati di progetto di sistema incorporati. I primi 3 della tabella seguente sono obbligatori, il che significa che è possibile sbloccare, rinominare e riordinare i file, ma non è possibile nasconderli o eliminarli. La modifica dello stato di un progetto è in genere un processo manuale. Tuttavia, a volte lo stato di un progetto viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Stato del progetto di sistema

Workfront dispone di 9 stati di progetto di sistema incorporati.

I primi 3 della tabella seguente sono obbligatori, il che significa che è possibile sbloccare, rinominare e riordinare i file, ma non è possibile nasconderli o eliminarli.

La modifica dello stato di un progetto è in genere un processo manuale. Tuttavia, esistono alcuni scenari descritti nell’elenco seguente quando lo stato di un progetto viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.

Con l’istanza Workfront vengono forniti i seguenti stati del progetto:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Stato del progetto di sistema</th> 
   <th>Questo stato del progetto si verifica quando</th> 
   <th>Cosa succede in questo stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificazione (stato richiesto)</td> 
   <td> <p>Il project manager sta pianificando la cronologia del progetto, l'assegnazione delle attività e le approvazioni. Il project manager imposta manualmente questo stato su un progetto.</p> <p>Suggerimento: È consigliabile impostare lo stato predefinito per i nuovi progetti in Workfront su Planning. In qualità di amministratore di Workfront, puoi modificare lo stato predefinito di tutti i nuovi progetti nell’area Progetti di Preferenze progetto.</p> </td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto non compilano l’elenco di lavoro. Solo le approvazioni e gli elementi di lavoro accettati vengono visualizzati nell'Elenco di lavoro principale.</p> <p>Non vengono inviate notifiche mentre un progetto ha questo stato.</p> <p>Si consiglia di apportare tutte le modifiche che possono attivare un aggiornamento alla cronologia del progetto o qualsiasi modifica alle attività e alle assegnazioni dei problemi, mentre il progetto è nello stato Planning. Questo riduce al minimo la quantità di notifiche ricevute dagli utenti.</p> <p>La timeline del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Corrente (stato richiesto)</td> 
   <td> <p>Gli utenti ci stanno lavorando. Il project manager deve ruotare un progetto su Current per segnalare che è stato avviato.</p> <p>Questo è lo stato predefinito per i nuovi progetti in Workfront.</p> <p>Suggerimento: In qualità di amministratore di Workfront, puoi modificare lo stato predefinito per i nuovi progetti nell’area Progetti delle Preferenze progetto. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi che vengono loro assegnati nel progetto compilano il loro Elenco di lavoro. Possono iniziare ad accettare il lavoro su attività e problemi e spostarli nella loro lista di lavoro.</p> <p>Inoltre, in un progetto corrente, vengono inviate agli utenti del team di progetto tutte le notifiche sulle modifiche della timeline, le assegnazioni, le azioni necessarie e le approvazioni.</p> <p>La timeline del progetto viene calcolata automaticamente dal sistema, se Tipo di aggiornamento del progetto è impostata su Automatico, Al cambiamento o Automatico e Al cambiamento.</p> <p>Suggerimento: È consigliabile mantenere al minimo gli adeguamenti dei piani di progetto quando un progetto si trova in questo stato in modo che gli utenti non ricevano troppe notifiche.</p> </td> 
  </tr> 
  <tr> 
   <td>Completa (stato richiesto)</td> 
   <td> <p> Il progetto è completato:</p> 
    <ul> 
     <li> <p>Se la modalità di completamento del progetto è impostata su Manuale, il project manager sceglie questo stato manualmente per informare gli utenti del team del progetto che cesseranno di lavorare al progetto.</p> </li> 
    </ul> 
    <ul> 
     <li>Se la modalità di completamento del progetto è impostata su Automatico, Workfront contrassegna automaticamente un progetto come Completo quando tutte le attività e i problemi del progetto sono contrassegnati come Completi. </li> 
    </ul> <p><b>IMPORTANTE</b>: È possibile contrassegnare un progetto come Completo solo quando vengono risolte tutte le attività, i problemi e le approvazioni del progetto.</p> </td> 
   <td>
    <ul>
     <li>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi che vengono loro assegnati nel progetto non compilano le richieste di lavoro o gli elenchi di lavoro.</li>
     <li>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, cessano di essere inviate agli utenti del team di progetto. </li>
     <li>La timeline del progetto non viene più calcolata dal sistema.</li>
     <li>Impossibile copiare il progetto.</li>
    </ul><p>È possibile impedire agli utenti di eseguire azioni aggiuntive quando un progetto è contrassegnato come Completo. </p><p>Per ulteriori informazioni su come limitare le azioni sui progetti contrassegnati come completi, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Morto</td> 
   <td>Il progetto non è ancora finito, ma a causa dei blocchi stradali, o della modifica dell'ambito di applicazione, il progetto non può continuare a essere messo a punto ed è stato abbandonato. Il project manager modifica lo stato su Dead per avvisare gli utenti del team di progetto che questo progetto non verrà mai completato e che non dovrebbero più lavorarci.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto scompaiono dal relativo elenco di lavoro.</p> <p>Le decisioni di approvazione non possono essere concesse a compiti o problemi.</p> <p>Le notifiche relative a modifiche della timeline, assegnazioni, azioni necessarie, approvazioni non vengono inviate agli utenti del team di progetto.</p> <p>La tempistica del progetto non viene calcolata automaticamente dal sistema, in quanto il progetto viene percepito come completato.</p> <p>È possibile impedire agli utenti di eseguire determinate azioni quando un progetto è contrassegnato come morto. Per ulteriori informazioni su come limitare le azioni sui progetti Dead, vedi <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>In sospeso</td> 
   <td>Il progetto non è ancora finito, ma a causa di alcuni ritardi, il progetto deve essere temporaneamente sospeso. Il project manager sceglie di utilizzare questo stato per avvisare gli utenti del team del progetto di interrompere il lavoro sul progetto, al momento attuale.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto scompaiono dal relativo elenco di lavoro. </p> <p>Le decisioni di approvazione non possono essere concesse a compiti o problemi.</p> <p>Le notifiche relative a modifiche della timeline, assegnazioni, azioni necessarie, approvazioni non vengono inviate agli utenti del team di progetto.</p> <p> <p><b>NOTA</b>: Quando si inserisce un progetto in blocco, la timeline del progetto non si interrompe. Il progetto può ancora essere mostrato come a rischio o in difficoltà anche se nessuno sta lavorando attivamente al progetto. È possibile che siano necessarie alcune regolazioni manuali delle date delle altre attività aperte quando si ripristina il progetto su Corrente, in modo che il progetto possa mostrare lo stato di avanzamento aggiornato.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Richiesto</td> 
   <td>Lo stato del progetto viene contrassegnato automaticamente come Richiesto dal sistema, quando il business case su una richiesta di progetto è stato completato e inviato per l’approvazione. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un business case, vedi <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisione dei progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi relativi al progetto a loro assegnato non compilano l’elenco di lavoro.</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La timeline del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Approvato</td> 
   <td>Lo stato del progetto viene contrassegnato automaticamente come Approvato, quando il business case su una richiesta di progetto è stato approvato. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un business case, vedi <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisione dei progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto non compilano l’elenco di lavoro.</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La timeline del progetto non viene calcolata automaticamente dal sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>Rifiutato</td> 
   <td>Lo stato del progetto viene contrassegnato automaticamente come Rifiutato, quando il business case su una richiesta di progetto viene rifiutato. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un business case, vedi <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisione dei progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto non compilano l’elenco di lavoro.</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La timeline del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>Lo stato del progetto viene contrassegnato automaticamente come Idea quando si invia una richiesta di progetto. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un business case, vedi <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisione dei progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati al progetto non compilano l’elenco di lavoro.</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La timeline del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Non è possibile modificare i seguenti stati del progetto in uno stato Dead, On Hold o Complete:
>
>* Richiesto
>* Idea
>* Approvato
>* Rifiutato (o equivalente)
>

