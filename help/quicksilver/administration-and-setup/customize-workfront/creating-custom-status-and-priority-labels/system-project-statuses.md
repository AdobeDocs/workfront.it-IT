---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Panoramica degli stati dei progetti di sistema
description: Workfront dispone di 9 stati di progetto di sistema incorporati. Le prime 3 nella tabella seguente sono obbligatorie, il che significa che è possibile sbloccarle, rinominarle e riordinarle, ma non è possibile nasconderle o eliminarle. La modifica dello stato di un progetto è in genere un processo manuale. Tuttavia, a volte lo stato di un progetto viene modificato automaticamente, a seconda di altre attività che si verificano nel sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 0%

---

# Panoramica degli stati dei progetti di sistema

<!--Audited: 12/2023-->

Workfront dispone di 9 stati di progetto di sistema incorporati.

Le prime 3 nella tabella seguente sono obbligatorie, il che significa che è possibile sbloccarle, rinominarle e riordinarle, ma non è possibile nasconderle o eliminarle.

La modifica dello stato di un progetto è in genere un processo manuale. Tuttavia, esistono alcuni scenari descritti nell’elenco seguente quando lo stato di un progetto viene modificato automaticamente, a seconda di altre attività che si verificano nel sistema.

Con l’istanza di Adobe Workfront, Workfront fornisce i seguenti stati del progetto:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Stato progetto di sistema</th> 
   <th>Questo stato del progetto si verifica quando</th> 
   <th>Cosa succede in questo stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pianificazione (stato obbligatorio)</td> 
   <td> <p>Il project manager sta pianificando la sequenza temporale del progetto, l'assegnazione delle attività e le approvazioni. Il project manager imposta questo stato manualmente su un progetto.</p> <p><b>SUGGERIMENTO</p> <p> È consigliabile impostare su Planning lo stato predefinito per i nuovi progetti in Workfront. In qualità di amministratore di Workfront, puoi modificare lo stato predefinito di tutti i nuovi progetti nell’area Progetti di Preferenze progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configurare le preferenze di progetto a livello di sistema</a>.</p></td> 
   <td> <p>Per impostazione predefinita (senza un filtro personalizzato), gli utenti del team di progetto possono visualizzare il progetto nei propri elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto non popolano il loro Work List (Elenco di lavoro). Nella sezione Elenco lavori dell’area Home vengono visualizzate solo le approvazioni e gli elementi di lavoro accettati.</p> <p>Quando un progetto è in questo stato, non viene inviata alcuna notifica.</p> <p>È consigliabile apportare tutte le modifiche che possono attivare un aggiornamento della sequenza temporale del progetto o qualsiasi modifica alle attività e alle assegnazioni dei problemi mentre il progetto è nello stato Pianificazione. In questo modo si riduce al minimo il numero di notifiche ricevute dagli utenti.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Corrente (stato obbligatorio)</td> 
   <td> <p>Gli utenti lavorano alle attività e ai problemi del progetto. Il project manager deve impostare un progetto su Corrente per segnalare che è stato avviato.</p> <p>Questo è lo stato predefinito per i nuovi progetti in Workfront.</p> <p><b>SUGGERIMENTO</b></p>

