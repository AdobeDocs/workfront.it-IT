---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Richiedi accesso agli oggetti
description: La visibilità degli oggetti in Adobe Workfront dipende dall’accesso a quel tipo di oggetto e dalle autorizzazioni per un singolo oggetto.
author: Becky
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 18b96a6d57dc358bfe52e813bc98d8eb19f37dba
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 1%

---

# Richiedi accesso agli oggetti

<!-- Audited: 4/2025 -->

La visibilità degli oggetti in Adobe Workfront dipende dall’accesso a quel tipo di oggetto e dalle autorizzazioni per un singolo oggetto.

>[!NOTE]
>
>Questo articolo descrive come richiedere le autorizzazioni per tutti gli oggetti ad eccezione dei seguenti:
>
>* Pianifica scenario in Adobe Workfront Scenario Planner. Per ulteriori informazioni, vedere [Richiedere l&#39;accesso a un piano in Pianificazione scenario](../../scenario-planner/request-access-to-plan.md). È necessaria una licenza aggiuntiva.
>
>* Visualizzazioni e aree di lavoro in Workfront Planning. Per ulteriori informazioni, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). È necessaria una licenza aggiuntiva.


L&#39;amministratore di Workfront configura l&#39;accesso a un tipo di oggetto nel proprio livello di accesso. Per ulteriori informazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Se hai bisogno di autorizzazioni per oggetti specifici in Workfront, puoi richiedere l’accesso a tali oggetti. Invece di inviare un messaggio e-mail all’amministratore di Workfront o al proprietario dell’oggetto per illustrare le tue esigenze, puoi richiedere ulteriori autorizzazioni o accessi in Workfront.

È possibile richiedere l&#39;accesso iniziale agli oggetti se qualcuno condivide con te un collegamento all&#39;oggetto oppure è possibile richiedere l&#39;accesso aggiuntivo agli oggetti per i quali disponi già delle autorizzazioni di visualizzazione. Ad esempio, potresti disporre delle autorizzazioni di visualizzazione per un progetto, ma è necessario aggiungervi attività. In questo caso, potete richiedere le autorizzazioni Contribute per il progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p> 
   <p>Oppure</p>
   <p>Corrente: Lavoro o versione successiva</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti a cui si richiedono le autorizzazioni</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprendere le regole di condivisione standard

Le seguenti regole di condivisione standard sono opzioni predefinite nel sistema Workfront e hanno effetto automaticamente:

* Gli utenti assegnati a un’attività o a un problema dispongono dell’accesso Contribute.
* I project manager, i responsabili di Portfolio e i responsabili di programma dispongono dell&#39;accesso Gestione per gli oggetti di loro proprietà.
* Gli utenti inclusi in una conversazione dispongono dell&#39;accesso di visualizzazione sull&#39;oggetto in cui si verifica la conversazione.
* Gli utenti assegnati come approvatori dispongono dell&#39;accesso di visualizzazione sull&#39;oggetto in attesa di approvazione.
* Quando si condivide un dashboard, anche tutti i report nel dashboard vengono condivisi con lo stesso accesso agli stessi utenti.
* I proprietari degli oggetti non sono in grado di estendere l&#39;accesso a un oggetto oltre il loro accesso a tale oggetto definito dall&#39;amministratore.

## Richiedi accesso

È possibile richiedere l&#39;accesso iniziale agli oggetti a cui non si dispone dell&#39;accesso oppure richiedere l&#39;accesso aggiuntivo agli oggetti a cui si dispone di accesso limitato.

