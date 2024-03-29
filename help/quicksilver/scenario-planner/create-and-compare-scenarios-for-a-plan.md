---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creare e confrontare scenari di piano nella Pianificazione scenario
description: Quando si pianifica la strategia a lungo termine dell'azienda, è possibile che all'inizio vi siano molte informazioni che non si hanno o non si pensano. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che le parti interessate possano accettare. L'esecuzione di un'analisi "what if" per creare più scenari per il piano può aiutare a prevedere e valutare con precisione le circostanze potenziali e, in ultima analisi, a sviluppare il miglior piano possibile.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 296de69a1c444659c60bcf767bdacdd9e6e36830
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 1%

---

# Creare e confrontare scenari di piano in [!DNL Scenario Planner]

Quando si pianifica la strategia a lungo termine dell&#39;azienda, è possibile che all&#39;inizio vi siano molte informazioni che non si hanno o non si pensano. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che le parti interessate possano accettare. L&#39;esecuzione di un&#39;analisi &quot;what if&quot; per creare più scenari per il piano può aiutare a prevedere e valutare con precisione le circostanze potenziali e, in ultima analisi, a sviluppare il miglior piano possibile.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o versione successiva</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alle funzionalità descritte in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Modifica l'accesso o versione successiva al [!DNL Scenario Planner]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere l’accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Creare scenari

Uno scenario è una copia di un piano. Puoi creare tutti gli scenari necessari. Tuttavia, consigliamo di ridurre al minimo il numero di scenari in modo da poterli confrontare facilmente.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

1. Creare un piano.

   Per informazioni sulla creazione di piani, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Il primo piano creato viene salvato automaticamente come &quot;[!UICONTROL Scenario iniziale].&quot;

1. Fai clic sulla freccia rivolta verso il basso accanto a uno scenario esistente, quindi fai clic sul pulsante **[!UICONTROL Copia]** icona.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Viene creato un nuovo scenario con le stesse informazioni dello scenario copiato. Viene automaticamente denominato &quot;[!UICONTROL Scenario 2]&quot; se si tratta del secondo scenario del piano, &quot;[!UICONTROL Scenario 3]&quot; se è il terzo, e così via. Non è possibile rinominare gli scenari. Non esiste un limite al numero di copie che è possibile effettuare.

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

     Per informazioni sulla creazione di iniziative, consulta [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Aggiornare le priorità delle iniziative
   * Regolare le informazioni sulle persone o sul budget
   * Rivedi e regola i conflitti di iniziativa nel tuo scenario

     Per informazioni sulla risoluzione dei conflitti, consulta [Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Clic **[!UICONTROL Salva piano]** per salvare le modifiche.

## Confronta scenari

Dopo aver creato gli scenari, puoi confrontarli per trovare quello migliore per la tua organizzazione.

1. Passare al piano per il quale si desidera confrontare gli scenari.
1. Clic **[!UICONTROL Confronta scenari]**. Viene visualizzata la pagina di confronto dello scenario.

   Tutti gli scenari esistenti per il piano vengono visualizzati in un formato di scheda affiancato. Lo scenario Iniziale viene sempre elencato per primo ed è statico.

   ![](assets/scenario-cards-overlapping-350x166.png)

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
      <td>Bdg</td> 
      <td>Budget totale definito per il piano in questo scenario. Per informazioni sui piani di budget, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Costi</td> 
      <td>I costi associati alle iniziative sullo scenario. Per informazioni sui costi, consulta <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilizzo</td> 
      <td>La percentuale di utilizzo del budget [!UICONTROL] per il piano in questo scenario. Per informazioni sulla percentuale di utilizzo del budget di [!UICONTROL], vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valore Netto</td> 
      <td>Il [!UICONTROL Net Value] del piano in questo scenario. Per informazioni sul [!UICONTROL Valore netto] di un piano, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Iniziative</td> 
      <td>Il numero di iniziative per il piano in questo scenario.</td> 
     </tr> 
     <tr> 
      <td>In conflitto</td> 
      <td>Il numero di iniziative che mostrano qualsiasi tipo di conflitto nel piano per questo scenario. Per informazioni sui conflitti di iniziative, vedi <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando le informazioni differiscono tra lo scenario iniziale e gli scenari aggiuntivi, accanto al valore modificato viene visualizzata una freccia verso l&#39;alto o verso il basso per indicare un aumento o una diminuzione di tale valore rispetto allo scenario iniziale.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Ad esempio, il budget, il numero di mansioni, il numero di iniziative potrebbero cambiare da uno scenario all&#39;altro.

1. Fai clic sul nome di uno scenario per accedervi e apportarvi modifiche.

   Per ulteriori informazioni, vedere [Creare scenari](#create-scenarios) in questo articolo.

1. Clic **[!UICONTROL Aggiungi descrizione]** per aggiungere una descrizione dello scenario

   Oppure

   Fai clic sul campo descrizione per aggiornarlo, quindi fai clic in un punto qualsiasi dello schermo per salvare le modifiche.

1. (Facoltativo) Fai clic su **[!UICONTROL Altro]** menu ![](assets/more-icon.png) a **[!UICONTROL Copia]** o **[!UICONTROL Elimina]** lo scenario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Quando copi uno scenario, questo viene visualizzato automaticamente nella pagina della scheda e viene rinominato in base al seguente pattern: &quot;[!UICONTROL Scenario] `<next number in order>`.&quot;

1. (Condizionale) Se hai fatto clic **[!UICONTROL Elimina]**, fai clic su **[!UICONTROL Sì, elimina]** per confermare.

   Non è possibile recuperare gli scenari eliminati.

   Per informazioni sull’eliminazione degli scenari, consulta [Eliminare i piani in [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Clic **[!UICONTROL Salva piano]** per salvare scenari e piani.
