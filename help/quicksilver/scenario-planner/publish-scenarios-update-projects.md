---
product-area: enterprise-scenario-planner-product-area
keywords: pubblicare,piani,progetti,scenario,scenari
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aggiornare o creare progetti pubblicando iniziative nel Planner scenario
description: È possibile creare progetti da iniziative esistenti e aggiornare progetti precedentemente collegati a iniziative pubblicando scenari in Adobe Workfront Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '1694'
ht-degree: 0%

---

# Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]

Pubblicazione di uno scenario da [!DNL Adobe Workfront Scenario Planner] esegue le seguenti operazioni:

* Crea progetti dalle iniziative sullo scenario e li collega insieme.
* Aggiorna i progetti già collegati alle iniziative sullo scenario con le informazioni dell&#39;iniziativa collegata. I progetti possono anche essere collegati a iniziative quando li importi in un piano. Per informazioni, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Livello di accesso*</p> </td> 
   <td> 
    <ul> 
    <li>accesso [!UICONTROL Edit] per [!DNL Scenario Planner] e progetti</li></ul>

<p><b>NOTA</b>

Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto</p> </td> 
   <td> 
    <ul> 
     <li>Autorizzazioni di [!UICONTROL Manage] per il piano </li> 
     <li>Autorizzazioni di gestione per progetti pubblicati</li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo ai progetti, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per ulteriori informazioni sull’accesso a [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## Prerequisiti

Prima di iniziare:

* È necessario creare e salvare un piano prima di poter pubblicare le iniziative da esso derivanti.

## Considerazioni sulla pubblicazione di iniziative in progetti

* Puoi pubblicare un solo scenario da un piano.
* Un&#39;iniziativa può essere collegata a un solo progetto.
* Un progetto può essere collegato a più di un&#39;iniziativa quando le iniziative appartengono a diversi piani.

   >[!TIP]
   >
   >Quando un progetto esiste su più piani e pubblichi informazioni sul progetto da tutti i piani, l’ultima pubblicazione sovrascrive l’esistente [!DNL Scenario Planner] informazioni sul progetto.

* Se sono state create iniziative sul piano importando i progetti nel piano, pubblicando l&#39;iniziativa si aggiornano anche i progetti collegati con le informazioni dell&#39;iniziativa.

   >[!TIP]
   >
   >È possibile importare lo stesso progetto in più piani. La pubblicazione potrebbe sovrascrivere le informazioni di iniziativa su un progetto collegato a più iniziative.

   Per informazioni sulla creazione di iniziative importando progetti, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Le modifiche apportate al progetto non vengono trasferite all&#39;iniziativa collegata.



## Pubblica iniziative

>[!IMPORTANT]
>
>Se apporti modifiche alle iniziative del piano, inclusa la risoluzione dei conflitti, devi ripubblicare l&#39;iniziativa affinché le nuove informazioni siano visibili sul progetto. Queste informazioni vengono visualizzate sui progetti collegati alle iniziative solo quando pubblichi l’iniziativa corrispondente. Per informazioni sulla risoluzione dei conflitti tra le iniziative, consulta [Risolvere i conflitti di iniziativa in [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **[!UICONTROL Scenari]**
1. (Facoltativo e condizionale) Per pubblicare da un piano esistente, fai clic sul pulsante **[!UICONTROL Filtro]** icona ![](assets/filter-nwepng.png) nell’angolo in alto a destra del piano e selezionare una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ALL]</td> 
      <td>Visualizza tutti i piani di tua proprietà o condivisi con te. Questa è l’impostazione predefinita. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL I miei piani]</td> 
      <td>Visualizza i piani creati.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Condiviso con me]</td> 
      <td> <p>Visualizza i piani non creati ma condivisi con te.</p> <p>Importante: Per poter pubblicare i piani devi disporre delle autorizzazioni di gestione per i piani condivisi con te. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Ricerca]** icona ![](assets/search-icon.png) e iniziare a digitare il nome di un piano per trovarlo rapidamente nell&#39;elenco.
