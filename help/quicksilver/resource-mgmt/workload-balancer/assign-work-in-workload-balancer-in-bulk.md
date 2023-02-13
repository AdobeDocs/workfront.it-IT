---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro in blocco utilizzando il bilanciamento del carico di lavoro
description: Puoi assegnare manualmente gli elementi di lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '1545'
ht-degree: 2%

---

# Assegnare il lavoro in blocco utilizzando il bilanciamento del carico di lavoro

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

Puoi assegnare manualmente gli elementi di lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront.

Per informazioni generali sull&#39;assegnazione del lavoro agli utenti che utilizzano il bilanciamento del carico di lavoro, vedi [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Pianificare, quando si utilizza il servizio di bilanciamento del carico di lavoro per un team o nell'area di determinazione origine </p>
   <p>Operazioni da eseguire quando si utilizza il servizio di bilanciamento del carico di lavoro di un progetto </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori ai progetti, alle attività e ai problemi che includono l'opzione Assegna assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni per l&#39;esecuzione di assegnazioni in serie nel servizio di bilanciamento del carico di lavoro

* È possibile gestire rapidamente le assegnazioni utente per più attività e problemi in uno o più progetti. Le modifiche nelle assegnazioni sono visibili immediatamente nel load balancer.
* Non è possibile assegnare risorse a elementi di lavoro completati o a elementi di un progetto completato.
* Quando assegni utenti in blocco, puoi effettuare le seguenti operazioni:

   * Assegnare un utente a tutti gli elementi di lavoro attualmente assegnati a un ruolo di lavoro.
   * Sostituisci le assegnazioni utente tra utenti diversi.
   * Annullare l’assegnazione di un utente da tutti i relativi elementi di lavoro.

**ESEMPI**

* L&#39;utente è responsabile dell&#39;assegnazione degli utenti per diversi nuovi progetti. I progetti sono stati creati in origine da modelli e i ruoli di lavoro sono già assegnati alle varie attività all’interno dei progetti. Si desidera assegnare un utente specifico, Jackie Simms, a tutte le attività attualmente assegnate a un ruolo di lavoro. È possibile utilizzare la funzione Assegna per assegnare queste attività a Jackie Simms.
* 45 attività su 3 progetti diversi sono assegnati a Jackie Simms. Jackie lascia l&#39;organizzazione e ora devi riassegnare le sue attività a un altro utente. È possibile utilizzare la funzione Sostituisci per assegnare queste attività alla nuova persona.
* 10 attività in 2 progetti diversi sono assegnate a un altro utente, Rick Kuvec. Ti rendi conto che Rick è stato assegnato a questi compiti per errore, ma non sei sicuro a chi devono essere assegnati in questo momento. È necessario annullare l&#39;assegnazione di Rick a tutte le attività contemporaneamente. È possibile utilizzare la funzione Annulla assegnazione per rimuovere Rick da queste attività.

## Assegnare il lavoro in blocco nel servizio di bilanciamento del carico di lavoro

1. Passa al servizio di bilanciamento del carico di lavoro in cui desideri assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro nell&#39;area Origine, nel progetto o a livello di team. Per ulteriori informazioni sulla posizione del servizio di bilanciamento del carico di lavoro in Workfront, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Fai clic su **Assegnazioni in blocco** ![](assets/bulk-assignments-wb.png) nella parte superiore del servizio di bilanciamento del carico di lavoro.

   Il pannello Assegnazioni in blocco si apre a destra del servizio di bilanciamento del carico di lavoro.

1. (Condizionale) Se accedi al servizio di bilanciamento del carico di lavoro dall&#39;area Origine o per un team, espandi la **Progetto: Nome** menu a discesa e utilizzare i modificatori di filtro per selezionare il progetto o i progetti per i quali si desidera eseguire le assegnazioni. È possibile selezionare i progetti per nome (opzione predefinita) o per stato.

