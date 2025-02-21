---
product-area: enterprise-scenario-planner-product-area
keywords: pubblicazione,piani,progetti,scenario,scenari
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario
description: Puoi creare progetti da iniziative esistenti e aggiornare progetti precedentemente collegati alle iniziative pubblicando scenari in Adobe Workfront Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]

La pubblicazione di uno scenario da [!DNL Adobe Workfront Scenario Planner] comporta le seguenti operazioni:

* Crea progetti dalle iniziative sullo scenario e li collega tra loro.
* Aggiorna i progetti già collegati alle iniziative sullo scenario con informazioni provenienti dall’iniziativa collegata. I progetti possono anche essere collegati alle iniziative quando vengono importati in un piano. Per informazioni, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per i nuovi piani Workfront Select o Workfront Prime. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso [!UICONTROL Edit] per i progetti [!DNL Scenario Planner] e [!UICONTROL]</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td>  <ul> 
     <li>Autorizzazioni [!UICONTROL Manage] per il piano </li> 
     <li>Autorizzazioni [!UICONTROL Manage] per i progetti pubblicati</li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare:

* È necessario creare e salvare un piano prima di poter pubblicare le iniziative da esso.
* L’impostazione Consenti agli utenti di creare progetti senza utilizzare un modello deve essere abilitata nell’area Preferenze progetto della Configurazione. Per informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Considerazioni sulla pubblicazione di iniziative nei progetti

* È possibile pubblicare un solo scenario da un piano.
* Un’iniziativa può essere collegata a un solo progetto.
* Un progetto può essere collegato a più di un’iniziativa quando le iniziative appartengono a piani diversi.

  >[!TIP]
  >
  >Quando un progetto esiste in più piani e si pubblicano informazioni nel progetto da tutti i piani, l&#39;ultima pubblicazione sovrascrive le informazioni esistenti di [!DNL Scenario Planner] sul progetto.

* Se sul piano sono state create iniziative importando progetti, la pubblicazione dell’iniziativa aggiorna anche i progetti collegati con informazioni sull’iniziativa.

  >[!TIP]
  >
  >Puoi importare lo stesso progetto in più piani. La pubblicazione potrebbe sovrascrivere le informazioni sull’iniziativa in un progetto collegato a più iniziative.

  Per informazioni sulla creazione di iniziative mediante l&#39;importazione di progetti, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Eventuali modifiche apportate al progetto non vengono trasferite all’iniziativa collegata.



## Pubblica iniziative

>[!IMPORTANT]
>
>Se si apportano modifiche alle iniziative nel piano, inclusa la risoluzione dei conflitti, è necessario ripubblicare l&#39;iniziativa affinché le nuove informazioni siano visibili nel progetto. Queste informazioni vengono visualizzate sui progetti collegati alle iniziative solo quando pubblichi l’iniziativa corrispondente. Per informazioni sulla risoluzione dei conflitti tra iniziative, vedere [Risolvere i conflitti tra iniziative in  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Facoltativo e condizionale) Se si desidera pubblicare da un piano esistente, fare clic sull&#39;icona **[!UICONTROL Filtro]** ![Icona Filtro](assets/filter-nwepng.png) nell&#39;angolo superiore destro del piano e selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tutto]</td> 
      <td>Visualizza tutti i piani di tua proprietà o condivisi con te. Questa è l'impostazione predefinita. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL I miei piani]</td> 
      <td>Visualizza i piani creati.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL condiviso con me]</td> 
      <td> <p>Visualizza i piani non creati ma condivisi con l'utente.</p> <p>Importante: per poter pubblicare i piani condivisi, è necessario disporre delle autorizzazioni [!UICONTROL Manage]. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Opzioni filtro a discesa](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cerca]** ![icona di ricerca](assets/search-icon.png) e inizia a digitare il nome di un piano per trovarlo rapidamente nell&#39;elenco.
