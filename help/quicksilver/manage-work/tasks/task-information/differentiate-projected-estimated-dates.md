---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Differenziare tra date previste e date stimate
description: Esistono diversi tipi di date che mostrano la cronologia delle attività tra quando possono iniziare e quando possono essere completate.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Differenziare tra date previste e date stimate

Esistono diversi tipi di date che mostrano la cronologia delle attività tra quando possono iniziare e quando possono essere completate. 

Di seguito sono riportate alcune date che mostrano la cronologia delle attività:

* Date di inizio e di completamento pianificate
* Date di inizio e di completamento previste
* Date di inizio e di scadenza stimate
* Date di inizio effettivo e di completamento effettivo

Questo articolo descrive le differenze tra le date previste e quelle previste per i progetti. Quando l’attività viene creata per la prima volta, in genere le date pianificate, previste e stimate devono corrispondere. Esistono alcune eccezioni. 

Per ulteriori informazioni sul progetto, sulle attività e sulle date di rilascio in Adobe Workfront, vedi [Panoramica delle date del progetto, dell’attività e del problema in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Panoramica delle date previste

Le date pianificate sono le date definite dal proprietario del progetto come date di inizio e di fine delle attività. 

L&#39;utente o il proprietario del progetto può modificare manualmente le date pianificate di un&#39;attività.

## Panoramica delle date effettive

Quando un&#39;attività viene creata per la prima volta, non dispone di date effettive, perché non è ancora iniziata né completata.

## Panoramica delle date previste e stimate

Durante la vita di un progetto, le date previste e stimate sono più in linea con la realtà del progetto, in quanto tengono conto di ciò che può influenzare l’inizio e la fine effettivi di un’attività. Questo li porta a cambiare dalle date pianificate.

Quando si lavora con date previste e stimate sulle attività, tenere presente quanto segue:

* Non è possibile modificare manualmente le date previste o stimate delle attività. Sono entrambi calcolati da Adobe Workfront.
* Quando si crea un&#39;attività, le date previste e stimate devono essere identiche e devono illustrare l&#39;ora effettiva in cui le attività possono iniziare o terminare.\
   Alcuni aggiornamenti apportati alle attività influiscono direttamente sui valori delle date previste e stimate. 

   Ad esempio, se l&#39;utente avvia o completa un&#39;attività, l&#39;attività visualizza le date di inizio effettivo e di completamento che influenzano le date previste e stimate dell&#39;attività. Inoltre, se un assegnatario dell&#39;attività modifica la data di commit, questa data influenza la data prevista dell&#39;attività.

## Differenza tra date previste e date stimate

La differenza tra le date previste e quelle stimate è la seguente:

* Le date previste vengono influenzate da un utente che apporta i seguenti aggiornamenti sull&#39;attività:

   * Aggiungere una data vincolo aggiungendo un vincolo task fisso
   * Aggiungere una data di commit

* Le date stimate tengono conto solo dei progressi reali su un&#39;attività in un determinato momento.

**Esempio:** Se si dispone di un&#39;attività con una data di inizio pianificata del 20 settembre e una data di completamento pianificata del 24 settembre e deve terminare con un vincolo, la data di completamento prevista sarà il 24 settembre. Questa attività ha una durata di 4 giorni.

La data di completamento stimata viene calcolata in base all&#39;avanzamento corrente del lavoro sull&#39;attività. Quindi, se oggi è il 23 settembre e l&#39;attività non è ancora iniziata, la Data del completamento stimato è il 27 settembre (dovrebbe essere completato dopo 4 giorni, supponendo che il lavoro sia iniziato oggi).

Se l’attività è stata completata al 50% oggi, la Data di completamento stimata è il 25 settembre (dovrebbe essere completata dopo 2 giorni, che è la metà della Durata dell’attività).

* [Comprendere quando le date previste vengono aggiornate sulle attività](#understand-when-projected-dates-update-on-tasks)
* [Quando le date stimate vengono aggiornate sulle attività](#understand-when-the-estimated-dates-update-on-tasks)

### Comprendere quando le date previste vengono aggiornate sulle attività {#understand-when-projected-dates-update-on-tasks}

Le date previste possono corrispondere ad altre date dell&#39;attività oppure sono un calcolo eseguito da Workfront che tiene conto dell&#39;avanzamento reale dell&#39;attività.

Nell’elenco seguente sono riportati diversi scenari in cui le date previste delle attività vengono modificate durante la durata di un progetto, a seconda di ciò che accade nella vita reale all’attività:

* Quando un’attività è contrassegnata come Completa:

   *Date previste = Date stimate = Date effettive*

* Quando un&#39;attività ha una data di inizio effettiva:

   *Data di inizio prevista = Data di inizio stimata = Data di inizio effettiva*

* Quando un&#39;attività non dispone di una data di inizio effettiva, ma è presente un vincolo forzato sulla data di inizio pianificata (deve iniziare il giorno) che si verifica in futuro:

   *Data inizio prevista = Data vincolo*

   Per informazioni sulla data del vincolo, vedere [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Quando un&#39;attività non dispone di una data di inizio effettiva e l&#39;attività non dispone di una data di vincolo forzata:

   *Data inizio prevista = la data successiva disponibile futura che rientra nel programma di lavoro*

* Quando l’assegnatario aggiorna la data di commit:

   *Data di completamento prevista = Data di commit*

   Per informazioni sulla data di commit, vedi [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Quando l&#39;attività non dispone di una data di commit aggiornata e l&#39;attività ha un vincolo forzato (deve terminare su) per la data di completamento pianificata futura:

   *Data completamento prevista = Data vincolo*

* Quando un&#39;attività non dispone di una data di commit aggiornata, di una data di vincolo forzata futura o di una data di vincolo passata:

   *Data completamento prevista = calcolo del sistema per la data di completamento in base all&#39;avanzamento corrente e al lavoro rimanente da eseguire*

### Quando le date stimate vengono aggiornate sulle attività {#understand-when-the-estimated-dates-update-on-tasks}

Rispetto agli scenari sopra descritti per le date previste, le date stimate riflettono sempre l’analisi reale di Workfront relativa all’avvio o al completamento dell’attività, indipendentemente dalle date di vincolo o di commit.

## Cosa influisce sulla timeline di un’attività

Di seguito sono riportati alcuni esempi di cosa può influenzare la cronologia reale di un&#39;attività: 

* avanzamento dell’attività in relazione alle date previste e al giorno corrente
* percentuale di completamento dell&#39;attività fino ad ora
* rapporto predecessore
* progressi precedenti
* assegnazione degli utenti

   >[!NOTE]
   >
   >L&#39;allocazione degli utenti può influenzare la Data di completamento stimata di un&#39;attività se influisce sulla velocità con cui l&#39;attività può essere completata. Ad esempio, se il tipo di durata dell&#39;attività è Basato su sforzo, è possibile completare l&#39;attività prima aggiungendo assegnatari. Di conseguenza, viene modificata la Data di completamento stimata.
