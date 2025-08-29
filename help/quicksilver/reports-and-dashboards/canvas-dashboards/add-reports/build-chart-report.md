---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Creare un rapporto di grafico in un dashboard di Canvas
description: È possibile aggiungere a un dashboard di Canvas un report di grafici che visualizza i dati sotto forma di barre, colonne, linee o grafici a torta.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: d76ad0d51f28191cbd04af950e10a2247414830e
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 0%

---

# Creare un rapporto di grafico in un dashboard di Canvas

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>&#x200B;>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi generare e aggiungere un rapporto di grafico a un dashboard di Canvas per visualizzare i dati come grafico a barre, a colonne, a linee o a torta.

![Report grafico](assets/chart-report-main.png)

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

È necessario creare un dashboard prima di creare un report grafico.

## Creare un rapporto di grafico in un dashboard di Canvas

Sono disponibili molte opzioni di configurazione per la creazione di un rapporto grafico. In questa sezione ti guideremo attraverso il processo generale di creazione di un elemento.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **Grafico**.

1. Nell&#39;angolo in alto a destra, fai clic su **Crea rapporto**.

1. (Facoltativo) Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un rapporto **Nome**.

   1. Immetti un rapporto **Descrizione**.

   1. Se lo desideri, deseleziona la casella **Mostra serie extra come &quot;Altro&quot;**.

      >[!NOTE]
      >
      >È possibile visualizzare in un grafico un massimo di 60 serie. Se questa casella è selezionata, tutte le serie al di sopra del limite vengono consolidate in un raggruppamento **Altro** nel grafico.

1. Segui i passaggi seguenti per configurare la sezione **Genera grafico**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Genera grafico** ![Genera grafico](assets/build-chart-icon.png).

   1. Nell&#39;elenco a discesa **Tipo di grafico** selezionare il tipo di grafico che si desidera creare:

      * **Barra**
      * **Colonna**
      * **Line**
      * **Torta**

   1. Nell&#39;elenco a discesa **Tipo colonna** selezionare il tipo di colonna:
      * **Semplice**
      * **Serie multiple**
      * **In pila**

   1. Selezionare il pulsante **Aggiorna campo** nella prima sezione, quindi individuare e selezionare il campo contenente i dati che verranno riepilogati nel grafico.
   1. Nell&#39;elenco a discesa **Tipo di aggregazione** selezionare la modalità di rollup dei dati per produrre l&#39;output del grafico.

   1. Seleziona il pulsante **Aggiorna campo** sotto la seconda sezione, quindi individua e seleziona il secondo campo da visualizzare nel grafico.

1. Segui i passaggi seguenti per configurare la sezione **Filtro**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro**![ Filtro](assets/filter-icon.png).
   1. Selezionare **Modifica filtro**.
   1. Fare clic su **Aggiungi condizione** e quindi specificare il campo in base al quale si desidera filtrare e il modificatore che definisce il tipo di condizione che il campo deve soddisfare.
   1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fai clic sull’operatore per modificarlo in O.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni colonna di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne espansione** ![Colonne espansione](assets/drilldown-column.png). I campi del grafico vengono visualizzati automaticamente come colonne nella sezione di anteprima a destra.

   1. (Facoltativo) Per aggiornare una delle configurazioni di colonna esistenti, seleziona la colonna da aggiornare nella sezione **Colonne correnti**, quindi aggiorna le informazioni desiderate (ad esempio etichetta, stato del collegamento e condizioni).

   1. Fare clic su **Aggiungi colonna** e quindi selezionare il campo che si desidera visualizzare come colonna nella tabella. Ripetere questo processo per ogni colonna che si desidera aggiungere.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni gruppo di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Impostazioni gruppo](assets/drilldown-group-icon.png).

   1. Fare clic sul pulsante **Aggiungi raggruppamento** e quindi selezionare il campo da creare come raggruppamento.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Creare un esempio di rapporto di grafico

In questa sezione verranno descritti i passaggi necessari per creare un istogramma in cui vengano visualizzate le attività scadute per proprietario del progetto.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **Grafico**.

1. Nell&#39;angolo in alto a destra, fai clic su **Crea rapporto**.

1. Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un report **Nome** (ad esempio *Attività scadute dal proprietario del progetto*).

   1. Immetti un rapporto **Descrizione**.

1. Segui i passaggi seguenti per configurare la sezione **Genera grafico**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Genera grafico**.

   1. Nel menu a discesa **Tipo di grafico**, selezionare **Colonna**.

   1. Nel menu a discesa **Tipo colonna**, selezionare **Semplice**.

   1. Seleziona il pulsante **Aggiorna campo** nella sezione **Asse inferiore (X)**, quindi individua e seleziona il campo **Attività** > **Progetto** > **Proprietario** > **Nome**.

      ![Aggiorna campo](assets/bottom-x-axis.png)

   1. Fai clic sul pulsante **Seleziona campo** sotto la sezione **Asse sinistro (Y)**, quindi individua e seleziona il campo **Attività** > **Nome**.

   1. Nel menu a discesa **Tipo di aggregazione**, selezionare **Conteggio**.

      ![Campo di tipo aggregazione](assets/left-y-axis.png)

1. Segui i passaggi seguenti per configurare la sezione **Filtro**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro**.

   1. Selezionare **Modifica filtro**.

   1. Fai clic su **Aggiungi condizione**.

   1. Fare clic nell&#39;area delle condizioni vuota, quindi selezionare **Scegli campo**.

   1. Selezionare il campo **Percentuale completata**.

   1. Nel menu a discesa **Operatori**, seleziona **Minore di**, quindi immetti *100* nel campo valutatore.

   1. Fai clic su **Aggiungi condizione**, quindi su **Scegli campo**.

   1. Seleziona il campo **Data di completamento pianificata**.

   1. Nel menu a discesa **Operatori**, seleziona **Minore di**.

   1. Imposta **Data relativa** su **ON**.

   1. Immetti *$$TODAY* nel campo valutatore.

      Per ulteriori informazioni sui caratteri jolly, vedere la sezione Variabili di filtro per i caratteri jolly basati sulla data nell&#39;articolo [Modifica filtri di report in un dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

      ![Campo valutatore](assets/add-condition.png)

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni colonna di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne espansione** ![Colonne espansione](assets/drilldown-column.png). I campi del grafico vengono visualizzati automaticamente come colonne nella sezione di anteprima a destra.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Assegnato a** > **Nome**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data inizio pianificata**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data di completamento pianificata**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data ultimo aggiornamento**.

   1. (Facoltativo) Per visualizzare l&#39;ora di aggiornamento, seleziona l&#39;opzione **Data ultimo aggiornamento** nel campo **Colonne correnti**, quindi seleziona un&#39;opzione relativa al valore dell&#39;ora nel menu a discesa **Formato data**.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni gruppo di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Impostazioni gruppo](assets/drilldown-group-icon.png).

   1. Fai clic sul pulsante **Aggiungi raggruppamento**, quindi seleziona il campo **Progetto** > **Nome**.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Considerazioni durante la creazione di un rapporto grafico

### Utilizzo del selettore di campo

L&#39;elenco a discesa **Sezioni** nella sezione **Genera grafico** è progettato per limitare le scelte in un selettore di campi in modo da semplificare la ricerca di un oggetto durante la creazione di un report di tabella. Per iniziare, selezionate un oggetto entità di base.

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