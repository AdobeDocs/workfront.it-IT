---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Stato delle attività del sistema
description: Sono necessari i tre stati predefiniti delle attività di sistema in Workfront, il che significa che è possibile sbloccarli, rinominarli e riordinarli, ma non è possibile nasconderli o eliminarli. È inoltre possibile aggiungere nuovi stati delle attività di sistema in base alle esigenze dell'organizzazione. La modifica dello stato di un'attività è in genere un processo manuale, ma talvolta lo stato di un'attività viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Stato delle attività del sistema

Sono necessari i tre stati predefiniti delle attività di sistema in Workfront, il che significa che è possibile sbloccarli, rinominarli e riordinarli, ma non è possibile nasconderli o eliminarli.

È inoltre possibile aggiungere nuovi stati delle attività di sistema in base alle esigenze dell&#39;organizzazione.

La modifica dello stato di un&#39;attività è in genere un processo manuale. Tuttavia, ci sono momenti descritti nel seguente elenco quando lo stato di un’attività viene modificato automaticamente, a seconda di altri fattori che si verificano nel sistema.

Con l’istanza Workfront vengono forniti i seguenti stati dell’attività:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Stato attività del sistema</th> 
   <th>Quando si verifica questo stato</th> 
   <th>Azioni che si verificano quando un'attività si trova in questo stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuovo (stato obbligatorio)</td> 
   <td>Questo è lo stato predefinito per ogni nuova attività creata.</td> 
   <td>Se l’attività si trova in un progetto con stato Corrente, l’attività viene visualizzata nella scheda Richieste di lavoro degli utenti assegnati alle attività. Gli utenti possono ora iniziare a lavorare sull’attività.</td> 
  </tr> 
  <tr> 
   <td>In corso (stato richiesto)</td> 
   <td>È possibile inserire un'attività in questo stato per indicare che il lavoro su tale attività è iniziato.</td> 
   <td> <p>Quando si contrassegna un'attività come In corso, l'attività mostra un valore per la data di inizio effettiva.</p> <p>L'avanzamento dell'attività non viene registrato finché non si aggiorna manualmente la percentuale di completamento dell'attività.</p> </td> 
  </tr> 
  <tr> 
   <td>Completa (stato richiesto)</td> 
   <td> <p>È possibile contrassegnare manualmente un'attività completata al termine del lavoro.</p> <p>Quando la modalità di tracciamento di un'attività è impostata su Completamento automatico, l'attività viene contrassegnata automaticamente come Completa quando raggiunge la data di completamento pianificata.</p> </td> 
   <td> <p>Al completamento di un’attività, la percentuale di completamento dell’attività viene contrassegnata come 100%. L’attività viene rimossa dall’elenco di lavoro del assegnatario nell’area Home al termine della procedura.</p> <p>Quando si contrassegna un'attività come Completa, l'attività visualizza un valore per la data di completamento effettivo.</p> <p><b>NOTA</b>: Se l'attività presenta problemi incompleti e si modifica lo stato dell'attività in Completato, lo stato diventa automaticamente Completa - Problemi in sospeso.</p> </td> 
  </tr> 
 </tbody> 
</table>
