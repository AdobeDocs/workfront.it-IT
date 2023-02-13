---
title: Rapporto sull’area Aggiornamenti
description: Rapporto sull’area Aggiornamenti
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# Rapporto sull’area Aggiornamenti

Il rapporto Scrittura contabile consente di visualizzare gli aggiornamenti di sistema dall’area Aggiornamenti di progetti, attività, problemi e altri oggetti precedentemente disponibili solo tramite l’API di Adobe Workfront. Anche se si tratta di un rapporto avanzato destinato a casi d’uso specifici, il formato più digeribile consente di creare rapporti più facilmente sull’attività del progetto e sugli aggiornamenti di sistema in Workfront.

>[!TIP]
>
>Il rapporto Scrittura contabile contiene solo gli aggiornamenti di sistema dall&#39;area Aggiornamenti degli oggetti. Per generare rapporti sui commenti rimasti nell’area Aggiornamenti, è necessario utilizzare il rapporto Nota .\
>Per ulteriori informazioni sul rapporto Nota, consulta [Visualizzare tutti gli aggiornamenti in un rapporto Nota](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)‍

Il rapporto Scrittura contabile può mostrare:

* Quante modifiche di stato si sono verificate
* Quando un&#39;attività o un problema è stato eliminato
* Modifica dei valori in importanti campi personalizzati nel corso del ciclo di vita di un progetto
* Quali date importanti sono cambiate nel corso del ciclo di vita di un progetto?
* Se il proprietario di un progetto è cambiato

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per gli oggetti che contengono le scritture contabili visualizzate nel rapporto</p> <p>Ottieni le autorizzazioni di gestione per il rapporto dopo averlo creato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di eseguire le azioni descritte in questo articolo, è necessario assicurarsi di quanto segue:

