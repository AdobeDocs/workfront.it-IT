---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione
description: Utilizzando la timeline di programmazione, è possibile gestire le assegnazioni utente, oltre a specificare il tempo assegnato a ciascun utente per un elemento di lavoro.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione

>[!IMPORTANT]
>  
><span class="preview">La funzionalità di pianificazione descritta in questo articolo è stata rimossa e rimossa da Adobe Workfront a partire dalla versione 23.1 di gennaio 2023.   </span>
>  
> <span class="preview"> Questo articolo verrà rimosso anche poco dopo la versione 23.1, all’inizio del 2023. Al momento, è consigliabile aggiornare di conseguenza tutti i segnalibri. </span>
> 
><span class="preview"> Ora puoi utilizzare il servizio di bilanciamento del carico di lavoro per pianificare il lavoro per le risorse. </span>
>  
> <span class="preview">Per informazioni sulla pianificazione delle risorse tramite il servizio di bilanciamento del carico di lavoro, consulta la sezione . [Il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Utilizzando la timeline di programmazione, è possibile gestire le assegnazioni utente, oltre a specificare il tempo assegnato a ciascun utente per un elemento di lavoro.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Accesso a progetti, attività e problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per progetti, attività e problemi</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti prima dell’assegnazione di attività e problemi nella cronologia di programmazione

Prima di iniziare a gestire le assegnazioni utente come descritto in questa sezione, acquisisci familiarità con il funzionamento della pianificazione delle risorse in Workfront, come descritto in [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Per gestire con successo le assegnazioni utente come descritto in questa sezione, è innanzitutto necessario assicurarsi che l&#39;utente, i progetti e le attività e i problemi soddisfino i prerequisiti descritti in [Prerequisiti per l’utilizzo degli strumenti di pianificazione in Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) sezione dell&#39;articolo [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Nelle sezioni seguenti viene descritto come modificare le assegnazioni utente manualmente, automaticamente o scambiando le assegnazioni in base all&#39;utente o al ruolo.

## Assegnazione manuale di attività o problemi non assegnati agli utenti

La timeline della pianificazione fornisce la visibilità necessaria per consentire agli utenti di completare l’attività o il problema.\
Per ulteriori informazioni sulla timeline della programmazione, vedi [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

È possibile assegnare singole attività e problemi agli utenti nella timeline della pianificazione dalle seguenti aree di Workfront:

* La sezione Pianificazione in Origine (quando si pianificano risorse per più progetti).
* La sezione Programmazione in un progetto (quando si pianificano le risorse per un singolo progetto).
* La sezione Pianificazione in un team (durante la pianificazione delle risorse per un team).

Le informazioni visualizzate nell&#39;area non assegnata nella parte superiore della cronologia della pianificazione variano a seconda dell&#39;area di Workfront in cui si utilizza la pianificazione delle risorse (dalla sezione Pianificazione (quando si pianificano risorse per più progetti), dalla sezione Pianificazione (quando si pianificano risorse per un singolo progetto) o dalla sezione Pianificazione (quando si pianificano risorse per un team). Per ulteriori informazioni, consulta la sezione . [Funzionalità disponibile nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) nell&#39;articolo [Panoramica delle aree di programmazione](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

A seconda dell’area di Workfront in cui viene visualizzata la timeline della pianificazione, solo alcuni utenti possono essere autorizzati a lavorare. Per ulteriori informazioni, consulta [Panoramica delle aree di programmazione](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Per assegnare le attività o i problemi non assegnati agli utenti nella timeline della pianificazione:

1. Passa alla timeline della programmazione per più progetti, per un singolo progetto o per un team:

   * **Per progetti multipli**:  Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
   * **Per un singolo progetto**: Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.
   * **Per un team**: Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Team**, seleziona un team e fai clic su **Bilanciamento del carico di lavoro** nel pannello a sinistra, seleziona **Pianificazione** dal menu a discesa in alto a sinistra.

   ![programmazione_contours.png](assets/scheduling-contours-350x139.png)

1. (Facoltativo) Crea un filtro per personalizzare il contenuto visualizzato nella timeline della pianificazione, come descritto in [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Ad esempio, per visualizzare i problemi nella timeline della pianificazione, devi creare un filtro.

1. (Facoltativo) Modifica l’intervallo di date visualizzato nella timeline della pianificazione, come descritto in [Regola l&#39;intervallo di date delle aree di programmazione](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Per assegnare un&#39;attività o un problema non assegnato, procedere come segue:

   * Trascinare l&#39;attività o il problema nella riga dell&#39;utente che si desidera assegnare.\
      Per un determinato utente vengono visualizzate al massimo 10 attività al giorno. È possibile espandere l’elenco per visualizzare tutte le attività attualmente assegnate a tale utente. (Dopo aver effettuato le assegnazioni nella tempistica di programmazione, potrebbero essere visualizzate temporaneamente più di 10 attività.)\
      Quando si trascina un elemento, vengono visualizzate le seguenti informazioni prima di rilasciare l&#39;attività o il problema e di completare l&#39;assegnazione:

   * Se le allocazioni degli utenti sono abilitate nella sequenza temporale di programmazione, gli indicatori di sovrallocazione rossi vengono visualizzati se il completamento dell&#39;assegnazione determina una sovrallocazione dell&#39;utente.\
      Per ulteriori informazioni sugli indicatori di sovrallocazione, consulta la sezione [Indicatori di allocazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) nell&#39;articolo [Gestione delle allocazioni utente nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Se la **Limitare le assegnazioni agli utenti con un ruolo corrispondente** nell’area Impostazioni è attivata l’opzione , gli utenti che non sono idonei a ricevere l’assegnazione sono disattivati. Se questa opzione è disabilitata, tutti gli utenti possono ricevere l&#39;assegnazione. L’opzione è attivata per impostazione predefinita.\
      Per ulteriori informazioni su questa opzione, consulta [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [Consenti assegnazioni utente indipendentemente dal ruolo e dall&#39;appartenenza al gruppo nelle aree di programmazione](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      Un indicatore di rilascio viene visualizzato nella riga dell’utente. Questo consente di vedere dove viene assegnato un elemento prima di eseguire l&#39;assegnazione.

      Espandi l’attività o il problema che desideri assegnare, fai clic sulla freccia a discesa nel **Assegnazioni** inizia a digitare il nome dell&#39;utente che desideri assegnare, quindi fai clic sul nome dell&#39;utente nell&#39;elenco a discesa.\
      ![schedario_task_espanso.png](assets/schedule-task-expanded-350x170.png)

1. (Condizionale) Dopo aver assegnato un&#39;attività o un problema non assegnato a un utente, è possibile modificare le assegnazioni esistenti per le attività e i problemi tra gli utenti nella sequenza temporale di programmazione. Quando si pianificano risorse per i progetti (nella scheda Pianificazione o nella scheda Staffing ), solo gli utenti con lo stesso ruolo possono ricevere l&#39;assegnazione.\
   Per riassegnare un’attività o un problema a un altro utente, trascina l’attività dalla riga di un utente alla riga di un altro utente.
1. (Facoltativo) Configura il numero di ore in cui ogni utente assegnato viene assegnato all&#39;attività o al problema, come descritto in [Gestione delle allocazioni utente nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
