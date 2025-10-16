---
product-area: resource-management
navigation-topic: resource-planning
title: Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo
description: È possibile preventivare le risorse in Adobe Workfront Resource Planner utilizzando le viste Progetto e Ruolo. Non è possibile preventivare le risorse utilizzando la vista Utente nella Programmazione delle risorse.
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# Risorse preventivate nella Programmazione delle risorse utilizzando le viste Progetto e Ruolo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

La funzione principale della Programmazione delle risorse è di preventivare le risorse per il lavoro da completare nei progetti.

>[!IMPORTANT]
>
>È possibile preventivare le risorse solo se si applicano le visualizzazioni **Visualizza per progetto** o **Visualizza per ruolo** alla Programmazione delle risorse.

Prima di iniziare a inserire le informazioni sul budget nella Programmazione delle risorse, vedere i seguenti articoli:

* [Panoramica sulla programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Accesso necessario per preventivare le risorse in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Panoramica di ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td>
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Modifica priorità e ore preventivate nella Programmazione risorse</p> <p>Modifica accesso ai dati finanziari per preventivare le risorse in base al costo</p> <p>Modifica accesso a progetti e utenti</p></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per i progetti per i quali si desidera preventivare le informazioni</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Risorse preventivate nella Programmazione risorse

* [Risorse budget nella visualizzazione Progetto](#budget-resources-in-the-project-view)
* [Risorse budget nella visualizzazione Ruolo](#budget-resources-in-the-role-view)
* [Risorse budget in blocco](#budget-resources-in-bulk)

### Risorse budget nella visualizzazione Progetto {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. Il **Planner** viene visualizzato per impostazione predefinita.
1. (Condizionale) Selezionare la visualizzazione **Visualizza per progetto**.
1. Espandi i progetti e le mansioni per gestire l’allocazione per il progetto, le mansioni o gli utenti.
1. Per allocare il budget per gli utenti, effettuare una delle seguenti operazioni:

   * Nella colonna **BDG**, specifica manualmente un numero di ore preventivate, FTE o costo per gli utenti.

   * Fai clic sul menu **Altro** per la mansione dell&#39;utente, quindi fai clic su **Imposta ore pianificate degli utenti come preventivate**.\
     Le ore preventivate di ciascun utente vengono calcolate utilizzando la seguente formula:

     `User Budgeted Hours = User Planned Hours`

1. Per allocare budget per le mansioni, eseguire una delle operazioni seguenti:

   * Nella colonna **BDG** specificare manualmente un numero di ore preventivate, FTE o costo per la mansione.

     >[!NOTE]
     >
     >Le ore preventivate per ruolo vengono aggiunte alle ore preventivate del progetto.

   * (Condizionale) Se hai ore preventivate per gli utenti, fai clic sul menu **Altro** per la mansione, quindi fai clic su **Ore preventivate utenti totali per la mansione**.\
     Le ore preventivate per ciascun ruolo vengono calcolate utilizzando la formula seguente:

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * Fai clic sul menu **Altro** per il progetto, quindi fai clic su **Imposta ore pianificate dei ruoli come preventivate**.\
     Le ore preventivate per ciascun ruolo vengono calcolate utilizzando la formula seguente:\
     *

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* Le ore preventivate per ruolo vengono aggiunte alle ore preventivate del progetto.
     >* Gli utenti possono essere preventivati sia per i ruoli principali che per quelli secondari.
     >* La **percentuale di disponibilità FTE** per i ruoli dell&#39;utente deve essere un numero diverso dallo 0% per le ore disponibili per visualizzare un valore nella pianificazione risorse per una mansione. Se un utente è associato a un ruolo con un valore di **Percentuale di disponibilità FTE** pari allo 0%, il valore Ore disponibili per tale ruolo è zero. In questo caso, il ruolo potrebbe mostrare un valore **netto** negativo.\
     >Per ulteriori informazioni su **Percentuale di disponibilità FTE** per le mansioni, vedere l&#39;articolo [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   * Nella colonna **BDG** specificare manualmente un numero di ore preventivate, FTE o costo per il progetto. In questo modo il numero di ore preventivate progetto viene distribuito a ogni ruolo del progetto. Esistono i seguenti scenari:

      * Se il numero di ore preventivate progetto specificato è uguale alle ore pianificate per il progetto, le ore preventivate per il ruolo corrispondono alle ore pianificate per il ruolo.
      * Se il numero di ore preventivate progetto specificato non è uguale alle ore pianificate per il progetto, le ore preventivate per ruolo vengono distribuite in base alla percentuale di ore pianificate necessarie per ciascun ruolo.\
        Ad esempio, se un progetto ha 20 ore pianificate e queste sono distribuite tra due mansioni (il consulente richiede 12 ore pianificate e il tecnico ne richiede 8) e si preventivano 30 ore per il progetto, le ore vengono distribuite come segue: il ruolo del consulente riceve 18 ore preventivate e il ruolo del tecnico riceve 12 ore preventivate.

1. Per allocare il budget per il progetto, eseguire una delle operazioni seguenti:

   * Preventivare i ruoli nel progetto, come descritto nel passaggio 7.\
     Le ore preventivate progetto vengono calcolate con la formula seguente:

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * Nella colonna **BDG** specificare manualmente un numero di ore preventivate, FTE o costo per il progetto.\
     Questo aggiorna le ore preventivate per il ruolo, come descritto nel passaggio 7.\
     ![budget_per_progetto.png](assets/budget-for-project-350x182.png)

1. Fai clic su **Salva**.\
   Dopo aver preventivato le risorse nella Programmazione risorse, le ore preventivate per le risorse ed eventuali costi associati vengono elencati nel Business Case di ogni progetto.\
   Per ulteriori informazioni sulla comprensione dell&#39;area Budget risorse del caso aziendale, vedere la sezione &quot;Budget risorse&quot; nell&#39;articolo [Panoramica delle aree del caso aziendale](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Seleziona la Vista utente per notare eventuali sovrassegnazioni o sottoutilizzi dell&#39;utente tra le Ore disponibili e quelle pianificate per ciascun utente. Le ore preventivate non sono visibili nella vista Utente.

   Per informazioni sul modo in cui Workfront calcola la disponibilità di un utente, vedere [Configurare le preferenze di gestione delle risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Risorse budget nella visualizzazione Ruolo {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

È necessario disporre dell&#39;accesso in modifica a Gestione risorse e dati finanziari e delle autorizzazioni di gestione finanziaria per i progetti al fine di preventivare le risorse nella Programmazione risorse. Se si dispone solo dell&#39;accesso Visualizzazione per almeno un progetto elencato in una mansione, non è possibile preventivare le allocazioni per la mansione nella visualizzazione Ruolo. Puoi comunque allocare budget per i progetti per i quali disponi delle autorizzazioni di gestione.

Per informazioni sull&#39;accesso necessario per l&#39;impostazione del budget delle risorse, vedere l&#39;articolo [Accesso necessario per il preventivo delle risorse in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Per preventivare le allocazioni nella Programmazione risorse nella vista Ruolo****:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront.

1. Fare clic su **Risorse**.
1. Il **Planner** viene visualizzato per impostazione predefinita.
1. (Condizionale) Seleziona la visualizzazione **Visualizza per ruolo**.
1. Espandi le mansioni e i progetti per gestire l’allocazione per il progetto, le mansioni o gli utenti.
1. Per allocare budget per gli utenti, effettuare una delle seguenti operazioni:

   * Nella colonna **BDG**, specifica manualmente un numero di ore preventivate, FTE o costo per gli utenti.
   * Fai clic sul menu **Altro** per il progetto, quindi fai clic su **Imposta ore pianificate degli utenti come preventivate**.\
     Le ore preventivate di ciascun utente vengono calcolate utilizzando la seguente formula:

     `User Budgeted Hours = User Planned Hours`

1. Per allocare budget per le mansioni, eseguire una delle operazioni seguenti:

   * Nella colonna **BDG** specificare manualmente un numero di ore preventivate, FTE o costo per le mansioni.\
     In questo modo le ore preventivate per ruolo vengono distribuite alle ore preventivate del progetto per i progetti che puoi gestire.

   * Fai clic sul menu **Altro** per la mansione, quindi fai clic su **Imposta ore pianificate dei progetti come preventivate.**Le ore preventivate per ruolo vengono calcolate utilizzando la formula seguente:\
     *

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *Le ore preventivate del progetto sono calcolate con la seguente formula:

     `Project Budgeted Hours = Project Planned Hours`

   * Nella colonna **BDG**, specifica manualmente un numero di ore preventivate, FTE o costo per i progetti elencati nella mansione.\
     Questo aggiunge il numero di ore preventivate progetto al ruolo.

   >[!NOTE]
   >
   >Gli utenti possono essere preventivati sia per i ruoli principali che per quelli secondari. La **percentuale di disponibilità FTE** per i ruoli dell&#39;utente deve essere un numero diverso dallo 0% per le ore disponibili per visualizzare un valore nella pianificazione risorse per una mansione. Se un utente è associato a un ruolo con un valore di **Percentuale di disponibilità FTE** pari allo 0%, il valore Ore disponibili per tale ruolo è zero. In questo caso, il ruolo potrebbe mostrare un valore **netto** negativo.\
   >Per ulteriori informazioni su **Percentuale di disponibilità FTE** per le mansioni, vedere l&#39;articolo [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Per allocare il budget per il progetto, eseguire una delle operazioni seguenti:

   * Nella colonna **BDG**, specifica manualmente un numero di ore preventivate, FTE o costo per i progetti.\
     Questo aggiorna anche le Ore preventivate per i ruoli con cui il progetto è elencato.

   * Fai clic sul menu **Altro** per la mansione, quindi fai clic su **Imposta ore pianificate dei progetti come preventivate**.\
     Le ore preventivate progetto vengono calcolate con la seguente formula:

     `Project Budgeted Hours = Project Planned Hours`

     Le ore preventivate del progetto vengono aggiunte alle ore preventivate del ruolo.

   * (Condizionale) Se hai preventivato le ore per gli utenti, fai clic sul menu **Altro** per il progetto, quindi fai clic su **Ore preventivate utenti totali per il progetto**.\
     Le ore preventivate progetto vengono calcolate utilizzando la formula seguente:

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_per_ruolo.png](assets/budget-by-role-350x181.png)

1. Fai clic su **Salva**.\
   Dopo aver preventivato le risorse nella Programmazione risorse, le ore preventivate per le risorse ed eventuali costi associati vengono elencati nel Business Case di ogni progetto.
Per ulteriori informazioni sulla comprensione dell&#39;area Budget risorse del caso aziendale, vedere l&#39;articolo [Risorse budget nel caso aziendale](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Facoltativo) Seleziona la visualizzazione **Visualizza per utente** per notare eventuali sovrassegnazioni o sottoutilizzo dell&#39;utente tra le ore disponibili e quelle pianificate per ogni utente. Le ore preventivate non sono visibili nella vista Visualizza per utente.

### Risorse budget in blocco {#budget-resources-in-bulk}

Quando si utilizzano i collegamenti rapidi, è possibile preventivare le allocazioni per le risorse in blocco. I collegamenti rapidi sono disponibili solo per le visualizzazioni Progetto e Ruolo.

![Opzioni di impostazione budget automatica](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Quando si utilizzano i collegamenti rapidi alle allocazioni di budget per le risorse, il budget viene applicato automaticamente solo ai periodi di tempo visualizzati sullo schermo. Se la timeline di un progetto si estende per un periodo di tempo più lungo di quello visualizzato sullo schermo, è necessario scorrere da sinistra a destra, quindi utilizzare i collegamenti rapidi per preventivare automaticamente le risorse.

Per preventivare le risorse in blocco:

1. Passa a .\
   Per ulteriori informazioni sull&#39;accesso alla Programmazione delle risorse, vedere la sezione &quot;Accedere alla Programmazione delle risorse&quot; nell&#39;articolo [Panoramica sulla Programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   Nell’elenco viene visualizzato un elenco di progetti che puoi gestire.

1. (Facoltativo) Espandi ciascun progetto per visualizzare un elenco di mansioni associate.\
   Oppure
1. (Facoltativo) Seleziona **Visualizza per ruolo**, quindi espandi ogni ruolo per visualizzare un elenco di progetti associati.
1. Passa il puntatore del mouse sul nome di un progetto o di una mansione.
1. Fai clic sull&#39;icona **Altro** ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)visualizzata all&#39;estrema destra del nome del progetto o del ruolo.

1. Fare clic su una delle opzioni disponibili per specificare automaticamente la quantità di ore preventivate (BDG) per altri oggetti.

   A seconda che sia stato fatto clic sull&#39;icona Altro su un progetto o su un ruolo, le opzioni per la definizione del budget in blocco sono diverse. La tabella seguente illustra le opzioni disponibili per i progetti e i ruoli:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Visualizzazione progetto</strong> </td> 
      <td><strong>Visualizzazione ruolo</strong> </td> 
     </tr> 
     <tr> 
      <td>Opzioni progetto</td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate dei ruoli come preventivate</strong>: selezionare questa opzione per fare in modo che le ore pianificate del ruolo diventino identiche alle ore pianificate. Il totale delle ore preventivate per i ruoli verrà visualizzato per le ore preventivate del progetto. </li> 
        <li><strong>Modifica date budget</strong>: selezionare questa opzione per spostare le ore preventivate in un altro intervallo temporale.<br>Per ulteriori informazioni sull'adeguamento delle date di impostazione del budget, vedere <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Adeguamento delle date di impostazione del budget in Pianificazione risorse</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate utenti come preventivate</strong>: selezionare questa opzione per fare in modo che le ore pianificate dell'utente siano identiche alle ore pianificate. </li> 
        <li><strong>Ore preventivate utenti totali per il progetto</strong>: selezionare questa opzione per aggiungere tutte le ore preventivate utente e visualizzare il totale come Ore preventivate per il progetto e per il ruolo. È consigliabile utilizzare questa opzione dopo aver preventivato manualmente gli utenti o aver utilizzato prima l’opzione precedente. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Opzioni Ruolo</td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate utenti come preventivate</strong>: selezionare questa opzione per fare in modo che le ore pianificate dell'utente siano identiche alle ore pianificate. </li> 
        <li><strong>Totale ore preventivate utenti per ruolo</strong>: selezionare questa opzione per aggiungere tutte le ore preventivate dell'utente e visualizzare il totale come Ore preventivate per il ruolo e il progetto. È consigliabile utilizzare questa opzione dopo aver preventivato manualmente gli utenti o aver utilizzato prima l’opzione precedente. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate dei progetti come preventivate</strong>: selezionare questa opzione per fare in modo che le ore pianificate del progetto siano identiche alle ore pianificate del progetto. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Alcune opzioni potrebbero non essere visualizzate se mancano alcuni prerequisiti per lavorare nella Programmazione delle risorse.
   >
   >
   >Per ulteriori informazioni sui prerequisiti che devono essere soddisfatti per una pianificazione precisa del budget in Pianificazione risorse, vedere la sezione &quot;Prerequisiti per l&#39;utilizzo in Pianificazione risorse&quot; nell&#39;articolo [Panoramica di Pianificazione risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   >Ad esempio, alcune delle opzioni potrebbero non essere visualizzate nei seguenti scenari:
   >
   >   
   >   
   >   * Quando i progetti non sono associati al Pool di Risorse
   >   * Quando i Pool di Risorse associati ai progetti non contengono utenti
   >   * Quando i gruppi di risorse associati ai progetti contengono utenti a cui non sono associati ruoli.
   >   
   >