* Tutti i campi su cui desideri creare rapporti vengono tracciati in Workfront. Puoi creare rapporti solo sui dati dell’area Aggiornamenti tracciata.

   Per scoprire come aggiungere i campi di cui si desidera tenere traccia in Workfront, consulta [Configurare gli aggiornamenti di sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Per tutti i campi personalizzati sui quali si desidera creare un rapporto, è impostata l’impostazione **Visualizza modifiche al campo nei feed di aggiornamento** abilitato.

   Per informazioni su come abilitare questa impostazione per un campo personalizzato, consulta la sezione . [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) nell&#39;articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Panoramica del report di immissione scritture contabili

Poiché il sistema di query del report Journal Entry viene aggiornato, può restituire un numero significativo di risultati. Per questo motivo, è consigliabile filtrare oggetti specifici, ad esempio progetti, programmi, portfolio, gruppi e così via, durante la creazione del rapporto.

Per ulteriori informazioni sui diversi tipi di oggetti in Workfront, consulta [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Poiché il report Journal Entry restituisce un numero di dati elevato, l&#39;esportazione e la consegna pianificata del report non sono supportate.

La visualizzazione predefinita del rapporto contiene le colonne seguenti:

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
   <td> <p><span style="font-weight: normal;">Nome del campo interessato. A seconda della modalità di impostazione del rapporto, questa colonna può contenere Stato, ID proprietario, Nome attività, Data completamento pianificato o altri campi.</span> </p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna per indicare che il campo elencato è un campo personalizzato.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Tipo di modifica</strong> </td> 
   <td> <p>Tipo di modifica apportata al campo interessato. A seconda delle regole di filtro impostate e delle azioni intraprese dagli utenti, in questo campo potrebbe comparire quanto segue:</p> 
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
   <td> <p>L'oggetto principale più alto nella gerarchia.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Limite</strong> </td> 
   <td> <p>Tipo di oggetto modificato.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Data inserimento</strong> </td> 
   <td> <p>Data di modifica del campo.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Modificato per nome</strong> </td> 
   <td> <p>Utente che ha modificato il campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per organizzare le informazioni in questo rapporto, puoi utilizzare il progetto di raggruppamento incorporato. Il raggruppamento di progetti fornisce un raggruppamento principale di Nome progetto e un raggruppamento secondario di Data di ingresso. È possibile applicare questo raggruppamento esistente durante la creazione del rapporto, oppure applicarlo durante la visualizzazione del rapporto.

Per informazioni su come impostare visualizzazioni, filtri e raggruppamenti desiderati per il rapporto, consulta la sezione pertinente:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Scopri le modifiche allo stato](#see-what-status-changes-occurred)
* [Vedi quando un&#39;attività o un problema è stato eliminato](#see-when-a-task-or-issue-was-deleted)
* [Scopri come i campi personalizzati sono cambiati nel corso del ciclo di vita di un progetto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Visualizzare come è cambiata la data di completamento pianificata nel corso del ciclo di vita di un progetto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Controlla se il proprietario di un progetto è cambiato](#see-if-the-owner-of-a-project-changed)

## Scopri le modifiche allo stato {#see-what-status-changes-occurred}

È possibile impostare il rapporto Scrittura contabile in modo da visualizzare:

* Quante modifiche di stato sono state apportate a un progetto, un&#39;attività o un problema

* Stato precedente prima della modifica
* Chi ha cambiato lo stato
* Quando si è verificata la modifica dello stato

Se desideri visualizzare lo stato di salute di un progetto, puoi anche impostare il rapporto in modo da visualizzare le stesse informazioni utilizzando il progetto **Condizione** campo .

Queste informazioni possono essere utilizzate per facilitare il controllo e per illustrare in che modo tu e la tua organizzazione pianificate.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Se desideri confrontare la differenza in giorni tra le modifiche della condizione, puoi utilizzare l’analisi avanzata.\
>Per ulteriori informazioni sull’analisi avanzata, consulta [Panoramica dell’analisi migliorata](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce Journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Viene caricato il generatore di report.

1. In **Colonne (visualizzazione)** aggiungi le colonne seguenti:

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
      <td> <p>Nome del campo interessato. In questo caso, <strong>status</strong> dovrebbe essere visualizzato in questa colonna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica apportata al campo interessato, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong>oppure <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato per nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato lo stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>Data di modifica dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore testuale</p> </td> 
      <td> <p>Chiave per lo stato precedente. Di seguito sono riportate le chiavi di stato per gli stati di progetto predefiniti:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Corrente</p> </li> 
        <li> <p><strong>AGGIUNTO</strong>: Morto</p> </li> 
        <li> <p><strong>ONH</strong>: Bloccato</p> </li> 
        <li> <p><strong>PLN</strong>: Pianificazione</p> </li> 
        <li> <p><strong>CPL</strong>: Completa</p> </li> 
        <li> <p><strong>REQ</strong>: Richiesto</p> </li> 
        <li> <p><strong>APR</strong>: Approvato</p> </li> 
        <li> <p><strong>REJ</strong>: Rifiutato</p> </li> 
        <li> <p><strong>IDA</strong>: Idea</p> </li> 
       </ul> <p>Se l’organizzazione ha impostato stati personalizzati, altre chiavi di stato potrebbero essere visualizzate in questa colonna. Per informazioni sullo stato personalizzato relativo a una chiave di stato, contatta l’amministratore di Workfront o l’amministratore di gruppo.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore testo</p> </td> 
      <td> <p>Chiave per lo stato aggiornato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>L'oggetto principale più alto per il campo che ha subito la modifica dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Limite</p> </td> 
      <td> <p>Il tipo di oggetto con la modifica dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome problema<br>(Facoltativo)</p> </td> 
      <td> <p>Nome del problema che ha subito una modifica dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome attività<br>(Facoltativo)</p> </td> 
      <td> <p>Nome dell'attività che ha subito una modifica dello stato.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull’aggiunta di colonne, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Filtri** scheda , fai clic su **Aggiungi regola filtro**, quindi aggiungi la regola di filtro **Nome campo** > **Uguale** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Per segnalare le modifiche alla condizione, puoi invece aggiungere la regola di filtro **Nome campo** > **Uguale** > **Condizione**.

   Per ulteriori informazioni sull’aggiunta di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per limitare lo stato attivo del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >Creazione di una regola di filtro che utilizza il modificatore **Contiene** può effettivamente aumentare i tempi di caricamento. Per questo motivo, si consiglia di utilizzare un modificatore diverso, come **Uguale** quando è possibile filtrare per un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, consulta [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. In **Raggruppamenti** scheda , fai clic su **Applicare un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull’aggiunta di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e chiudi**.

   Viene caricato il nuovo rapporto.

## Vedi quando un&#39;attività o un problema è stato eliminato {#see-when-a-task-or-issue-was-deleted}

È possibile impostare il rapporto Scrittura contabile in modo da visualizzare:

* Quali attività o problemi sono stati eliminati
* Chi ha eliminato un&#39;attività o un problema

Per vedere quando un&#39;attività o un problema è stato eliminato:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce Journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Viene caricato il generatore di report.

1. In **Colonne (visualizzazione)** aggiungi le colonne seguenti:

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
      <td> <p>Il tipo di oggetto eliminato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Il tipo di cambiamento che si è verificato. La <strong>Elimina</strong> il cambiamento viene visualizzato in questa colonna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>Data di eliminazione dell'attività o del problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato per nome</p> </td> 
      <td> <p>Nome dell'utente che ha eliminato l'attività o il problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> </td> 
      <td> <p>Nome del progetto per il quale sono state eliminate attività o problemi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull’aggiunta di colonne, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Filtri** scheda , fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Tipo di modifica** > **Uguale** > **Elimina**
   * **ID progetto** > **Uguale** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   Per ulteriori informazioni sull’aggiunta di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per limitare lo stato attivo del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >Creazione di una regola di filtro che utilizza il modificatore **Contiene** può effettivamente aumentare i tempi di caricamento. Per questo motivo, si consiglia di utilizzare un modificatore diverso, come **Uguale** quando è possibile filtrare per un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, consulta [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facoltativo) In **Raggruppamenti** scheda , fai clic su **Applicare un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull’aggiunta di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e chiudi**.

   Viene caricato il nuovo rapporto.

## Scopri come i campi personalizzati sono cambiati nel corso del ciclo di vita di un progetto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Puoi tenere traccia delle modifiche importanti apportate al campo nel corso del progetto. A questo scopo, è possibile impostare la voce del giornale di registrazione per tenere traccia di:

* Aggiunta, aggiornamento o modifica di determinati campi personalizzati
* Quando si sono verificate queste modifiche
* Chi ha apportato le modifiche

Per vedere come sono cambiati i campi personalizzati nel corso del ciclo di vita di un progetto:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce Journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Viene caricato il generatore di report.

1. In **Colonne (visualizzazione)** aggiungi le colonne seguenti:

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
      <td> <p>Nome del campo personalizzato interessato.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna per indicare che il campo elencato è un campo personalizzato.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Tipo di modifica apportata al campo interessato, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong>oppure <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato per nome</p> </td> 
      <td> <p>Nome dell’utente che ha aggiornato il campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>Data di modifica del valore nel campo personalizzato.</p> <p>È consigliabile ordinare in base a questo campo in ordine decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore numerico</p> </td> 
      <td> <p>Valore del numero precedente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore numerico</p> </td> 
      <td> <p>Il valore del numero corrente nel campo personalizzato.</p> </td> 
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
      <td> <p>Valore di testo precedente nel campo personalizzato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore testo</p> </td> 
      <td> <p>Valore di testo corrente nel campo personalizzato.</p> <p>Se il campo personalizzato è un campo typeahead, la variabile <strong>Nuovo valore testo</strong> visualizza l'ID oggetto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull’aggiunta di colonne, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Filtri** scheda , fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Nome campo voce giornale di registrazione** > **Contiene** > **DE**

      >[!TIP]
      >
      >Per limitare questo rapporto a campi personalizzati specifici, aggiungi la regola di filtro **Nome campo voce giornale di registrazione** > **Uguale** > **`<custom field>`**.

   * **ID progetto** > **Uguale** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   Per ulteriori informazioni sull’aggiunta di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per limitare lo stato attivo del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >Creazione di una regola di filtro che utilizza il modificatore **Contiene** può effettivamente aumentare i tempi di caricamento. Per questo motivo, si consiglia di utilizzare un modificatore diverso, come **Uguale** quando è possibile filtrare per un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, consulta [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. In **Raggruppamenti** scheda , fai clic su **Applicare un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull’aggiunta di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e chiudi**.

   Viene caricato il nuovo rapporto.

## Visualizzare come è cambiata la data di completamento pianificata nel corso del ciclo di vita di un progetto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

È possibile impostare il rapporto Scrittura contabile per mostrare la frequenza con cui la Data completamento pianificata cambia nel corso della vita di un progetto.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce Journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Viene caricato il generatore di report.

1. In **Colonne (visualizzazione)** aggiungi le colonne seguenti:

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
      <td> <p>Nome del campo interessato.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> viene visualizzato in questa colonna per indicare che il campo elencato è un campo personalizzato.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td>Il tipo di modifica apportata, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong>oppure <strong>Modifica</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato per nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato la data di completamento pianificato del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td> <p>Data di modifica della data di completamento pianificata del progetto.</p> <p>È consigliabile ordinare in base a questo campo in ordine decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>L'oggetto principale più alto per il campo per il quale è stata modificata la data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Limite</p> </td> 
      <td> <p>L'oggetto con la modifica della data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Vecchio valore data</p> </td> 
      <td> <p>Valore precedente per la data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nuovo valore data</p> </td> 
      <td> <p>Valore corrente per la data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> <p>(Facoltativo)</p> </td> 
      <td> <p>Nome del progetto per il quale è stata modificata la data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome attività</p> <p>(Facoltativo)</p> </td> 
      <td> <p>Nome delle attività nel progetto per le quali è stata modificata la data di completamento pianificata.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome Issue</p> <p>(Facoltativo)</p> </td> 
      <td>Nome dei problemi del progetto che presentano la modifica della data di completamento pianificata.</td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull’aggiunta di colonne, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Filtri** scheda , fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Nome campo** > **Uguale** > **Data**
   * **ID progetto** > **Uguale** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Per ulteriori informazioni sull’aggiunta di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per limitare lo stato attivo del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >Creazione di una regola di filtro che utilizza il modificatore **Contiene** può effettivamente aumentare i tempi di caricamento. Per questo motivo, si consiglia di utilizzare un modificatore diverso, come **Uguale** quando è possibile filtrare per un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, consulta [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. In **Raggruppamenti** scheda , fai clic su **Applicare un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull’aggiunta di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e chiudi**.

   Viene caricato il nuovo rapporto.

## Controlla se il proprietario di un progetto è cambiato {#see-if-the-owner-of-a-project-changed}

È possibile impostare il rapporto Scrittura contabile per mostrare il numero di modifiche apportate dal proprietario del progetto o dal responsabile del progetto nel corso della sua vita.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi seleziona **Voce Journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Viene caricato il generatore di report.

1. In **Colonne (visualizzazione)** aggiungi le colonne seguenti:

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
      <td>Nome del campo interessato. La <strong>ownerID</strong> viene visualizzato in questa colonna.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tipo di modifica</p> </td> 
      <td> <p>Il tipo di modifica apportata, ad esempio <strong>Aggiungi</strong>, <strong>Elimina</strong>oppure <strong>Modifica</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>L'oggetto principale più alto per il progetto con il proprietario del progetto aggiornato.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data inserimento</p> </td> 
      <td>Data di modifica del proprietario del progetto.<br>È consigliabile ordinare in base a questo campo in ordine decrescente.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modificato per nome</p> </td> 
      <td> <p>Nome dell'utente che ha aggiornato il proprietario del progetto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Info aggiuntive 1</p> </td> 
      <td> <p>Il proprietario del progetto corrente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Info aggiuntive 2</p> </td> 
      <td> <p>Il proprietario del progetto precedente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome progetto</p> </td> 
      <td> <p>Progetto con il campo Proprietario del progetto aggiornato.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Per ulteriori informazioni sull’aggiunta di colonne, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In **Filtri** scheda , fai clic su **Aggiungi regola filtro**, quindi aggiungi quanto segue:

   * **Nome campo** > **Uguale** > **ownerID**
   * **ID progetto** > **Uguale** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   Per ulteriori informazioni sull’aggiunta di filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per limitare lo stato attivo del rapporto e ridurre i tempi di caricamento, aggiungi un prompt.

   Oppure

   Crea regole di filtro aggiuntive per includere progetti, attività o problemi specifici.

   >[!IMPORTANT]
   >
   >Creazione di una regola di filtro che utilizza il modificatore **Contiene** può effettivamente aumentare i tempi di caricamento. Per questo motivo, si consiglia di utilizzare un modificatore diverso, come **Uguale** quando è possibile filtrare per un progetto specifico o un ID oggetto di livello superiore.

   Per informazioni su come aggiungere un prompt, consulta [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facoltativo) In **Raggruppamenti** scheda , fai clic su **Applicare un raggruppamento esistente**, quindi seleziona **Progetto**.

   Per ulteriori informazioni sull’aggiunta di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fai clic su **Salva e chiudi**.

   Viene caricato il nuovo rapporto.