<p> In qualità di amministratore di Workfront, puoi modificare lo stato predefinito dei nuovi progetti nell’area Progetti di Preferenze progetto. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </td> 
   <td> <p>Per impostazione predefinita (senza un filtro personalizzato), gli utenti del team di progetto possono visualizzare il progetto nei propri elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto popolano il loro Work List (Elenco di lavoro). Possono iniziare ad accettare il lavoro su attività e problemi e spostarli nel loro elenco Lavori in corso.</p> <p>In un progetto corrente, tutte le notifiche relative a modifiche della sequenza temporale, assegnazioni, azioni necessarie e approvazioni vengono inviate agli utenti del team del progetto.</p> <p>La linea temporale del progetto viene calcolata automaticamente dal sistema, se il tipo di aggiornamento del progetto è impostato su Automatico, Su modifica o Automatico e Su modifica.</p> <p><b>SUGGERIMENTO</b></p> <p> È consigliabile ridurre al minimo le modifiche apportate al piano di progetto quando un progetto è in questo stato, in modo che gli utenti non ricevano troppe notifiche.</p> </td> 
  </tr> 
  <tr> 
   <td>Completo (stato obbligatorio)</td> 
   <td> <p> Tutte le attività e i problemi del progetto sono completati e il progetto è completato.</p> 
     <p>Se la Modalità di completamento del progetto è impostata su Manuale, il project manager sceglie questo stato manualmente per informare gli utenti del team di progetto di interrompere il lavoro sul progetto.</p> 
    <p>Se la Modalità di completamento del progetto è impostata su Automatico, Workfront contrassegna automaticamente un progetto come Completato quando tutte le attività e i problemi del progetto sono contrassegnati come Completati. 
    <p><b>IMPORTANTE</b> </p>
    <p>È possibile contrassegnare un progetto come Completo solo quando vengono risolte tutte le attività, i problemi e le approvazioni relativi al progetto.</p> </td> 
   <td>
    <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto non popolano le loro richieste di lavoro o gli elenchi Lavori su. </p>
    <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, cessano di essere inviate agli utenti del team di progetto.</p>
    <p>La sequenza temporale del progetto non viene più calcolata dal sistema. </p>
    <p>Impossibile copiare il progetto.</p>
    <p>È possibile impedire agli utenti di eseguire azioni aggiuntive quando un progetto è contrassegnato come Completato. </p><p>Per ulteriori informazioni su come limitare le azioni sui progetti contrassegnati come Completati, vedi <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Morto</td> 
   <td>Il progetto non è ancora terminato, ma a causa di blocchi stradali o di cambiamenti di portata, il progetto non può continuare a essere elaborato ed è stato abbandonato. Il project manager imposta lo stato su Inattivo per avvisare gli utenti del team che il progetto non verrà mai completato e che non dovrebbero più lavorarci.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto scompaiono dal loro Work List (Elenco di lavoro).</p> <p>Le decisioni di approvazione non possono essere concesse ad attività o problemi.</p> <p>Le notifiche relative a modifiche della sequenza temporale, assegnazioni, azioni necessarie e approvazioni non vengono inviate agli utenti del team di progetto.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema, in quanto il progetto viene percepito come completato.</p> <p>Puoi impedire agli utenti di eseguire determinate azioni quando un progetto è contrassegnato come Inattivo. Per ulteriori informazioni su come limitare le azioni sui progetti inattivi, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>In sospeso</td> 
   <td>Il progetto non è ancora terminato, ma a causa di alcuni ritardi, deve essere temporaneamente sospeso. Il project manager sceglie di utilizzare questo stato per avvisare gli utenti del team di progetto di interrompere il lavoro sul progetto al momento.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto scompaiono dal loro Work List (Elenco di lavoro). </p> <p>Le decisioni di approvazione non possono essere concesse ad attività o problemi.</p> <p>Le notifiche relative a modifiche della sequenza temporale, assegnazioni, azioni necessarie e approvazioni non vengono inviate agli utenti del team di progetto.</p> <p> <p><b>NOTA</b></p>  <p>Quando si blocca un progetto, la sequenza temporale del progetto non si interrompe. Il progetto può ancora essere visualizzato come A rischio o In difficoltà anche se nessuno sta lavorando attivamente al progetto. Quando si ripristina il progetto su Corrente, potrebbe essere necessario apportare alcune modifiche manuali alle date delle attività aperte rimanenti, in modo che il progetto possa mostrare lo stato di avanzamento aggiornato.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Richiesto</td> 
   <td>Lo stato del progetto viene automaticamente contrassegnato come Richiesto dal sistema, quando il business case su una richiesta di progetto è stato completato e inviato per l'approvazione. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un caso di business, consulta <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Esamina progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi del progetto assegnati non popolano il proprio Work List (Elenco di lavoro).</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Approvato</td> 
   <td>Lo stato del progetto viene automaticamente contrassegnato come Approvato, quando il business case su una richiesta di progetto è stato approvato. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un caso di business, consulta <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Esamina progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita (senza un filtro personalizzato), gli utenti del team di progetto possono visualizzare il progetto nei propri elenchi Progetti nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto non popolano il loro Work List (Elenco di lavoro).</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>Rifiutato</td> 
   <td>Lo stato del progetto viene automaticamente contrassegnato come Rifiutato quando il business case su una richiesta di progetto è stato rifiutato. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un caso di business, consulta <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Esamina progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto non popolano il loro Work List (Elenco di lavoro).</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>Lo stato del progetto viene automaticamente contrassegnato come Idea quando si invia una richiesta di progetto, prima di completare il Business Case. Per ulteriori informazioni sulla richiesta di un progetto utilizzando un caso di business, consulta <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Esamina progetti richiesti</a>.</td> 
   <td> <p>Per impostazione predefinita, gli utenti del team di progetto non possono visualizzare il progetto negli elenchi Progetti (senza un filtro personalizzato) nell’area Progetti di Workfront. Le attività e i problemi assegnati a loro nel progetto non popolano il loro Work List (Elenco di lavoro).</p> <p>Tutte le notifiche relative al progetto, ad eccezione di una notifica di modifica dello stato, non vengono inviate ad alcun utente.</p> <p>La sequenza temporale del progetto non viene calcolata automaticamente dal sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>I seguenti stati del progetto non possono essere modificati in Dead (Inattivo), On Hold (In sospeso) o Complete (Completato):
>
>* Richiesto
>* Idea
>* Approvato
>* Rifiutato (o equivalente)
>
