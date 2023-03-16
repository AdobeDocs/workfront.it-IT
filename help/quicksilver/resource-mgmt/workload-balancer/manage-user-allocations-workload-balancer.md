---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Gestire le allocazioni di utenti nel load balancer
description: In qualità di Gestione risorse, puoi assegnare il lavoro agli utenti e gestire le loro allocazioni giornaliere, settimanali o mensili dal servizio di bilanciamento del carico di lavoro.
author: Alina
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2785'
ht-degree: 0%

---

# Gestire le allocazioni di utenti nel load balancer

In qualità di Gestione risorse, è possibile assegnare il lavoro agli utenti e gestire le loro allocazioni giornaliere, settimanali o mensili dal servizio di bilanciamento del carico di lavoro per assicurarsi che gli vengano assegnate una quantità di ore che si adattano alle loro pianificazioni disponibili.

## Requisiti di accesso {#access-requirements}

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare quando si utilizza il servizio di bilanciamento del carico di lavoro nell'area Origine</p>
   <p>Lavoro, quando si utilizza il bilanciamento del carico di lavoro di un team o di un progetto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione a livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o versioni successive che includono Assegna assegnazioni alle attività e ai problemi per i quali si desidera gestire le allocazioni. </p> <p>Oppure </p> <p>Consente di gestire le autorizzazioni per le attività per le quali si desidera aggiornare l'orario pianificato, oltre ad aggiornare le allocazioni. Per informazioni sull’aggiornamento delle ore pianificate nel servizio di bilanciamento del carico di lavoro, consulta la sezione <a href="#update-task-planned-hours-when-managing-user-allocations">Aggiorna le ore pianificate dell'attività durante la gestione delle allocazioni degli utenti</a> in questo articolo. </p> <p>Per informazioni sulle autorizzazioni delle attività, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md">Condividere un’attività </a><span> e per informazioni sulle autorizzazioni relative ai problemi, vedi</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md">Condividere un problema </a></span>. </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Comprendere le allocazioni degli utenti

Le allocazioni degli utenti sono quantità di ore che indicano il tempo che un utente deve trascorrere in un dato giorno o giorno feriale, settimana o mese per completare l&#39;elemento di lavoro. Sono inclusi nelle ore pianificate dell&#39;elemento di lavoro.

