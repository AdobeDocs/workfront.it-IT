---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Creazione e confronto di scenari di piano in Scenario Planner
description: Quando pianifichi la strategia a lungo termine della tua azienda, ci sono molte informazioni che potresti non avere o a cui pensare all'inizio. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che i tuoi stakeholder possano accettare. Effettuare un’analisi "cosa succede se" per creare più scenari per il piano può aiutarti a prevedere e valutare con precisione le potenziali circostanze e, in ultima analisi, a sviluppare il piano migliore possibile.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# Creare e confrontare scenari di piano in [!DNL Scenario Planner]

Quando pianifichi la strategia a lungo termine della tua azienda, ci sono molte informazioni che potresti non avere o a cui pensare all&#39;inizio. Ci vuole tempo e sperimentazione per arrivare a una strategia finale che i tuoi stakeholder possano accettare. Effettuare un’analisi &quot;cosa succede se&quot; per creare più scenari per il piano può aiutarti a prevedere e valutare con precisione le potenziali circostanze e, in ultima analisi, a sviluppare il piano migliore possibile.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Modifica accesso o superiore al [!DNL Scenario Planner]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare scenari

Uno scenario è una copia di un piano. Puoi creare tutti gli scenari necessari. Tuttavia, consigliamo di mantenere al minimo il numero di scenari in modo da poterli confrontare facilmente.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

1. Crea un piano.

   Per informazioni sulla creazione dei piani, consulta [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Il primo piano creato viene salvato automaticamente come &quot;[!UICONTROL Scenario iniziale].&quot;

1. Fai clic sulla freccia rivolta verso il basso accanto a uno scenario esistente, quindi fai clic sul pulsante **[!UICONTROL Copia]** icona.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Viene creato un nuovo scenario con le stesse informazioni dello scenario copiato. Viene automaticamente denominato &quot;[!UICONTROL Scenario 2]&quot; se è il secondo scenario del tuo piano, &quot;[!UICONTROL Scenario 3]&quot; se è la terza, e così via. Non è possibile rinominare gli scenari.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Aggiorna il nuovo scenario in uno dei seguenti modi:

   * Creare, aggiornare o eliminare iniziative

      >[!TIP]
      >
      >Quando elimini un&#39;iniziativa in uno scenario, questa viene rimossa solo dallo scenario selezionato, non da tutti gli scenari.

      Per informazioni sulla creazione di iniziative, consulta [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Aggiornare le priorità delle iniziative
   * Regolare le informazioni sulle persone o sul budget
   * Rivedi e regola i conflitti di iniziativa nel tuo scenario

      Per informazioni sulla risoluzione dei conflitti, vedere [Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.

## Confronta scenari

Dopo aver creato i tuoi scenari, puoi confrontarli per trovare quello migliore per la tua organizzazione.

1. Passa al piano di cui desideri confrontare gli scenari.
1. Fai clic su **[!UICONTROL Confronto degli scenari]**. Viene visualizzata la pagina di confronto degli scenari.

   Tutti gli scenari esistenti per il piano vengono visualizzati in formato scheda affiancata. Lo scenario iniziale viene sempre elencato per primo ed è statico.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Facoltativo) Scorri verso destra per visualizzare tutte le schede dello scenario.

   Le seguenti informazioni vengono visualizzate in una scheda scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nome dello scenario</td> 
      <td> <p>Un nome generato automaticamente da Workfront e non può essere modificato. Ad esempio, "[!UICONTROL Initial Scenario]", "[!UICONTROL Scenario 2]" e così via. </p> </td> 
     </tr> 
     <tr> 
      <td>Descrizione dello scenario</td> 
      <td>Una voce manuale in cui è possibile descrivere le specifiche dello scenario. </td> 
     </tr> 
     <tr> 
      <td>Ruoli processo disponibili</td> 
      <td>Numero di ruoli di lavoro disponibili nel budget del piano per la sua durata. </td> 
     </tr> 
     <tr> 
      <td>Ruoli richiesti</td> 
      <td>Il numero di ruoli di lavoro richiesti, in base alle iniziative. </td> 
     </tr> 
     <tr> 
      <td>Bdg</td> 
      <td>Il budget totale definito per il piano in questo scenario. Per informazioni sul budget relative ai piani, consulta <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Costi</td> 
      <td>I costi associati alle iniziative sullo scenario. Per informazioni sui costi, consulta <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilizzo</td> 
      <td>La percentuale di utilizzo del budget del piano in questo scenario. Per informazioni sulla percentuale di utilizzo del budget, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valore Netto</td> 
      <td>Valore netto [!UICONTROL] del piano in questo scenario. Per informazioni sul [!UICONTROL Valore netto] di un piano, vedere <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Panoramica dei piani in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Iniziative</td> 
      <td>Numero di iniziative per il piano in questo scenario.</td> 
     </tr> 
     <tr> 
      <td>In conflitto</td> 
      <td>Numero di iniziative che mostrano qualsiasi tipo di conflitto nel piano per questo scenario. Per informazioni sui conflitti di iniziative, vedi <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando le informazioni sono diverse tra lo scenario iniziale e gli scenari aggiuntivi, accanto al valore modificato viene visualizzata una freccia su o giù per indicare un aumento o una diminuzione di tale valore, rispetto allo scenario iniziale.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Ad esempio, il budget, il numero di ruoli di lavoro e il numero di iniziative potrebbero variare da uno scenario all’altro.

1. Fare clic sul nome di uno scenario per accedervi e apportare modifiche.

   Per ulteriori informazioni, consulta la sezione [Creare scenari](#create-scenarios) in questo articolo.

1. Fai clic su **[!UICONTROL Aggiungi descrizione]** per aggiungere una descrizione dello scenario

   Oppure

   Fai clic sul campo di descrizione per aggiornarlo, quindi fai clic in un punto qualsiasi della schermata per salvare le modifiche.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Altro]** menu ![](assets/more-icon.png) a **[!UICONTROL Copia]** o **[!UICONTROL Elimina]** lo scenario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Quando copi uno scenario, questo viene visualizzato automaticamente nella pagina della scheda e viene rinominato in base al seguente pattern: &quot;[!UICONTROL Scenario] `<next number in order>`.&quot;

1. (Condizionale) Se hai fatto clic su **[!UICONTROL Elimina]**, fai clic su **[!UICONTROL Sì, eliminalo]** per confermare.

   Impossibile recuperare gli scenari eliminati.

   Per informazioni sull&#39;eliminazione degli scenari, vedere [Elimina i piani nel [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare gli scenari e il piano.
