---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica sui tipi di ritardo
description: Lag è il tempo che deve trascorrere dopo il completamento di un predecessore imposto fino a quando l'attività dipendente può iniziare (Lag positivo) o il tempo che un'attività dipendente può iniziare prima dell'inizio del predecessore (Lag negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Panoramica sui tipi di ritardo

<!-- Audited: 01/2024 -->

Lag è il tempo che deve trascorrere dopo il completamento pianificato di un predecessore fino a quando l&#39;attività dipendente può iniziare (Lag positivo) o il tempo che un&#39;attività dipendente può iniziare prima dell&#39;inizio del predecessore (Lag negativo).

Le date Pianificato, Previsto e Stimato delle attività successore vengono calcolate tenendo conto del ritardo e delle date Pianificato, Previsto e Stimato Inizio (Completamento) delle attività predecessori.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: Piano </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipi di Lag {#lag-types}

Un esempio di un&#39;attività che richiederebbe un tempo di ritardo potrebbe essere la segatura di alberi in legname. Se il legno appena tagliato deve asciugarsi per un certo periodo prima di poter essere tagliato, allora ci sarebbe un ritardo tra il taglio degli alberi e la segatura in legname.

Nella tabella seguente sono illustrati i tipi di ritardo e la modalità di indicazione del tempo per ciascuno di essi:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Valore</strong> </p> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Giorni (g o de)</p> </td> 
   <td> <p>Il ritardo tra due attività collegate dalla dipendenza viene misurato in giorni lavorativi. Questo è il tipo di Lag predefinito. </p> <p>Se ad esempio esiste una relazione Fine-Inizio con un ritardo di 2 giorni lavorativi e l'attività predecessore termina venerdì, l'attività dipendente inizia mercoledì. I giorni del fine settimana non vengono conteggiati come parte del ritardo. </p> <p>Nota: il limite massimo di ritardo per i giorni è 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorni di calendario (c o ce)</p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato in giorni di calendario, inclusi festività e fine settimana. </p> <p>Nota: sebbene questo tipo di ritardo conteggi i giorni non lavorativi come parte del ritardo, un'attività dipendente non può mai iniziare in un giorno non lavorativo. Se questo tipo di ritardo fa iniziare l'attività dipendente in un giorno non lavorativo, la data di inizio pianificata dell'attività dipendente viene programmata per il giorno lavorativo successivo. </p> <p>Se ad esempio esiste una relazione Fine-Inizio con un ritardo di 2 giorni di calendario e l'attività predecessore termina giovedì, l'attività dipendente inizia il lunedì anziché la domenica. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentuale (p o pe)</p> </td> 
   <td> <p>Il ritardo viene espresso come percentuale del tempo stimato per il completamento dell'attività predecessore. </p> <p>Se ad esempio esiste una relazione Fine-Inizio con un ritardo del 20% su un'attività predecessore di 10 giorni, il sistema calcolerà il numero di giorni che rappresentano il 20% della durata dell'attività predecessore e utilizzerà tale valore come ritardo. In questo caso, trascorrerebbero 2 giorni dal completamento dell’attività. </p>

<p><b>NOTA</b></p> Il limite massimo di ritardo per la percentuale è 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorno della settimana (w o we) </p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato indicando i giorni della settimana che contiene la data di completamento pianificata del predecessore.</p> <p>Per questo Tipo di Lag, ogni giorno della settimana è associato a un numero:</p> 
    <ul> 
     <li>Domenica=1</li> 
     <li>Lunedì=2</li> 
     <li>Martedì=3</li> 
     <li>Mercoledì=4</li> 
     <li>Giovedì=5</li> 
     <li>Venerdì=6</li> 
     <li>Sabato=7</li> 
    </ul> <p>Se si desidera indicare che la data di inizio pianificata del successore deve essere un martedì della settimana corrente e il martedì è precedente alla data di completamento pianificata del predecessore, è necessario codificare il successore con la seguente formula: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTA</b></p>

Se si calcola che la data di inizio del successore sia un martedì specifico e tale giorno sia passato per la settimana corrente, la data di inizio pianificata dell&#39;attività successore corrisponderà al giorno (martedì) della settimana successiva, se disponibile. </p> <p>Se si desidera indicare che il ritardo deve essere un sabato della settimana corrente e il sabato è successivo alla data di completamento pianificata del predecessore, è necessario codificare il successore con la seguente formula:</p> <p><code>4fs+7w</code> </p> <p>Se sabato è un giorno non lavorativo, come data di inizio pianificata del successore viene selezionato il successivo giorno disponibile dopo sabato (per indicare un ritardo positivo). </p>

<p>Questo non si applica alle eccezioni di pianificazione. Nel caso in cui anche una data sia un'eccezione di pianificazione e la data di inizio del successore venga calcolata per essere quel giorno, il sistema tenta di trovare la data disponibile più vicina, ovvero il giorno della settimana specificato nell'espressione precedente.</p>

<p>Ad esempio, se la data di inizio è calcolata come un determinato martedì e tale giorno è un'eccezione della pianificazione e l'ritardo del predecessore è positivo, verrà scelto il martedì successivo (se anche questo è un giorno lavorativo) come data di inizio del successore. Se il ritardo è negativo, il sistema sceglie il martedì precedente come data di inizio.</p>

<p>Per indicare le settimane passate o future, è possibile aggiungere un numero prima del numero del giorno per il tipo di ritardo. </p> <p>Ad esempio, per indicare il lunedì di 10 settimane fa, è possibile utilizzare questo codice per indicare il predecessore del successore:</p> <p><code>4fs-102w</code> </p> <p>10 indica 10 settimane fa e 2 è il numero assegnato a lunedì. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorno della settimana non zero (k o ke)</p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato in modo identico al tipo di ritardo Giorno della settimana, tranne nel caso in cui il tempo del predecessore termini nello stesso giorno della settimana specificata. Il tempo di ritardo viene quindi calcolato sulla settimana adiacente (+/-). </p> <p>In questo caso, il tempo di ritardo non può mai essere 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lag negativo

È possibile utilizzare un Lag negativo per indicare la necessità o la capacità dell&#39;attività di iniziare prima della fine dell&#39;attività predecessore.

Quando si utilizzano i tag negativi, considera le seguenti regole:

* Un ritardo negativo non può far precedere o precedere le date di inizio/fine di un&#39;attività dalle date di inizio/fine pianificate del progetto. Queste date sono specificate nel campo Pianifica da del progetto.

  In questo caso, considera quanto segue:

   * Pianifica il progetto dalla data di completamento.
   * Per l&#39;ultima attività del progetto è necessario utilizzare il vincolo Deve finire su attività. Si consiglia di assegnare all&#39;attività una durata sufficiente per tenere conto di tutte le attività del progetto. Le altre attività funzionano correttamente con il vincolo Il più presto possibile.

* L&#39;utilizzo di una relazione di tipo predecessore Fine-Inizio con le attività potrebbe generare un messaggio di errore.

  In questo caso, considera quanto segue:

   * Impostare una relazione predecessore Fine-Fine tra le attività.
   * La durata dell&#39;attività successore deve essere uguale o superiore al numero previsto di giorni di ritardo tra le attività.

## Indicare i tipi di ritardo e di ritardo sulle attività

È possibile indicare i tipi di ritardo sulle attività quando si definiscono le relazioni predecessori.

### Indicare i tipi di ritardo nella sezione Predecessori di un&#39;attività {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Passare a un&#39;attività per la quale si desidera definire il predecessore e il Tipo di Lag.
1. Fai clic su **Predecessori** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro** e quindi su **Predecessori**.
1. Fai clic su **Aggiungi predecessore**.
1. (Facoltativo) Se desideri aggiungere un predecessore per più progetti, sostituisci il nome del **progetto principale** con un altro progetto.
1. Inizia a digitare il nome dell&#39;attività predecessore, quindi selezionalo quando viene visualizzato nell&#39;elenco.
1. Selezionare il **tipo di dipendenza**.

   Per ulteriori informazioni sui tipi di dipendenza predecessori, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specificare un valore di **Lag** utilizzando un valore numerico. È possibile specificare numeri negativi per indicare un ritardo negativo.
1. Seleziona tra le seguenti opzioni per identificare il tipo di ritardo che desideri indicare per il tuo predecessore:

   * **Giorni**
   * **Giorni di calendario**
   * **Percentuale**
   * **Giorno della settimana**
   * **Giorno della settimana (diverso da zero)**

     Per ulteriori informazioni su questi tipi di Lag e su come vengono calcolati, vedere la sezione [Tipi di Lag](#lag-types) in questo articolo.

1. Fai clic su **Salva**.

### Indicare i tipi di ritardo in un elenco delle attività  {#indicate-lag-types-in-a-task-list}

1. Passare a un elenco di attività e selezionare la visualizzazione **Standard**.

1. Fai clic nella colonna **Predecessori** corrispondente all&#39;attività per la quale desideri specificare un predecessore e un ritardo.
1. Immetti quanto segue senza spazi:

   * numero dell&#39;attività che si desidera indicare come predecessore dell&#39;attività selezionata
   * abbreviazione del tipo di relazione che si desidera indicare tra le attività

     Per ulteriori informazioni sulle abbreviazioni per i tipi di dipendenza, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * un **+** per un ritardo positivo o un **-** per un ritardo negativo

   * l&#39;ammontare del ritardo
   * l’abbreviazione del Tipo di Lag che desideri utilizzare

     Per ulteriori informazioni sulle abbreviazioni per i tipi di Lag, vedere la sezione [Tipi di Lag](#lag-types) in questo articolo.

   Ad esempio, per indicare che un&#39;attività ha un predecessore e un ritardo positivo di 2 giorni, immettere `1fs+2d` nella colonna Predecessori.

1. Premi Invio sulla tastiera per salvare le modifiche apportate all’attività.