Questo articolo descrive come aggiornare le allocazioni giornaliere, settimanali o mensili per gli utenti assegnati a attività o problemi. Per informazioni sulla gestione delle allocazioni complessive per gli utenti e i ruoli di lavoro per le attività, vedere [Gestione delle ore di allocazione di utenti e ruoli sulle attività](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [Panoramica sull&#39;allocazione utente](#user-allocation-overview)
* [Criteri che ripristinano le allocazioni degli utenti](#criteria-that-reset-user-allocations)

### Panoramica sull&#39;allocazione utente {#user-allocation-overview}

Puoi visualizzare l’allocazione degli utenti sotto forma di ore o come valore percentuale nel servizio di bilanciamento del carico di lavoro. È possibile regolare ore o percentuali.

Le allocazioni degli utenti sono incluse nel numero di ore pianificate di un elemento di lavoro. Per informazioni sull&#39;orario pianificato, vedi [Panoramica sull’orario pianificato](../../manage-work/tasks/task-information/planned-hours.md).

L&#39;attività Orari pianificati viene distribuita equamente tra tutti i giorni entro la durata dell&#39;attività per l&#39;utente assegnato all&#39;attività. Ad esempio, se un&#39;attività ha una durata di 5 giorni e un totale di 10 ore pianificate, il numero di allocazioni giornaliere per l&#39;attività è di 2 ore. L&#39;allocazione settimanale è di 10 ore. Ciò significa che un utente è assegnato per lavorare sull&#39;attività per 2 ore al giorno. Tuttavia, puoi modificare manualmente l’allocazione giornaliera per l’utente utilizzando il load Balancer.

>[!CAUTION]
>
>Il servizio di bilanciamento del carico di lavoro visualizza solo fino a 1000 ore pianificate per elemento di lavoro e fino a 1000 giorni di durata di un elemento. Le allocazioni nel servizio di bilanciamento del carico di lavoro vengono visualizzate come zero dopo il raggiungimento del limite di 1000 ore o 1000 giorni. È consigliabile suddividere le attività in sottoattività più piccole per adattarsi a un numero maggiore di ore pianificate o per durate superiori a 1000 giorni.

Quando si individuano allocazioni giornaliere, settimanali o mensili per attività o problemi nel load balancer, tenere presente quanto segue:

* È possibile visualizzare le allocazioni giornaliere, settimanali e mensili degli utenti agli elementi di lavoro. Abilitare la visualizzazione Settimana o Mese per visualizzare le allocazioni settimanali o mensili.
* Puoi utilizzare il servizio di bilanciamento del carico di lavoro per modificare l’allocazione giornaliera, settimanale o mensile degli utenti alle attività o ai problemi. Per informazioni sulla regolazione della visualizzazione del bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   >[!NOTE]
   >
   >È consigliabile prendere una decisione in quale intervallo di tempo (giornaliero, settimanale o mensile) si desidera utilizzare sempre per gestire le allocazioni degli utenti e non passare tra di essi per gli stessi elementi di lavoro. L&#39;aggiornamento delle allocazioni settimanali per lo stesso utente per il quale sono state precedentemente aggiornate le allocazioni giornaliere modifica l&#39;allocazione giornaliera per l&#39;utente.

* È possibile aggiornare le allocazioni sia per i giorni lavorativi che per quelli non lavorativi.
* Quando Workfront calcola automaticamente l&#39;allocazione giornaliera per l&#39;attività, sono importanti le marche temporali per le date di inizio e di completamento pianificato degli elementi di lavoro e per la pianificazione del progetto.

>[!INFO]
>
> Ad esempio, un&#39;attività potrebbe avere una Durata di 2 giorni e 2 ore pianificate e un&#39;ora di inizio pianificata è pari a 12:00 PM il primo giorno della durata con un utente e un programma di progetto che termina alle 5 del pomeriggio. La capacità dell&#39;utente per il primo giorno è di 5 ore. La capacità dell&#39;utente per il secondo giorno è di 8 ore (se la pianificazione inizia alle 9).
>
>Workfront calcola l’allocazione delle 2 ore nei 2 giorni della durata utilizzando la seguente formula:
>
>
```
>
>   Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours
>```
>
>  Per il nostro esempio, le ore di allocazione giornaliere sono:
>   
>  (2 / 13) * 5 = 0, 77 ore di allocazione per il primo giorno
>
>  (2 / 13) * 8 = 1, 23 ore di allocazione per il secondo giorno
>
>  Nei calcoli di cui sopra, 13 rappresenta il totale delle ore disponibili per l&#39;attività: 5 + 8 = 13



* Due utenti in fusi orari o pianificazioni diversi in fusi orari diversi rispetto a quelli degli utenti assegnati possono far sì che le quantità di allocazione vengano visualizzate in modo diverso a due utenti che visualizzano gli stessi elementi di lavoro.

* Quando un utente ha pianificato l’orario di inattività, il giorno o la parte del giorno vengono visualizzati in uno sfondo grigio. Se l’amministratore di Workfront ha abilitato l’impostazione Ora utente di disattivazione nell’area Configurazione per tenere conto del tempo di inattività dell’utente, le ore assegnate vengono spostate nel giorno successivo disponibile nella timeline. Se l’impostazione è disabilitata, le ore allocate rimangono nel giorno contrassegnato per l’ora di inattività e l’utente viene visualizzato come sovrassegnato. Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!TIP]
   >
   >Se il tempo di inattività è stato contrassegnato dopo l&#39;assegnazione dell&#39;utente a un elemento di lavoro, è necessario ricalcolare la timeline del progetto per visualizzare l&#39;allocazione spostata. Per informazioni, consulta [Ricalcolare le timeline dei progetti](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* Se sono assegnati più utenti all&#39;attività, la quantità di ore pianificate viene distribuita in modo uniforme a ciascun utente prima, quindi in modo uniforme a ogni giorno entro la durata dell&#39;attività. Questa distribuzione diventa l&#39;allocazione di ogni utente all&#39;attività.

   Ad esempio, potrebbero esistere i seguenti scenari:

   * Per un’attività con una durata di 2 giorni e con 10 ore pianificate assegnate a un utente, l’allocazione giornaliera per l’utente è di 5 ore al giorno per impostazione predefinita.
   * Per un’attività con una durata di 2 giorni e con 10 ore pianificate assegnate a due utenti, l’allocazione giornaliera per ciascun utente è di 2,5 ore al giorno per impostazione predefinita.

* Se un&#39;attività o un problema è stato completato prima della data di completamento pianificata, viene rilevato il numero di ore assegnate per i giorni rimanenti e non viene conteggiato per l&#39;allocazione complessiva dell&#39;utente. Viene visualizzato solo quando sono abilitate sia l&#39;icona Mostra allocazioni che l&#39;impostazione Mostra date previste. Per ulteriori informazioni sull&#39;abilitazione delle impostazioni nel servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/allocations-struck-through-highlighted-350x39.png)

* Quando un utente viene sovrapassegnato, le ore assegnate vengono visualizzate con uno sfondo rosso nel campo utente.
* Quando l’utente viene sottoallocato o allocato una quantità uguale di ore al tempo disponibile programmato, le ore vengono visualizzate con sfondo blu.
* Puoi visualizzare l’allocazione degli utenti in una visualizzazione grafico nella riga utente. Per informazioni sull’abilitazione della visualizzazione grafico per le allocazioni degli utenti, consulta la sezione &quot;Navigare nel bilanciamento del carico di lavoro&quot; nell’articolo [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/user-allocation-chart-350x237.png)

### Criteri che ripristinano le allocazioni degli utenti {#criteria-that-reset-user-allocations}

Non tutte le modifiche dell&#39;attività attivano le allocazioni modificate per la ridistribuzione. Tuttavia, esistono alcune azioni che potrebbero ripristinare le allocazioni già corrette sulle risorse e ridistribuirle in modo uniforme a tutti i giorni durante la durata dell&#39;elemento di lavoro per ciascuno degli assegnatari.

>[!NOTE]
>
>Se non è stata modificata la distribuzione automatica delle allocazioni sugli elementi di lavoro, le ore vengono ridistribuite in modo uniforme tra tutti gli assegnatari in caso di modifica del numero di assegnatari, della durata di un&#39;attività o della quantità di ore pianificate sull&#39;elemento di lavoro.

* [Azioni che ripristinano le allocazioni corrette](#actions-that-reset-adjusted-allocations)
* [Azioni che non ripristinano le allocazioni corrette](#actions-that-do-not-reset-adjusted-allocations)

#### Azioni che ripristinano le allocazioni corrette {#actions-that-reset-adjusted-allocations}

Le azioni seguenti ripristinano o modificano le allocazioni giornaliere, settimanali o mensili per gli utenti dopo averle modificate manualmente come descritto in [Modificare le allocazioni degli utenti](#modify-user-allocations) in questo articolo:

* Quando si accorcia la lunghezza di un elemento di lavoro che riduce la quantità di giorni nella relativa Durata, le ore allocate corrette dai giorni perduti vengono aggiunte all&#39;importo di allocazione dell&#39;ultimo giorno dell&#39;elemento di lavoro.
* Quando si modifica la quantità di ore pianificate su un&#39;assegnazione o sull&#39;elemento di lavoro, il nuovo numero di ore pianificate viene ridistribuito in modo uniforme per l&#39;intera durata dell&#39;elemento di lavoro.
* Quando si aggiunge o si rimuove un assegnatario a un elemento di lavoro e questo determina la modifica delle ore pianificate dell&#39;attività, i valori corretti vengono ridistribuiti in modo uniforme.

#### Azioni che non ripristinano le allocazioni corrette {#actions-that-do-not-reset-adjusted-allocations}

Le seguenti modifiche a un elemento di lavoro non attivano le allocazioni corrette per reimpostare o modificare:

* Quando si spostano i giorni di un elemento di lavoro ma la quantità di giorni in Durata non viene modificata, i valori allocati modificati rimangono invariati e passano alle nuove date.
* Quando si aumenta la Durata di un elemento di lavoro che aumenta il numero di giorni nella sua Durata, le ore assegnate modificate rimangono uguali per i giorni corretti. Altri giorni vengono aggiunti all&#39;elemento di lavoro con 0 ore allocate.
* Quando si aggiunge o si rimuove un assegnatario a un elemento di lavoro e questo non determina la modifica delle ore pianificate dell&#39;elemento, i valori regolati rimangono gli stessi.

## Individua ore pianificate nel servizio di bilanciamento del carico di lavoro

È possibile modificare le allocazioni degli utenti alle attività o ai problemi utilizzando il servizio di bilanciamento del carico di lavoro individuando l&#39;orario pianificato delle attività o dei problemi assegnati agli utenti.

Quando si visualizzano le ore pianificate nel load balancer, considera quanto segue:

* Il totale delle ore pianificate per un&#39;attività o un problema viene visualizzato accanto all&#39;attività o al nome del problema a sinistra del servizio di bilanciamento del carico di lavoro.

* Il totale delle ore pianificate per un progetto viene visualizzato accanto al Nome progetto a sinistra del servizio di bilanciamento del carico di lavoro. Rappresenta il totale delle ore pianificate per tutte le attività e i problemi elencati nel progetto nel servizio di bilanciamento del carico di lavoro e non tutte le ore pianificate del progetto.
* Il tempo allocato ogni giorno o settimanalmente per tutte le attività e per tutti i progetti viene visualizzato solo quando si abilita manualmente l&#39;impostazione Mostra allocazioni. Per informazioni sull&#39;abilitazione delle impostazioni nel servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Modificare le allocazioni degli utenti {#modify-user-allocations}

Come parte dell&#39;assegnazione del lavoro agli utenti, è possibile modificare le allocazioni degli utenti nel servizio di bilanciamento del carico di lavoro per garantire che non vengano mai sovrassegnate o per garantire un preciso equilibrio di ore tra le risorse. Per informazioni sull’identificazione della sovrallocazione di un utente, consulta la sezione . [Panoramica sull&#39;allocazione utente](#user-allocation-overview) in questo articolo.

1. Assicurati di avere attività e problemi assegnati agli utenti. Per informazioni sull&#39;assegnazione di lavoro agli utenti nel servizio di bilanciamento del carico di lavoro, vedi [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Vai al servizio di bilanciamento del carico di lavoro .
1. (Facoltativo) Fai clic su **Settimana** o **Mese** per gestire le allocazioni settimanali o mensili per gli utenti.

   ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. In **Lavoro assegnato** individuare l&#39;utente per il quale si desidera modificare manualmente l&#39;allocazione e fare clic sulla freccia rivolta a destra a sinistra del nome utente per espandere l&#39;utente.

   ![](assets/wb-highlight-on-name-caret-350x106.png)

1. Fai clic sulla freccia rivolta a destra a sinistra del nome del progetto per espandere il progetto e visualizzare gli elementi di lavoro a cui l’utente è assegnato.

   >[!TIP]
   >
   >È possibile modificare le allocazioni degli utenti solo per attività e problemi. Non è possibile modificare le allocazioni degli utenti per i progetti.

1. (Facoltativo) Fai clic sul pulsante **Icona Mostra allocazioni** ![](assets/show-allocations-icon-small.png) per visualizzare le allocazioni per tutti gli elementi di lavoro.

   Il nome delle attività e dei progetti viene sostituito con l’assegnazione dell’utente per l’attività o il progetto.

1. (Facoltativo) Fai clic sul pulsante **Impostazioni** icona ![](assets/gear-icon-settings.png) e selezionare una delle seguenti opzioni:

   1. **Includi ore da problemi**. Questo consente di gestire le allocazioni dei problemi oltre alle allocazioni delle attività.
   1. **Mostra lavoro completato** . Vengono visualizzati gli elementi completati e pianificati nella timeline per cui gestisci le allocazioni.
   1. **Mostra il tempo rimanente** opzione . Il numero totale di ore per ogni utente (nella riga utente) cambia. Con questa impostazione abilitata, il servizio di bilanciamento del carico di lavoro visualizza le ore disponibili per il lavoro di ogni utente, anziché il numero di ore per le quali è stato allocato.

      >[!TIP]
      >
      >La modifica delle allocazioni quando questa impostazione è abilitata fa diminuire il numero totale nella riga utente.

   1. **Progetto** in **Seleziona tema colore** sezione . Questo consente di visualizzare ogni progetto e i rispettivi elementi di lavoro in colori unici e di comprendere più facilmente quali elementi appartengono a un progetto.
   1. **Percentuale** in **Visualizza l&#39;allocazione degli utenti in** sezione . In questo modo le allocazioni vengono visualizzate come valore percentuale. La capacità dell’utente in base alla pianificazione è considerata al 100%. Ad esempio, se un utente è associato a una pianificazione di 8 ore al giorno, 8 ore equivale a una capacità del 100%. Se si desidera allocare l&#39;utente a lavorare 4 ore al giorno, è necessario aggiornare l&#39;allocazione al 50%.

      >[!NOTE]
      >
      >L&#39;amministratore di Workfront decide quale pianificazione utilizzare nel sistema per calcolare la capacità dell&#39;utente nell&#39;area Gestione risorse dell&#39;installazione. Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).


1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-menu.png) per un elemento di lavoro, quindi fare clic su **Modifica allocazioni**.

![](assets/more-menu-on-task-wb-nwe.png)

Oppure

Fare doppio clic sul giorno, la settimana o il mese nella barra di un&#39;attività o di un problema.

Le caselle di allocazione diventano modificabili.

1. Fare clic all&#39;interno della casella di ogni allocazione giornaliera, settimanale o mensile per aggiornare manualmente la quantità di ore o il valore percentuale per il quale si desidera allocare l&#39;utente ogni giorno, settimana o mese, quindi fare clic sul pulsante **Salva** icona ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Fai clic sul pulsante **Annulla** icona ![](assets/cancel-allocations-wb.png) per rimuovere le allocazioni modificate.

   ![](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   Le allocazioni per l&#39;aggiornamento dell&#39;utente.

   >[!TIP]
   >
   >Se un&#39;attività o un problema è stato completato prima della data di completamento pianificata, viene rilevato il numero di ore assegnate per i giorni rimanenti e non viene conteggiato per l&#39;allocazione complessiva dell&#39;utente. Viene visualizzato solo quando sono abilitate sia l&#39;icona Mostra allocazioni che l&#39;impostazione Mostra date previste.

   Esistono i seguenti scenari:

   * Per le attività con tipi di durata non semplici o per problemi, il totale delle allocazioni deve corrispondere all&#39;attività Orari pianificati prima di poter fare clic sull&#39;icona del segno di spunta.
   * Per le attività con durata semplice, il totale delle allocazioni può essere superiore o inferiore alle ore pianificate e puoi fare clic sull&#39;icona del segno di spunta anche se non corrispondono. Viene inoltre aggiornato il numero di ore pianificate per l’attività. È necessario disporre delle autorizzazioni corrette e dell&#39;accesso per aggiornare le ore pianificate sulle attività dal servizio di bilanciamento del carico di lavoro.

      >[!TIP]
      >
      >L&#39;icona Blocca viene visualizzata a destra del nome dell&#39;attività quando si inizia a regolare le allocazioni per indicare che l&#39;attività ha un tipo di durata semplice.

      ![](assets/lock-icon-on-simple-task-in-the-balancer-350x119.png)
   Per ulteriori informazioni sulle condizioni che devono essere soddisfatte per aggiornare le ore pianificate nel servizio di bilanciamento del carico di lavoro, consulta la seguente sezione in questo articolo: [Aggiorna le ore pianificate dell&#39;attività durante la gestione delle allocazioni degli utenti](#update-task-planned-hours-when-managing-user-allocations). Per informazioni sui tipi di durata dell&#39;attività, vedere [Panoramica del tipo di durata e durata dell’attività](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Condizionale) Se l&#39;attività viene assegnata a più utenti, ripetere questi passaggi per ogni utente assegnato all&#39;attività per aggiornare le allocazioni per ogni utente.

   Chiunque abbia accesso per visualizzare il servizio di bilanciamento del carico di lavoro e visualizzare gli stessi utenti e gli stessi progetti gestiti ora visualizza l’allocazione aggiornata per gli utenti gestiti.

## Aggiorna le ore pianificate dell&#39;attività durante la gestione delle allocazioni degli utenti {#update-task-planned-hours-when-managing-user-allocations}

È possibile aggiornare l&#39;orario pianificato di un&#39;attività durante la gestione delle allocazioni degli utenti nel servizio di bilanciamento del carico di lavoro per l&#39;attività. Ciò si verifica quando il totale delle ore assegnate aggiornate non corrisponde al totale originale delle ore pianificate per un&#39;attività.

>[!IMPORTANT]
>
>* L’aggiornamento dell’orario pianificato per le attività può influire sull’avanzamento del progetto.
>* L&#39;aggiornamento manuale delle ore pianificate modificando le allocazioni giornaliere può avere un impatto sulle ore pianificate durante la rimozione delle assegnazioni dalle attività in futuro. Per ulteriori informazioni, consulta [Panoramica sull’orario pianificato](../../manage-work/tasks/task-information/planned-hours.md).
>
>* Non è possibile aggiornare le ore pianificate per i problemi aggiornando le allocazioni nel servizio di bilanciamento del carico di lavoro.
>


Questo è possibile quando esistono le seguenti condizioni:

* Hai le autorizzazioni e l’accesso corretti per gestire le ore pianificate dal servizio di bilanciamento del carico di lavoro. Questi includono:

   * Gestisci le autorizzazioni per le attività.
   * Aggiorna le ore pianificate nell&#39;accesso al servizio di bilanciamento del carico di lavoro nell&#39;area Gestione risorse del livello di accesso.

   Per ulteriori informazioni sull&#39;accesso necessario per utilizzare il servizio di bilanciamento del carico di lavoro, consulta la sezione seguente in questo articolo: [Requisiti di accesso](#access-requirements) .

* L&#39;attività ha un tipo di durata semplice.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the statement above might include other duration types in the future)</p>
  -->
