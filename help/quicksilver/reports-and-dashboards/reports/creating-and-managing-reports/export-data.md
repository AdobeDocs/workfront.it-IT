---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Esportare i dati
description: 'Alcuni dei motivi per esportare i dati sono: EDIT ME.'
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '2182'
ht-degree: 0%

---

# Esportare i dati

Puoi esportare i dati di Adobe Workfront da vari elenchi, rapporti, dashboard e ricerche.
Le informazioni contenute nel presente articolo non si applicano alle seguenti esportazioni:

* Esportazione di informazioni dai report grafici.

   Per ulteriori informazioni sull&#39;esportazione di un report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Esportazione di informazioni dal diagramma di Gantt.

   Per ulteriori informazioni sull&#39;esportazione del diagramma di Gantt, vedere [Esportare il Diagramma di Gantt in PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Esportazione di informazioni dal planner risorse.

   Per ulteriori informazioni sull&#39;esportazione delle informazioni dal Planner risorse, vedere &quot;Opzione di esportazione&quot; in [Panoramica sulla navigazione in planner risorse](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Alcuni dei motivi per esportare i dati sono:

* Desideri fornire una copia cartacea dei tuoi dati a un utente esterno a Workfront.
* Desideri inviare i risultati di un rapporto come allegato a un utente esterno.
* Vuoi creare un backup esterno dei tuoi dati Workfront.
* Esiste un limite per visualizzare solo 2.000 risultati su una pagina all&#39;interno dell&#39;applicazione Web Workfront. Se il report produce più di 2.000, puoi esportare il report in uno qualsiasi dei formati indicati di seguito e visualizzare tutti i risultati del report in un unico elenco.