* [Richiedi accesso iniziale](#request-initial-access)
* [Richiedi accesso aggiuntivo](#request-additional-access)

### Richiedi accesso iniziale  {#request-initial-access}

Se non disponi ancora dell’accesso a un oggetto e accedi a tale oggetto da un collegamento, viene visualizzata una schermata in cui ti viene comunicato che non disponi dell’accesso per visualizzare le informazioni.

Per richiedere l&#39;accesso iniziale a un oggetto:

1. Fai clic su **Richiedi accesso**. Viene visualizzata la finestra di dialogo **Richiedi accesso**.

1. (Condizionale) Se più utenti dispongono dell’accesso appropriato per concederti l’accesso aggiuntivo, accanto al nome dell’utente viene visualizzata una freccia a discesa. Seleziona dall’elenco a discesa l’utente che riceverà la richiesta di accesso.

   Nell’elenco a discesa vengono visualizzati solo 10 utenti, disposti in ordine alfabetico. Per ulteriori informazioni sull&#39;ordine degli utenti elencati in questo menu a discesa, vedere [Gerarchia dei menu a discesa &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dall’elenco a discesa, seleziona il tipo di accesso richiesto.
1. (Facoltativo) Nel campo **P.S.**, inserisci una nota che indichi il motivo per cui hai bisogno di accesso aggiuntivo.

   ![Finestra di dialogo Richiedi accesso](assets/request-access-to-project.png)

1. Fai clic su **Richiedi accesso**.

<!--
If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator.

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)
-->

### Richiedi accesso aggiuntivo {#request-additional-access}

Per richiedere accesso aggiuntivo a un oggetto per il quale si dispone già di accesso limitato:

1. Vai all’oggetto a cui desideri richiedere l’accesso aggiuntivo.

1. Fai clic sul menu **Altro** a destra del nome del progetto, quindi fai clic su **Richiedi accesso aggiuntivo**.

   ![Richiedi accesso aggiuntivo](assets/more-menu-request-more-access.png)

1. (Condizionale) Se più utenti dispongono dell’accesso appropriato per concederti l’accesso aggiuntivo, accanto al nome dell’utente viene visualizzata una freccia a discesa. Seleziona dall’elenco a discesa l’utente che riceverà la richiesta di accesso.

   Nell’elenco a discesa vengono visualizzati solo 10 utenti, disposti in ordine alfabetico. Per ulteriori informazioni sull&#39;ordine degli utenti elencati in questo menu a discesa, vedere [Gerarchia dei menu a discesa &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dall’elenco a discesa, seleziona il livello di accesso richiesto.
1. (Facoltativo) Nel campo **P.S.**, inserisci una nota che indichi il motivo per cui hai bisogno di accesso aggiuntivo.

   ![Finestra di dialogo Richiedi accesso](assets/request-access-to-project.png)

1. Fai clic su **Richiedi accesso**.

## Gerarchia dei menu a discesa Richiedi accesso e Richiedi altro accesso {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Comprendere la gerarchia degli utenti elencati nei menu a discesa Richiedi accesso e Richiedi accesso aggiuntivo](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Informazioni sul proprietario di un oggetto](#understand-the-owner-of-an-object)

### Comprendere la gerarchia di utenti elencati nei menu a discesa Richiedi accesso e Richiedi altro accesso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Quando si popolano gli elenchi Richiedi accesso o Richiedi altro accesso sugli oggetti, Workfront seleziona un elenco di un massimo di 10 utenti che soddisfano vari ruoli che possono concedere l’accesso agli oggetti all’utente che lo richiede. L’elenco risultante viene quindi ordinato in base al nome in ordine alfabetico crescente.

L’ordine degli utenti nei menu a discesa Richiedi accesso o Richiedi altro accesso è determinato dalle seguenti regole:

* Il primo utente nell&#39;elenco è l&#39;oggetto &quot;proprietario&quot;, come descritto in [Informazioni sul proprietario di un oggetto](#understand-the-owner-of-an-object).
* L&#39;elenco viene quindi compilato con gli utenti con i quali l&#39;oggetto viene condiviso singolarmente. Sono elencati in ordine alfabetico.
* L’elenco viene quindi popolato ulteriormente con gli utenti che ottengono l’accesso richiesto tramite la condivisione con i loro team, gruppi o aziende. Sono elencati in ordine alfabetico.
* Se l’elenco è vuoto, vengono aggiunti gli amministratori di Workfront in modo che ci sia sempre qualcuno da cui richiedere l’accesso. Sono elencati in ordine alfabetico.
* Ogni utente dell&#39;elenco deve disporre dell&#39;accesso richiesto all&#39;oggetto e dell&#39;accesso per condividere l&#39;oggetto.

### Informazioni sul proprietario di un oggetto {#understand-the-owner-of-an-object}

Il proprietario di un oggetto è definito come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Oggetto</strong> </th> 
   <th><strong>Definizione del proprietario dell'oggetto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Progetti</td> 
   <td>Il proprietario è il proprietario del progetto oppure, se manca o non dispone dell'accesso necessario, il proprietario del portfolio principale. <p>Potrebbero non essere la stessa persona del creatore del progetto. </p></td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>Il proprietario è l'assegnatario principale oppure, se manca o non dispone dell'accesso necessario, il proprietario del progetto in cui risiede l'attività, come definito in precedenza. <p>Potrebbero non essere la stessa persona del creatore dell'attività. </p></td> 
  </tr> 
  <tr> 
   <td>Problemi</td> 
   <td> <p>Il proprietario è il contatto principale del problema oppure, se manca o non dispone dell’accesso necessario, il proprietario del progetto su cui risiede il problema, come definito in precedenza. </p> <p>Potrebbero non essere la stessa persona del creatore del problema. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Il proprietario è Portfolio Owner. <p>Potrebbero non essere la stessa persona del creatore del portfolio. </p></td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td>Il proprietario è il proprietario del documento (l'utente che ha caricato il documento) oppure, se manca o non dispone dell'accesso necessario, il proprietario dell'oggetto in cui si trova il documento.</td> 
  </tr> 
  <tr> 
   <td>Rapporti e dashboard</td> 
   <td>Il proprietario è il creatore del report o del dashboard. </td> 
  </tr> 
  <tr> 
   <td>Calendari</td> 
   <td>Il proprietario è il creatore del calendario. A tutti gli utenti è assegnato un calendario per impostazione predefinita. Sono considerati il proprietario di quel calendario. </td> 
  </tr> 
  <tr> 
   <td>Filtri, viste e raggruppamenti</td> 
   <td>Il creatore è il proprietario di un filtro, di una visualizzazione o di un raggruppamento. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Piani</span> </td> 
   <td> <p><span>Il proprietario è il creatore del piano.</span> </p> <p>È necessaria una licenza aggiuntiva. </p> <p><span>Per informazioni su Workfront Scenario Planner, vedere</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica di Scenario Planner</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Obiettivi</td> 
   <td> <p>Il proprietario è l'utente designato come Proprietario. Potrebbero non essere la stessa persona del creatore dell'obiettivo. </p> <p>È necessaria una licenza aggiuntiva. </p> <p>Per informazioni sugli obiettivi di Workfront, consulta <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Panoramica sugli obiettivi di Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


