---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Creare un rapporto personalizzato
description: Scopri come creare rapporti per fornire l’accesso alle informazioni di cui hai bisogno in Adobe Workfront. Puoi utilizzare uno qualsiasi dei rapporti incorporati disponibili in Workfront oppure creare rapporti personalizzati da zero.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 1%

---


# Creare un rapporto personalizzato

Scopri come creare rapporti per fornire l’accesso alle informazioni di cui hai bisogno in Adobe Workfront. Puoi utilizzare uno qualsiasi dei rapporti incorporati disponibili in Workfront oppure creare rapporti personalizzati da zero.

Per ulteriori informazioni sui rapporti incorporati, vedi [Utilizzare i report incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md). Per informazioni sulla creazione di un rapporto copiandolo, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

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
   <td> <p>Ottieni le autorizzazioni di gestione per il report creato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un rapporto {#create-a-report}

Per vedere un video sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](#Walk-thr) sotto.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi selezionare il tipo di oggetto desiderato per il rapporto.

   Viene caricato il generatore di report.

   Per informazioni specifiche sui rapporti sugli oggetti disponibili, consulta la sezione . [Rapporto sugli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Puoi anche creare un rapporto creando una copia di un rapporto esistente. Per ulteriori informazioni, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Nel generatore di report, aggiungi quanto segue al report:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Funzione</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Colonne (Visualizzazione)</td> 
      <td> <p>L’aggiunta di colonne al rapporto determina le informazioni contenute nel rapporto.</p> <p>Per informazioni su come aggiungere una colonna, consulta <a href="#add-columns-view-to-a-report" class="MCXref xref">Aggiungere colonne (visualizzare) a un rapporto</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Raggruppamenti</td> 
      <td> <p>L’aggiunta di raggruppamenti al rapporto determina l’organizzazione del rapporto.</p> <p>Per scoprire come aggiungere un raggruppamento, consulta <a href="#add-groupings-to-a-report" class="MCXref xref">Aggiungere raggruppamenti a un rapporto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtri</td> 
      <td> <p>L’aggiunta di regole di filtro al rapporto determina le informazioni visualizzate nel rapporto.</p> <p>Per informazioni su come aggiungere un filtro, consulta <a href="#add-filters-to-a-report" class="MCXref xref">Aggiungere filtri a un rapporto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Diagramma</td> 
      <td> <p>L’aggiunta di un grafico al rapporto determina la modalità di visualizzazione delle informazioni presenti nel rapporto.</p> <p>Per informazioni su come aggiungere un grafico, consulta <a href="#add-a-chart-to-a-report" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In qualsiasi punto del processo di creazione del rapporto, fai clic su **Applica** per salvare le modifiche.
1. Al termine, fai clic su **Salva e chiudi**.

### Aggiungere colonne (visualizzare) a un rapporto {#add-columns-view-to-a-report}

1. Inizia a creare un rapporto come descritto in [Creare un rapporto](#create-a-report) in questo articolo.
1. Nel generatore di report, seleziona il **Colonne (visualizzazione)** per identificare le colonne da visualizzare nel rapporto.
1. (Facoltativo) Fai clic su **Applicare una visualizzazione esistente** per utilizzare una visualizzazione esistente.

   Per ulteriori informazioni sulla creazione di una nuova visualizzazione, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Per aggiungere una nuova colonna, fai clic su **Aggiungi colonna**.

   Oppure

   Per modificare una colonna esistente, seleziona la colonna da modificare, quindi fai clic sulla (x) accanto al nome corrente.

1. Inizia a digitare il campo da aggiungere. Se il campo è disponibile, viene compilato per ciascun oggetto in cui può essere associato. Fai clic sul nome del campo per aggiungerlo alla colonna.

   Per ulteriori informazioni sui campi visualizzati nelle colonne, vedere [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Facoltativo) In **Impostazioni colonna** area, selezionare **Ordina per colonna** per ordinare i valori nella colonna in ordine crescente in ordine alfabetico decrescente, indicare se l’elenco deve utilizzare questa colonna come primo ordinamento.

   È possibile disporre di più livelli di ordinamento in una visualizzazione di report se si desidera ordinare in base al valore in una prima colonna, al valore in una seconda colonna, e così via.

   Se più risultati sono identici in base al primo criterio di ordinamento, vengono ordinati in base all’ordine del secondo criterio di ordinamento. Se più risultati sono identici in base al primo e al secondo criterio di ordinamento, vengono ordinati in base al terzo ordinamento, ecc.

   >[!NOTE]
   >
   >Se si aggiunge un campo che fa riferimento a un oggetto troppo lontano dall&#39;oggetto su cui si esegue il reporting, potrebbe non essere possibile ordinare in base a questo campo.\
   >Ad esempio, un report di problema non può essere ordinato in base al campo Proprietario progetto perché fa riferimento a 3 oggetti aggiuntivi: Progetto, Proprietario e Nome. Tuttavia, puoi comunque aggiungere questo campo a un report del problema e visualizzare le relative informazioni.\
   >Per ulteriori informazioni sui riferimenti incrociati nei rapporti, consulta la sezione &quot;Advanced Reporting Part 1 of 3&quot; nella sezione [Percorso di apprendimento di Reports and Dashboards](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).

1. (Facoltativo) Se utilizzi i raggruppamenti e desideri riepilogare (aggregare) le informazioni in una colonna, fai clic sul pulsante **Riepiloga questa colonna per** elenco a discesa nella **Impostazioni colonna** , quindi seleziona l’opzione che desideri utilizzare per aggregare le informazioni nella colonna.

   Le informazioni aggregate vengono visualizzate nella colonna nelle righe di raggruppamento.

   ![Riepilogo aggregato dei raggruppamenti](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Per ulteriori informazioni sul riepilogo dei dati in una colonna, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Le seguenti eccezioni si applicano agli oggetti principali (ad esempio, le attività principali) quando si aggregano valori per i seguenti campi nei raggruppamenti:
   >
   >* Tutti i campi relativi al numero e alla divisa, ad eccezione delle ore effettive (ad esempio, Costo manodopera pianificato/effettivo, Costo spesa pianificato/effettivo, Costo pianificato/effettivo, Ore pianificate) aggregano solo i valori relativi alle attività figlio e alle attività autonome. Non aggregano i valori per le attività principali o le attività principali dei genitori.
   >* Le ore effettive aggregano i valori per le attività principali e le attività autonome; non aggregano i numeri relativi alle attività principali o alle attività figlio per le attività padre.
   >* I campi dati personalizzati per i valori di numero e valuta aggregano tutte le attività: genitori, figli, genitori di genitori e compiti autonomi.


   Per ulteriori informazioni sull’utilizzo dei raggruppamenti in un rapporto, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Facoltativo) Fai clic su **Opzioni avanzate** per specificare le seguenti informazioni per la colonna:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta colonna personalizzata</td> 
      <td> <p>Specifica un’etichetta personalizzata per la colonna. Questa etichetta sostituisce l’etichetta predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato campo</td> 
      <td> <p>Selezionare il formato in cui si desidera visualizzare i valori per i campi della colonna.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra questa colonna quando in un dashboard</td> 
      <td> <p>Seleziona questa opzione per visualizzare questa colonna su un dashboard, quando il rapporto viene visualizzato accanto a un altro rapporto. Se questa opzione non è selezionata, questa colonna non viene visualizzata quando il rapporto viene visualizzato in una dashboard in cui i rapporti vengono visualizzati affiancati.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Regole colonna</td> 
      <td> <p>Fai clic su <strong>Aggiungi una regola per questa colonna</strong> per aggiungere la formattazione condizionale alla colonna. Dopo aver aggiunto una regola, puoi definire gli stili di campo e testo per la modalità di visualizzazione dei campi corrispondenti a tale regola. Fai clic su <strong>Aggiungi regola</strong> dopo aver definito la regola. Per ulteriori informazioni sulla formattazione condizionale in una visualizzazione, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Utilizzare la formattazione condizionale nelle visualizzazioni</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Applica** per applicare le modifiche apportate finora e continuare a modificarle con le seguenti opzioni.

   Fai clic su **Salva e chiudi** se hai finito di modificare le colonne del rapporto e desideri salvarlo.

### Aggiungere raggruppamenti a un rapporto {#add-groupings-to-a-report}

1. Inizia a creare un rapporto come descritto in [Creare un rapporto](#create-a-report) in questo articolo.
1. Nel generatore di report, seleziona il **Raggruppamenti** per identificare come raggruppare gli elementi nel rapporto.
1. Fai clic su **Aggiungi raggruppamento** per aggiungere un nuovo raggruppamento.

   Oppure

   Scegli **Applicare un raggruppamento esistente** per selezionare un raggruppamento esistente
   ![](assets/nwe-add-grouping-350x230.png)

1. Inizia a digitare il campo da aggiungere come raggruppamento. Se il campo è disponibile, viene compilato per ciascun oggetto in cui può essere associato. Fai clic sul nome del campo per aggiungerlo al raggruppamento.
1. (Facoltativo) Per creare un raggruppamento in modalità testo, fai clic su **Passa alla modalità testo**. Per ulteriori informazioni sull’utilizzo della modalità testo, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Per ulteriori informazioni sulla creazione di nuovi raggruppamenti, vedi [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Facoltativo) Seleziona **Comprimi questo raggruppamento per impostazione predefinita** se desideri che i risultati in questo raggruppamento vengano visualizzati compressi anziché espansi.

   Questa impostazione è disabilitata per impostazione predefinita e i risultati del raggruppamento vengono sempre visualizzati in un elenco espanso.

   >[!TIP]
   >
   >* Quando si regolano manualmente i raggruppamenti quando si visualizza un elenco, Workfront ricorda le preferenze manuali fino a quando non si disconnette. Quando si effettua di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
   >* I risultati di un raggruppamento vengono sempre espansi dopo l’accesso da un elemento grafico.


1. (Facoltativo) È possibile scegliere di creare un raggruppamento di matrici per visualizzare i risultati in un formato griglia.

   Per ulteriori informazioni sulla creazione di un rapporto sulla matrice, vedi [Creare un rapporto sulla matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Fai clic su **Applica** per applicare le modifiche apportate finora e continuare a modificarle con le seguenti opzioni.

   Fai clic su **Salva e chiudi** se hai finito di modificare i raggruppamenti nel rapporto e desideri salvare il rapporto.

### Aggiungere filtri a un rapporto {#add-filters-to-a-report}

1. Inizia a creare un rapporto come descritto in [Creare un rapporto](#create-a-report) in questo articolo.
1. Nel generatore di report, seleziona il **Filtri** per identificare la quantità di informazioni da includere nel rapporto.
1. Fai clic su **Aggiungere una regola filtro** per aggiungere un filtro personalizzato.\
   Oppure\
   Scegli **Applicare un filtro esistente** per utilizzare un filtro esistente.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Se hai fatto clic su **Aggiungere una regola filtro**, inizia a digitare il campo da aggiungere come filtro. Se il campo è disponibile, viene compilato per ciascun oggetto in cui può essere associato. Fai clic sul nome del campo per aggiungerlo al filtro.\
   Utilizza i modificatori di filtro per creare il filtro. Per ulteriori informazioni sui modificatori dei filtri, consulta [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Per ulteriori informazioni sulla creazione di nuovi filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facoltativo) Per creare un filtro in modalità testo, fai clic su **Passa alla modalità testo**.

   Per ulteriori informazioni sull’utilizzo della modalità testo, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Fai clic su **Applica** una volta completata la modifica dei filtri nel rapporto, potrai applicare le modifiche apportate finora e continuare a modificarlo con le seguenti opzioni.

   Fai clic su **Salva e chiudi** se il rapporto e si desidera salvarlo.

### Aggiungere un grafico a un report {#add-a-chart-to-a-report}

1. Inizia a creare un rapporto come descritto in [Creare un rapporto](#create-a-report) in questo articolo.
1. Nel generatore di report, seleziona il **Grafico** selezionare il tipo di grafico da aggiungere.

   ![](assets/nwe-add-a-chart-350x247.png)

   Per ulteriori informazioni sulla creazione di un grafico in un rapporto, consulta [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Fai clic su **Applica** per applicare le modifiche apportate finora e continuare a modificarle con le seguenti opzioni.

   Fai clic su **Salva e chiudi** se hai finito di modificare il rapporto e desideri salvarlo.