Puoi esportare manualmente un rapporto dall’interfaccia di Workfront oppure pianificare una consegna per un rapporto che ti verrà inviata in un secondo momento. Per ulteriori informazioni sulla pianificazione dei rapporti consegnati, vedi [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido a rapporti, dashboard, calendari da esportare</p> <p>Visualizzare o accedere in modo più elevato agli oggetti visualizzati in un elenco per esportare l’elenco</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un report o dashboard per esportare il report o il dashboard</p> <p>Visualizzare o concedere autorizzazioni superiori agli oggetti visualizzati in un elenco per esportare l’elenco</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

È necessario creare il rapporto prima di esportarne i dati.

Per ulteriori informazioni sulla creazione di rapporti, vedi [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Formati e limiti di esportazione

* [Formati di esportazione](#export-formats)
* [Limiti di esportazione](#export-limits)

### Formati di esportazione {#export-formats}

Le informazioni possono essere esportate nei seguenti formati:

* PDF (Lettera orizzontale o verticale, legale, contabile e A4)
* Excel (.xls)
* Excel (.xlsx)
* Delimitato da tabulazioni

>[!NOTE]
>
>Le dashboard possono essere stampate o esportate solo in un file .pdf.

### Limiti di esportazione {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Esistono diverse limitazioni relative al modo in cui i rapporti vengono visualizzati in Workfront e al modo in cui vengono esportati tramite un’esportazione manuale, un rapporto consegnato o tramite l’API.

* **50.000 righe:** Il numero di righe di dati consentite in un&#39;esportazione di report per file .pdf e delimitati da tabulazioni.

   * Per i file Excel .xls questo limite è **65.000 righe**.
   * Per i file Excel .xlsx questo limite è **100.000 righe**.
   * Questi limiti escludono le intestazioni di colonna e le righe per i raggruppamenti nel rapporto. Ad esempio, se in un rapporto sono presenti 6 raggruppamenti e 50.000 righe o dati, il file esportato avrà 50.000 righe.

   >[!IMPORTANT]
   >
   >L’esportazione di un rapporto che include un riferimento a una raccolta all’interno di una colonna può causare un errore, anche se il rapporto si trova entro i limiti di esportazione elencati. Se la raccolta di riferimento è troppo grande, il processo di esportazione si interrompe e si verifica quindi un errore.
   >
   >Per evitare questo errore, escludere le colonne che fanno riferimento a raccolte di grandi dimensioni o ridurre la dimensione delle raccolte a cui si fa riferimento prima dell’esportazione.

   Se il rapporto contiene più elementi di questi limiti, viene visualizzato un errore di errore che indica che l’esportazione non è riuscita. Riduci il numero di elementi visualizzati sullo schermo a un numero minore o uguale a questi limiti per poter esportare i risultati.

   Se il rapporto contiene più di 50.000/65.000/100.000 righe e desideri esportare tutti i dati, è consigliabile utilizzare filtri o prompt per ottenere carichi di dati più ridotti ed eseguire più esportazioni.

   Per informazioni sull’utilizzo dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   Per informazioni sull&#39;utilizzo dei prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Tali limiti si applicano:

   * Esportazione manuale di un report.
   * Un rapporto pianificato.
   * Un’esportazione tramite un’integrazione API.
   * Dati esportati tramite un avvio a scatto.

      Per ulteriori informazioni sull&#39;esportazione dei dati tramite i Avvio a calci, vedi [Esportare dati da Adobe Workfront tramite Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

      >[!NOTE]
      >
      >È possibile esportare 50.000 righe in un file di avvio, anche se è possibile esportare i dati solo in un file in formato Excel. 

   * Esportazione delle informazioni di utilizzo per un progetto.

      Per ulteriori informazioni sull&#39;esportazione delle informazioni sull&#39;utilizzo di un progetto, vedi [Panoramica del rapporto Utilizzo risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Dimensione del file di 10 MB:** Limite di dimensioni del file per qualsiasi rapporto esportato pianificato per la consegna. Se un file esportato allegato a un&#39;e-mail ha dimensioni superiori a 5 MB, viene inviato via e-mail un collegamento in cui è possibile scaricare il file invece del rapporto esportato allegato.
* **65.530 collegamenti ipertestuali:** Questo è un limite imposto da Excel sui documenti che contengono più di 65.530 collegamenti ipertestuali. Questi documenti non possono essere aperti quando vengono esportati manualmente o inviati in un rapporto consegnato. Si noti che un documento Excel può contenere solo 200 righe di dati, ma se il documento contiene più di 65.530 collegamenti, il documento non viene aperto. Questo limite esiste solo per i file Excel, non per gli altri formati supportati. 
* **256 colonne**: Questo è un limite imposto da Excel sui documenti che contengono più di 256 colonne. Questi documenti non possono essere esportati manualmente o inviati in un rapporto consegnato. Questo limite esiste solo per i file Excel, non per gli altri formati supportati.

Se tenti di esportare dati oltre il limite, potresti non ricevere tutti i dati previsti nell’esportazione. Piuttosto, viene prodotto un rapporto modificato entro i limiti stabiliti.

Inoltre, i rapporti che richiedono più di 60 minuti per essere eseguiti verranno interrotti.

In caso di dubbi o problemi relativi al limite, contatta il supporto tecnico Workfront.

## Esportare i dati

* [Esportare dati da un report o da un elenco](#export-data-from-a-report-or-list)
* [Esportare dati da un dashboard](#export-data-from-a-dashboard)

### Esportare dati da un report o da un elenco {#export-data-from-a-report-or-list}

1. Passa al rapporto o all’elenco da esportare.
1. Seleziona gli elementi da esportare. (Selezionando singoli articoli vengono esportati solo gli articoli selezionati.)

   Ad esempio, in un progetto, selezionare le attività da esportare.

   Oppure

   Lascia deselezionati tutti gli elementi per esportare l’intero elenco.

1. Fai clic su **Esporta**, quindi seleziona un formato.

   >[!NOTE]
   Per esportare un rapporto Dashboard, è necessario disporre di una licenza Piano.\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   Oppure

   Fai clic sul pulsante **Esporta** icona ![](assets/export-icon-nwe.png), quindi seleziona un formato.

   Le opzioni disponibili per l’esportazione di PDF dipendono dalle impostazioni internazionali specificate nelle impostazioni utente di Workfront:

   * Nord America - lettera (predefinita), legale, libro contabile, A4

      <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Tutte le posizioni al di fuori del Nord America - A3, A4 (predefinito), lettera, legale, libro contabile

      <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Condizionale) A seconda del sistema operativo utilizzato, potrebbe essere possibile aprire o salvare il file. Aprire il file con l&#39;applicazione associata o salvarlo sul disco rigido.
1. Continua con [Utilizzare il documento esportato](#use-the-exported-document).

### Esportare dati da un dashboard {#export-data-from-a-dashboard}

È possibile stampare le informazioni da un dashboard o esportarle come file .pdf.

Per ulteriori informazioni sull’esportazione di dati da un dashboard, consulta [Esportare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utilizzare il documento esportato {#use-the-exported-document}

* [Nomi di file](#file-names)
* [Titoli](#titles)
* [Marca temporale](#timestamps)
* [Formattazione](#formatting)
* [Collegamenti](#links)
* [Branding](#branding)

### Nomi di file {#file-names}

Sia che si esporta un elenco di oggetti o un rapporto, il file esportato avrà un nome file e un titolo. È possibile trovare il file esportato sul computer facendo riferimento al nome del file. Il titolo del rapporto fornisce agli utenti un’indicazione di cosa rappresenta il file esportato quando lo condividi con loro.

* [Nomi di file per gli elenchi esportati](#file-names-for-exported-lists)
* [Nomi di file per i rapporti esportati](#file-names-for-exported-reports)

#### Nomi di file per gli elenchi esportati {#file-names-for-exported-lists}

Quando si esporta un elenco di oggetti, il tipo di oggetto viene visualizzato nel file esportato nel nome e nel titolo dell’elenco.

Quando si esporta un elenco di attività o problemi, la **Nome file** può essere uno dei seguenti:

* Quando si esportano gli elenchi di attività e problemi in un progetto:

   * *Nome_progetto_Esportato_Attività*(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*
   * *Il_nome_progetto_Esportato_Problemi*(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*

* Quando si esportano gli elenchi di attività e problemi in un task (sottotask):

   * **Nome_progetto_attività_Nome_attività_Esportato_Attività**(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*
   * **Il_nome_progetto_il_nome_attività_Esportato_Problemi**(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*

Quando si esporta un elenco di qualsiasi altro oggetto da un progetto in un file PDF, il nome del file del documento esportato indica il tipo di oggetti esportati.\
Ad esempio, il nome del file può essere:

* *Exported_Users*, quando si esporta la scheda Persone nel progetto(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*
* *Rischi_Esportati*, quando si esporta un elenco di rischi sul progetto(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*

#### Nomi di file per i rapporti esportati {#file-names-for-exported-reports}

Quando si esporta un report, il nome file del report esportato è:

*Nome_report*(*in formati PDF, Excel, Excel (.xlsx) o delimitati da tabulazioni)*

### Titoli {#titles}

Quando si esporta un elenco di oggetti, solo il file in formato PDF avrà un titolo. Se si esporta un elenco o un rapporto in formato Excel, Excel (.xlsx) o Tab, il file non ha un titolo.

* [Titoli per gli elenchi esportati](#titles-for-exported-lists)
* [Titoli per i rapporti esportati](#titles-for-exported-reports)

#### Titoli per gli elenchi esportati {#titles-for-exported-lists}

Quando si esportano gli elenchi di attività e problemi di un progetto in un file PDF, il titolo del documento esportato è uno dei seguenti:

* *Nome progetto - Attività esportate*
* *Nome progetto - Problemi esportati*

Quando si esportano gli elenchi Attività e Problemi in un&#39;attività in un file PDF, il riquadro del documento esportato è uno dei seguenti:

* *Nome progetto - Nome attività - Attività esportate*
* *Nome progetto - Nome attività - Problemi esportati*

Quando si esporta un elenco di qualsiasi altro oggetto da un progetto a un file PDF, il titolo del documento esportato indica il tipo di oggetti esportati.\
Ad esempio, il titolo può essere:

* *Utenti esportati*, durante l’esportazione della scheda Persone nel progetto.
* *Rischi esportati*, quando si esporta un elenco dei rischi relativi al progetto.

#### Titoli per i rapporti esportati {#titles-for-exported-reports}

Un rapporto esportato in un file PDF avrà un titolo.

Se il rapporto viene esportato in formato Excel, Excel (.xlsx) o Tab, il rapporto esportato non avrà un titolo. Il titolo del file esportato è il nome del report così come viene visualizzato nell&#39;applicazione Web Workfront.

Se il report ha una descrizione, verrà incluso nel file esportato.

### Marca temporale {#timestamps}

Una marca temporale viene visualizzata sul documento esportato dal contesto dell’utente che ha esportato l’elemento.

La marca temporale include:

* Data
* Ora
* Fuso orario in cui è stato esportato l’elemento

A seconda del tipo di documento esportato, le marche temporali vengono visualizzate in varie posizioni:

* **PDF:** Le marche temporali vengono visualizzate nel piè di pagina di ogni pagina e nel nome del file.
* **Excel:** Le marche temporali vengono visualizzate nel nome del file.

### Formattazione {#formatting}

Quando si esporta un progetto in formato .pdf, tutte le sottoattività vengono visualizzate con un rientro rispetto alle attività principali. Gli elenchi esportati non comprimono le attività principali.

Quando un rapporto viene inviato o pianificato per una consegna, viene sempre visualizzata la scheda predefinita di un rapporto, a meno che il rapporto non disponga di una visualizzazione speciale.

Se il report ha una formattazione speciale nell&#39;applicazione Web, il report deve essere consegnato con la formattazione speciale quando le schede Dettagli e Matrice vengono consegnate solo per i file .pdf ed Excel.

>[!NOTE]
Se i dati che stai esportando contengono colonne condivise ed esporti in formato Excel o Tab Delimited, queste colonne sono separate nel file esportato.

Per ulteriori informazioni su come personalizzare la formattazione in un rapporto, consulta [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Collegamenti {#links}

I collegamenti possono puntare a qualsiasi oggetto in Workfront che supporta il collegamento. Quando si esporta un elenco in Workfront in formato .pdf, tutti i collegamenti supportati presenti nel documento originale rimangono attivi nel documento esportato.

>[!TIP]
Se la linea `valueformat=HTML` viene visualizzato in modalità testo per una colonna di campi personalizzata e i valori di collegamento non vengono visualizzati in un file .pdf esportato. È necessario immettere ulteriori righe di codice per la colonna in modalità testo.
Ad esempio, se disponi di un campo personalizzato denominato Open Q1 Projects contenente collegamenti, aggiungi il seguente codice:

```
link.url=customDataLabelsAsString(Open Q1 Projects)
linkedname=direct
```

Quando si esporta in un formato Excel, nel file esportato vengono inclusi solo i collegamenti agli oggetti all’interno di Workfront e sono supportati solo in posizioni in cui è possibile selezionare per consentire i collegamenti nei documenti Excel esportati, ad esempio le consegne di rapporti.

## Branding {#branding}

Se il tuo amministratore Workfront ha aggiunto all’istanza Workfront un marchio personalizzato per la barra di navigazione globale, i file .pdf esportati includono anche il tuo logo personalizzato.

I dati esportati in qualsiasi altro formato non possono essere personalizzati con il tuo logo.

Per ulteriori informazioni sul branding dell&#39;istanza Workfront e della barra di navigazione globale, consulta [Brand your Adobe Workfront instance](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
