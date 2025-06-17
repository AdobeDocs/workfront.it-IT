---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica sulla navigazione di Programmazione delle risorse
description: La pianificazione delle risorse di Adobe Workfront consente di comprendere facilmente la disponibilità delle risorse e il tempo pianificato necessario per completare il lavoro sui progetti. Puoi quindi gestire l’allocazione degli utenti e delle loro mansioni sui progetti a cui sono assegnati.
author: Lisa
feature: Resource Management
exl-id: 5a1be723-e3ac-443a-9c09-85e8839fcbef
source-git-commit: af7789f3a4c7443854639fd60bcf0661217b37ae
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 2%

---

# Panoramica sulla navigazione di Pianificazione risorse

<!-- Audited: 5/2025 -->

Adobe Workfront Resource Planner consente di comprendere facilmente la disponibilità delle risorse e il tempo pianificato necessario per completare il lavoro sui progetti. Puoi quindi gestire l’allocazione degli utenti e delle loro mansioni sui progetti a cui sono assegnati.

>[!TIP]
>
>Non è possibile gestire l&#39;allocazione dei team sulle attività a cui sono assegnati nella Programmazione delle risorse.

Devi soddisfare i prerequisiti necessari per utilizzare completamente la Programmazione delle risorse. Per ulteriori informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

![Pianificazione risorse](assets/resource-planner-overview.png)

Le sezioni seguenti descrivono tutte le aree della Programmazione delle risorse.

## Timeline dei progetti

![Calendario sequenza temporale](assets/calendar-months.png)


Utilizza il calendario nella parte superiore della Programmazione delle risorse per spostarti nella timeline dei progetti che stai visualizzando. Per impostazione predefinita, la timeline inizia con il mese corrente.

Per ulteriori informazioni sulla modifica dell&#39;intervallo di tempo dell&#39;indicatore cronologico visualizzato nella Programmazione delle risorse, vedere la sezione [Selezione dell&#39;intervallo di tempo](#timeframe-selection) in questo articolo.

## Selezione dell’intervallo temporale  {#timeframe-selection}

![Selezione intervallo temporale](assets/timeframe-selection.png)

Per impostazione predefinita, la Programmazione delle risorse mostra le informazioni sulle risorse per 3 o 4 mesi alla volta, a partire dal mese corrente. Il numero di periodi di tempo visualizzati dipende dalla larghezza dello schermo.

>[!TIP]
>
>Nella pianificazione risorse non è possibile visualizzare più di 4 periodi di tempo alla volta.

Per spostarsi nella timeline, fate clic sulle frecce avanti e indietro per spostarvi avanti e indietro. È quindi possibile selezionare una delle seguenti opzioni di intervallo di date nella Programmazione delle risorse facendo clic sui pulsanti appropriati:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Settimana</td> 
      <td>Visualizza le informazioni per settimana.<br>Il numero della settimana viene visualizzato accanto alle date nell'intestazione della colonna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mese</td> 
      <td> Visualizza le informazioni per mese.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trimestre</td> 
      <td>Visualizza le informazioni per trimestre.<br>Il numero del trimestre viene visualizzato accanto alle date nell'intestazione della colonna.<br>I trimestri personalizzati non vengono visualizzati nella Programmazione delle risorse. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Oggi</td> 
      <td>Torna al mese, alla settimana o al trimestre odierno.</td> 
     </tr> 
    </tbody> 
   </table>

## Selezione della vista Progetto/Ruolo/Utente

![Visualizza per progetto, ruolo o utente](assets/view-by-drop-down.png)

È possibile modificare la visualizzazione nella Programmazione delle risorse in base alla modalità di visualizzazione delle informazioni.

Per impostazione predefinita, la Programmazione delle risorse viene visualizzata nella Vista utente. È possibile modificare la visualizzazione in Visualizzazioni progetto o Ruolo. Quando la si modifica in un&#39;altra visualizzazione, la scelta diventa la visualizzazione predefinita.

