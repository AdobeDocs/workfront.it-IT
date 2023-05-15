---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei tipi di ritardo
description: Ritardo è la quantità di tempo che deve trascorrere dopo il completamento di un predecessore applicato fino a quando l'attività dipendente può iniziare (Ritardo positivo), o la quantità di tempo che un'attività dipendente può iniziare prima dell'avvio del predecessore (Ritardo negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ad6ade3ff700f1e73c05dfc59aa0108a5d113f2e
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Panoramica dei tipi di ritardo

Ritardo è la quantità di tempo che deve trascorrere dopo il completamento di un predecessore applicato fino a quando l&#39;attività dipendente può iniziare (Ritardo positivo), o la quantità di tempo che un&#39;attività dipendente può iniziare prima dell&#39;avvio del predecessore (Ritardo negativo).

Le date previste, previste e stimate delle attività successive vengono calcolate tenendo conto del ritardo e delle date di inizio (completamento) previste, previste e stimate delle attività precedenti.

## Requisiti di accesso

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Indicazione dei tipi di ritardo e ritardo sulle attività

È possibile indicare tipi di ritardo per le attività quando si definiscono le relazioni predecessori.

* [Indicare i tipi di ritardo nella sezione Predecessori di un&#39;attività](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [Indicare i tipi di ritardo in un elenco di attività](#indicate-lag-types-in-a-task-list)

### Indicare i tipi di ritardo nella sezione Predecessori di un&#39;attività {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Passare a un&#39;attività per la quale si desidera definire il predecessore e il tipo di ritardo.
1. Fai clic su **Predecessori** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro** e quindi **Predecessori**.
1. Fai clic su **Aggiungi predecessore**.
1. (Facoltativo) Per aggiungere un predecessore tra progetti diversi, sostituisci il **Progetto padre** nome con un altro progetto.
1. Iniziare a digitare il nome dell&#39;attività predecessore, quindi selezionarla quando viene visualizzata nell&#39;elenco.
1. Seleziona la **Tipo di dipendenza**.

   Per ulteriori informazioni sui tipi di dipendenza predecessore, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specifica una **Ritardo** utilizzando un valore numerico. È possibile specificare numeri negativi per indicare un ritardo negativo.
1. Selezionare tra le seguenti opzioni per identificare il tipo di ritardo da indicare per il predecessore:

   * **Giorni**
   * **Giorni di Calendario**
   * **Percentuale**
   * **Giorno della settimana**
   * **Giorno della settimana (Non-Zero)**

      Per ulteriori informazioni su questi tipi di tag e su come vengono calcolati, consulta la sezione . [Panoramica sui tipi di ritardo](#lag-types-overview) in questo articolo.

1. Fai clic su **Salva**.

### Indicare i tipi di ritardo in un elenco di attività  {#indicate-lag-types-in-a-task-list}

1. Passa a un elenco di attività e seleziona la **Standard** Visualizza dal **Visualizza** menu a discesa.

1. Fai clic all’interno del **Predecessori** la colonna corrispondente all&#39;attività per la quale si desidera specificare un predecessore e una quantità di ritardo.
1. Inserisci quanto segue senza spazi:

   * il numero dell&#39;attività da indicare come predecessore dell&#39;attività selezionata
   * abbreviazione del tipo di dipendenza che si desidera indicare tra le attività

      Per ulteriori informazioni sulle abbreviazioni per Tipi di dipendenza, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * o **+** per un ritardo positivo o per un **-** per un ritardo negativo

   * l&#39;importo del ritardo
   * l&#39;abbreviazione del tipo di tag che si desidera utilizzare.

      Per ulteriori informazioni sulle abbreviazioni per i tipi di tag, consulta la sezione . [Panoramica sui tipi di ritardo](#lag-types-overview) in questo articolo.
   Ad esempio, per indicare che un&#39;attività ha un predecessore e un ritardo positivo di 2 giorni, immettere

   ```
   1fs+2d
   ```

   nella colonna Predecessori.

1. Fai clic su Invio sulla tastiera per salvare le modifiche apportate all’attività.

## Panoramica sui tipi di ritardo {#lag-types-overview}

Un esempio di attività che richiederebbe un ritardo potrebbe essere la segatura degli alberi in legname. Se il legno appena tagliato deve asciugarsi per un periodo di tempo prima che possa essere tagliato, allora ci sarebbe un ritardo tra tagliare gli alberi e segarli in legname.

La tabella seguente illustra i tipi di margine e come indicare il periodo di tempo per ciascuno di essi:

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
   <td> <p>Giorni (d)</p> </td> 
   <td> <p>Il ritardo tra due attività collegate dalla dipendenza viene misurato nei giorni lavorativi. Tipo di contrassegno predefinito. </p> <p>Ad esempio, se esiste una dipendenza di fine-inizio con un ritardo di 2 giorni lavorativi e l'attività predecessore termina il venerdì, l'attività dipendente inizia il mercoledì. I giorni del weekend non contano come parte del ritardo. </p> <p>Nota: Il limite massimo di ritardo per i giorni è di 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorni calendario (c)</p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato nei giorni di calendario, compresi i giorni festivi e i fine settimana. </p> <p>Nota: Anche se questo tipo di ritardo conta i giorni non lavorativi come parte del ritardo, un'attività dipendente non può mai iniziare da un giorno non lavorativo. Se questo tipo di ritardo fa sì che l'attività dipendente inizi in un giorno non lavorativo, la data di inizio pianificata dell'attività dipendente è pianificata per il giorno lavorativo successivo. </p> <p>Ad esempio, se esiste una dipendenza di fine inizio con un ritardo di 2 giorni di calendario e l'attività predecessore termina il giovedì, l'attività dipendente inizia il lunedì invece di una domenica. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentuale (p o pe)</p> </td> 
   <td> <p>Il ritardo è espresso in percentuale del tempo stimato per completare l'attività predecessore. </p> <p>Ad esempio, se esiste una dipendenza di fine-inizio con un ritardo del 20% su un'attività predecessore di 10 giorni, il sistema calcolerà il numero di giorni che rappresentano il 20% della durata dell'attività dei predecessori e lo utilizzerà come ritardo. In questo caso sarebbero 2 giorni dopo il completamento dell'attività. </p>

<p><b>NOTA</b></p> Il limite massimo di ritardo per la percentuale è del 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorno della settimana (w) </p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato indicando i giorni della settimana della settimana che contiene la data di completamento pianificata del predecessore.</p> <p>Per questo tipo di ritardo, ogni giorno della settimana è associato a un numero:</p> 
    <ul> 
     <li>domenica=1</li> 
     <li>Lunedì=2</li> 
     <li>Martedì=3</li> 
     <li>Mercoledì=4</li> 
     <li>Giovedì=5</li> 
     <li>Venerdì=6</li> 
     <li>Sabato=7</li> 
    </ul> <p>Se si desidera indicare che la data di inizio pianificata del successore deve essere impostata su un martedì della settimana corrente e il martedì è precedente alla data di completamento pianificata del predecessore, è necessario codificare il successore con la seguente formula: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTA</b></p>

Se il martedì passato per la settimana della data di completamento pianificata del predecessore, la data di inizio prevista dell&#39;attività successore è il primo giorno lavorativo disponibile della settimana. </p> <p>Se si desidera indicare che il ritardo deve essere uguale a un sabato della settimana corrente e il sabato è successivo alla data di completamento pianificata del predecessore, è necessario codificare il successore con la seguente formula:</p> <p>4fs+7w</code> </p> <p>Se il sabato è un giorno non lavorativo, il giorno successivo disponibile dopo il sabato (per indicare un ritardo positivo) viene selezionato come Data inizio prevista del successore. </p>

<p>Ciò non si applica alle eccezioni di pianificazione. Nel caso in cui una data sia anche un'eccezione di pianificazione e la data di inizio del successore sia calcolata come quel giorno, il sistema cerca di trovare la data disponibile più vicina, ovvero il giorno della settimana specificato nell'espressione predecessore.</p>

<p>Ad esempio, se la data di inizio è calcolata come un certo martedì e quel giorno è un'eccezione di pianificazione e il ritardo del predecessore è positivo, il martedì successivo (se è anche un giorno lavorativo) verrà scelto come data di inizio del successore. Se il ritardo è negativo, il sistema sceglie il martedì precedente come data di inizio.</p>

<p>Per indicare le settimane passate o future, è possibile aggiungere un numero davanti al numero del giorno per il tipo di ritardo. </p> <p>Ad esempio, per indicare il lunedì di 10 settimane fa, puoi utilizzare questo codice per indicare il predecessore del tuo successore:</p> <p><code>4fs-102w</code> </p> <p>10 indica 10 settimane fa e 2 è il numero assegnato a Lunedì. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Giorno della settimana non zero (k)</p> </td> 
   <td> <p>Il ritardo tra due attività viene misurato in modo identico al tipo di ritardo Giorno della settimana, a meno che l'ora del predecessore termini lo stesso giorno della settimana specificata. Il tempo di ritardo viene quindi calcolato sulla settimana adiacente (+/-). </p> <p>In questo caso, il tempo di ritardo non può mai essere 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica sui ritardi negativi

È possibile utilizzare un ritardo negativo per indicare la necessità o la capacità dell&#39;attività di iniziare prima della fine dell&#39;attività predecessore.

Quando si utilizzano tag negativi, considera le seguenti regole:

* Ritardo negativo non può forzare le date di inizio/fine di un&#39;attività prima o dopo le date di inizio/fine previste del progetto. Queste date sono specificate nel campo Pianificazione da del progetto.

   In questo caso, considera quanto segue:

   * Pianifica il progetto da data di completamento.
   * L&#39;ultima attività del progetto deve utilizzare il Vincolo di completamento obbligatorio per attività. Si consiglia di assegnare all’attività una durata sufficiente per tenere conto di tutte le attività del progetto. Le attività rimanenti funzionano bene con il vincolo Il prima possibile.

* L&#39;utilizzo di una relazione predecessore Fine-Inizio con le attività potrebbe generare un messaggio di errore.

   In questo caso, considera quanto segue:

   * Impostare una relazione predecessore Fine-Fine tra le attività.
   * La durata del compito successivo deve essere uguale o superiore al numero previsto di giorni di ritardo tra i compiti.
