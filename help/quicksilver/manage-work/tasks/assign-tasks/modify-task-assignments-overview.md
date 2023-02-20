---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Panoramica sulla modifica delle assegnazioni di attività
description: È possibile assegnare attività a o annullare l’assegnazione di attività da utenti, team o ruoli di lavoro. Puoi assegnare più risorse contemporaneamente oppure una sola risorsa. È possibile assegnare un'attività alla volta o più attività in blocco.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Panoramica sulla modifica delle assegnazioni di attività

È possibile assegnare attività a o annullare l’assegnazione di attività da utenti, team o ruoli di lavoro. Puoi assegnare più risorse contemporaneamente oppure una sola risorsa. È possibile assegnare un&#39;attività alla volta o più attività in blocco.

>[!TIP]
>
>È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
>
>Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
>
>* Riassegna l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.
>


Questo articolo contiene informazioni generali sull&#39;impatto della modifica delle assegnazioni di attività. Per informazioni su come assegnare le attività, vedere i seguenti articoli:

* Per informazioni sull&#39;assegnazione delle attività, vedere [Assegnare le attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md) e [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Per informazioni sulla modifica delle assegnazioni per più attività nell&#39;area Pianificazione, vedere &quot;Modificare più assegnazioni di utenti in attività nelle aree Programmazione&quot;.
* Per informazioni sull&#39;assegnazione di attività tramite il servizio di bilanciamento del carico di lavoro, consulta [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Alcune informazioni in questo articolo si applicano anche alle assegnazioni a problemi. Per ulteriori informazioni sull’assegnazione dei problemi e considerazioni aggiuntive, consulta [Modifica della panoramica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quando modificare le assegnazioni utente sulle attività

È possibile modificare le assegnazioni utente per le attività per diversi motivi, tra cui:

* Gli utenti si uniscono o lasciano il team
* Un utente prende una vacanza che si estende oltre le date di scadenza del task

   >[!NOTE]
   >
   >Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un ruolo o un utente specifico viene impostato come assegnatario per più attività e si desidera modificare rapidamente tutti gli elementi da assegnare a un utente o ruolo diverso

## Considerazioni relative a più assegnazioni a ruoli, team e utenti del processo

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di un ruolo di lavoro associato al loro profilo. Per informazioni sull’associazione degli utenti ai ruoli di lavoro, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Le attività o i problemi vengono solitamente assegnati per la prima volta a uno o più ruoli o a un team. Quando i progetti sono pronti per essere avviati, potrebbe essere necessario assegnarli anche agli utenti.\
   Se un’attività o un problema viene assegnato a uno o più ruoli e poi si assegna anche un utente, Adobe Workfront decide quale ruolo di lavoro associare all’utente aggiuntivo (se presente) in base alle regole seguenti:

   * Se è assegnato un solo ruolo di lavoro e corrisponde al ruolo principale dell&#39;utente, l&#39;attività o il problema viene assegnato solo all&#39;utente che svolge il ruolo primario.
   * Se sono assegnati più ruoli e almeno uno dei ruoli corrisponde ai ruoli secondari dell&#39;utente, l&#39;attività o il problema viene assegnato all&#39;utente che esegue uno dei loro Altri ruoli, che Workfront seleziona in modo casuale in presenza di più corrispondenze, nonché a eventuali ruoli aggiuntivi assegnati.
   * Se sono assegnati uno o più ruoli di lavoro e non vi sono corrispondenze con i ruoli dell&#39;utente, l&#39;attività o il problema viene assegnato sia al ruolo o ai ruoli che all&#39;utente.

* Se un&#39;attività o un problema viene assegnato a un team e si assegna anche un utente, l&#39;attività o il problema rimane assegnato sia al team che all&#39;utente.

## La rimozione degli assegnatari influisce sulle ore delle attività e sulle percentuali di allocazione

La rimozione degli utenti può influenzare le ore di attività e le percentuali di allocazione. L&#39;effetto che la rimozione di un utente ha sull&#39;attività dipende dal tipo di durata selezionato per l&#39;attività. Per informazioni sul tipo di durata, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Quando si elimina un utente da un&#39;attività con i seguenti tipi di durata:

* **Semplice:** Le ore pianificate assegnate a tale utente vengono sottratte dalle ore pianificate totali dell&#39;attività.

   >[!IMPORTANT]
   >
   >Questo potrebbe influire negativamente sul piano di progetto, in quanto modifica le ore pianificate totali per l&#39;attività e il progetto.

* **Sforzo guidato:** La percentuale di allocazione non cambia per gli altri utenti.
* **Assegnazione calcolata:** Le percentuali di allocazione di altri utenti vengono corrette in modo che il totale sia uguale a 100%.
* **Lavoro calcolato:** La percentuale di allocazione non cambia per gli altri utenti.

## Considerazioni sull&#39;annullamento dell&#39;assegnazione delle attività

È possibile rimuovere le assegnazioni da un&#39;attività alla volta oppure rimuovere le assegnazioni da più attività in blocco.

Per ulteriori informazioni sulla rimozione delle assegnazioni dalle attività in blocco, vedere [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Quando si rimuovono le assegnazioni dalle attività, tenere presente quanto segue:

* Quando si annulla l&#39;assegnazione di un utente da un&#39;attività, l&#39;attività rimane assegnata al ruolo di processo che l&#39;utente ha eseguito sull&#39;attività.
* Quando si annulla l&#39;assegnazione di un ruolo di lavoro o di un team da un&#39;attività, l&#39;attività rimane non assegnata se non viene assegnata ad altre risorse.
