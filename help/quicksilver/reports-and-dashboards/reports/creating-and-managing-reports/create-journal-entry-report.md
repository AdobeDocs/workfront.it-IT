---
title: Rapporto sull'area Aggiornamenti con un rapporto sulle scritture contabili
description: Il rapporto Voce diario evidenzia gli aggiornamenti di sistema dall’area Aggiornamenti di progetti, attività, problemi e altri oggetti precedentemente disponibili solo tramite l’API Adobe Workfront. Anche se si tratta di un rapporto avanzato destinato a casi d’uso specifici, il formato più digeribile consente di creare un rapporto più semplice sull’attività del progetto e sugli aggiornamenti del sistema in Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 577761ff5d1fb59db104df5995af953a0b5e6c0c
workflow-type: tm+mt
source-wordcount: '2771'
ht-degree: 4%

---

# Rapporto sull&#39;area Aggiornamenti con un rapporto Voce diario

<!-- Audited: 11/2024 -->

Il rapporto Voce diario evidenzia gli aggiornamenti di sistema dall’area Aggiornamenti di progetti, attività, problemi e altri oggetti precedentemente disponibili solo tramite l’API Adobe Workfront. Anche se si tratta di un rapporto avanzato destinato a casi d’uso specifici, il formato più digeribile consente di creare un rapporto più semplice sull’attività del progetto e sugli aggiornamenti del sistema in Workfront.

>[!TIP]
>
>Il rapporto Voce diario contiene solo gli aggiornamenti di sistema dall&#39;area Aggiornamenti degli oggetti. Per creare rapporti sui commenti rimasti nell&#39;area Aggiornamenti, è necessario utilizzare il rapporto Nota.\
>Per ulteriori informazioni sul report Note, vedere [Visualizzare tutti gli aggiornamenti in un report Note](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md).

Il rapporto Voce diario può mostrare:

* Quante modifiche di stato si sono verificate
* Quando un&#39;attività o un problema è stato eliminato
* Modifica dei valori nei campi personalizzati importanti nel corso del ciclo di vita di un progetto
* Quali date importanti sono cambiate nel corso del ciclo di vita di un progetto?
* Se il proprietario di un progetto cambia

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
      <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per gli oggetti che contengono le voci diario visualizzate nel report</p> <p>Dopo la creazione, otterrai le autorizzazioni di gestione per il report</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter eseguire le azioni descritte in questo articolo, è necessario verificare quanto segue:

