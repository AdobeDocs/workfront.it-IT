---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Panoramica delle aree di programmazione
description: Nelle sezioni seguenti viene descritto dove è possibile accedere all’area di pianificazione all’interno di Adobe Workfront, nonché alle funzionalità disponibili nell’area di pianificazione.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Panoramica delle aree di programmazione

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


Nelle sezioni seguenti viene descritto dove è possibile accedere all’area di pianificazione all’interno di Adobe Workfront, nonché alle funzionalità disponibili nell’area di pianificazione.

## Aree Workfront che consentono di pianificare le risorse

In Workfront puoi pianificare le risorse nelle seguenti aree:

* **Per tutti i progetti per i quali sei il gestore delle risorse** (dal **Pianificazione** Area) L&#39;area di programmazione in Workfront consente ai responsabili delle risorse di effettuare assegnazioni di risorse tra più progetti.

* **Per un singolo progetto quando sei membro del team del progetto** (dal **Pianificazione** area di un progetto):

   L&#39;area Programmazione all&#39;interno di un progetto consente ai membri del team del progetto di assegnare il lavoro del progetto agli utenti del team del progetto.

* **Per un singolo team sei membro di** (dal **Pianificazione** sezione del team) La sezione Pianificazione di un team consente ai membri del team di assegnare il lavoro già assegnato al team da più progetti a singoli membri del team.

## Funzionalità disponibile nell&#39;area Pianificazione