Per informazioni sui modificatori del filtro Workfront, consulta [Filtri e modificatori di condizioni](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>Il nome del progetto viene selezionato per impostazione predefinita quando si accede al servizio di bilanciamento del carico di lavoro per un progetto.

![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Facoltativo) Fai clic su **Selezionare le attività del progetto** per selezionare l&#39;attività o le attività per le quali si desidera eseguire le assegnazioni, quindi nella **Attività: Nome** menu a discesa, selezionare le attività per nome (opzione predefinita) o Stato e utilizzare i modificatori di filtro per cercare attività specifiche.

Per informazioni sui modificatori del filtro Workfront, consulta [Filtri e modificatori di condizioni](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>Non è possibile selezionare le attività in uno stato Completo.

![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

>[!TIP]
>
>Lasciare vuota questa selezione se si desidera eseguire assegnazioni in serie per problemi e attività.

1. (Facoltativo) Fai clic sul pulsante **Elimina** icona ![](assets/delete.png) accanto a uno dei criteri selezionati

   Oppure

   Fai clic su **Cancella tutto** nell’angolo in alto a destra del pannello Assegnazioni in serie per rimuovere tutte le selezioni.

1. Seleziona una delle opzioni seguenti e continua con i passaggi descritti di seguito:

   * [Assegna utente](#assign-user)
   * [Sostituisci utente](#replace-user)
   * [Revoca assegnazione utente](#unassign-user)

   >[!TIP]
   >
   >Se nessun elemento corrisponde ai filtri selezionati, queste opzioni sono disattivate.

### Assegna utente {#assign-user}

Quando assegni un utente utilizzando le assegnazioni in blocco nel servizio di bilanciamento del carico di lavoro, si verificano le seguenti situazioni:

* Un utente viene assegnato a tutti gli elementi di lavoro attualmente assegnati a un ruolo specifico all’interno dei progetti selezionati.
* L&#39;utente non viene assegnato ai seguenti tipi di elementi di lavoro:

   * Elementi già assegnati a un utente.
   * Elementi completati.

* Se l’utente selezionato non è associato al ruolo specificato, il ruolo viene sostituito dall’utente nel ruolo primario dell’utente.

Per assegnare un utente agli elementi di lavoro precedentemente assegnati ai ruoli di lavoro:

1. Inizia ad assegnare gli elementi di lavoro utilizzando le assegnazioni in blocco nel servizio di bilanciamento del carico di lavoro come descritto in precedenza e seleziona **Assegna**.

1. In **Assegnazione ruolo** fare clic sulla freccia a discesa per scegliere da un elenco di ruoli. Vengono visualizzati solo i ruoli attualmente assegnati all’interno dei progetti specificati. Questo è un campo obbligatorio.

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. In **Utente da assegnare** fare clic sulla freccia a discesa per scegliere da un elenco di utenti consigliati o per digitare il nome di un altro utente.

   Seleziona gli utenti dalle seguenti aree:

   * **Assegnazioni suggerite**: Utenti che possono svolgere il ruolo selezionato e che soddisfano i criteri per le assegnazioni avanzate. Per ulteriori informazioni, consulta [Panoramica delle assegnazioni intelligenti](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Altre assegnazioni**: Tutti gli utenti del sistema che possono svolgere il ruolo selezionato.

      >[!TIP]
      >
      >Nell’area Altre assegnazioni sono elencati solo i primi 50 utenti.
   Dopo aver selezionato un utente, in Workfront viene visualizzata una nota relativa al numero di elementi a cui verrà assegnato l’utente specificato e al ruolo che sostituirà.

   >[!TIP]
   >
   >Tutti i ruoli dell’utente vengono visualizzati nell’elenco, sotto il nome dell’utente.


1. Fai clic su **Assegna**.

   I ruoli specificati vengono sostituiti con gli utenti selezionati.

   Viene visualizzata una conferma del numero di elementi di lavoro a cui è stato sostituito il ruolo selezionato con l’utente selezionato.

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Sostituisci utente {#replace-user}

È possibile sostituire un utente già assegnato agli elementi di lavoro con un altro utente nei progetti selezionati.

Quando sostituisci un utente con un altro utente utilizzando le assegnazioni in blocco nel servizio di bilanciamento del carico di lavoro, si verificano le seguenti situazioni:

* L&#39;utente di sostituzione viene assegnato a tutti gli elementi di lavoro attualmente assegnati a un utente originale all&#39;interno dei progetti selezionati.

* Il nuovo utente non viene assegnato agli elementi di lavoro già contrassegnati come Completato.
* Se il ruolo associato al primo utente non corrisponde a nessuno dei ruoli del secondo utente, il secondo utente viene assegnato nel relativo ruolo primario.

Per sostituire un utente con un altro utente:

1. Inizia ad assegnare gli elementi di lavoro nel servizio di bilanciamento del carico di lavoro come descritto sopra e seleziona **Sostituisci**.
1. In **Utente attualmente assegnato** fare clic sulla freccia a discesa per scegliere da un elenco di utenti. Vengono visualizzati solo gli utenti attualmente assegnati a elementi di lavoro incompleti all’interno dei progetti specificati. Questo è un campo obbligatorio.

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. In **Utente da assegnare** fare clic sulla freccia a discesa per scegliere da un elenco di utenti consigliati o per digitare un altro nome utente. Gli utenti elencati nell’elenco per impostazione predefinita corrispondono ai criteri per le assegnazioni avanzate. Per ulteriori informazioni, consulta [Panoramica delle assegnazioni intelligenti](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront visualizza una nota sul numero di elementi in cui l’utente attualmente assegnato sostituirà il secondo utente e quali ruoli sostituirà.

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Fai clic su **Sostituisci**.

   Il primo utente selezionato viene sostituito dal secondo utente in tutti gli elementi di lavoro del progetto selezionato.

   Viene visualizzata una conferma del numero di elementi di lavoro per i quali l&#39;assegnazione utente originale è stata sostituita con il secondo utente selezionato.

### Revoca assegnazione utente {#unassign-user}

È possibile annullare l’assegnazione di un utente da tutti gli elementi di lavoro a cui l’utente è assegnato nei progetti selezionati.

Quando si annulla l’assegnazione di un utente da tutte le assegnazioni utilizzando le assegnazioni in blocco nel bilanciamento del carico di lavoro, si verificano le seguenti situazioni:

* L&#39;utente specificato viene rimosso da tutti gli elementi di lavoro a cui è assegnato.
* Se l’utente non assegnato è associato ai ruoli di lavoro, i ruoli di lavoro rimangono assegnati agli elementi di lavoro quando l’utente viene rimosso.

* Se l&#39;utente specificato viene assegnato agli elementi di lavoro completati, l&#39;utente rimane assegnato a tali elementi di lavoro.

Per ulteriori informazioni sulle assegnazioni di ruoli utente e processo, vedere [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Per annullare l&#39;assegnazione di un utente dagli elementi di lavoro nei progetti selezionati o per le attività o i problemi selezionati in cui sono assegnati:

1. Inizia ad assegnare gli elementi di lavoro nel servizio di bilanciamento del carico di lavoro come descritto sopra e seleziona **Annulla assegnazione**.

1. In **Utente da annullare l&#39;assegnazione** fare clic sulla freccia a discesa per scegliere da un elenco di utenti. Vengono visualizzati solo gli utenti attualmente assegnati a elementi di lavoro incompleti all’interno dei progetti specificati. Questo è un campo obbligatorio.

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   In Workfront viene visualizzata una nota sul numero di elementi in cui l’utente attualmente assegnato verrà disassegnato.

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Fai clic su **Annulla assegnazione**.\
   Viene visualizzata una conferma del numero di elementi di lavoro in cui l’utente specificato è stato rimosso.

 
