---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Creare un rapporto KPI in un dashboard Area di lavoro
description: È possibile aggiungere a un dashboard Canvas un rapporto KPI che visualizzi in modo evidente un singolo indicatore KPI aggregato.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d76ad0d51f28191cbd04af950e10a2247414830e
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 0%

---

# Creare un rapporto KPI in un dashboard Area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>&#x200B;>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi generare e aggiungere un rapporto KPI a un dashboard di Canvas che rappresenti visivamente i dati chiave degli indicatori di prestazioni sotto forma di numero, da utilizzare per visualizzare le prestazioni dei progetti e dei team.

![Esempio di report KPI](assets/kpi-example-main.png)

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>piano Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td> 
<p>Corrente: Piano </p> 
<p>Nuovo: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Modificare l’accesso a rapporti, dashboard e calendari</p>
  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisiti

È necessario creare un dashboard prima di creare un rapporto KPI.

## Creare un rapporto KPI in un dashboard Area di lavoro

Sono disponibili molte opzioni di configurazione per la creazione di un rapporto KPI. In questa sezione ti guideremo attraverso il processo generale di creazione di un elemento.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **KPI**.

1. Nell&#39;angolo superiore destro fare clic su **Crea report**.

1. Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un rapporto **Nome**.
   1. Immetti un rapporto **Descrizione**.

      >[!NOTE]
      >
      >La descrizione verrà utilizzata come didascalia sotto il valore dell’indicatore KPI. Se non si immette una descrizione, verrà generata automaticamente una didascalia in base all&#39;aggregatore e al tipo di aggregazione selezionati nei passaggi seguenti.

1. Segui i passaggi seguenti per configurare la sezione **Genera KPI**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Genera KPI** ![Genera KPI](assets/build-kpi-icon.png).

   1. Fare clic su **Seleziona campo** e quindi specificare il campo che si desidera aggiungere al report.

   1. Nell&#39;elenco a discesa **Tipo di aggregazione** selezionare la modalità di rollup dei dati per produrre l&#39;output KPI. Le opzioni in questo campo variano a seconda del tipo di campo selezionato nel passaggio precedente.

1. Segui i passaggi seguenti per configurare la sezione **Filtro**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selezionare **Modifica filtro**.

   1. Fare clic su **Aggiungi condizione** e quindi specificare il campo in base al quale si desidera filtrare e il modificatore che definisce il tipo di condizione che il campo deve soddisfare.

   1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fai clic sull’operatore per modificarlo in O.

      Per ulteriori informazioni sui filtri, vedere [Modificare i filtri dei report in un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni colonna di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne espansione** ![Colonne espansione](assets/drilldown-column.png). I campi del grafico vengono visualizzati automaticamente come colonne nella sezione di anteprima a destra.

   1. (Facoltativo) Per aggiornare una delle configurazioni di colonna esistenti, seleziona la colonna da aggiornare nella sezione **Colonne correnti** e quindi aggiorna le informazioni desiderate (ad esempio etichetta, stato del collegamento e regole di formattazione).

   1. Fare clic su **Aggiungi colonna** e quindi selezionare il campo che si desidera visualizzare come colonna nella tabella. Ripetere questo processo per ogni colonna che si desidera aggiungere.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni gruppo di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Icona gruppo di espansione](assets/drilldown-group-icon.png).

   1. Fare clic sul pulsante **Aggiungi raggruppamento** e quindi selezionare il campo da creare come raggruppamento.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Creare un esempio di rapporto KPI

In questa sezione verranno descritti i passaggi necessari per creare un report KPI che visualizzi le approvazioni di documenti in sospeso.

Per ulteriori informazioni sugli esempi di report KPI, vedere [Creare un dashboard di report per la revisione e le approvazioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **KPI**.

1. Nell&#39;angolo superiore destro fare clic su **Crea report**.

1. Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Digitare *In sospeso* nel campo **Nome**.
   1. Digitare *Approvazioni in sospeso* nel campo **Descrizione**. Viene visualizzata come didascalia sotto il valore dell&#39;indicatore KPI.

1. Segui i passaggi seguenti per configurare la sezione **Genera KPI**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Genera KPI** ![Genera KPI](assets/build-kpi-icon.png).

   1. Fare clic su **Seleziona campo**.

   1. Individua e seleziona la cartella **Approvazione documento**.

   1. Seleziona **Stato**.

   1. Nel menu a discesa **Tipo di aggregazione**, selezionare **Conteggio**.

1. Segui i passaggi seguenti per configurare la sezione **Filtro**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selezionare **Modifica filtro**.

   1. Fai clic su **Aggiungi condizione**.

   1. Fai clic sul filtro delle condizioni vuoto, fai clic su **Scegli un campo**, quindi scegli **Stato**.
   1. Lascia l&#39;operatore come **Uguale**, quindi digita _in attesa di revisione_ nella casella di testo.
      ![Esempio di filtro KPI in sospeso](assets/pending-kpi-filter.png)
1. Fai clic su **Salva** nell&#39;angolo in alto a destra dello schermo.

## Considerazioni durante la creazione di un rapporto KPI

### Utilizzo del selettore di campo

L&#39;elenco a discesa **Sezioni** nella sezione **Genera KPI** è progettato per limitare le scelte in un selettore di campi in modo da semplificare la ricerca di un oggetto durante la creazione di un report di tabella. Per iniziare, selezionate un oggetto entità di base.

* **Tutte le sezioni**: tutti i tipi di oggetto in Workfront Workflow e Workfront Planning.
* **Oggetti Workfront**: oggetti flusso di lavoro Workfront nativi.
* **Tipi di record di pianificazione**: tipi di record personalizzati definiti in Workfront Planning.

![Elenco a discesa delle sezioni](assets/sections-dropdown.png)

Una volta selezionato l&#39;oggetto entità di base, l&#39;elenco a discesa **Sezioni** viene aggiornato con le opzioni del tipo di campo applicabili tra cui scegliere.

* **Tutte le sezioni**: campi nativi, campi personalizzati e oggetti correlati.
* **Tutti i campi**: campi nativi e personalizzati (escluse le relazioni).
* **Campi personalizzati**: campi definiti dal cliente in un modulo personalizzato o in un record Planning.
* **Campi Workfront**: solo campi nativi.
* **Relazioni**: record connessi.

![Selezione di oggetti segnalabili](assets/reportable-objects-selection.png)

### Riferimento a oggetti figlio

Le relazioni disponibili per colonne aggiuntive, opzioni di filtro e attributi di raggruppamento sono in genere limitate agli oggetti più in alto nella gerarchia degli oggetti di Workfront oppure dispongono di una singola selezione sull&#39;oggetto dell&#39;entità di base del report. Esistono alcune eccezioni a questo, tra cui:

* Progetto > Attività
* Approvazione documento > Fasi di approvazione documento
* Fasi di approvazione documento > Partecipanti fase di approvazione documento

Quando si utilizza una delle relazioni padre-figlio elencate sopra, nella tabella viene visualizzata una riga per ogni record figlio connesso all&#39;oggetto padre.


