---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Generare un rapporto del grafico in una dashboard dell’area di lavoro
description: È possibile aggiungere a un dashboard Canvas un report grafico che visualizza i dati come grafico a barre, a colonne, a linee o a torta.
author: Courtney
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '1814'
ht-degree: 7%

---

# Generare un rapporto del grafico in una dashboard dell’area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Durante questa fase, alcune parti della caratteristica potrebbero non essere complete o funzionare come previsto. Inviate un feedback relativo alla vostra esperienza seguendo le istruzioni nella sezione [Fornisci feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) nell&#39;articolo Panoramica della versione beta dei dashboard di Canvas.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, vedere [Contattare l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

È possibile creare e aggiungere un report grafico a un dashboard dell&#39;area di lavoro per visualizzare i dati come grafico a barre, a colonne, a linee o a torta.

![Report grafico](assets/chart-report-main.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Piano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Modificare l’accesso a report, dashboard e calendari</p>
  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisiti

Per creare un report grafico, è necessario creare un dashboard.

## Generare un rapporto del grafico in una dashboard dell’area di lavoro

Sono disponibili molte opzioni di configurazione per la creazione di un rapporto grafico. In questa sezione ti guideremo attraverso il processo generale di creazione di un elemento.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard**, immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report**, seleziona **Crea report**.

1. Sul lato sinistro, selezionare **Grafico**.

1. Nell&#39;angolo in alto a destra, fai clic su **Crea rapporto**.

1. (Facoltativo) Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un rapporto **Nome**.

   1. Immetti un rapporto **Descrizione**.

   1. Se lo desideri, deseleziona la casella **Mostra serie extra come &quot;Altro&quot;**.

      >[!NOTE]
      >
      >È possibile visualizzare in un grafico un massimo di 60 serie. Se questa casella è selezionata, tutte le serie al di sopra del limite vengono consolidate in un raggruppamento **Altro** nel grafico.
1. Scegliere il tipo di grafico da creare:
   * [Grafico a barre, a colonne o a linee](#bar-column-or-line-chart)
   * [Grafico a torta](#pie-chart)

### Grafico a barre, a colonne o a linee

>[!NOTE]
>
>Potrebbero essere presenti campi aggiuntivi a seconda del tipo di campo selezionato. Le opzioni descritte di seguito sono standard per tutti i tipi di campo.


1. Nel pannello a sinistra, fai clic sull&#39;icona **Crea grafico** ![Crea grafico](assets/build-chart-icon.png).

1. Nell&#39;elenco a discesa **Tipo di grafico**, selezionare **Barra**, **Colonna** o **Riga**.
1. Nel secondo menu a discesa, seleziona il tipo di barra, colonna o riga:
   * **Semplice**
   * **Serie multiple**
   * **In pila**

1. Nella sezione **Asse inferiore (X)**, selezionare il **Campo aggiornamento**, quindi individuare e selezionare il campo contenente i dati che verranno riepilogati nel grafico.
1. Nell&#39;elenco a discesa **Tipo di aggregazione** selezionare la modalità di rollup dei dati per produrre l&#39;output del grafico.
1. (Facoltativo) Aggiungi un’etichetta di asse nello spazio fornito.
1. (Facoltativo) Attiva **Nascondi asse**.
1. (Facoltativo) Immettere un **valore riga di riferimento** per impostare una destinazione o una soglia nel grafico.
1. Scegliere un tipo di **riga** dal menu a discesa.
1. Seleziona il pulsante **Aggiorna campo** sotto la seconda sezione, quindi individua e seleziona il secondo campo da visualizzare nel grafico.


### Grafico a torta

>[!NOTE]
>
>Potrebbero essere presenti campi aggiuntivi a seconda del tipo di campo selezionato. Le opzioni descritte di seguito sono standard per tutti i tipi di campo.


1. Nel pannello a sinistra, fai clic sull&#39;icona **Crea grafico** ![Crea grafico](assets/build-chart-icon.png).

1. Nell&#39;elenco a discesa **Tipo di grafico**, selezionare **Barra**.
1. Nella sezione **Metrica**, selezionare il **Campo aggiornamento**, quindi individuare e selezionare il campo contenente i dati che verranno riepilogati nel grafico.
1. Nel menu a discesa **Tipo di aggregazione**, selezionare la modalità di rollup dei dati per produrre l&#39;output del grafico.
1. Nella sezione **Segmento**, selezionare il **Campo aggiornamento**, quindi individuare e selezionare il campo che contiene i segmenti che si desidera visualizzare nel grafico a torta.
1. (Facoltativo) Nella sezione **Torta**, attiva **Mostra etichette segmento** per visualizzare le etichette dei segmenti.
1. (Facoltativo) Attiva **Mostra totale** per visualizzare il totale al centro del grafico. Quando questa opzione è attivata, sono disponibili opzioni aggiuntive per visualizzare un&#39;etichetta centrale e scegliere il formato del valore.

>[!NOTE]
>
>I tipi di aggregazione vengono visualizzati come segue:
>
>* Conta tipi di aggregazione: il valore centrale visualizzato è un conteggio di tutti i segmenti del grafico.
>* Somma tipi di aggregazione: il valore centrale visualizzato è il totale aggregato del valore numerico o di valuta.
>* Tipi di aggregazione Media, Massimo e Minimo: il valore centrale visualizza di conseguenza il valore medio, Massimo o Minimo.

1. (Facoltativo) Nella sezione Legenda, attiva **Mostra legenda** per visualizzare la legenda del grafico.

1. (Facoltativo) Scegli una **Posizione legenda** dal menu a discesa.

## Configura impostazioni report grafico aggiuntive

### Filtri

Segui i passaggi riportati di seguito per configurare la sezione **Filtro**:

1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro**![ Filtro](assets/filter-icon.png).
1. Selezionare **Modifica filtro**.
1. Fare clic su **Aggiungi condizione** e quindi specificare il campo in base al quale si desidera filtrare e il modificatore che definisce il tipo di condizione che deve soddisfare il campo.
1. (Facoltativo) Fare clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fare clic sull&#39;operatore per modificarlo in OR.

### Impostazioni espansione

Seguire i passaggi riportati di seguito per configurare la sezione **Impostazioni colonna di espansione**:

1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne espansione** ![Colonne espansione](assets/drilldown-column.png). I campi del grafico vengono visualizzati automaticamente come colonne nella sezione di anteprima a destra.

1. (Facoltativo) Per aggiornare una delle configurazioni di colonna esistenti, seleziona la colonna da aggiornare nella sezione **Colonne correnti**, quindi aggiorna le informazioni desiderate (ad esempio etichetta, stato del collegamento e condizioni).

1. Fare clic su **Aggiungi colonna** e quindi selezionare il campo che si desidera visualizzare come colonna nella tabella. Ripetere questa procedura per ogni colonna da aggiungere.

### Impostazioni del gruppo di espansione

Seguire i passaggi riportati di seguito per configurare la sezione **Impostazioni gruppo di espansione**:

1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Impostazioni gruppo](assets/drilldown-group-icon.png).

1. Fai clic sul pulsante **Aggiungi raggruppamento** e seleziona il campo da creare come raggruppamento.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Creare un esempio di rapporto di grafico

In questa sezione verranno descritti i passaggi necessari per creare un istogramma in cui vengano visualizzate le attività scadute per proprietario del progetto.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report**, seleziona **Crea report**.

1. Sul lato sinistro, selezionare **Grafico**.

1. Nell&#39;angolo in alto a destra, fai clic su **Crea rapporto**.

1. Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un report **Nome** (ad esempio *Attività scadute dal proprietario del progetto*).

   1. Immettere un rapporto **Descrizione**.

1. Seguire i passaggi riportati di seguito per configurare la sezione **Crea grafico**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Crea grafico**.

   1. Nell&#39;elenco a discesa **Tipo di grafico**, selezionare **Colonna**.

   1. Nell&#39;elenco a discesa **Tipo di colonna**, selezionare **Semplice**.

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

   1. Fare clic su **Aggiungi condizione**, quindi su **Scegli campo**.

   1. Seleziona il campo **Data di completamento pianificata**.

   1. Nel menu a discesa **Operatori**, seleziona **Minore di**.

   1. Attiva/disattiva **Imposta data relativa** su **ON**.

   1. Immetti *$$TODAY* nel campo valutatore.

      Per ulteriori informazioni sui caratteri jolly, vedere la sezione Variabili di filtro per i caratteri jolly basati sulla data nell&#39;articolo [Modifica filtri di report in un dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

      ![Campo valutatore](assets/add-condition.png)

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni colonna di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne espansione** ![Colonne espansione](assets/drilldown-column.png). I campi del grafico vengono visualizzati automaticamente come colonne nella sezione di anteprima a destra.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Assegnato a** > **Nome**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data inizio prevista**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data di completamento pianificata**.

   1. Fai clic su **Aggiungi colonna**, quindi seleziona il campo **Data ultimo aggiornamento**.

   1. (Facoltativo) Per visualizzare l&#39;ora di aggiornamento, selezionare l&#39;opzione **Data ultimo aggiornamento** nel campo **Colonne correnti**, quindi selezionare un&#39;opzione per il valore dell&#39;ora nell&#39;elenco a discesa **Formato data**.

1. Seguire i passaggi riportati di seguito per configurare la sezione **Impostazioni gruppo di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Impostazioni gruppo](assets/drilldown-group-icon.png).

   1. Fai clic sul pulsante **Aggiungi raggruppamento**, quindi seleziona il campo **Progetto** > **Nome**.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Considerazioni durante la creazione di un report grafico

### Report con dati finanziari

Gli utenti con accesso in visualizzazione o modifica ai dati finanziari nel livello di accesso continueranno a visualizzare i dati finanziari nelle visualizzazioni del dashboard di Canvas, anche se l&#39;autorizzazione Visualizza contabilità viene rimossa a livello di task o di progetto.

* Gli utenti che non dispongono dei diritti relativi ai dati finanziari a livello di accesso non vedranno i dati finanziari nei rapporti.
* Gli utenti che possono vedere i dati finanziari, li vedono solo per i record per i quali dispongono già delle autorizzazioni di visualizzazione (progetti, attività, problemi, ecc.). Non potranno vedere i valori finanziari per i record a cui non possono accedere.
* Per evitare che persone non autorizzate possano accedere a dati finanziari, chi crea i rapporti deve valutare attentamente se includere dati finanziari nelle dashboard e con chi condividere le dashboard stesse.

Si tratta di un limite noto e prevediamo di affrontarlo il più rapidamente possibile.

### Utilizzo del selettore di campo

Il menu a discesa **Sezioni** nella sezione **Crea grafico** è progettato per restringere le scelte in un selettore di campi per facilitare la ricerca di un oggetto durante la creazione di un report di tabella. Per iniziare, selezionare un oggetto entità di base.

* **Tutte le sezioni**: tutti i tipi di oggetto in Workfront Workflow e Workfront Planning.
* **Oggetti Workfront**: oggetti del flusso di lavoro Workfront nativi.
* **Tipi di record di Planning**: tipi di record personalizzati definiti in Workfront Planning.

![Menu a discesa Sezioni](assets/sections-dropdown.png)

Una volta selezionato l&#39;oggetto entità di base, il menu a discesa **Sezioni** viene aggiornato con le opzioni dei tipi di campo applicabili tra cui scegliere.

* **Tutte le sezioni**: campi nativi, campi personalizzati e oggetti correlati.
* **Tutti i campi**: sia i campi nativi che quelli personalizzati (escluse le relazioni).
* **Campi personalizzati**: campi definiti dal cliente in un modulo personalizzato o in un record di Planning.
* **Campi Workfront**: solo campi nativi.
* **Relazioni**: record connessi.

![Selezione oggetti riportabili](assets/reportable-objects-selection.png)

### Riferimento a oggetti figlio

Le relazioni disponibili per colonne aggiuntive, opzioni di filtro e attributi di raggruppamento sono in genere limitate agli oggetti più in alto nella gerarchia degli oggetti di Workfront oppure dispongono di una singola selezione sull&#39;oggetto dell&#39;entità di base del report. Esistono alcune eccezioni a questo, tra cui:

* Progetto > Attività
* Approvazione documento > Fasi approvazione documento
* Fasi approvazione documento > Partecipanti fase approvazione documento

Quando si utilizza una delle relazioni padre-figlio elencate in precedenza, nella tabella verrà visualizzata una riga per ogni record figlio connesso all&#39;oggetto padre.