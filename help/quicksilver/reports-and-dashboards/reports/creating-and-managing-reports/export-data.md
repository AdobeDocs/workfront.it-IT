---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Esporta dati
description: Puoi esportare i dati di Adobe Workfront da vari elenchi, report, dashboard e ricerche.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '2255'
ht-degree: 0%

---

# Esporta dati

<!-- Audited: 12/2023 -->

Puoi esportare i dati di Adobe Workfront da vari elenchi, report, dashboard e ricerche.

Alcuni dei motivi per cui esportare i dati sono:

* Desideri fornire una copia cartacea dei tuoi dati a un utente esterno a Workfront.
* Si desidera inviare i risultati di un report come allegato a un utente esterno.
* Si desidera creare un backup esterno dei dati Workfront.
* È previsto un limite per la visualizzazione di soli 2.000 risultati in una pagina all’interno dell’applicazione web Workfront. Se il report produce più di 2.000, è possibile esportare il report in uno qualsiasi dei formati disponibili e visualizzare tutti i risultati in un unico elenco.

Puoi esportare un rapporto manualmente dall’interfaccia di Workfront, oppure pianificare la consegna di un rapporto che ti verrà inviato in un secondo momento. Per ulteriori informazioni sulla pianificazione dei report consegnati, vedi [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Le informazioni contenute nel presente articolo non si applicano alle seguenti esportazioni:

* Esportazione di informazioni dai report grafico.

  Per ulteriori informazioni sull&#39;esportazione di un report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Esportazione di informazioni dal diagramma di Gantt.

  Per ulteriori informazioni sull&#39;esportazione del grafico Gantt, vedere [Esportare il grafico Gantt in PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Esportazione di informazioni dalla Programmazione risorse.

  Per ulteriori informazioni sull&#39;esportazione delle informazioni dalla Programmazione delle risorse, vedere &quot;Opzione di esportazione&quot; in [Panoramica sulla navigazione di Programmazione delle risorse](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
    <p>Nuovo: Chiaro o superiore</p>
    <p>oppure</p>
    <p>Corrente: revisione o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a report, dashboard e calendari per l’esportazione di report</p> <p>Accesso di visualizzazione o superiore agli oggetti visualizzati in un elenco per esportare l'elenco</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o concedere autorizzazioni superiori a un report o a un dashboard per esportare il report o il dashboard</p> <p>Visualizza o autorizzazioni superiori per gli oggetti visualizzati in un elenco per esportare l'elenco</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per esportare i dati del report è necessario crearlo.

Per ulteriori informazioni sulla creazione di report, vedere [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) o [Creare una copia di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Formati e limiti di esportazione

### Formati di esportazione {#export-formats}

Le informazioni possono essere esportate nei seguenti formati:

* PDF (Lettera orizzontale o verticale, Legale, Contabilità generale e A4)
* Excel (.xls)
* Excel (.xlsx)
* Delimitato in tabella

>[!NOTE]
>
>I dashboard possono essere stampati o esportati solo in un file .pdf.

### Limiti di esportazione {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Esistono diverse limitazioni relative al modo in cui i rapporti vengono visualizzati in Workfront e al modo in cui vengono esportati tramite un’esportazione manuale, un rapporto consegnato o tramite l’API.

* **50.000 celle:** il numero massimo di celle consentito in un&#39;esportazione di report per file Excel.
* **50.000 righe:** il numero di righe di dati consentite in un&#39;esportazione di report per file .pdf e delimitati da tabulazioni.

   * Per i file .xls di Excel, questo limite è **65.000 righe**.
   * Per i file .xlsx di Excel, questo limite è **100.000 righe**.
   * Questi limiti escludono le intestazioni di colonna e le righe per i raggruppamenti nel rapporto. Ad esempio, se in un rapporto sono presenti 6 raggruppamenti e 50.000 righe di dati, il file esportato avrà 50.000 righe.

  >[!IMPORTANT]
  >
  >L’esportazione di un rapporto che include un riferimento a una raccolta all’interno di una colonna può causare un errore, anche se il rapporto si trova entro i limiti di esportazione elencati. Se la raccolta a cui si fa riferimento è troppo grande, il processo di esportazione va in timeout e successivamente genera un errore.
  >
  >Per evitare questo errore, escludi le colonne che fanno riferimento a raccolte di grandi dimensioni o riduci le dimensioni delle raccolte a cui si fa riferimento prima dell’esportazione.

  Se il report contiene più elementi di questi limiti, viene visualizzato un messaggio di errore che indica che l&#39;esportazione non ha esito positivo. Riduci il numero di elementi visualizzati sullo schermo a un numero minore o uguale a questi limiti per poter esportare i risultati.

  Se il report contiene più di 50.000/65.000/100.000 righe e si desidera esportare tutti i dati, è consigliabile utilizzare i filtri o i prompt per ottenere carichi di dati inferiori ed eseguire più esportazioni.

  Per informazioni sull&#39;utilizzo dei filtri, vedere [Panoramica dei filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Per informazioni sull&#39;utilizzo dei prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Questi limiti si applicano a:

   * Esportazione manuale di un report.
   * Un rapporto pianificato.
   * Un’esportazione tramite un’integrazione API.
   * Dati esportati tramite kick-start.

     Per ulteriori informazioni sull&#39;esportazione di dati tramite Kick-Start, vedere [Esportare dati da Adobe Workfront tramite Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >È possibile esportare 50.000 righe in un file di avvio, anche se è possibile esportare i dati solo in un file in formato Excel.

   * Esportazione delle informazioni sull&#39;utilizzo per un progetto.

     Per ulteriori informazioni sull&#39;esportazione delle informazioni sull&#39;utilizzo per un progetto, vedere [Panoramica del report Utilizzo risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Dimensione file 10 MB:** Limite dimensione file per qualsiasi report esportato pianificato per la consegna. Se un file esportato allegato a un messaggio e-mail supera i 5 MB, viene inviato un collegamento tramite e-mail in cui è possibile scaricare il file, anziché il report esportato allegato.
* **65.530 collegamenti ipertestuali:** Si tratta di un limite imposto da Excel ai documenti che contengono più di 65.530 collegamenti ipertestuali. Non è possibile aprire questi documenti quando vengono esportati manualmente o inviati in un report consegnato. Si noti che un documento di Excel può contenere solo 200 righe di dati, ma se il documento contiene più di 65.530 collegamenti, il documento non si apre. Questo limite esiste solo per i file Excel e non per gli altri formati supportati. 
* **256 colonne**: limite imposto da Excel ai documenti contenenti più di 256 colonne. Questi documenti non possono essere esportati manualmente o inviati in un report consegnato. Questo limite esiste solo per i file Excel e non per gli altri formati supportati.

  >[!IMPORTANT]
  >
  >L’esportazione di un rapporto che include una colonna Rapporti può causare un errore anche se il rapporto si trova entro i limiti di esportazione elencati.
  >
  >Se utilizzi la funzione di esportazione per condividere con altri utenti un rapporto contenente una colonna Rapporti, puoi condividere il rapporto rendendolo pubblico. Per ulteriori informazioni su come rendere pubblico un report, vedere [Condividere un report in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Se utilizzi la funzione di esportazione per valutare i dati esternamente, ti consigliamo invece di utilizzare Workfront Data Connect. Per ulteriori informazioni, vedere [Panoramica di Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Se tenti di esportare dati oltre il limite, potresti non ricevere tutti i dati previsti nell’esportazione. Piuttosto, un rapporto modificato viene prodotto entro il limite.

Inoltre, l’esecuzione dei rapporti che richiedono più di 60 minuti verrà interrotta.

In caso di dubbi o problemi relativi al limite, contattare il supporto tecnico Workfront.

## Esporta dati

### Esportare dati da un report o elenco {#export-data-from-a-report-or-list}

1. Passare al report o all&#39;elenco da esportare.
1. Seleziona gli elementi da esportare. Se si selezionano singoli articoli, vengono esportati solo gli articoli selezionati.

   Ad esempio, in un progetto, seleziona le attività da esportare.

   Oppure

   Lascia deselezionati tutti gli elementi per esportare l’intero elenco.

1. Fai clic su **Esporta**, quindi seleziona un formato.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   Oppure

   Fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export-icon-nwe.png), quindi seleziona un formato.

   Le opzioni disponibili per l&#39;esportazione PDF dipendono dalle impostazioni internazionali specificate nelle impostazioni utente di Workfront:

   * Nord America - lettera (predefinita), legale, contabilità generale, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Tutte le ubicazioni al di fuori del Nord America - A3, A4 (impostazione predefinita), lettera, legale, contabilità generale

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Condizionale) A seconda del sistema operativo in uso, è possibile che sia possibile aprire o salvare il file. Aprire il file con l&#39;applicazione associata o salvarlo sul disco rigido.
1. Continua con [Utilizza il documento esportato](#use-the-exported-document).

### Esportare dati da un dashboard {#export-data-from-a-dashboard}

È possibile stampare le informazioni da un dashboard oppure esportarle come file PDF.

Per ulteriori informazioni sull&#39;esportazione di dati da un dashboard, vedere [Esportare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utilizzare il documento esportato {#use-the-exported-document}

* [Nomi file](#file-names)
* [Titoli](#titles)
* [Marca temporale](#timestamps)
* [Formattazione](#formatting)
* [Collegamenti](#links)
* [Branding](#branding)

### Nomi file {#file-names}

Indipendentemente dall&#39;esportazione di un elenco di oggetti o di un report, il file esportato avrà un nome e un titolo. È possibile trovare il file esportato nel computer facendo riferimento al nome del file. Il titolo del report fornirà agli utenti un’indicazione di ciò che il file esportato rappresenta quando lo condividi con loro.

#### Nomi di file per elenchi esportati {#file-names-for-exported-lists}

Quando si esporta un elenco di oggetti, il tipo di oggetto viene visualizzato nel file esportato nel nome e nel titolo dell&#39;elenco.

Quando si esporta un elenco di attività o problemi, **Nome file** può essere uno dei seguenti:

* Quando si esportano gli elenchi di attività e problemi in un progetto:

   * *Le attività nome_progetto_esportato*(*in PDF, Excel, Excel (.xlsx) o nei formati delimitati da tabulazioni)*
   * *Il_nome_progetto_Problemi_esportati*(*in PDF, Excel, Excel (.xlsx) o Formati delimitati da tabulazioni)*

* Quando si esportano elenchi di attività e problemi in un’attività (sottoattività):

   * **Il_nome_progetto_l_nome_attività_Attività_esportate**(*in PDF, Excel, Excel (.xlsx) o nei formati delimitati da tabulazioni)*
   * **Nome_progetto_nome_attività_problemi_esportati**(*in PDF, Excel, Excel (.xlsx) o formati delimitati da tabulazioni)*

Quando esportate un elenco di qualsiasi altro oggetto da un progetto a un file PDF, il nome del file del documento esportato indica il tipo di oggetto esportato.\
Ad esempio, il nome del file può essere:

* *Utenti_esportati*, durante l&#39;esportazione della scheda Persone nel progetto (*in PDF, Excel, Excel (.xlsx) o nei formati delimitati da tabulazioni)*
* *Rischi_esportati*, durante l&#39;esportazione di un elenco di rischi nel progetto (*in PDF, Excel, Excel (.xlsx) o nei formati delimitati da tabulazioni)*

#### Nomi di file per i report esportati {#file-names-for-exported-reports}

Quando si esporta un report, il nome file del report esportato è:

*Nome_report*(*nei formati PDF, Excel, Excel (.xlsx) o delimitato da tabulazioni)*

### Titoli {#titles}

Quando si esporta un elenco di oggetti, solo il file nel formato PDF avrà un titolo. Se si esporta un elenco o un report in formato Excel, Excel (.xlsx) o Tab Delimited, il file non ha un titolo.

#### Titoli per elenchi esportati {#titles-for-exported-lists}

Quando si esportano gli elenchi di attività e problemi di un progetto in un file PDF, il titolo del documento esportato è uno dei seguenti:

* *Nome progetto - Attività esportate*
* *Nome progetto - Problemi esportati*

Quando si esportano gli elenchi di attività e problemi di un&#39;attività in un file PDF, il riquadro del documento esportato è uno dei seguenti:

* *Nome progetto - Nome attività - Attività esportate*
* *Nome progetto - Nome attività - Problemi esportati*

Quando esportate un elenco di qualsiasi altro oggetto da un progetto a un file PDF, il titolo del documento esportato indica il tipo di oggetto esportato.\
Ad esempio, il titolo può essere:

* *Utenti esportati*, durante l&#39;esportazione della scheda Persone nel progetto.
* *Rischi esportati*, durante l&#39;esportazione di un elenco di rischi nel progetto.

#### Titoli per i rapporti esportati {#titles-for-exported-reports}

Un report esportato in un file PDF avrà un titolo.

Se il report viene esportato in Excel, Excel (.xlsx) o Tab Delimited, il report esportato non avrà un titolo. Il titolo del file esportato è il nome del report visualizzato nell&#39;applicazione Web Workfront.

Se il report ha una descrizione, viene incluso nel file esportato.

### Marca temporale {#timestamps}

Nel documento esportato viene visualizzata una marca temporale dal contesto dell&#39;utente che ha esportato l&#39;elemento.

La marca temporale include:

* Data
* Ora
* Fuso orario in cui l&#39;elemento è stato esportato

A seconda del tipo di documento esportato, le marche temporali vengono visualizzate in varie posizioni:

* **PDF:** i timestamp vengono visualizzati nel piè di pagina di ogni pagina e nel nome del file.
* **Excel:** Le marche temporali sono visualizzate nel nome del file.

### Formattazione {#formatting}

Quando si esporta un progetto in formato .pdf, tutte le sottoattività vengono visualizzate come rientrate rispetto alle attività padre. Gli elenchi esportati non comprimono alcuna attività padre.

Quando un rapporto viene inviato o pianificato per una consegna, viene sempre visualizzata la scheda predefinita del rapporto, a meno che questo non abbia una visualizzazione speciale.

Se il report ha una formattazione speciale nell’applicazione web, il report deve essere consegnato con la formattazione speciale quando vengono distribuite le schede Dettagli e Matrice, solo per i file .pdf ed Excel.

>[!NOTE]
>
>Se i dati che si stanno esportando contengono colonne condivise ed esportate in un formato Excel o Tab Delimited, queste colonne vengono separate nel file esportato.

Per ulteriori informazioni su come personalizzare la formattazione in un report, vedere [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Collegamenti {#links}

I collegamenti possono puntare a qualsiasi oggetto in Workfront che supporta il collegamento. Quando si esporta un elenco in Workfront in formato .pdf, tutti i collegamenti supportati presenti nel documento originale rimangono attivi nel documento esportato.

>[!TIP]
>
>Se la riga `valueformat=HTML` viene visualizzata in modalità testo per una colonna di campi personalizzati e i valori dei collegamenti non vengono visualizzati in un file .pdf esportato, è necessario immettere ulteriori righe di codice nella colonna in modalità testo.
>
>Ad esempio, se disponi di un campo personalizzato denominato Apri progetti Q1 contenente collegamenti, aggiungi il seguente codice:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Quando si esegue l&#39;esportazione in un formato Excel, nel file esportato vengono inclusi solo i collegamenti agli oggetti all&#39;interno di Workfront e sono supportati solo nelle posizioni in cui è possibile selezionare l&#39;opzione per consentire i collegamenti nei documenti Excel esportati, ad esempio le consegne dei report.

## Branding {#branding}

>[!IMPORTANT]
>
>Il branding si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Adobe Experience Cloud.
>
>Se la tua organizzazione è stata integrata in Adobe Experience Cloud, il branding non è disponibile.

Se l’amministratore di Workfront ha aggiunto un branding personalizzato all’istanza Workfront per la barra di navigazione globale, i file .pdf esportati includono anche il logo personalizzato.

I dati esportati in altri formati non possono essere personalizzati con il logo.

Per ulteriori informazioni sul branding dell&#39;istanza Workfront e sulla barra di navigazione globale, consulta [Personalizzare il tuo marchio nell&#39;istanza Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
