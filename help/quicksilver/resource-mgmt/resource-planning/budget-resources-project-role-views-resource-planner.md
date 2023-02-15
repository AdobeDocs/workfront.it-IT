---
product-area: resource-management
navigation-topic: resource-planning
title: Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo
description: È possibile preventivare le risorse in Adobe Workfront Resource Planner utilizzando le visualizzazioni Progetto e Ruolo . Non è possibile preventivare le risorse utilizzando la visualizzazione Utente nel Planner risorse.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

La funzione principale di Resource Planner consiste nel preventivare le risorse per il lavoro che deve essere completato sui progetti.

>[!IMPORTANT]
>
>È possibile eseguire il budget delle risorse solo se si applica il **Visualizza per progetto** o **Visualizza per ruolo** visualizza il planner risorse.

Prima di iniziare a generare informazioni sul budget nel Planner risorse, vedere i seguenti articoli:

* [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Accesso necessario alle risorse di budget in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Modifica priorità e ore di budget nel Planner risorse</p> <p>Modifica l'accesso ai dati finanziari alle risorse di budget per costo</p> <p>Modifica accesso a progetti e utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti per i quali si desidera assegnare al budget le informazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Risorse di budget nel planner risorse

* [Risorse di budget nella vista Progetto](#budget-resources-in-the-project-view)
* [Risorse di budget nella vista Ruolo](#budget-resources-in-the-role-view)
* [Risorse di bilancio in blocco](#budget-resources-in-bulk)

### Risorse di budget nella vista Progetto {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.
1. La **Planner** viene visualizzato per impostazione predefinita.
1. (Condizionale) Seleziona la **Visualizza per progetto** visualizza.
1. Espandere i progetti e i ruoli del processo per gestire l’allocazione per il progetto, i ruoli o gli utenti.
1. Per allocare il budget per gli utenti, effettuare una delle seguenti operazioni:

   * In **BDG** specifica manualmente un numero di ore, FTE o costi a budget per gli utenti.

   * Fai clic sul pulsante **Altro** menu relativo al ruolo dell&#39;utente, quindi fare clic su **Imposta le ore pianificate degli utenti come a budget**.\
      Le ore previste per ogni utente vengono calcolate utilizzando la seguente formula:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Per allocare il budget per i ruoli di lavoro, eseguire una delle operazioni seguenti:

   * In **BDG** specificare manualmente un numero di ore, FTE o costo preventivati per il ruolo di lavoro.

      >[!NOTE]
      >
      >Le ore previste per il ruolo vengono aggiunte alle ore previste per il progetto.

   * (Condizionale) Se hai preventivato le ore per gli utenti, fai clic sul pulsante **Altro** menu per il ruolo del lavoro, quindi fare clic su **Ore previste totali per il ruolo degli utenti**.\
      Le ore previste per ciascun ruolo vengono calcolate utilizzando la seguente formula:

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * Fai clic sul pulsante **Altro** per il progetto, quindi fai clic su **Imposta ore pianificate dei ruoli come budget**.\
      Le ore previste per ciascun ruolo vengono calcolate utilizzando la seguente formula:\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* Le ore previste per il ruolo vengono aggiunte alle ore previste per il progetto.
      >* Gli utenti possono essere iscritti in budget sia per i ruoli primari che per quelli secondari.
      >* La **Percentuale di disponibilità FTE** per i ruoli dell&#39;utente deve essere un numero diverso da 0% per le ore disponibili per visualizzare un valore nel planner risorse per un ruolo di lavoro. Se un utente è associato a un ruolo con uno 0% **Percentuale di disponibilità FTE**, il valore Ore disponibili è zero per quel ruolo di lavoro. In questo caso, il ruolo potrebbe mostrare un negativo **Valore netto**.\
         >Per ulteriori informazioni sulla **Percentuale di disponibilità FTE** per i ruoli di lavoro, consulta l’articolo [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * In **BDG** specifica manualmente un numero di ore, FTE o costi a budget per il progetto. In questo modo viene distribuito il numero di ore previste per il progetto a ogni ruolo del progetto. Esistono i seguenti scenari:

      * Se il numero di ore previste per il progetto specificato è uguale a ore pianificate per il progetto, le ore previste per il ruolo corrispondono alle ore pianificate per il ruolo.
      * Se il numero di ore previste per il progetto specificato non è uguale a quello delle ore pianificate per il progetto, le ore previste per il ruolo vengono distribuite in base alla percentuale di ore pianificate necessarie per ciascun ruolo.\
         Ad esempio, se un progetto ha 20 ore pianificate e viene distribuito tra due ruoli di lavoro (il consulente richiede 12 ore pianificate e l’ingegnere richiede 8 ore pianificate) e si preventivano 30 ore per il progetto, le ore vengono distribuite come segue: il ruolo Consulente riceve 18 ore previste in budget e il ruolo Ingegnere riceve 12 ore previste in budget.

1. Per assegnare il budget al progetto, effettuare una delle seguenti operazioni:

   * Eseguire il budget dei ruoli del progetto, come descritto nel passaggio 7.\
      L&#39;orario previsto del progetto viene calcolato con la seguente formula:

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * In **BDG** specifica manualmente un numero di ore, FTE o costi a budget per il progetto.\
      Questo aggiorna le ore previste per il ruolo, come descritto nel passaggio 7.\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Fai clic su **Salva**.\
   Dopo aver effettuato il budget delle risorse nel Planner risorse, le ore previste per le risorse e i relativi costi vengono elencati nel Business Case di ogni progetto.\
   Per ulteriori informazioni sulla comprensione dell&#39;area di budget delle risorse del Business Case, vedere la sezione &quot;Resource Budgeting&quot; nell&#39;articolo [Panoramica delle aree del Business Case](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facoltativo) Selezionare la visualizzazione Utente per notare eventuali sovrassegnazioni o sottoutilizzazioni degli utenti tra le ore disponibili e pianificate per ogni utente. Le ore con budget non sono visibili nella visualizzazione Utente.

   Per informazioni sul modo in cui Workfront calcola la disponibilità di un utente, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Risorse di budget nella vista Ruolo {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

È necessario disporre dell&#39;accesso Modifica alle autorizzazioni Gestione risorse e Dati finanziari e Gestione finanziaria per i progetti al fine di allocare risorse al budget nel Planner risorse. Se si dispone solo dell&#39;accesso Visualizza ad almeno un progetto elencato in un ruolo di lavoro, non è possibile allocare in budget il ruolo nella visualizzazione Ruolo. È comunque possibile allocare fondi per i progetti in cui si dispone delle autorizzazioni di gestione.

Per informazioni sull&#39;accesso necessario per le risorse di budget, consulta l&#39;articolo [Accesso necessario alle risorse di budget in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Per eseguire il budget delle allocazioni nel Planner risorse nella vista Ruolo***:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.
1. La **Planner** viene visualizzato per impostazione predefinita.
1. (Condizionale) Seleziona la **Visualizza per ruolo** visualizza.
1. Espandere i ruoli e i progetti per gestire l&#39;allocazione per il progetto, i ruoli o gli utenti.
1. Per allocare il budget per gli utenti, eseguire una delle operazioni seguenti:

   * In **BDG** specifica manualmente un numero di ore, FTE o costi a budget per gli utenti.
   * Fai clic sul pulsante **Altro** per il progetto, quindi fai clic su **Imposta le ore pianificate degli utenti come a budget**.\
      Le ore previste per ogni utente vengono calcolate utilizzando la seguente formula:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Per allocare il budget per i ruoli di lavoro, eseguire una delle operazioni seguenti:

   * In **BDG** specificare manualmente un numero di ore, FTE o costo preventivati per i ruoli di lavoro.\
      Questo distribuisce le ore previste per il ruolo alle ore previste per il budget del progetto per i progetti a cui si ha accesso per la gestione.

   * Fai clic sul pulsante **Altro** menu per il ruolo del lavoro, quindi fare clic su **Imposta ore pianificate dei progetti come previste.**L&#39;orario previsto per il ruolo viene calcolato con la seguente formula:\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *L&#39;orario previsto del progetto viene calcolato con la seguente formula:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * In **BDG** specificare manualmente un numero di ore, FTE o costi a budget per i progetti elencati sotto il ruolo di lavoro.\
      Questo aggiunge al ruolo il numero di ore previste per il progetto.
   >[!NOTE]
   >
   >Gli utenti possono essere iscritti in budget sia per i ruoli primari che per quelli secondari. La **Percentuale di disponibilità FTE** per i ruoli dell&#39;utente deve essere un numero diverso da 0% per le ore disponibili per visualizzare un valore nel planner risorse per un ruolo di lavoro. Se un utente è associato a un ruolo con uno 0% **Percentuale di disponibilità FTE**, il valore Ore disponibili è zero per quel ruolo di lavoro. In questo caso, il ruolo potrebbe mostrare un negativo **Valore netto**.\
   >Per ulteriori informazioni sulla **Percentuale di disponibilità FTE** per i ruoli di lavoro, consulta l’articolo [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Per assegnare il budget al progetto, effettuare una delle seguenti operazioni:

   * In **BDG** specificare manualmente un numero di ore, FTE o costi a budget per i progetti.\
      Vengono inoltre aggiornati gli orari previsti per i ruoli in cui è elencato il progetto.

   * Fai clic sul pulsante **Altro** menu per il ruolo del lavoro, quindi fare clic su **Imposta ore pianificate dei progetti come budget**.\
      Le ore in budget del progetto vengono calcolate con la seguente formula:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      Le ore previste per il progetto vengono aggiunte alle ore previste per il ruolo.

   * (Condizionale) Se hai preventivato le ore per gli utenti, fai clic sul pulsante **Altro** per il progetto, quindi fai clic su **Ore in budget totali per gli utenti per il progetto**.\
      L&#39;ora in budget del progetto viene calcolata utilizzando la seguente formula:

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Fai clic su **Salva**.\
   Dopo aver effettuato il budget delle risorse nel Planner risorse, le ore previste per le risorse e i relativi costi vengono elencati nel Business Case di ogni progetto.\
   Per ulteriori informazioni sulla comprensione dell&#39;area Resource Budgeting del Business Case, vedere l&#39;articolo [Risorse di budget nel Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Facoltativo) Seleziona la **Visualizza per utente** visualizza per notare eventuali sovrassegnazioni o sottoutilizzazioni degli utenti tra le ore disponibili e pianificate per ogni utente. Le ore con budget non sono visibili nella visualizzazione Visualizza per utente.

### Risorse di bilancio in blocco {#budget-resources-in-bulk}

È possibile eseguire il budget delle allocazioni per le risorse in blocco quando si utilizzano collegamenti rapidi. I collegamenti rapidi sono disponibili solo per le visualizzazioni Progetto e Ruolo .

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Quando si utilizzano i collegamenti rapidi alle allocazioni di budget per le risorse, il budget viene applicato automaticamente solo ai periodi di tempo visualizzati sullo schermo. Se la timeline di un progetto si estende per un periodo di tempo più lungo di quello visualizzato sullo schermo, è necessario scorrere da sinistra a destra, quindi utilizzare i collegamenti rapidi per eseguire il budget automatico delle risorse.

Per eseguire il budget in massa delle risorse:

1. Vai a .\
   Per ulteriori informazioni sull&#39;accesso al planner risorse, vedere la sezione &quot;Accedere al planner risorse&quot; nell&#39;articolo [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   Nell’elenco viene visualizzato un elenco dei progetti che è possibile gestire.

1. (Facoltativo) Espandi ogni progetto per visualizzare un elenco di ruoli di lavoro associati ad esso.\
   Oppure
1. (Facoltativo) Seleziona **Visualizza per ruolo**, quindi espandi ogni ruolo per visualizzare un elenco di progetti associati ad esso.
1. Passa il puntatore del mouse sul nome di un progetto o di un ruolo di lavoro.
1. Fai clic sul pulsante **Altro** icona ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)visualizzato all’estrema destra del nome del progetto o del ruolo.

1. Fare clic su una delle opzioni disponibili per specificare automaticamente la quantità di ore previste (BDG) per gli altri oggetti.

   A seconda che tu abbia fatto clic sull’icona Altro su un progetto o su un ruolo, le opzioni per l’impostazione in budget differiscono. La tabella seguente illustra le opzioni disponibili per i progetti e i ruoli:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Vista Project</strong> </td> 
      <td><strong>Vista ruolo</strong> </td> 
     </tr> 
     <tr> 
      <td>Opzioni progetto</td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate dei ruoli come budget</strong>: Selezionare questa opzione per fare in modo che le ore previste del ruolo diventino identiche alle ore pianificate. Il totale delle ore previste per i ruoli verrà visualizzato per le ore previste del progetto. </li> 
        <li><strong>Adeguamento date budget</strong> : Selezionare questa opzione per spostare l'orario previsto in un arco temporale diverso.<br>Per ulteriori informazioni sulla regolazione delle date di budget, vedere <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Adeguare le date di budget nel Planner risorse</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Imposta le ore pianificate degli utenti come a budget</strong>: Selezionare questa opzione per fare in modo che le ore previste per l'utente diventino identiche alle ore pianificate. </li> 
        <li><strong>Ore in budget totali per gli utenti per il progetto</strong>: Selezionare questa opzione per aggiungere tutti gli orari a budget dell'utente e visualizzare il totale come ore a budget per il progetto e per il ruolo. È consigliabile utilizzare questa opzione dopo aver inserito manualmente i budget degli utenti oppure aver utilizzato prima l’opzione precedente. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Opzioni ruolo</td> 
      <td> 
       <ul> 
        <li><strong>Imposta le ore pianificate degli utenti come a budget</strong>: Selezionare questa opzione per fare in modo che le ore previste dell'utente diventino identiche alle ore pianificate. </li> 
        <li><strong>Ore previste totali per il ruolo degli utenti</strong>: Selezionare questa opzione per aggiungere tutte le ore previste dell'utente e visualizzare il totale come ore previste per il ruolo e il progetto. È consigliabile utilizzare questa opzione dopo aver inserito manualmente i budget degli utenti oppure aver utilizzato prima l’opzione precedente. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Imposta ore pianificate dei progetti come budget</strong>: Selezionare questa opzione per fare in modo che il progetto Ore previste diventi identico a Ore programmate del progetto. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Alcune delle opzioni potrebbero non essere visualizzate se mancano alcuni dei prerequisiti per lavorare nel Planner risorse.
   >
   >
   >Per ulteriori informazioni sui prerequisiti che è necessario soddisfare per un&#39;accurata allocazione del budget in Resource Planner, vedere la sezione &quot;Prerequisiti per lavorare nel Resource Planner&quot; nella sezione [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md) articolo.\
   >Ad esempio, alcune delle opzioni potrebbero non essere visualizzate nei seguenti scenari:
   >
   >   
   >   
   >   * Quando i progetti non sono associati al pool di risorse
   >   * Quando i pool di risorse associati ai progetti non contengono utenti
   >   * Quando i pool di risorse associati ai progetti contengono utenti a cui non è associato alcun ruolo di lavoro.