Nell&#39;area di pianificazione vengono visualizzate le attività e i problemi e le assegnazioni di risorse correnti.\
![resource_programmazione_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Strumenti di filtro e scambio](#filter-and-swap-tools)
* [Selezione data](#date-selection)
* [Area non assegnata](#unassigned-area)
* [Utenti e ruoli](#users-and-roles)
* [Timeline di programmazione](#scheduling-timeline)

### Strumenti di filtro e scambio {#filter-and-swap-tools}

* **Strumento filtro:** Consente di filtrare il contenuto visualizzato nella timeline della pianificazione. Per ulteriori informazioni sull’utilizzo dello strumento Filtro, consulta [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Strumento di scambio:** (Disponibile solo quando si pianificano risorse per progetti dalla scheda Pianificazione o Staffing) Consente di assegnare, sostituire o annullare rapidamente l’assegnazione degli utenti alle attività in più progetti. Per ulteriori informazioni, consulta [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Selezione data {#date-selection}

È possibile regolare l’intervallo di date per il quale i dati vengono visualizzati nella timeline di pianificazione. Per impostazione predefinita, l’intervallo di date è di 2 settimane (14 giorni consecutivi, compresi i fine settimana) a partire dal giorno corrente.

### Area non assegnata {#unassigned-area}

* [Quando si pianificano risorse come gestore risorse (per più progetti nell&#39;area Pianificazione)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Quando si pianificano risorse come membro del team del progetto (da un progetto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Quando si pianificano risorse come membro del team (da un team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Quando si pianificano risorse come gestore risorse (per più progetti nell&#39;area Pianificazione) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

La **Non assegnato** nella timeline della pianificazione vengono visualizzate solo le attività e i problemi che soddisfano tutti i seguenti criteri:

* Non assegnato a un utente.
* Non assegnato a un team.\
   Se l&#39;attività o il problema è assegnato a un team, viene comunque visualizzato nella **Non assegnato** area se l&#39;attività o il problema viene assegnato anche a un ruolo in aggiunta all&#39;assegnazione del team.\
   Se le attività o i problemi dispongono di assegnazioni di ruoli di lavoro aggiuntive non eseguite da un utente, vengono visualizzati anche.\
   Ad esempio, un’attività viene assegnata a 3 ruoli di lavoro: Designer, Product Manager e Developer. È possibile assegnare questa attività all’utente A che dispone di un ruolo di lavoro di Designer e all’utente B che dispone di un ruolo di responsabile del prodotto. In questo scenario, l&#39;attività è ancora visibile nell&#39;area Non assegnata nella timeline di pianificazione, in quanto il ruolo del lavoro Sviluppatore non viene assegnato a un utente.

#### Quando si pianificano risorse come membro del team del progetto (da un progetto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

La **Non assegnato** nella parte superiore della timeline della pianificazione vengono visualizzate le attività e i problemi che soddisfano i seguenti criteri:

* Associato al progetto ma non assegnato ad alcun utente del team di progetto.\
   Le attività associate al progetto e assegnate a un utente del team di progetto vengono visualizzate nella riga dell’utente a cui sono assegnate le attività.
* Associato al progetto ma assegnato a un membro che non fa parte del team del progetto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Quando si pianificano risorse come membro del team (da un team)** {#when-scheduling-resources-as-a-team-member-from-a-team}

La **Non assegnato** nella parte superiore della timeline della pianificazione vengono visualizzate le attività e i problemi che soddisfano i seguenti criteri:

* Assegnato al team e a nessun altro utente del team.\
   Le attività assegnate sia al team che a un utente del team vengono visualizzate nella riga dell&#39;utente a cui sono assegnate le attività.
* Assegnato sia al team che a un utente che non è membro del team.

### Utenti e ruoli {#users-and-roles}

* [Quando si pianificano risorse come gestore risorse (per più progetti nell&#39;area Pianificazione)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Quando si pianificano risorse come membro del team del progetto (da un progetto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Quando si pianificano risorse come membro del team (da un team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Quando si pianificano risorse come gestore risorse (per più progetti nell&#39;area Pianificazione) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Gli utenti idonei per l’assegnazione di una delle attività non assegnate si trovano sotto la sezione **Non assegnato** area. Gli utenti sono disponibili nella tempistica di pianificazione per l’assegnazione di un’attività o di un problema nelle seguenti circostanze:

* Per impostazione predefinita, gli utenti vengono visualizzati nella timeline della pianificazione solo quando dispongono di un ruolo di lavoro definito nel sistema (il ruolo di lavoro principale o secondario) e tale ruolo di lavoro corrisponde al ruolo di lavoro assegnato a un&#39;attività o a un problema attualmente visibile nel **Non assegnato** area sulla timeline della programmazione. È possibile disattivare questa funzionalità per consentire l&#39;assegnazione di attività e problemi a qualsiasi utente, indipendentemente dal fatto che l&#39;utente abbia un ruolo definito sul proprio profilo utente che corrisponda all&#39;assegnazione del ruolo dell&#39;attività o del problema a cui è assegnato. Per ulteriori informazioni, consulta [Consenti assegnazioni utente indipendentemente dal ruolo e dall&#39;appartenenza al gruppo nelle aree di programmazione](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Un utente e le attività assegnate all&#39;utente possono essere visualizzate più volte nella timeline di pianificazione se l&#39;utente dispone di più ruoli di lavoro designati nel sistema Workfront.\
   Gli utenti rimangono sulla timeline della pianificazione dopo aver ricevuto un’attività o un problema, anche se non vi sono altre attività o problemi con un’assegnazione di ruolo corrispondente. Questo consente di apportare le modifiche necessarie dopo l’assegnazione.\
   Se l&#39;attività non viene assegnata a un ruolo di lavoro, vengono visualizzati tutti gli utenti che soddisfano i requisiti del filtro. Per ulteriori informazioni sul filtro, vedi [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Sono stati designati nella **Utenti** nel campo **Filtro** scheda .\
   Per ulteriori informazioni sul filtro, vedi [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Quando si pianificano le risorse per un team (nella scheda Lavorazione), viene visualizzata anche l&#39;assegnazione del team.

Nella timeline vengono visualizzati anche tutti gli altri problemi o attività assegnati a tali utenti.

Puoi visualizzare il livello di allocazione degli utenti in un dato giorno, come descritto in [Gestione delle allocazioni utente nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Le attività che non dispongono almeno delle autorizzazioni di Contribute vengono visualizzate come una barra grigia nella timeline della programmazione.

#### Quando si pianificano risorse come membro del team del progetto (da un progetto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Ciascun membro del team viene sempre visualizzato nella timeline della programmazione, indipendentemente dalle assegnazioni dei ruoli degli utenti e dalle assegnazioni dei ruoli delle attività nell&#39;area Non assegnata.

Se un utente dispone di più ruoli di lavoro definiti nel sistema, l&#39;utente viene visualizzato più volte nella timeline di pianificazione quando viene soddisfatto uno dei seguenti criteri:

* Sono presenti attività o problemi visualizzati nel **Non assegnato** area assegnata ai ruoli di lavoro associati all’utente.
* Sono presenti attività o problemi nel progetto a cui sono stati assegnati ruoli di lavoro e tali attività o problemi vengono assegnati a un utente con tale ruolo definito nel sistema.

#### Quando si pianificano risorse come membro del team (da un team) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Ciascun membro del team viene sempre visualizzato nella timeline della programmazione, indipendentemente dalle assegnazioni dei ruoli degli utenti e dalle assegnazioni dei ruoli delle attività nell&#39;area Non assegnata.

Puoi visualizzare il livello di allocazione degli utenti in un dato giorno, come descritto in [Gestione delle allocazioni utente nelle aree di programmazione](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Attività per le quali non si dispone almeno delle autorizzazioni di Contribute da visualizzare come barra grigia nella timeline della programmazione.

### Timeline di programmazione {#scheduling-timeline}

* **Contenuto predefinito:** Per impostazione predefinita, tutte le attività che soddisfano i requisiti definiti nella sezione [Prerequisiti per attività e problemi](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) in [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) l’articolo su tutti i progetti con lo stato Corrente viene visualizzato nella timeline della pianificazione.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Per personalizzare ciò che viene visualizzato nella timeline della pianificazione, inclusa la visualizzazione di problemi e progetti con uno stato diverso, utilizza il filtro , come descritto in [Filtrare le informazioni nell&#39;area Pianificazione](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Per un determinato utente vengono visualizzate al massimo 10 attività al giorno. È possibile espandere l’elenco per visualizzare tutte le attività attualmente assegnate a tale utente.

* **Attività principali:** La visualizzazione delle attività principali nella timeline dipende da diverse impostazioni. Per ulteriori informazioni, vedere la sezione &quot;Configurare la visualizzazione delle attività principali sulla timeline di pianificazione&quot; nella sezione [Configurare le impostazioni nelle aree di programmazione](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) articolo.

* **Codifica del colore:** Le attività e i problemi nella timeline della pianificazione vengono codificati in base al colore del progetto a cui appartengono. Non puoi personalizzare il colore associato a un progetto specifico.

   Quando si pianifica il lavoro per i team (dalla scheda Staffing ), i colori vengono utilizzati solo se il valore **Mostra tutte le attività utente** è abilitata. Per ulteriori informazioni, consulta la sezione &quot;Configurare la visualizzazione delle attività principali nella timeline di pianificazione&quot; nella sezione [Configurare le impostazioni nelle aree di programmazione](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) articolo.

* **Durata attività:** Le durate delle attività sono rappresentate nella timeline di ogni attività (l’attività si estende fisicamente per il numero di giorni uguali alla durata). Non è possibile regolare la durata dell&#39;attività dalla timeline di pianificazione.

* **Ora di disattivazione:** Il tempo di inattività è rappresentato nella timeline della programmazione da un indicatore grigio chiaro nella colonna del giorno per il quale è pianificato il tempo di inattività per un determinato utente.\
   Per ogni utente viene configurato il time off in base alle seguenti informazioni:

   Calendario personale dell&#39;utente. Per ulteriori informazioni sul calendario di timeout personale, vedi [Configurare l’ora personale di inattività in Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   La pianificazione assegnata all&#39;utente. Questa potrebbe essere la pianificazione predefinita o personalizzata. Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Fine settimana:** I fine settimana sono rappresentati nella timeline della programmazione come ombreggiatura grigia chiara nei sabati e la domenica. I giorni della settimana impostati come fine settimana nella timeline della pianificazione non sono configurabili. È possibile pianificare gli utenti per il lavoro durante il fine settimana.
