---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Panoramica sulla modifica delle assegnazioni delle attività
description: È possibile assegnare o annullare l'assegnazione di attività a utenti, team o mansioni. È possibile assegnare più risorse contemporaneamente oppure una sola risorsa. È possibile assegnare un'attività alla volta oppure più attività in blocco.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Panoramica sulla modifica delle assegnazioni delle attività

È possibile assegnare o annullare l&#39;assegnazione di attività a utenti, team o mansioni. È possibile assegnare più risorse contemporaneamente oppure una sola risorsa. È possibile assegnare un&#39;attività alla volta oppure più attività in blocco.

>[!TIP]
>
>Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
>
>Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
>
>* Riassegnare l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.
>

Questo articolo contiene informazioni generali sull&#39;impatto della modifica delle assegnazioni delle attività. Per informazioni su come assegnare le attività, vedere gli articoli seguenti:

* Per informazioni sull&#39;assegnazione delle attività, vedere [Assegna attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md) e [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Per informazioni sulla modifica delle assegnazioni per più attività nell&#39;area Pianificazione, vedere &quot;Modificare le assegnazioni di più utenti alle attività nelle aree Pianificazione&quot;.
* Per informazioni sull’assegnazione delle attività tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Alcune informazioni contenute in questo articolo si applicano anche alle assegnazioni ai problemi. Per ulteriori informazioni sull’assegnazione dei problemi e considerazioni aggiuntive, consulta [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quando modificare le assegnazioni utente per le attività

È possibile modificare le assegnazioni utente per le attività per diversi motivi, tra cui:

* Gli utenti si uniscono o lasciano il team
* Un utente prende una vacanza che si estende oltre le date di scadenza dell’attività

  >[!NOTE]
  >
  >Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un ruolo o un utente specifico viene impostato come assegnatario di più attività e si desidera modificare rapidamente tutti gli elementi da assegnare a un altro utente o ruolo

## Considerazioni per più assegnazioni a mansioni, team e utenti

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di una mansione associata al loro profilo. Per informazioni sull&#39;associazione degli utenti ai ruoli, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Le attività o i problemi vengono in genere prima assegnati a una o più mansioni o a un team. Quando i progetti sono pronti per essere avviati, potrebbe essere necessario assegnarli anche agli utenti.\
  Se un’attività o un problema è assegnato a uno o più ruoli e successivamente si assegna anche un utente, Adobe Workfront decide quale ruolo associare all’utente aggiuntivo (se presente) in base alle seguenti regole:

   * Se è stata assegnata una sola mansione e questa corrisponde alla mansione principale dell’utente, l’attività o il problema viene assegnato solo all’utente che svolge la sua mansione principale.
   * Se sono stati assegnati più ruoli e almeno uno dei ruoli corrisponde ai ruoli secondari dell’utente, l’attività o il problema viene assegnato all’utente che svolge uno dei suoi Altri ruoli, che Workfront seleziona in modo casuale in caso di più corrispondenze, nonché a eventuali ruoli aggiuntivi assegnati.
   * Se sono state assegnate una o più mansioni e non vi sono corrispondenze ai ruoli dell’utente, l’attività o il problema viene assegnato sia al ruolo o alle mansioni che all’utente.

* Se un’attività o un problema è assegnato a un team e si assegna anche un utente, l’attività o il problema rimane assegnato sia al team che all’utente.

## Effetti della rimozione degli assegnatari sulle ore delle attività e sulle percentuali di allocazione

La rimozione degli utenti può influire sulle ore delle attività e sulle percentuali di allocazione. L&#39;effetto della rimozione di un utente sull&#39;attività dipende dal Tipo di durata selezionato per l&#39;attività. Per informazioni sul Tipo di Durata, vedi [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Quando si elimina un utente da un&#39;attività con i seguenti Tipi di durata:

* **Semplice:** Le ore pianificate assegnate a tale utente vengono sottratte dalle ore pianificate totali dell&#39;attività.

  >[!IMPORTANT]
  >
  >Questo potrebbe influire negativamente sul piano del progetto, in quanto modifica le ore pianificate totali per l&#39;attività e il progetto.

* **Impegno:** La percentuale di allocazione non cambia per gli altri utenti.
* **Assegnazione calcolata:** Le percentuali di allocazione di altri utenti vengono adeguate in modo che il totale sia uguale al 100%.
* **Lavoro calcolato:** La percentuale di allocazione non cambia per gli altri utenti.

## Considerazioni sull’annullamento dell’assegnazione delle attività

È possibile rimuovere assegnazioni da un&#39;attività alla volta oppure da più attività in blocco.

Per ulteriori informazioni sulla rimozione di assegnazioni da attività in blocco, vedere [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Quando si rimuovono assegnazioni da attività, tenere presente quanto segue:

* Quando si annulla l&#39;assegnazione di un utente a un&#39;attività, l&#39;attività rimane assegnata alla mansione che l&#39;utente ha svolto per l&#39;attività.
* Quando si annulla l&#39;assegnazione di una mansione o di un team a un&#39;attività, l&#39;attività rimane non assegnata se non è assegnata ad altre risorse.
