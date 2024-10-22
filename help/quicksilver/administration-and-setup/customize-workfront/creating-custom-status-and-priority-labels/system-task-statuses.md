---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Stati attività di sistema
description: I tre stati delle attività di sistema incorporati in Workfront sono obbligatori e consentono di sbloccarli, rinominarli e riordinarli, ma non di nasconderli o eliminarli. È inoltre possibile aggiungere nuovi stati delle attività di sistema in base alle esigenze dell'organizzazione. La modifica dello stato di un'attività è in genere un processo manuale, ma a volte lo stato di un'attività viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Stati attività di sistema

I tre stati delle attività di sistema incorporati in Workfront sono obbligatori e consentono di sbloccarli, rinominarli e riordinarli, ma non di nasconderli o eliminarli.

È inoltre possibile aggiungere nuovi stati delle attività di sistema in base alle esigenze dell&#39;organizzazione.

La modifica dello stato di un&#39;attività è in genere un processo manuale. Tuttavia, ci sono momenti descritti nel seguente elenco quando lo stato di un&#39;attività viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.

Nell’istanza di Workfront vengono forniti i seguenti stati delle attività:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Stato attività di sistema</th> 
   <th>Quando si verifica questo stato</th> 
   <th>Azioni che si verificano quando un'attività si trova in questo stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuovo (stato obbligatorio)</td> 
   <td>Questo è lo stato predefinito per ogni nuova attività creata.</td> 
   <td>Se l'attività si trova in un progetto con lo stato Corrente, l'attività viene visualizzata nella scheda Richieste di lavoro degli utenti assegnati alle attività. Gli utenti possono ora iniziare a lavorare sull’attività.</td> 
  </tr> 
  <tr> 
   <td>In corso (stato obbligatorio)</td> 
   <td>È possibile inserire un'attività in questo stato per indicare che il lavoro su tale attività è iniziato.</td> 
   <td> <p>Quando si contrassegna un'attività come In corso, viene visualizzato un valore per Data di inizio effettiva.</p> <p>L'avanzamento dell'attività viene registrato solo dopo l'aggiornamento manuale della percentuale di completamento dell'attività.</p> </td> 
  </tr> 
  <tr> 
   <td>Completo (stato obbligatorio)</td> 
   <td> <p>È possibile contrassegnare manualmente un'attività come completata al completamento del relativo lavoro.</p> <p>Quando la Modalità di registrazione di un'attività è impostata su Completamento automatico, l'attività viene automaticamente contrassegnata come Completata quando raggiunge la Data di completamento pianificata.</p> </td> 
   <td> <p>Quando un'attività viene completata, la percentuale di completamento dell'attività viene contrassegnata come 100%. L’attività viene rimossa dall’elenco Il mio lavoro dell’assegnatario nell’area Home al termine.</p> <p>Quando si contrassegna un'attività come Completata, viene visualizzato un valore per Data di completamento effettiva.</p> <p><b>NOTA</b>: se l'attività presenta problemi incompleti e lo stato dell'attività viene modificato in Completato, lo stato viene automaticamente modificato in Completato - Problemi in sospeso.</p> </td> 
  </tr> 
 </tbody> 
</table>
