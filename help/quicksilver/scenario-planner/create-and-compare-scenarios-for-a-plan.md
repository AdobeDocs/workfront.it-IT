---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creare e confrontare scenari di piano nella Pianificazione scenario
description: Quando si pianifica la strategia a lungo termine dell'azienda, è possibile che all'inizio vi siano molte informazioni che non si hanno o non si pensano. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che le parti interessate possano accettare. L'esecuzione di un'analisi "what if" per creare più scenari per il piano può aiutare a prevedere e valutare con precisione le circostanze potenziali e, in ultima analisi, a sviluppare il miglior piano possibile.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---

# Crea e confronta scenari di piano in [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Quando si pianifica la strategia a lungo termine dell&#39;azienda, è possibile che all&#39;inizio vi siano molte informazioni che non si hanno o non si pensano. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che le parti interessate possano accettare. L&#39;esecuzione di un&#39;analisi &quot;what if&quot; per creare più scenari per il piano può aiutare a prevedere e valutare con precisione le circostanze potenziali e, in ultima analisi, a sviluppare il miglior piano possibile.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] pacchetto</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Se hai un pacchetto Workfront diverso, contatta il rappresentante Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Light] o versione successiva</p> 
   <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
    <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sull&#39;accesso alla Pianificazione scenario, vedere [Accesso necessario per utilizzare la [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Per informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Creare scenari

Uno scenario è una copia di un piano. Puoi creare tutti gli scenari necessari. Tuttavia, consigliamo di ridurre al minimo il numero di scenari in modo da poterli confrontare facilmente.

{{step1-to-scenario-planner}}

1. Creare un piano o fare clic sul nome di un piano esistente.

   Per informazioni sulla creazione dei piani, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Il primo piano creato viene salvato automaticamente come &quot;[!UICONTROL scenario iniziale]&quot;.

1. Fai clic sulla freccia rivolta verso il basso accanto a uno scenario esistente, quindi fai clic sull&#39;icona **[!UICONTROL Copia]**.

   ![Copia scenario](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Viene creato un nuovo scenario con le stesse informazioni dello scenario copiato. Viene automaticamente denominato &quot;[!UICONTROL Scenario 2]&quot; se si tratta del secondo scenario del piano, &quot;[!UICONTROL Scenario 3]&quot; se si tratta del terzo e così via. Non è possibile rinominare gli scenari. Non esiste un limite al numero di copie che è possibile effettuare.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Aggiorna il nuovo scenario in uno dei seguenti modi:

   * Creare, aggiornare o eliminare iniziative

     >[!TIP]
     >
     >Quando elimini un’iniziativa in uno scenario, questa viene rimossa solo dallo scenario selezionato e non da tutti gli scenari.

     Per informazioni sulla creazione delle iniziative, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Aggiornare le priorità delle iniziative
   * Regolare le informazioni sulle persone o sul budget
   * Rivedi e regola i conflitti di iniziativa nel tuo scenario

     Per informazioni sulla risoluzione dei conflitti, vedere [Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.

## Confronta scenari

Dopo aver creato gli scenari, puoi confrontarli per trovare quello migliore per la tua organizzazione.

1. Passare al piano per il quale si desidera confrontare gli scenari.
1. Fai clic su **[!UICONTROL Confronta scenari]**. Viene visualizzata la pagina di confronto dello scenario.

   Tutti gli scenari esistenti per il piano vengono visualizzati in un formato di scheda affiancato. Lo scenario Iniziale viene sempre elencato per primo ed è statico.

   ![Schede Senario](assets/scenario-cards-overlapping-350x166.png)

1. (Facoltativo) Scorri verso destra per visualizzare tutte le schede scenario.

   In una scheda scenario vengono visualizzate le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nome dello scenario</td> 
      <td> <p>Nome generato automaticamente da Workfront e non modificabile. Ad esempio, "[!UICONTROL Scenario iniziale]", "[!UICONTROL Scenario 2]" e così via. </p> </td> 
     </tr> 
     <tr> 
      <td>Descrizione scenario</td> 
      <td>Voce manuale in cui è possibile descrivere le specifiche dello scenario. </td> 
     </tr> 
     <tr> 
      <td>Mansioni disponibili</td> 
      <td>Il numero di mansioni disponibili nel budget del piano per la sua durata. </td> 
     </tr> 
     <tr> 
      <td>Ruoli richiesti</td> 
      <td>Il numero di ruoli richiesti, in base alle iniziative. </td> 
     </tr> 
     <tr> 
      <td>Budget</td> 
      <td>Budget totale definito per il piano in questo scenario. Per informazioni di budget sui piani, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Costi</td> 
      <td>I costi associati alle iniziative sullo scenario. Per informazioni sui costi, vedere <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilizzo</td> 
      <td>La percentuale di utilizzo del budget [!UICONTROL] per il piano in questo scenario. Per informazioni sulla percentuale di utilizzo del budget di [!UICONTROL], vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica sui piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valore Netto</td> 
      <td>Il [!UICONTROL Net Value] del piano in questo scenario. Per informazioni sul [!UICONTROL Valore Netto] di un piano, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica sui piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Iniziative</td> 
      <td>Il numero di iniziative per il piano in questo scenario.</td> 
     </tr> 
     <tr> 
      <td>In conflitto</td> 
      <td>Il numero di iniziative che mostrano qualsiasi tipo di conflitto nel piano per questo scenario. Per informazioni sui conflitti di iniziative, vedere <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando le informazioni differiscono tra lo scenario iniziale e gli scenari aggiuntivi, accanto al valore modificato viene visualizzata una freccia verso l&#39;alto o verso il basso per indicare un aumento o una diminuzione di tale valore rispetto allo scenario iniziale.
   >
   >
   >![Frecce nelle schede scenario](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Ad esempio, il budget, il numero di mansioni, il numero di iniziative potrebbero cambiare da uno scenario all&#39;altro.

1. Fai clic sul nome di uno scenario per accedervi e apportarvi modifiche.

   Per ulteriori informazioni, consulta la sezione [Creare scenari](#create-scenarios) in questo articolo.

1. Fai clic su **[!UICONTROL Aggiungi descrizione]** per aggiungere una descrizione dello scenario

   Oppure

   Fai clic sul campo descrizione per aggiornarlo, quindi fai clic in un punto qualsiasi dello schermo per salvare le modifiche.

1. (Facoltativo) Fai clic sul menu **[!UICONTROL Altro]** ![Icona Altro](assets/more-icon.png) per **[!UICONTROL Copiare]** o **[!UICONTROL Eliminare]** lo scenario.

   ![Copia o elimina scenario](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Quando copi uno scenario, questo viene automaticamente visualizzato nella pagina della scheda e viene rinominato in base al seguente pattern: &quot;[!UICONTROL Scenario] `<next number in order>`.&quot;

1. (Condizionale) Se hai fatto clic su **[!UICONTROL Elimina]**, fai clic su **[!UICONTROL Sì, elimina]** per confermare.

   Non è possibile recuperare gli scenari eliminati.

   Per informazioni sull&#39;eliminazione degli scenari, vedere [Eliminare i piani in [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare gli scenari e il piano.