1. (Condizionale) Per pubblicare da un nuovo piano, crea un piano.

   Per informazioni sulla creazione dei piani, consulta [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Facoltativo) Fare clic sul nome di un piano esistente e creare nuovi scenari per il piano.

   Per informazioni sulla creazione di scenari per un piano, vedi [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facoltativo) Aggiornare le iniziative di un piano esistente o nuovo o crearne di nuovi.

   Per informazioni sulla creazione di iniziative, consulta [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Fai clic su **[!UICONTROL Salva piano]**.
1. Seleziona lo scenario da pubblicare nel **[!UICONTROL Scenario iniziale]** menu a discesa, quindi fai clic su **[!UICONTROL Vai a Pubblica]** ![](assets/go-to-publish-button-icon.png) nell&#39;angolo in alto a destra.

   Oppure

   Fai clic su **[!UICONTROL Confronto degli scenari]**, passa il puntatore sulla scheda dello scenario da cui vuoi pubblicare, quindi fai clic su **[!UICONTROL Vai a Pubblica]** ![](assets/go-to-publish-button-icon.png).

   La [!UICONTROL Pubblicare iniziative] viene visualizzata una pagina con un elenco di tutte le iniziative nello scenario. Se una delle iniziative è stata precedentemente pubblicata, l’icona del progetto ![](assets/project-icon-sp.png) viene visualizzato dopo il nome e la **[!UICONTROL Ultima pubblicazione]** La data viene compilata nell’elenco.

   >[!TIP]
   >
   >Anche le iniziative create tramite l’importazione di progetti visualizzano l’icona del progetto ![](assets/project-icon-sp.png) al diritto del loro nome

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Facoltativo e condizionale) Per pubblicare da un piano esistente, fai clic sul pulsante **[!UICONTROL Filtro]** icona ![](assets/filter-nwepng.png) nell’angolo in alto a destra del piano e selezionare una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ALL]</td> 
      <td>Visualizza tutte le iniziative dello scenario selezionato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Visualizza le iniziative pubblicate in precedenza da te o da un altro utente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Annulla pubblicazione]</td> 
      <td> <p>Visualizza le iniziative non pubblicate. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Ricerca]** icona ![](assets/search-icon.png) e inizia a digitare il nome di un&#39;iniziativa per trovarla rapidamente nell&#39;elenco.
1. Seleziona una o più iniziative da cui pubblicare e creare o aggiornare progetti, quindi fai clic su **[!UICONTROL Pubblicare iniziative]**.

   Questo crea un nuovo progetto da ogni iniziativa selezionata o aggiorna i progetti esistenti connessi, se le iniziative pubblicate erano già collegate a un progetto.

   >[!TIP]
   >
   >I nuovi progetti hanno lo stesso nome delle iniziative pubblicate.

