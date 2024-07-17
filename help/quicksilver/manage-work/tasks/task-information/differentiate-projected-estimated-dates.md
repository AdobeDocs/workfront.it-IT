---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Differenziare tra date previste e date stimate
description: Esistono diversi tipi di date che mostrano la sequenza temporale delle attività tra le date di inizio e di completamento.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# Differenziare tra date previste e date stimate

Esistono diversi tipi di date che mostrano la sequenza temporale delle attività tra le date di inizio e di completamento. Di seguito sono riportate alcune date in cui viene visualizzata la sequenza temporale delle attività:

* Date Pianificate di Inizio e Completamento
* Date di inizio previste e date di completamento previste
* Date di inizio e di scadenza stimate
* Date effettive di inizio e di completamento

Questo articolo descrive le differenze tra le date stimate e quelle previste per i progetti.

Quando l&#39;attività viene creata per la prima volta, le date pianificate, previste e stimate devono in genere corrispondere. Esistono alcune eccezioni. 

Per ulteriori informazioni sulle date del progetto, dell&#39;attività e del problema in Adobe Workfront, vedere [Panoramica sulle date del progetto, dell&#39;attività e del problema in Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Panoramica delle date pianificate

Le Date Pianificate sono le date definite dal proprietario del progetto come date di inizio e fine delle attività. L&#39;utente o il proprietario del progetto può modificare manualmente le date pianificate di un&#39;attività.

## Panoramica delle date effettive

Quando un&#39;attività viene creata per la prima volta, non presenta date effettive perché non è ancora iniziata né completata.

## Panoramica delle date previste e stimate

Durante il ciclo di vita di un progetto, le Date previste e quelle stimate sono più in linea con la realtà del progetto, in quanto tengono conto di ciò che può influenzare l&#39;inizio e la fine effettivi di un&#39;attività. Questo li fa cambiare dalle Date Pianificate.

Quando si utilizzano le date previste e stimate per le attività, tenere presente quanto segue:

* Non è possibile modificare manualmente le date previste o stimate delle attività. Sono entrambi calcolati da Adobe Workfront.
* Quando si crea un&#39;attività, le date Prevista e Stimata devono essere identiche e devono indicare le ore effettive in cui le attività possono iniziare o finire.\
  Alcuni aggiornamenti apportati alle attività influiscono direttamente sui valori delle date previste e stimate. 

  Se ad esempio l&#39;utente avvia o completa un&#39;attività, verranno visualizzate le Date di inizio e di completamento effettive che influenzano le date previste e stimate dell&#39;attività. Inoltre, se un assegnatario dell&#39;attività modifica la Data impegno, questa data influisce sulla Data prevista dell&#39;attività.

## Differenza tra date previste e date stimate

La differenza tra le date previste e quelle stimate è:

* Le Date Previste sono influenzate dall&#39;esecuzione dei seguenti aggiornamenti sull&#39;attività da parte di un utente:

   * Aggiungere una data vincolo aggiungendo un vincolo attività fisso
   * Aggiungi una data di conferma

* Le Date Stimate tengono conto solo dei progressi reali di un&#39;attività in un determinato momento.

**Esempio:** se un&#39;attività ha una data di inizio pianificata del 20 settembre e una data di completamento pianificata del 24 settembre e deve finire entro il vincolo, la data di completamento prevista del 24 settembre. Questa attività ha una durata di 4 giorni.

La data di completamento stimata viene calcolata in base all&#39;avanzamento corrente del lavoro dell&#39;attività. Quindi, se oggi è il 23 settembre e l’attività non è ancora iniziata, la data di completamento stimata è il 27 settembre (dovrebbe essere completata dopo 4 giorni, supponendo che il lavoro sia iniziato oggi).

Se l&#39;attività è completata al 50% oggi, la data di completamento stimata è il 25 settembre (deve essere completata dopo 2 giorni, che corrisponde alla metà della durata dell&#39;attività).


### Informazioni sull&#39;aggiornamento delle date previste per le attività {#understand-when-projected-dates-update-on-tasks}

Le Date previste possono corrispondere ad altre date dell&#39;attività oppure sono un calcolo eseguito da Workfront che prende in considerazione l&#39;avanzamento reale dell&#39;attività.

Nell&#39;elenco seguente vengono visualizzati diversi scenari in cui le date previste delle attività vengono modificate durante il ciclo di vita di un progetto in base all&#39;andamento reale dell&#39;attività:

* Quando un’attività è contrassegnata come Completa:

  *Date previste = Date stimate = Date effettive*

* Quando un&#39;attività ha una data di inizio effettiva:

  *Data inizio prevista = Data inizio prevista = Data inizio effettiva*

* Quando un&#39;attività non ha una data di inizio effettiva, ma esiste un vincolo forzato sulla data di inizio pianificata (deve iniziare il) che è nel futuro:

  *Data Inizio Prevista = Data Vincolata*

  Per informazioni sulla Data Vincolata, consulta [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Quando un&#39;attività non ha una data di inizio effettiva e non ha una data vincolo forzata:

  *Data di inizio prevista = la prossima data disponibile nel futuro che rientra nella programmazione lavorativa*

* Quando l’assegnatario aggiorna la Data impegno:

  *Data completamento Prevista = Data Conferma*

  Per informazioni sulla data di conferma, vedere [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Se all&#39;attività non è associata una data di completamento aggiornata e all&#39;attività è associato un vincolo forzato (Deve finire al) per la data di completamento pianificata nel futuro:

  *Data di completamento Prevista = Data Vincolata*

* Se un&#39;attività non dispone di una Data impegno aggiornata, di una Data vincolo forzata nel futuro o di una Data vincolo nel passato:

  *Data completamento prevista = calcolo di sistema per la Data completamento in base all&#39;avanzamento corrente e al lavoro rimanente*

### Comprendere quando l&#39;aggiornamento delle Date Stimate viene eseguito sulle attività {#understand-when-the-estimated-dates-update-on-tasks}

Rispetto agli scenari descritti in precedenza per le Date previste, le Date stimate riflettono sempre l&#39;analisi reale di Workfront relativa al momento in cui l&#39;attività verrà avviata o completata, indipendentemente dalle Date vincolo o impegno.

## Effetti sulla sequenza temporale di un&#39;attività

Di seguito sono riportati alcuni esempi di ciò che può influenzare la sequenza temporale effettiva di un&#39;attività: 

* Avanzamento dell’attività in relazione alle date pianificate e al giorno corrente
* Percentuale di completamento dell&#39;attività fino ad ora
* Relazione del predecessore
* Avanzamento del predecessore
* Allocazione utente

  >[!NOTE]
  >
  >L&#39;allocazione degli utenti può influenzare la Data di completamento stimata di un&#39;attività se influisce sulla velocità con cui l&#39;attività può essere completata. Ad esempio, se il tipo di durata dell&#39;attività è Basato sulle risorse, è possibile completare prima l&#39;attività aggiungendo gli assegnatari. Di conseguenza, la data di completamento stimata cambia.
