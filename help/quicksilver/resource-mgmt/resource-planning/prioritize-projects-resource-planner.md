---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Assegnare priorità ai progetti nel planner risorse
description: I progetti sono elencati in ordine di priorità nel Planner risorse con il progetto più importante nella parte superiore.
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# Assegnare priorità ai progetti nel planner risorse

I progetti sono elencati in ordine di priorità nel Planner risorse con il progetto più importante nella parte superiore.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Modifica priorità e ore di budget nel Planner risorse</p> <p>Modificare l’accesso a Dati finanziari, Progetti e Utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti per i quali si desidera assegnare il budget alle informazioni con la possibilità di gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Ordine predefinito dei progetti nel Planner risorse

Per impostazione predefinita, i progetti sono elencati nella Vista progetto del Planner risorse tenendo conto dei criteri riportati di seguito.

>[!IMPORTANT]
>
>I progetti vengono elencati in base ai tre criteri seguenti solo la prima volta che si apre il Planner risorse. Tuttavia, questa priorità predefinita diventa automaticamente la priorità personalizzata e non può essere ripristinata alla priorità originale ogni volta che si esegue una delle seguenti operazioni:
>
>* Quando fai clic su Salva in qualsiasi momento.
>* Quando si modifica manualmente la priorità di pianificazione del progetto. Per informazioni sulla modifica manuale della priorità di pianificazione del progetto, consulta la sezione [Modificare manualmente la priorità di pianificazione del progetto](#manually-change-the-project-planning-priority) in questo articolo.
>
>Una volta che la priorità del progetto diventa la priorità personalizzata, eventuali modifiche nelle informazioni del progetto non influiscono più sull’ordine dei progetti che utilizzano questi criteri. In seguito, puoi assegnare priorità ai progetti solo manualmente.

I criteri predefiniti originali per elencare i progetti nella visualizzazione Progetto sono i seguenti, in questo ordine:

1. Punteggio di allineamento sul progetto.\
   Per ulteriori informazioni sul punteggio di allineamento del progetto, consulta [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. In base alla data di inizio prevista del progetto (se il campo Allineamento è nullo o corrisponde a più progetti).
1. Alfabeticamente (se il campo Allineamento è null o è lo stesso e la data di inizio pianificato è la stessa per diversi progetti).

Quando si lavora con le priorità del progetto nel Planner risorse, tenere presente quanto segue:

* Puoi personalizzare manualmente la priorità del progetto solo quando applichi la visualizzazione Progetto. Viene inoltre modificato l’ordine dei progetti nel Planner risorse.
* Quando si applicano le visualizzazioni Ruolo o Utente nel Planner risorse, i progetti vengono visualizzati nello stesso ordine di priorità stabilito nella visualizzazione Progetto.
* L’ordine dei progetti nel Planner risorse è univoco per te. Altri utenti possono visualizzare gli stessi progetti nel Planner risorse, ma in un ordine diverso. Non è possibile creare rapporti sul campo Priorità pianificazione progetto. Questo è visibile solo nel Planner risorse e funge da flag per assegnare la priorità ai progetti.

I progetti associati a un portfolio possono avere una priorità a livello di portfolio. È possibile abilitare la visualizzazione della priorità del portfolio di un progetto nel Planner risorse, oltre alla priorità Planner risorse. Puoi anche ordinare i progetti in base alla loro priorità di portafoglio.

## Modificare manualmente la priorità di pianificazione del progetto {#manually-change-the-project-planning-priority}

Per riordinare i progetti in Resource Planner è necessario disporre dell&#39;accesso Modifica a Gestione risorse e delle autorizzazioni Gestione risorse per i progetti.

Attribuendo ai progetti una nuova priorità, puoi classificarli in ordine di importanza.

Per modificare la priorità di pianificazione del progetto:

1. Vai a **Planner risorse**.

1. Fare clic all&#39;interno del campo a sinistra del nome del progetto che contiene un numero e immettere un numero per modificare la priorità di pianificazione, quindi premere Invio.\
   ![](assets/mceclip4.png)\
   Oppure\
   Passa il puntatore del mouse sul nome del progetto e fai clic sull’indicatore a sinistra del nome del progetto, trascinalo e rilascialo nel punto corretto per modificare la priorità.

   ![drag_and_drop_projects_RP_1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Quando selezioni i numeri per assegnare priorità ai progetti, seleziona i numeri più bassi per le priorità più importanti e quelli più alti per le priorità più basse (meno importanti). Quando si modifica il numero di priorità di un progetto in un numero inferiore (priorità più elevata), tutti gli altri progetti nel Planner risorse vengono spostati verso il basso nell’elenco (diventano meno importanti).\
   Quando si modifica il numero di priorità di un progetto in un numero maggiore (priorità inferiore), tutti gli altri progetti nel Planner risorse vengono inseriti nell’elenco (diventano più importanti).

1. Fai clic su **Salva**.\
   L’ordine dei progetti cambia in base alle selezioni effettuate e questo diventa la priorità del progetto personalizzato nel Planner risorse. Altri utenti non possono visualizzare l&#39;ordine di priorità dei progetti nel Planner risorse, anche se potrebbero visualizzare gli stessi progetti nei rispettivi Planner risorse.

## Ordinare i progetti in base alla priorità Portfolio nel planner risorse

>[!IMPORTANT]
>
>La tua azienda deve disporre di un piano Business o Workfront superiore per assegnare la priorità ai progetti in Portfoli Optimizer.
>
>Per ulteriori informazioni sui piani Workfront, vedi [I nostri piani](https://www.workfront.com/plans).
>
>Per informazioni sulla priorità dei progetti in Portfoli Optimizer, vedi [Assegnare priorità ai progetti in Portfoli Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Apri **Planner risorse** in **Visualizzazione progetto**.
1. Fai clic sul pulsante **Impostazioni** icona.
1. Abilita la **Visualizzare le priorità del Portfolio** impostazione per visualizzare le priorità del progetto in base al Portfolio a cui sono assegnate. La priorità dei progetti in base al loro portfolio viene visualizzata accanto alla priorità Planner risorse. Questa impostazione è disabilitata per impostazione predefinita.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Le priorità del portfolio dei progetti vengono visualizzate solo nella vista Progetto del Planner risorse.

1. Fai clic su **Ordine** ordinare i progetti in base alle priorità del portafoglio.

   Se disponi di progetti che appartengono a più di un portfolio, puoi visualizzare più progetti con la stessa priorità del portfolio nel Planner risorse. In questo caso, i progetti con la stessa priorità di portafoglio sono elencati in base ai seguenti criteri, in questo ordine:

   1. Punteggio dell&#39;Allineamento
   1. Data di inizio pianificata
   1. Nome progetto

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. Fai clic su **Salva**.

## L&#39;effetto della modifica della priorità di pianificazione del progetto sulle ore disponibili per l&#39;utente

La priorità di pianificazione del progetto influisce sulle ore disponibili degli utenti. Gli utenti associati al progetto con priorità più elevata mostrano la disponibilità massima per la colonna Ore disponibili (AVL) per il progetto, in base alle loro pianificazioni.

Gli stessi utenti associati al secondo progetto in ordine di priorità mostreranno un valore Orari disponibili che rappresenta la differenza tra l’intero importo di Ore disponibili e quello già preventivato per il primo progetto nella colonna Orari a budget e così via. Per informazioni sulle risorse di budget nel Planner risorse, vedere [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Se per un utente non sono state previste ore in budget per il primo progetto (in ordine di priorità), ma per il secondo progetto sono state previste ore in budget per lo stesso utente, l’utente mostrerà l’intera quantità di ore disponibili per entrambi i progetti.

Si consiglia di aggiornare la colonna Orari a budget per gli utenti nell’ordine dei progetti nel Planner risorse, in modo da visualizzare in modo preciso le ore disponibili per l’utente in qualsiasi momento.

>[!NOTE]
>
>Poiché la priorità di pianificazione del progetto è univoca per ogni gestore di risorse, il secondo progetto prioritario potrebbe essere un primo progetto prioritario per un altro utente che visualizza gli stessi progetti nel relativo planner risorse. Se un altro gestore di risorse esegue il budget di una risorsa per il primo progetto, le ore disponibili diminuiranno per la risorsa per il primo progetto in base a tale modifica.
>
>L’utente che calcola il budget delle ore assegna prima tale risorsa e riduce il numero di ore disponibili per tale risorsa in tutto il sistema. La quantità di ore disponibili deve essere aggiornata per tutti gli utenti non appena le ore previste vengono salvate per una risorsa nel planner risorse.
>
>Per ulteriori informazioni sulle ore disponibili, consulta [Disponibilità e assegnazione delle risorse](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