1. (Condizionale) Effettuare una delle seguenti operazioni:

   * Se hai pubblicato un&#39;iniziativa, fai clic su **[!UICONTROL Vedi progetto associato]** aprire il progetto creato o aggiornato dall’iniziativa.
   * Se hai pubblicato più di un&#39;iniziativa, fai clic su **[!UICONTROL Vedere progetti associati]** per aprire un elenco dei progetti pubblicati da iniziative. [!DNL Workfront] applica [!DNL Scenario Planner] I progetti vengono filtrati per impostazione predefinita nell’elenco dei progetti. I progetti pubblicati più di recente vengono visualizzati in cima all’elenco.

      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Per visualizzare le informazioni relative al progetto, visitare i seguenti siti:

   * **La [!UICONTROL Aggiornamenti] sezione**: Viene pubblicato un aggiornamento per indicare che il progetto è stato creato o aggiornato dall’iniziativa . L&#39;aggiornamento contiene il nome dell&#39;iniziativa che ha creato o aggiornato il progetto e il nome collegato del piano che contiene l&#39;iniziativa. Puoi fare clic sul nome del piano nell&#39;aggiornamento per aprire il piano nel [!DNL Scenario Planner].

      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **La [!UICONTROL Panoramica] area [!UICONTROL Dettagli progetto] sezione**: Nuovo [!DNL Scenario Planner] in questo ambito viene creata una sezione che contiene informazioni dell’iniziativa collegata.

      ![](assets/scenario-planner-on-project-details-350x135.png)

      Le seguenti informazioni relative all&#39;iniziativa sono pubblicate nel [!DNL Scenario Planner] area [!UICONTROL Dettagli progetto] sezione:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Iniziativa Durata]</span> </td> 
        <td><span>La durata dell'iniziativa corrispondente quando il progetto è collegato a un'iniziativa. Questo campo non è modificabile.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data ultima pubblicazione]</span> </td> 
        <td><span>Data dell’ultima pubblicazione del progetto da un’iniziativa corrispondente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Iniziativa Data di inizio]</span> </td> 
        <td><span>Il primo giorno del mese di inizio dell'iniziativa, quando il progetto è collegato a un'iniziativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data di fine dell’iniziativa]</span> </td> 
        <td><span>L'ultimo giorno del mese di fine dell'iniziativa, quando il progetto è collegato a un'iniziativa. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>Ruoli del lavoro dell’iniziativa in FTE e ore</span> </td> 
        <td> <p>Informazioni sui ruoli di lavoro associati e le relative assegnazioni di tempo per l'iniziativa. Ciò include:</p> 
         <ul> 
          <li>Nome del ruolo del lavoro</li> 
          <li>Numero di ETP</li> 
          <li> <p>Numero di ore per tutti gli ETP</p> <p>È possibile stimare la quantità di ruoli di lavoro necessari per il piano o l'iniziativa utilizzando ore o FTE.</p> <p>Per ulteriori informazioni, consulta <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani nel planner dello scenario</a>. </p> </li> 
         </ul> 
      <p><b>SUGGERIMENTO</b>

      Se il numero di ruoli di lavoro è diverso per ogni mese nell’iniziativa, in questo campo viene visualizzata la quantità massima di ruoli necessaria per l’iniziativa. Ad esempio, se hai bisogno di 1 Consulente per gennaio e 2 per febbraio, la colonna visualizza 2FTE e la corrispondente quantità di ore per 2 FTE per tutti i mesi.</p> </td>
      </tr> 
      </tbody> 
     </table>

      >[!NOTE]
      >
      >Tutti gli utenti con [!UICONTROL Visualizza] l’accesso al progetto può visualizzare [!DNL Scenario Planner] nella sezione [!UICONTROL Panoramica] area. Puoi controllare se questa area viene visualizzata nella [!UICONTROL Dettagli] utilizzando un modello di layout. Se agli utenti non è associato un modello di layout, questa area viene visualizzata per impostazione predefinita.
      >
      >   
      >   
      >   * Per informazioni sull&#39;aggiunta o la rimozione di aree nel [!UICONTROL Dettagli] utilizzando un modello di layout, vedi [Personalizzare [!UICONTROL Dettagli] visualizzare utilizzando un modello di layout](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
      >   * Per ulteriori informazioni sulla visualizzazione delle informazioni in [!UICONTROL Panoramica] area [!UICONTROL Dettagli progetto], vedi [[!UICONTROL Gestisci] informazioni nel progetto [!UICONTROL Panoramica] area](../manage-work/projects/manage-projects/understand-project-overview-area.md).


   * **La [!UICONTROL Assegnazione ruolo] nel pannello [!UICONTROL Bilanciamento del carico di lavoro] o l&#39;elenco delle attività del progetto**: Le informazioni sulla ripartizione dei ruoli dell&#39;iniziativa si popolano in questo settore, oltre alle assegnazioni di ruolo sul progetto.

      Per ulteriori informazioni, consulta [Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

      ![](assets/role-allocation-panel-350x174.png)

      Qualsiasi modifica delle date o delle risorse del progetto non incide sull&#39;iniziativa corrispondente o su uno dei settori del progetto che contengono informazioni sull&#39;iniziativa.

   * **La [!UICONTROL Budget risorse] area [!UICONTROL Business case] del progetto**: Una nuova opzione per la gestione delle risorse del progetto tramite [!DNL Scenario Planner] vengono aggiunte informazioni nella sezione [!UICONTROL Budget risorse] area [!UICONTROL Business case] del progetto.

      Per ulteriori informazioni, consulta [Risorse di bilancio [!UICONTROL Business case] utilizzando [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      ![](assets/sp-in-business-case-selected-350x110.png)

1. (Facoltativo) Consulta le seguenti informazioni nella sezione [!DNL Scenario Planner] dopo aver pubblicato uno scenario:

   * Lo scenario pubblicato diventa il primo scenario dopo la pubblicazione delle iniziative.
   * Non puoi pubblicare da nessun altro scenario dopo aver pubblicato uno scenario almeno una volta.
   * La [!UICONTROL Vai a Pubblica] l’opzione viene rimossa da tutti gli altri scenari dopo che almeno un’iniziativa è stata pubblicata da uno scenario.
   * Accanto alle icone di progetto delle iniziative pubblicate nel piano viene visualizzato un indicatore verde.

      ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Un indicatore verde &quot;Pubblicato&quot; viene visualizzato nella parte superiore dello scenario e nella scheda dello scenario e il campo Pubblicato viene popolato nella scheda dello scenario che indica il numero di iniziative nello scenario che sono state pubblicate.

      ![](assets/published-scenario-highlighted-350x632.png)

      >[!TIP]
      >
      >Se tutti i progetti pubblicati dalle iniziative dello scenario vengono cancellati, l&#39;indicazione che lo scenario è stato pubblicato viene eliminata. Per informazioni, consulta [Eliminare progetti](../manage-work/projects/manage-projects/delete-projects.md).

1. (Facoltativo) Aggiornare le informazioni sull&#39;iniziativa e ripetere il processo descritto sopra per ripubblicare l&#39;iniziativa e aggiornare le informazioni sull&#39;iniziativa sul progetto collegato.

   Per informazioni sulle iniziative di modifica, vedi [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


