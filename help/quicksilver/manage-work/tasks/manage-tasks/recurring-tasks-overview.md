---
content-type: overview
product-area: projects
keywords: ricorrente,ricorrente,ricorrente
navigation-topic: manage-tasks
title: Panoramica delle attività ricorrenti
description: Panoramica delle attività ricorrenti
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# Panoramica delle attività ricorrenti

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Puoi creare attività ricorrenti per attività da ripetere come parte di un singolo progetto.

Questo articolo illustra informazioni e considerazioni sulla creazione e la modifica di attività ricorrenti.

Per informazioni sulla creazione di attività ricorrenti in Adobe Workfront, vedere [Creare attività ricorrenti](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Panoramica e considerazioni sulle attività ricorrenti

È possibile scegliere di creare attività ricorrenti per indicare il lavoro ripetibile durante la durata di un progetto.

Ad esempio, durante un progetto IT, è probabile che il software debba essere sottoposto a backup a intervalli regolari. La creazione di un&#39;attività ricorrente per questa attività riduce il tempo necessario per impostare più attività singole.

Quando crei attività ricorrenti in Workfront, tieni presente quanto segue:

* Impossibile aggiungere attività ricorrenti a un modello.
* Impossibile aggiungere una frequenza di ricorrenza a un&#39;attività esistente.
* Le attività ricorrenti vengono visualizzate come sottoattività o figli per l&#39;occorrenza principale che viene visualizzata come attività padre.
* Non è possibile allegare un&#39;approvazione a un&#39;attività padre ricorrente.
* Workfront trasferisce la maggior parte dei campi aggiornati per la ricorrenza padre durante la creazione alle attività figlio. I campi seguenti non vengono trasferiti alle attività figlio quando vengono create:

   * Il Vincolo attività delle attività figlio viene modificato automaticamente in:

      * Deve iniziare il per i progetti pianificati dalla data di inizio.
      * Deve completare il per i progetti pianificati a partire dalla data di completamento.

   * I documenti allegati all&#39;elemento padre non vengono trasferiti agli elementi figlio.

* Le seguenti modifiche si verificano sull&#39;attività padre dopo aver indicato che l&#39;attività è ricorrente:

   * Il campo Durata viene rinominato in Durata per Occorrenza per l&#39;attività padre. Rimane la Durata per le attività figlio.
   * Lo stato è disattivato per l&#39;attività padre e viene automaticamente impostato su Nuovo per le attività figlio. L&#39;attività padre viene completata automaticamente e lo stato viene aggiornato a Completo quando tutti gli elementi figlio vengono completati.
   * Gli unici tipi di durata disponibili per le attività ricorrenti sono:

      * Semplice
      * Impegno Aggiuntivo
* La Durata e le Ore pianificate indicate per una nuova attività ricorrente sono la Durata e le Ore pianificate di ciascuna occorrenza. La durata dell&#39;attività padre è il tempo che intercorre tra la data di inizio pianificata della prima attività e la data di completamento pianificata dell&#39;attività più recente. Le ore pianificate dell&#39;attività padre corrispondono al totale di tutte le ore pianificate di tutte le occorrenze.

## Considerazioni sulla modifica di attività ricorrenti

Alcune modifiche apportate a un elemento padre attività ricorrente potrebbero non essere aggiornate su tutte le occorrenze esistenti. Le attività figlio che mostrano lo stato di avanzamento o che sono state aggiornate singolarmente non verranno aggiornate quando si aggiorna l&#39;attività padre. Workfront ritiene che un&#39;attività mostri progressi nelle seguenti situazioni:

* Lo stato viene aggiornato e l’attività non è più Nuova
* La percentuale di completamento dell&#39;attività è superiore a zero
* L&#39;attività ha relazioni predecessori

La tabella seguente illustra se le modifiche apportate al trigger padre vengono aggiornate sugli elementi figlio che non sono stati modificati singolarmente o se mostrano lo stato di avanzamento:

| Campi aggiornati sull&#39;attività padre | Trasferimento degli aggiornamenti a elementi figlio non modificati o a elementi figlio senza avanzamento registrato |
|---|---|
| Frequenza di ricorrenza* | ✔ |
| Assegnazioni | ✔ |
| Nome | ✔ |
| Descrizione | ✔ |
| Priorità | ✔ |
| Durata | ✔ |
| Lavoro Necessario | ✔ |
| Tipo Cst | ✔ |
| Tipo di Reddito | ✔ |
| Livellamento Risorse | ✔ |
| Ritardo di Livellamento | ✔ |
| Vincolo attività | Non aggiorna gli elementi figlio |
| Allega o rimuovi Forms personalizzato | Non aggiorna gli elementi figlio |
| Tipo di Durata | Non aggiorna gli elementi figlio |
| Informazioni modulo personalizzato | Non aggiorna gli elementi figlio |

{style="table-layout:auto"}

&#42; Esistono i seguenti scenari quando si aggiorna la Frequenza di ricorrenza di un&#39;attività padre:

* Se si modifica la Frequenza di ricorrenza per un&#39;attività padre esistente, le sottoattività esistenti vengono eliminate e sostituite con nuove sottoattività che seguono la nuova frequenza di ricorrenza se non mostrano alcun avanzamento e se non sono state aggiornate manualmente.
* Se si modifica la Frequenza di ricorrenza per un&#39;attività padre esistente, le sottoattività che mostrano l&#39;avanzamento non vengono eliminate. A questo punto, queste attività sono considerate separate dalla ricorrenza.

&#42;&#42; le assegnazioni effettuate sull&#39;attività padre vengono applicate a tutte le sottoattività nella ricorrenza. Eventuali modifiche apportate all&#39;assegnazione nell&#39;attività padre sostituiscono le singole assegnazioni nell&#39;attività secondaria. Se l&#39;attività mostra lo stato di avanzamento, l&#39;assegnazione non cambia.

 