1. (Condizionale) Per pubblicare da un nuovo piano, crea un piano.

   Per informazioni sulla creazione dei piani, vedere [Creare e modificare i piani in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. (Facoltativo) Fare clic sul nome di un piano esistente e creare nuovi scenari per il piano.

   Per informazioni sulla creazione di scenari per un piano, vedere [Creare e confrontare scenari di piano in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facoltativo) Aggiorna le iniziative di un piano esistente o nuovo o creane di nuovi.

   Per informazioni sulla creazione delle iniziative, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Fare clic su **[!UICONTROL Salva piano]**.
1. Seleziona lo scenario da pubblicare dal menu a discesa **[!UICONTROL Scenario iniziale]**, quindi fai clic su **[!UICONTROL Vai a pubblicazione]** ![Vai a pubblicazione](assets/go-to-publish-button-icon.png) nell&#39;angolo in alto a destra.

   Oppure

   Fai clic su **[!UICONTROL Confronta scenari]**, passa il puntatore del mouse sulla scheda dello scenario da cui desideri pubblicare, quindi fai clic su **[!UICONTROL Vai a pubblicazione]** ![Vai a pubblicazione](assets/go-to-publish-button-icon.png).

   Viene visualizzata la pagina [!UICONTROL Pubblica iniziative] in cui è riportato un elenco di tutte le iniziative incluse nello scenario. Se una delle iniziative è stata pubblicata in precedenza, l&#39;icona del progetto ![icona progetto](assets/project-icon-sp.png) viene visualizzata dopo il nome e la data **[!UICONTROL Ultima pubblicazione]** viene inserita nell&#39;elenco.

   >[!TIP]
   >
   >Le iniziative create importando progetti visualizzano anche l&#39;icona del progetto ![Icona del progetto](assets/project-icon-sp.png) a destra del nome

   ![Icona del progetto e data dell&#39;ultima pubblicazione](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Facoltativo e condizionale) Se si desidera pubblicare da un piano esistente, fare clic sull&#39;icona **[!UICONTROL Filtro]** ![Icona Filtro](assets/filter-nwepng.png) nell&#39;angolo superiore destro del piano e selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tutto]</td> 
      <td>Visualizza tutte le iniziative dello scenario selezionato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL pubblicato]</td> 
      <td>Visualizza le iniziative pubblicate in precedenza da te o da un altro utente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL non pubblicato]</td> 
      <td> <p>Visualizza le iniziative non pubblicate. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Filtro iniziative](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Ricerca]** ![Icona Ricerca](assets/search-icon.png) e inizia a digitare il nome di un&#39;iniziativa per trovarla rapidamente nell&#39;elenco.
1. Seleziona una o più iniziative per pubblicarle e creare o aggiornare i progetti da esse, quindi fai clic su **[!UICONTROL Pubblica iniziative]**.

   Questo crea un nuovo progetto da ciascuna iniziativa selezionata o aggiorna i progetti connessi esistenti, se le iniziative pubblicate erano già collegate a un progetto.

   >[!TIP]
   >
   >I nuovi progetti hanno lo stesso nome delle iniziative pubblicate.

