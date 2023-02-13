---
content-type: overview
product-area: projects
keywords: ricorrente,ripetuto,ripetuto
navigation-topic: manage-tasks
title: Panoramica delle attività ricorrenti
description: Panoramica delle attività ricorrenti
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '615'
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

Per informazioni su come creare attività ricorrenti in Adobe Workfront, consulta [Creare attività ricorrenti](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Panoramica e considerazioni sulle attività ricorrenti

È possibile scegliere di creare attività ricorrenti per indicare il lavoro ripetibile durante la durata di un progetto.

Ad esempio, durante un progetto IT, è probabile che sia necessario eseguire il backup del software a intervalli regolari. La creazione di un’attività ricorrente per questa attività riduce il tempo necessario per impostare più attività individuali.

Quando crei attività ricorrenti in Workfront, considera quanto segue:

* Non è possibile aggiungere attività ricorrenti a un modello.
* Non è possibile aggiungere una frequenza di ricorrenza a un&#39;attività esistente.
* Le attività ricorrenti vengono visualizzate come sottoattività o elementi secondari per l&#39;occorrenza principale che viene visualizzata come attività principale.
* Non è possibile allegare un&#39;approvazione a un&#39;attività ricorrente padre.
* Workfront trasferisce la maggior parte dei campi aggiornati per la ricorrenza padre durante la creazione alle attività figlio. I campi seguenti non vengono trasferiti alle attività figlio quando vengono create:

   * Il Vincolo attività delle attività figlio cambia automaticamente in:

      * Deve iniziare il giorno per i progetti pianificati a partire dalla data di inizio.
      * È necessario completare i progetti pianificati a partire dalla data di completamento.
   * I documenti allegati al genitore non vengono trasferiti ai figli.


* Le seguenti modifiche si verificano sull&#39;attività principale dopo aver indicato che l&#39;attività è ricorrente:

   * Il campo Durata viene rinominato in Durata per Occorrenza per l&#39;attività principale. Resta la Durata per le attività dei bambini.
   * Lo stato è disattivato nell&#39;attività principale e viene impostato automaticamente su Nuovo negli elementi secondari. L&#39;attività padre viene completata automaticamente e lo stato viene aggiornato su Completato al completamento di tutti gli elementi figlio.
   * Gli unici tipi di durata disponibili per le attività ricorrenti sono:

      * Semplice
      * Impegno Aggiuntivo

## Considerazioni sulla modifica di attività ricorrenti

Alcune modifiche apportate a un&#39;attività padre ricorrente potrebbero non essere aggiornate su tutte le ricorrenze esistenti. Le attività secondarie che mostrano l’avanzamento o che sono state aggiornate singolarmente non vengono aggiornate quando si aggiorna l’elemento padre. Workfront ritiene che un’attività presenti dei progressi nelle seguenti situazioni:

* Lo stato viene aggiornato e l’attività non è più Nuova
* La percentuale di completamento dell&#39;attività è superiore a zero
* L&#39;attività ha relazioni precedenti

La tabella seguente illustra se le modifiche apportate agli aggiornamenti del trigger padre sugli elementi secondari che non sono stati modificati singolarmente o mostrano lo stato di avanzamento:

| Campi aggiornati sull’attività principale | Aggiornamenti trasferiti a figli o figli non modificati senza avanzamento registrato |
|---|---|
| Frequenza ricorrenza* | ↓ |
| Assegnazioni&#42;&#42; | ✔ |
| Nome | ✔ |
| Descrizione | ✔ |
| Priorità | ✔ |
| Durata | ✔ |
| Lavoro Necessario | ✔ |
| Tipo Cst | ✔ |
| Tipo di ricavo | ✔ |
| Livellamento Risorse | ✔ |
| Ritardo di Livellamento | ✔ |
| Vincolo attività | Non aggiorna i figli |
| Allega o rimuovi Forms personalizzato | Non aggiorna i figli |
| Tipo di durata | Non aggiorna i figli |
| Informazioni sul modulo personalizzato | Non aggiorna i figli |

{style=&quot;table-layout:auto&quot;}

&#42; Quando si aggiorna la frequenza di ricorrenza di un&#39;attività principale si verificano i seguenti scenari:

* Se si modifica la frequenza di ricorrenza in un&#39;attività padre esistente, le sottoattività esistenti vengono eliminate e sostituite con nuove sottoattività che seguono la nuova frequenza di ricorrenza se non mostrano alcun avanzamento e se non le si sono aggiornate manualmente.
* Se si modifica la frequenza di ricorrenza in un&#39;attività padre esistente, le sottoattività che mostrano l&#39;avanzamento non vengono eliminate. Queste attività sono considerate separate dalla ricorrenza a questo punto.

&#42;&#42; Le assegnazioni eseguite sull&#39;attività padre vengono applicate a tutte le sottoattività della ricorrenza. Qualsiasi modifica apportata all&#39;assegnazione nell&#39;attività padre sostituisce le singole assegnazioni nell&#39;attività secondaria. Se l&#39;attività mostra l&#39;avanzamento, l&#39;assegnazione non viene modificata.

 
