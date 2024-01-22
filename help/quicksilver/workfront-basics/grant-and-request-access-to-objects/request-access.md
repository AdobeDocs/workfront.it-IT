---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Richiedi accesso agli oggetti
description: La visibilità degli oggetti in Adobe Workfront dipende dall’accesso a quel tipo di oggetto e dalle autorizzazioni per un singolo oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---

# Richiedi accesso agli oggetti

La visibilità degli oggetti in Adobe Workfront dipende dall’accesso a quel tipo di oggetto e dalle autorizzazioni per un singolo oggetto.

>[!NOTE]
>
>Questo articolo descrive come richiedere le autorizzazioni per tutti gli oggetti ad eccezione dei piani in Adobe Workfront Scenario Planner. Per informazioni sulla richiesta di accesso ai piani, vedere [Richiedere l&#39;accesso a un piano nella Pianificazione scenario](../../scenario-planner/request-access-to-plan.md). È necessaria una licenza aggiuntiva.

L&#39;amministratore di Workfront configura l&#39;accesso a un tipo di oggetto nel proprio livello di accesso. Per ulteriori informazioni, consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Se hai bisogno di autorizzazioni per oggetti specifici in Workfront, puoi richiedere l’accesso a tali oggetti. Invece di inviare un messaggio e-mail all’amministratore di Workfront o al proprietario dell’oggetto per illustrare le tue esigenze, puoi richiedere un accesso aggiuntivo (o autorizzazioni) in Workfront.

È possibile richiedere l&#39;accesso iniziale agli oggetti se qualcuno condivide con te un collegamento all&#39;oggetto oppure richiedere l&#39;accesso aggiuntivo agli oggetti che visualizzi.

Ad esempio, potresti disporre delle autorizzazioni di visualizzazione per un progetto, ma è necessario aggiungere attività a tale progetto. In questo caso, potete richiedere le autorizzazioni Contribute per il progetto.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti a cui si richiedono le autorizzazioni</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Comprendere le regole di condivisione standard

Le seguenti regole di condivisione standard hanno effetto automatico, in quanto sono impostate come opzioni predefinite nel sistema Workfront.

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

Se non disponi ancora dell’accesso a un oggetto e accedi a tale oggetto da un collegamento, viene visualizzata una schermata che ti informa che non hai accesso alla visualizzazione delle informazioni.

Per richiedere l&#39;accesso iniziale a un oggetto:

1. Clic **Richiedi accesso**.\
   Il **Richiedi accesso** viene visualizzata.

1. (Condizionale) Se più utenti dispongono dell’accesso appropriato per concederti l’accesso aggiuntivo, viene visualizzata una freccia a discesa accanto al nome dell’utente.
1. Seleziona dall’elenco a discesa l’utente che desideri ricevere la richiesta di accesso.\
   Nell’elenco a discesa vengono visualizzati solo 10 utenti. L’elenco è ordinato alfabeticamente.\
   Per ulteriori informazioni sull’ordine degli utenti elencati in questo menu a discesa, consulta  [Gerarchia dei menu a discesa &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dall’elenco a discesa, seleziona il tipo di accesso richiesto.
1. (Facoltativo) In **P.S.** , specifica una nota all’utente sul motivo per cui hai bisogno di accesso aggiuntivo.

   ![](assets/request-access-dialog-350x314.png)

Se non disponi dei diritti di livello di accesso per un oggetto e tenti di accedere a tale oggetto da un collegamento, viene visualizzata una schermata che ti informa di contattare l’amministratore di Workfront.

Ad esempio, se non disponi dell’accesso al portfolio, ma ti è stato assegnato un collegamento a un portfolio, visualizzerai il seguente messaggio:\
![](assets/permission-request-initial2-350x96.png)

### Richiedi accesso aggiuntivo {#request-additional-access}

Per richiedere accesso aggiuntivo a un oggetto per il quale si dispone già di accesso limitato:

1. Passare all&#39;oggetto per il quale si desidera richiedere l&#39;accesso aggiuntivo.

1. Fai clic su **Altro** a destra del nome del progetto, quindi fai clic su **Richiedi altro accesso**.

   ![](assets/request-access-in-project-350x201.png)

1. (Condizionale) Se più utenti dispongono dell’accesso appropriato per concederti l’accesso aggiuntivo, viene visualizzata una freccia a discesa accanto al nome dell’utente.
1. Seleziona dall’elenco a discesa l’utente che desideri ricevere la richiesta di accesso.\
   Nell’elenco a discesa vengono visualizzati solo 10 utenti. L’elenco è ordinato alfabeticamente.\
   Per ulteriori informazioni sull’ordine degli utenti elencati in questo menu a discesa, consulta  [Gerarchia dei menu a discesa &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dall’elenco a discesa, seleziona il livello di accesso richiesto.
1. (Facoltativo) In **P.S.** specificare una nota relativa al motivo per cui è necessario un accesso aggiuntivo.
1. Clic **Richiedi accesso**.\
   ![](assets/request-access-dialog-350x314.png)

## Gerarchia dei menu a discesa &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Comprendere la gerarchia di utenti elencati nei menu a discesa Richiedi accesso e Richiedi altro accesso](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Informazioni sul proprietario di un oggetto](#understand-the-owner-of-an-object)

### Comprendere la gerarchia di utenti elencati nei menu a discesa Richiedi accesso e Richiedi altro accesso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Quando si popolano gli elenchi &quot;Richiedi accesso&quot; o &quot;Richiedi più accesso&quot; sugli oggetti, Workfront seleziona un elenco di un massimo di dieci utenti che soddisfano vari ruoli nella condivisione dell’oggetto, come descritto di seguito. Questi utenti possono concedere l&#39;accesso all&#39;oggetto all&#39;utente che lo richiede.\
L’elenco risultante viene quindi ordinato in base al nome in ordine alfabetico crescente.\
Workfront visualizza fino a 10 utenti negli elenchi &quot;Richiedi accesso&quot; e &quot;Richiedi accesso aggiuntivo&quot;.

L’ordine degli utenti nei menu a discesa &quot;Richiedi accesso&quot; o &quot;Richiedi accesso aggiuntivo&quot; è determinato dalle seguenti regole:

* Il primo utente nell&#39;elenco è l&#39;oggetto &quot;proprietario&quot;, come descritto in [Informazioni sul proprietario di un oggetto](#understand-the-owner-of-an-object).
* L&#39;elenco viene quindi compilato con gli utenti con cui l&#39;oggetto viene condiviso singolarmente. Sono elencati in ordine alfabetico.
* L’elenco viene quindi compilato con gli utenti che ottengono l’accesso richiesto tramite la condivisione con i loro team, gruppi o aziende. Sono elencati in ordine alfabetico.
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
   <td>Il proprietario è il proprietario del Portfolio. <p>Potrebbero non essere la stessa persona del creatore del portfolio. </p></td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td>Il proprietario è il proprietario del documento (l'utente che ha caricato il documento) oppure, se manca o non dispone dell'accesso necessario, il proprietario dell'oggetto in cui si trova il documento.</td> 
  </tr> 
  <tr> 
   <td>Rapporti e dashboard</td> 
   <td>Il proprietario è il creatore, il report o la dashboard. </td> 
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
   <td> <p><span>Il proprietario è il creatore del piano.</span> </p> <p>È necessaria una licenza aggiuntiva. </p> <p><span>Per informazioni su Workfront Scenario Planner, consulta</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica sulla pianificazione degli scenari</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Obiettivi</td> 
   <td> <p>Il proprietario è l'utente designato come Proprietario. Potrebbero non essere la stessa persona del creatore dell'obiettivo. </p> <p>È necessaria una licenza aggiuntiva. </p> <p>Per informazioni sugli obiettivi di Workfront, consulta <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Panoramica sugli obiettivi di Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