1. (Condizionale) Effettua una delle seguenti operazioni:

   * Se hai pubblicato un&#39;iniziativa, fai clic su **[!UICONTROL Vedi il progetto associato]** per aprire il progetto creato o aggiornato dall&#39;iniziativa.
   * Se hai pubblicato più di un&#39;iniziativa, fai clic su **[!UICONTROL Visualizza progetti associati]** per aprire un elenco di progetti pubblicati dalle iniziative. [!DNL Workfront] applica il filtro [!DNL Scenario Planner] progetti all&#39;elenco dei progetti per impostazione predefinita. I progetti pubblicati più di recente sono elencati per primi.

     ![Pianificazione scenario dopo la pubblicazione delle iniziative](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Vai alle seguenti aree per visualizzare le informazioni sull’iniziativa sul progetto:

   * **Sezione [!UICONTROL Aggiornamenti]**: un aggiornamento viene pubblicato per indicare che il progetto è stato creato o aggiornato dall&#39;iniziativa. L’aggiornamento contiene il nome dell’iniziativa che ha creato o aggiornato il progetto e il nome collegato del piano che contiene l’iniziativa. È possibile fare clic sul nome del piano nell&#39;aggiornamento per aprirlo in [!DNL Scenario Planner].

     ![Conferma del flusso di aggiornamento della pubblicazione](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **L&#39;area [!UICONTROL Panoramica] della sezione [!UICONTROL Dettagli progetto]**: viene creata una nuova sezione [!DNL Scenario Planner] in quest&#39;area che contiene le informazioni dell&#39;iniziativa collegata.

     ![Pianificazione scenario nei dettagli del progetto](assets/scenario-planner-on-project-details-350x135.png)

     Le seguenti informazioni sull&#39;iniziativa sono pubblicate nell&#39;area [!DNL Scenario Planner] della sezione [!UICONTROL Dettagli progetto]:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Durata iniziativa]</span> </td> 
        <td><span>La durata dell'iniziativa corrispondente quando il progetto è collegato a un'iniziativa. Questo campo non è modificabile.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data Ultima Pubblicazione]</span> </td> 
        <td><span>Data dell'ultima pubblicazione del progetto da un'iniziativa corrispondente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>Primo giorno del mese di inizio dell'iniziativa, quando il progetto è collegato a un'iniziativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>Ultimo giorno della fine del mese dell'iniziativa, quando il progetto è collegato a un'iniziativa. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Informazioni sulle mansioni associate e sulle loro allocazioni di tempo per l’iniziativa. Ciò include:</p> 
         <ul> 
          <li>Nome mansione</li> 
          <li>Numero di FTE</li> 
          <li> <p>Numero di ore per tutti gli FTE</p> <p>Puoi stimare la quantità di mansioni necessarie per il piano o l’iniziativa utilizzando ore o FTE.</p> <p>Per ulteriori informazioni, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani nella Pianificazione scenario</a>. </p> </li> 
         </ul> 
      <p><b>SUGGERIMENTO</b>

     Se il numero di mansioni è diverso per ogni mese nell’iniziativa, questo campo mostra la quantità massima di mansioni necessarie per l’iniziativa. Ad esempio, se hai bisogno di 1 Consulente per gennaio e 2 per febbraio, nella colonna vengono visualizzati 2 FTE e l’importo corrispondente di ore per 2 FTE per tutti i mesi.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Tutti gli utenti con accesso [!UICONTROL View] al progetto possono visualizzare la sezione [!DNL Scenario Planner] nell&#39;area [!UICONTROL Overview]. Puoi controllare se quest&#39;area viene visualizzata nella sezione [!UICONTROL Dettagli] utilizzando un modello di layout. Se agli utenti non è associato un modello di layout, questa area viene visualizzata per impostazione predefinita.
     >
     >   
     >   
     >   * Per informazioni sull&#39;aggiunta o la rimozione di aree nella sezione [!UICONTROL Dettagli] tramite un modello di layout, vedere [Personalizzare la visualizzazione [!UICONTROL Dettagli] tramite un modello di layout](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Per ulteriori informazioni sulla visualizzazione delle informazioni nell&#39;area [!UICONTROL Panoramica] di [!UICONTROL Dettagli progetto], vedere [[!UICONTROL Gestisci] informazioni nell&#39;area [!UICONTROL Panoramica] del progetto](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **Il pannello [!UICONTROL Allocazione ruoli] nel [!UICONTROL Bilanciatore dei carichi di lavoro] o nell&#39;elenco delle attività del progetto**: informazioni sull&#39;allocazione dei ruoli nell&#39;iniziativa vengono popolate in quest&#39;area, oltre alle allocazioni dei ruoli nel progetto.

     Per ulteriori informazioni, vedere [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![Pannello allocazione ruoli](assets/role-allocation-panel-350x174.png)

     Eventuali modifiche alle date o alle risorse del progetto non influiscono sull’iniziativa corrispondente o su una qualsiasi delle aree del progetto che contengono informazioni sull’iniziativa.

   * **L&#39;area [!UICONTROL Budget risorse] del [!UICONTROL Business Case] del progetto**: è stata aggiunta una nuova opzione per la gestione delle risorse del progetto utilizzando le informazioni di [!DNL Scenario Planner] nell&#39;area [!UICONTROL Budget risorse] del [!UICONTROL Business Case] del progetto.

     Per ulteriori informazioni, vedere [Risorse budget in [!UICONTROL Business Case] utilizzando  [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![Pianificazione scenario nel caso di business](assets/sp-in-business-case-selected-350x110.png)

1. (Facoltativo) Dopo la pubblicazione di uno scenario, esaminare le seguenti informazioni in [!DNL Scenario Planner]:

   * Lo scenario pubblicato diventa il primo scenario dopo la pubblicazione delle iniziative da esso derivanti.
   * Non puoi pubblicare da nessun altro scenario dopo aver pubblicato uno scenario almeno una volta.
   * L&#39;opzione [!UICONTROL Vai alla pubblicazione] è stata rimossa da tutti gli altri scenari dopo la pubblicazione di almeno un&#39;iniziativa da uno scenario.
   * Accanto alle icone di progetto delle iniziative pubblicate nel piano viene visualizzato un indicatore verde.

     ![Indicatore per iniziativa pubblicata](assets/indicator-for-published-initiative-icon-350x119.png)

   * Nella parte superiore dello scenario e sulla scheda dello scenario viene visualizzato un indicatore verde &quot;Pubblicato&quot; e il campo Pubblicato viene popolato sulla scheda dello scenario, indicando il numero di iniziative nello scenario che sono state pubblicate.

     ![Scenario pubblicato](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Se tutti i progetti pubblicati dalle iniziative dello scenario vengono eliminati, l’indicazione che lo scenario è stato pubblicato viene rimossa. Per informazioni, vedere [Elimina progetti](../manage-work/projects/manage-projects/delete-projects.md).

1. (Facoltativo) Aggiornare le informazioni sull&#39;iniziativa e ripetere il processo descritto in precedenza per ripubblicare l&#39;iniziativa e aggiornare le informazioni sull&#39;iniziativa sul progetto collegato.

   Per informazioni sulla modifica delle iniziative, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