* Tutti i campi (inclusi i campi personalizzati) su cui desideri creare rapporti vengono tracciati in Workfront. È possibile creare rapporti solo sui dati dell&#39;area Aggiornamenti tracciati.

  Per informazioni su come aggiungere i campi di cui si desidera tenere traccia in Workfront, vedere [Configurare gli aggiornamenti di sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Panoramica del rapporto Voce diario

Poiché il report Voce diario esegue query sugli aggiornamenti di sistema, può restituire un numero significativo di risultati. Per questo motivo, è consigliabile filtrare in base a oggetti specifici, ad esempio progetti, programmi, portfolio, gruppi e così via, durante la creazione del report.

Per ulteriori informazioni sui diversi tipi di oggetti in Workfront, vedere [Informazioni sugli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Poiché il rapporto Voce diario restituisce una quantità eccessiva di dati, l&#39;esportazione e la consegna pianificata del rapporto non sono supportate.

La visualizzazione predefinita per questo report contiene le colonne seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo</th> 
   <th>Spiegazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Nome Campo</strong> </td> 
   <td> <p><span style="font-weight: normal;">Nome del campo interessato. A seconda della modalità di impostazione del report, questa colonna potrebbe contenere i campi Stato, ID proprietario, Nome attività, Data di completamento pianificata o altri campi.</span> </p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna, indica che il campo elencato è un campo personalizzato.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Tipo di modifica</strong> </td> 
   <td> <p>Tipo di modifica apportata al campo interessato. A seconda delle regole di filtro impostate e delle azioni eseguite dagli utenti, in questo campo potrebbero essere visualizzati i seguenti elementi:</p> 
    <ul> 
     <li> <p>Aggiungi</p> </li> 
     <li> <p>Controllo</p> </li> 
     <li> <p>Elimina</p> </li> 
     <li> <p>Digest</p> </li> 
     <li> <p>Modifica</p> </li> 
     <li> <p>Ripristina</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Top ObjCode</strong> </td> 
   <td> <p>L'oggetto padre più alto nella gerarchia.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Ambito</strong> </td> 
   <td> <p>Tipo di oggetto modificato.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Data di ingresso</strong> </td> 
   <td> <p>Data in cui il campo è stato modificato.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Modificato per nome</strong> </td> 
   <td> <p>Utente che ha modificato il campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per organizzare le informazioni in questo report, è possibile utilizzare il raggruppamento predefinito denominato Progetto. Il raggruppamento di progetti consente di ottenere un raggruppamento principale di Nome progetto e un raggruppamento secondario di Data di ingresso. Puoi applicare questo raggruppamento esistente durante la creazione del rapporto oppure durante la visualizzazione del rapporto.

Per informazioni su come impostare le visualizzazioni, i filtri e i raggruppamenti desiderati per il rapporto, consulta la sezione pertinente:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Visualizza le modifiche di stato avvenute](#see-what-status-changes-occurred)
* [Vedere quando un&#39;attività o un problema è stato eliminato](#see-when-a-task-or-issue-was-deleted)
* [Scopri come sono cambiati i campi personalizzati nel corso del ciclo di vita di un progetto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Guarda come è cambiata la data di completamento pianificata nel corso del ciclo di vita di un progetto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Verifica se il proprietario di un progetto è cambiato](#see-if-the-owner-of-a-project-changed)

## Visualizzare le modifiche di stato {#see-what-status-changes-occurred}

È possibile impostare il rapporto Scrittura contabile in modo da visualizzare:

* Quante modifiche di stato sono state apportate a un progetto, a un’attività o a un problema

* Lo stato precedente al cambiamento
* Chi ha cambiato lo stato
* Quando è avvenuta la modifica dello stato

Per visualizzare lo stato di un progetto, è inoltre possibile impostare il report in modo che visualizzi le stesse informazioni utilizzando il campo **Condizione** del progetto.

Queste informazioni possono essere utilizzate per facilitare il controllo e per illustrare il livello di pianificazione dell&#39;azienda.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Reports**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce diario**.

   ![Seleziona voce diario](assets/nwe-select-journal-entry-350x273.png)

   Il generatore di report viene caricato.

1. Nella scheda **Colonne (visualizzazione)**, aggiungi le colonne seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonna</th> 
      <th>Spiegazione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Campo</p> </td> 
      <td> <p>Nome del campo interessato. In questo caso, <strong>status</strong> deve essere visualizzato in questa colonna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica apportata al campo interessato, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong> o <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato da Nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato lo stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>La data in cui lo stato è stato modificato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore testuale</p> </td> 
      <td> <p>Chiave per lo stato precedente. Di seguito sono riportate le chiavi di stato per gli stati predefiniti del progetto:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: corrente</p> </li> 
        <li> <p><strong>DED</strong>: inattivo</p> </li> 
        <li> <p><strong>ONH</strong>: In attesa</p> </li> 
        <li> <p><strong>PLN</strong>: pianificazione</p> </li> 
        <li> <p><strong>CPL</strong>: completato</p> </li> 
        <li> <p><strong>RICHIESTA</strong>: richiesta</p> </li> 
        <li> <p><strong>APR</strong>: Approvato</p> </li> 
        <li> <p><strong>REJ</strong>: Rifiutato</p> </li> 
        <li> <p><strong>IDA</strong>: idea</p> </li> 
       </ul> <p>Se l’organizzazione ha impostato stati personalizzati, in questa colonna potrebbero essere visualizzate altre chiavi di stato. Per informazioni sullo stato personalizzato correlato a una chiave di stato, contatta l’amministratore di Workfront o l’amministratore del gruppo.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore testo</p> </td> 
      <td> <p>Chiave per lo stato aggiornato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cod. ogg. superiore</p> </td> 
      <td> <p>L'oggetto padre di livello più alto per il campo il cui stato è stato modificato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Limite</p> </td> 
      <td> <p>Tipo di oggetto con stato modificato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome problema<br>(facoltativo)</p> </td> 
      <td> <p>Nome del problema con stato modificato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome attività<br>(facoltativo)</p> </td> 
      <td> <p>Il nome dell'attività che ha avuto un cambiamento di stato.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull&#39;aggiunta di colonne, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**, quindi aggiungi la regola filtro **Nome campo** > **Uguale** > **stato**.

   ![Filtro stato voce diario](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Per generare report sulle modifiche delle condizioni, è invece possibile aggiungere la regola di filtro **Nome campo** > **Uguale** > **Condizione**.

   Per ulteriori informazioni sull&#39;aggiunta di filtri, vedere [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per restringere l’ambito del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >La creazione di una regola di filtro che utilizza il modificatore **Contains** può aumentare i tempi di caricamento. Per questo motivo, è consigliabile utilizzare un modificatore diverso come **Equal** quando possibile per filtrare un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Nella scheda **Raggruppamenti**, fai clic su **Applica un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Il nuovo rapporto viene caricato.

## Vedere quando un&#39;attività o un problema è stato eliminato {#see-when-a-task-or-issue-was-deleted}

È possibile impostare il rapporto Scrittura contabile in modo da visualizzare:

* Quali attività o problemi sono stati eliminati
* Chi ha eliminato un’attività o un problema

Per vedere quando un&#39;attività o un problema è stato eliminato:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Reports**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce diario**.

   ![Seleziona voce diario](assets/nwe-select-journal-entry-350x273.png)

   Il generatore di report viene caricato.

1. Nella scheda **Colonne (visualizzazione)**, aggiungi le colonne seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonna</th> 
      <th>Spiegazione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Limite</p> </td> 
      <td> <p>Tipo di oggetto eliminato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica eseguita. La modifica <strong>Elimina</strong> viene visualizzata in questa colonna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>La data in cui l’attività o il problema è stato eliminato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato da Nome</p> </td> 
      <td> <p>Nome dell’utente che ha eliminato l’attività o il problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> </td> 
      <td> <p>Nome del progetto in cui sono state eliminate le attività o i problemi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull&#39;aggiunta di colonne, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**, quindi aggiungi i seguenti filtri:

   * **Cambia tipo** > **Uguale** > **Elimina**
   * **ID progetto** > **Uguale** > **&lt; nome progetto >**

     <!--WRITER check link; this png file has spaces
     [![Task or issue deleted](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Per ulteriori informazioni sull&#39;aggiunta di filtri, vedere [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per restringere l’ambito del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >La creazione di una regola di filtro che utilizza il modificatore **Contains** può aumentare i tempi di caricamento. Per questo motivo, è consigliabile utilizzare un modificatore diverso come **Equal** quando possibile per filtrare un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facoltativo) Nella scheda **Raggruppamenti**, fai clic su **Applica un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Il nuovo rapporto viene caricato.

## Scopri come sono cambiati i campi personalizzati nel corso del ciclo di vita di un progetto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Puoi tenere traccia di importanti modifiche di campo nel corso del progetto. A tale scopo, è possibile impostare la voce del diario per tenere traccia di:

* Se sono stati aggiunti, aggiornati o modificati alcuni campi personalizzati
* Quando si sono verificati questi cambiamenti
* Chi ha apportato le modifiche

Per vedere come sono cambiati i campi personalizzati nel corso del ciclo di vita di un progetto:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Reports**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce diario**.

   ![Seleziona voce diario](assets/nwe-select-journal-entry-350x273.png)

   Il generatore di report viene caricato.

1. Nella scheda **Colonne (Visualizzazione)**, accertati di avere o fai clic su **Aggiungi colonna** per aggiungere le colonne seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonna</th> 
      <th>Spiegazione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Campo</p> </td> 
      <td> <p>Nome del campo personalizzato interessato.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna, indica che il campo elencato è un campo personalizzato.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica apportata al campo interessato, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong> o <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato da Nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato il campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>Data in cui è stato modificato il valore nel campo personalizzato.</p> <p>È necessario ordinare in base a questo campo in ordine decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore numerico</p> </td> 
      <td> <p>Il numero precedente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore numerico</p> </td> 
      <td> <p>Il valore numerico corrente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore data</p> </td> 
      <td> <p>Il valore della data precedente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore data</p> </td> 
      <td> <p>Il valore della data corrente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore testuale</p> </td> 
      <td> <p>Il valore di testo precedente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore testo</p> </td> 
      <td> <p>Il valore del testo corrente nel campo personalizzato.</p> <p>Se il campo personalizzato è un campo typeahead, la colonna <strong>New Text Value</strong> visualizza l'ID dell'oggetto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull&#39;aggiunta di colonne, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Filtri**, fai clic su **Aggiungi una regola di filtro**, quindi aggiungi i seguenti filtri:

   * **Nome campo voce diario** > **Contiene** > **DE**

     >[!TIP]
     >
     >Per limitare il report a campi personalizzati specifici, aggiungere la regola di filtro **Nome campo voce diario** > **Uguale** > **&lt; nome campo personalizzato>**.

   * **ID progetto** > **Uguale** > **&lt; progetto >**.

   ![Filtro modifiche modulo personalizzato](assets/qs-custom-form-changes-filter-350x92.png)

   Per ulteriori informazioni sull&#39;aggiunta di filtri, vedere [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per restringere l’ambito del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >La creazione di una regola di filtro che utilizza il modificatore **Contains** può aumentare i tempi di caricamento. Per questo motivo, è consigliabile utilizzare un modificatore diverso come **Equal** quando possibile per filtrare un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Nella scheda **Raggruppamenti**, fai clic su **Applica un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Il nuovo rapporto viene caricato.

## Scopri come è cambiata la data di completamento pianificata nel corso del ciclo di vita di un progetto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

È possibile impostare il rapporto Scrittura contabile per visualizzare la frequenza con cui la data di completamento pianificata cambia nel corso della vita di un progetto.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Reports**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce diario**.

   ![Seleziona voce diario](assets/nwe-select-journal-entry-350x273.png)

   Il generatore di report viene caricato.

1. Nella scheda **Colonne (visualizzazione)**, aggiungi le colonne seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonna</th> 
      <th>Spiegazione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Campo</p> </td> 
      <td> <p>Nome del campo interessato.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna, indica che il campo elencato è un campo personalizzato.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td>Tipo di modifica, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong> o <strong>Modifica</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato da Nome</p> </td> 
      <td> <p>Il nome dell’utente che ha aggiornato la Data di completamento pianificata del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>La data in cui è stata modificata la Data di completamento pianificata del progetto.</p> <p>È necessario ordinare in base a questo campo in ordine decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cod. ogg. superiore</p> </td> 
      <td> <p>L'oggetto padre di livello più alto per il campo per il quale è stata modificata la Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Limite</p> </td> 
      <td> <p>L’oggetto per il quale è stata modificata la Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore data</p> </td> 
      <td> <p>Il valore precedente per Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore data</p> </td> 
      <td> <p>Il valore corrente per Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> <p>(Facoltativo)</p> </td> 
      <td> <p>Il nome del progetto per il quale è stata modificata la Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome attività</p> <p>(Facoltativo)</p> </td> 
      <td> <p>Nome delle attività del progetto per le quali è stata modificata la Data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Issue</p> <p>(Facoltativo)</p> </td> 
      <td>Nome dei problemi del progetto per i quali è stata modificata la Data di completamento pianificata.</td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull&#39;aggiunta di colonne, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Nome Campo** > **Uguale** > **Data**
   * **ID progetto** > **Uguale** > **&lt; nome progetto >**.

   ![Filtro modifica data di completamento pianificata](assets/qs-planned-completion-date-change-filter-350x91.png)

   Per ulteriori informazioni sull&#39;aggiunta di filtri, vedere [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per restringere l’ambito del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >La creazione di una regola di filtro che utilizza il modificatore **Contains** può aumentare i tempi di caricamento. Per questo motivo, è consigliabile utilizzare un modificatore diverso come **Equal** quando possibile per filtrare un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Nella scheda **Raggruppamenti**, fai clic su **Applica un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Il nuovo rapporto viene caricato.

## Verifica se il proprietario di un progetto è cambiato {#see-if-the-owner-of-a-project-changed}

È possibile impostare il rapporto Voce diario per visualizzare il numero di modifiche apportate dal proprietario del progetto o dal project manager nel corso della vita di un progetto.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **Reports**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce diario**.

   ![Seleziona voce diario](assets/nwe-select-journal-entry-350x273.png)

   Il generatore di report viene caricato.

1. Nella scheda **Colonne (visualizzazione)**, aggiungi le colonne seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonna</th> 
      <th>Spiegazione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Campo</p> </td> 
      <td>Nome del campo interessato. Il <strong>ownerID</strong> viene visualizzato in questa colonna.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong> o <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Cod. ogg. superiore</p> </td> 
      <td> <p>L’oggetto principale di livello più alto per il progetto per il quale è stato aggiornato il proprietario del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td>La data in cui il proprietario del progetto è stato modificato.<br>È necessario ordinare in base a questo campo in ordine decrescente.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato da Nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato il proprietario del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Info aggiuntive 1</p> </td> 
      <td> <p>Il proprietario corrente del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Info aggiuntive 2</p> </td> 
      <td> <p>Il precedente proprietario del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> </td> 
      <td> <p>Progetto per il quale è stato aggiornato il campo Proprietario progetto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull&#39;aggiunta di colonne, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Nome campo** > **Uguale** > **ownerID**
   * **ID progetto** > **Uguale** > **&lt; nome progetto >**.

   ![Filtro modifica proprietario](assets/qs-owner-changes-filter-350x94.png)

   Per ulteriori informazioni sull&#39;aggiunta di filtri, vedere [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per restringere l’ambito del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >La creazione di una regola di filtro che utilizza il modificatore **Contains** può aumentare i tempi di caricamento. Per questo motivo, è consigliabile utilizzare un modificatore diverso come **Equal** quando possibile per filtrare un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facoltativo) Nella scheda **Raggruppamenti**, fai clic su **Applica un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e Chiudi**.

   Viene visualizzato il nuovo rapporto sulle scritture contabili.