Quando si modifica la vista, vengono modificate anche le seguenti informazioni:

* La gerarchia degli oggetti (informazioni nelle righe della Programmazione delle risorse).
* Le informazioni sull&#39;allocazione delle ore (informazioni nelle colonne della Programmazione delle risorse).

  Per ulteriori informazioni sulla visualizzazione delle colonne nella Programmazione delle risorse in base alla visualizzazione selezionata, vedere [Verificare la disponibilità e l&#39;allocazione delle risorse mediante la Programmazione delle risorse di Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Per visualizzare informazioni accurate in Pianificazione risorse, devi soddisfare una serie di prerequisiti. Per ulteriori informazioni sui prerequisiti, vedere la sezione Prerequisiti per l&#39;utilizzo della pianificazione delle risorse nell&#39;articolo [Panoramica sulla pianificazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Per modificare la visualizzazione nella Programmazione delle risorse, selezionare una delle visualizzazioni seguenti nel menu a discesa Visualizza per:

* [Visualizza per progetto](#view-by-project)
* [Visualizza per ruolo](#view-by-role)
* [Visualizza per utente](#view-by-user)

### Visualizza per progetto {#view-by-project}

Quando selezioni la Vista progetto nella Programmazione risorse, tieni presente quanto segue:

* Puoi visualizzare i progetti per i quali disponi delle autorizzazioni di visualizzazione.
* Quando accedi alla Programmazione delle risorse per la prima volta, puoi vedere i progetti filtrati dal Filtro predefinito.\
  Per ulteriori informazioni, vedere [Informazioni sul filtro nella pianificazione risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).

* Il numero di elementi visualizzati o che è possibile esportare dalla visualizzazione Progetto è limitato per migliorare le prestazioni.\
  Per ulteriori informazioni, vedere la sezione Limitazioni nella visualizzazione del progetto nell&#39;articolo [Limitazioni di visualizzazione di Programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

* I progetti sono elencati in ordine di priorità nella visualizzazione Progetto.\
  Per ulteriori informazioni, vedere la sezione [Priorità di pianificazione del progetto](#project-planning-priority) in questo articolo.

* Man mano che espandi ciascun progetto, puoi visualizzare le mansioni associate.

* Espandendo ogni ruolo, è possibile visualizzare gli utenti ad esso associati. Scorri per caricare più ruoli e utenti in ciascun progetto.

* Quando si applica questa visualizzazione, la somma di Ore ruolo, FTE o Costo corrisponde alle ore progetto, FTE o Costo.

* Nella vista Progetto è possibile visualizzare le seguenti informazioni su ore, FTE o Costo:

   * Disponibile
   * Pianificato
   * Preventivato
   * Varianza
   * Netto

     Per ulteriori informazioni, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

### Visualizza per ruolo {#view-by-role}

Quando si seleziona la Vista ruolo nella Programmazione risorse, tenere presente quanto segue:

* È necessario disporre almeno dell&#39;accesso di visualizzazione a Gestione risorse e delle autorizzazioni di visualizzazione per i progetti per visualizzare i ruoli associati a tali progetti.
* Puoi espandere ogni ruolo per visualizzare un elenco di progetti e ogni progetto per visualizzare un elenco di utenti che possono svolgere tali ruoli nei progetti.
* Per migliorare le prestazioni, il numero di elementi visualizzati o che è possibile esportare dalla Vista ruolo è limitato.\
  Per ulteriori informazioni, vedere la sezione Limitazioni nella visualizzazione Ruolo in [Limitazioni di visualizzazione di Programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

* I progetti sono elencati nel Ruolo nello stesso ordine di priorità in cui sono elencati nella Vista Progetto.
* Quando si applica questa visualizzazione, la somma di Ore progetto, FTE o Costo corrisponde alle ore ruolo, FTE o Costo.
* Nella vista Ruolo è possibile visualizzare le seguenti informazioni su ore, FTE o Costo:

   * Disponibile
   * Pianificato
   * Preventivato
   * Varianza
   * Netto

     Per ulteriori informazioni, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

### Visualizza per utente {#view-by-user}

È possibile visualizzare la Pianificazione risorse nella Vista utente per comprendere la differenza tra le Ore pianificate e le Ore o FTE disponibili per gli utenti o per visualizzare la quantità di Ore effettive registrate.

Non è possibile preventivare le risorse quando si applica la Vista utente alla Programmazione risorse. È necessario preventivare le risorse utilizzando le viste Progetto o Ruolo e utilizzare la vista Utente per verificare l&#39;allocazione e la disponibilità degli utenti in relazione al lavoro pianificato.

La Vista utente è la vista predefinita della Programmazione delle risorse.

Quando selezioni la Vista utente nella Programmazione risorse, tieni presente quanto segue:

* Puoi visualizzare tutti gli utenti per i quali disponi delle autorizzazioni di visualizzazione, fino a 2.000 utenti, che sono attivi e hanno effettuato l’accesso ad Adobe Workfront almeno una volta. Filtra l’elenco degli utenti per team, mansione o pool per visualizzare gli utenti associati solo a tali entità.
* Se l&#39;elenco degli utenti è stato filtrato in base ai progetti, è possibile espandere solo gli utenti associati ai progetti filtrati e visualizzare le informazioni sulle ore.\
  Per ulteriori informazioni, vedere [Informazioni sul filtro nella pianificazione risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).

* Per migliorare le prestazioni, il numero di elementi visualizzati o che è possibile esportare dalla visualizzazione utente è limitato.\
  Per ulteriori informazioni, vedere la sezione Limitazioni nella visualizzazione utente in [Limitazioni di visualizzazione della programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

* I progetti sono elencati con il nome dell&#39;utente nello stesso ordine di priorità in cui sono elencati nella visualizzazione Progetto.\
  Per ulteriori informazioni, vedere la sezione [Priorità di pianificazione del progetto](#project-planning-priority) in questo articolo.

* Se agli utenti non è associata alcuna mansione, i valori di Ore o FTE sono elencati nella sezione Nessun ruolo.
* Quando questa visualizzazione viene applicata, la somma delle ore progetto o FTE corrisponde alle ore utente o FTE.

  >[!TIP]
  >
  >Non è possibile visualizzare l&#39;allocazione e la disponibilità degli utenti in base al costo nella visualizzazione utente.

* Le autorizzazioni di progetto e attività determinano ciò che viene visualizzato sotto i nomi degli utenti visualizzati nella Visualizzazione utente.

  Esistono i seguenti scenari:

   * Se non disponi delle autorizzazioni necessarie per visualizzare i progetti e le attività o i problemi assegnati agli utenti visualizzati nella Programmazione delle risorse, tali elementi sono elencati nelle sezioni Elementi inaccessibili. In questo caso, queste sezioni sostituiscono le sezioni Progetto o Attività.

   * Se non disponi delle autorizzazioni necessarie per visualizzare i progetti, ma puoi accedere per visualizzare le attività o i problemi relativi, i progetti, le attività e i problemi vengono elencati con i nomi degli utenti a essi assegnati.
   * Se disponi delle autorizzazioni necessarie per visualizzare i progetti, ma non le attività o i problemi relativi, viene visualizzato il nome del progetto e le attività e i problemi sono elencati nella sezione Elementi inaccessibili.

     Per ulteriori informazioni, vedere [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).


* Nella vista Utente è possibile visualizzare le seguenti informazioni sull&#39;ora e sull&#39;FTE:

   * Disponibile
   * Pianificato
   * Effettivo
   * Differenza tra Pianificato ed Effettivo
   * Percentuale di allocazione pianificata

     Per ulteriori informazioni, vedere [Visualizza ore disponibili, pianificate ed effettive o FTE nella pianificazione risorse quando si utilizza la visualizzazione utente](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)

## Nome progetto

Puoi visualizzare i seguenti progetti nella Programmazione delle risorse:

* Progetti per i quali disponi delle autorizzazioni di visualizzazione. Devi anche avere accesso a Visualizza gestione risorse nel tuo livello di accesso.

  Per informazioni, vedere [Accesso necessario per preventivare le risorse in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Progetti limitati dal filtro applicato alla pianificazione risorse.

  Per ulteriori informazioni, vedere [Informazioni sul filtro nella pianificazione risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  >[!NOTE]
  >
  >È consigliabile utilizzare i filtri per ridurre il numero di progetti visualizzati nella Programmazione delle risorse.

## Priorità pianificazione progetto {#project-planning-priority}

I progetti sono elencati in ordine di priorità nella Programmazione delle risorse, con il progetto più importante in alto. La priorità è indicata da un numero davanti al nome del progetto.

![Priorità pianificazione progetto](assets/project-ranking.png)

Puoi anche abilitare un’impostazione per visualizzare le priorità dei progetti in base ai loro portfolio quando sono associati a un portfolio. Per informazioni, vedere [Assegnare priorità ai progetti nella Programmazione delle risorse](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

## Nome Ruolo

Nella pianificazione risorse sono elencate le seguenti categorie di mansioni:

* Ruoli assegnati alle attività.
* I ruoli che non sono assegnati ad attività, ma che sono i ruoli principali degli utenti associati ai pool di risorse dei progetti.
* I ruoli secondari degli utenti assegnati alle attività in tali ruoli.
* Ruoli secondari di utenti che dispongono di una percentuale valida di disponibilità FTE nel proprio profilo.\
  Per ulteriori informazioni sulla percentuale di disponibilità FTE per le mansioni, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>I ruoli assegnati ai problemi vengono elencati anche quando l’impostazione Includi ore da problema è abilitata. Per ulteriori informazioni sull&#39;abilitazione delle ore di problema nella Programmazione delle risorse, consulta la sezione [Impostazioni](#settings).

## Nome utente

Gli utenti elencati nelle visualizzazioni Progetto e Ruolo nella Programmazione delle risorse appartengono ai gruppi di risorse associati ai progetti.\
Per ulteriori informazioni, vedere [Associare i pool di risorse agli utenti](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

Tutti gli utenti che hai accesso alla visualizzazione e che hanno effettuato l’accesso a Workfront almeno una volta vengono visualizzati nella visualizzazione utente.

Nelle visualizzazioni Progetto e Ruolo, gli utenti possono essere elencati nei seguenti tipi di ruoli:

* Il loro ruolo principale
* Il loro ruolo secondario, nei seguenti scenari:

   * Se il ruolo secondario dispone di un numero valido per la percentuale di disponibilità FTE nel profilo utente.
   * Se l’utente è assegnato ad attività in tali ruoli.
Per ulteriori informazioni sulla percentuale di disponibilità FTE per una mansione, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nessuna sezione Ruolo e Nessuna sezione Utente

### Nessuna sezione Ruolo  {#no-role-section}

Quando un utente appartiene a un pool di risorse associato a un progetto, ma non ha una mansione associata, viene visualizzato nella sezione Nessun ruolo invece di sotto un ruolo specifico.

Non è possibile preventivare le ore per un utente in una sezione Nessun ruolo. L&#39;utente deve avere almeno una mansione associata a lui per essere preventivato per il lavoro.


### Nessuna sezione utente  {#no-user-section}

Quando si assegna un&#39;attività a un team o si lascia l&#39;attività non assegnata, le ore pianificate vengono visualizzate nella sezione Nessun utente, che viene visualizzata nella sezione Nessun ruolo della Programmazione delle risorse. Queste attività non vengono visualizzate nella Programmazione delle risorse quando si utilizza la visualizzazione Visualizza per utente.

È possibile visualizzare la quantità di ore pianificate attribuite alle attività del progetto nella sezione Nessun utente della Pianificazione risorse, ma non è possibile eseguire il budget per queste allocazioni.

![Nessuna sezione utente](assets/no-user.png)

## Filtri

Utilizzando i filtri, puoi limitare le informazioni visualizzate nella Programmazione delle risorse.

![Pulsante Filtro](assets/filter-button.png)

Per ulteriori informazioni sul filtro in Pianificazione risorse, vedere [Informazioni sul filtro in Pianificazione risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

## Impostazioni {#settings}

Nell&#39;area Impostazioni è possibile attivare o disattivare le opzioni per visualizzare o nascondere le informazioni nella Programmazione delle risorse. Per aprire la finestra di dialogo Impostazioni di programmazione delle risorse, fare clic sull&#39;icona Impostazioni nell&#39;angolo superiore destro della pagina.

![Icona delle impostazioni di Programmazione delle risorse](assets/settings-icon.png)

Da qui, puoi abilitare una o entrambe le seguenti impostazioni:

* **Includi ore da problemi**: vengono visualizzate le ore pianificate da problemi.

  Quando abiliti questa impostazione, considera quanto segue:

   * Il nome dell’utente assegnato ai problemi viene visualizzato nella mansione ad essi associata sul problema. È possibile specificare le ore preventivate per l&#39;utente e la mansione nelle visualizzazioni Progetto e Ruolo.
   * I problemi a cui sono assegnati gli utenti sono elencati sotto i nomi delle mansioni nella vista Utente.

     >[!IMPORTANT]
     >
     >Quando le date di inizio pianificato e di completamento del problema sono al di fuori della timeline del progetto, le ore pianificate per il problema vengono visualizzate in base alle date del problema. Ad esempio, se la timeline del progetto è compresa tra gennaio e marzo, ma la timeline dei problemi è in agosto, le ore pianificate per i problemi vengono visualizzate nel periodo di agosto.


* **Visualizza priorità Portfolio**: visualizza le priorità del progetto in base al Portfolio a cui sono assegnate.

  Per informazioni sull&#39;assegnazione delle priorità ai progetti nella Programmazione delle risorse, vedere [Assegnare priorità ai progetti nella Programmazione delle risorse](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).


  ![Impostazioni di programmazione delle risorse](assets/resource-planner-settings.png)

## Opzione a schermo intero

Puoi visualizzare la Programmazione delle risorse a schermo intero per aumentare la quantità di informazioni che puoi visualizzare sullo schermo. Questa opzione è disponibile per tutte le viste.

Per visualizzare la Programmazione delle risorse a schermo intero, fai clic sull’icona Schermo intero nell’angolo in alto a destra della pagina.

![RP_sull_sccreen_area_User_View__1_.png](assets/rp-full-screen-icon-highlighted-user-view--350x260.png)

Una volta espansa la schermata, puoi fare clic sull’icona Chiudi schermo intero per tornare alla visualizzazione precedente.

## Opzione di esportazione

![Pulsante Esporta](assets/export-button-highlighted-resource-planner-350x92.png)

È possibile esportare le informazioni in un file di Excel (.xlsx) da qualsiasi visualizzazione della Programmazione delle risorse.

Per informazioni sull&#39;esportazione di informazioni dalla Programmazione delle risorse, vedere [Esportare informazioni dalla Programmazione delle risorse](../../resource-mgmt/resource-planning/export-resource-planner.md).

Puoi gestire la quantità di informazioni e la visualizzazione del file esportato.

Per informazioni sulle informazioni esportabili dalla Programmazione delle risorse e su come gestire l&#39;aspetto del file esportato, vedere [Limitazioni di visualizzazione della Programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).
