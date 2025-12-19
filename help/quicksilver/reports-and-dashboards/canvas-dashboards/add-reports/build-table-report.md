---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Creare un rapporto di tabella in un dashboard di Canvas
description: Puoi aggiungere un rapporto di tabella a un dashboard di Canvas per visualizzare i dati in formato tabella.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: d7caaa0871263fb8ef4224a9c298778f3ee2454a
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 2%

---

# Creare un rapporto di tabella in un dashboard di Canvas

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, vedere [Contattare l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi aggiungere un rapporto di tabella a un dashboard di Canvas per visualizzare i dati in formato tabella.

![Esempio di report tabella](assets/table-example-main.png)

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
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td> 
<p>Standard </p> 
<p>Piano</p> 
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

È necessario creare un dashboard prima di creare un rapporto di tabella.


## Creare un rapporto di tabella in un dashboard di Canvas

Sono disponibili molte opzioni di configurazione per la creazione di un rapporto di tabella. In questa sezione ti guideremo attraverso il processo generale di creazione di un elemento.

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **Tabella**.

1. Nell&#39;angolo superiore destro fare clic su **Crea report**.

1. (Facoltativo) Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Immetti un rapporto **Nome**.

   1. Immetti un rapporto **Descrizione**.

1. Segui i passaggi seguenti per configurare la sezione **Tabella di compilazione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne tabella** ![Icona Genera tabella](assets/drilldown-column.png).

   1. Fare clic su **Aggiungi colonna** e quindi selezionare il campo che si desidera visualizzare come colonna nella tabella. La colonna viene visualizzata nella sezione di anteprima a destra.



   1. Ripetere il passaggio precedente per ogni colonna da aggiungere.

1. Segui i passaggi seguenti per configurare la sezione **Filtro**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selezionare **Modifica filtro**.

   1. Fare clic su **Aggiungi condizione** e quindi specificare il campo in base al quale si desidera filtrare e il modificatore che definisce il tipo di condizione che il campo deve soddisfare. La colonna viene visualizzata nella sezione di anteprima a destra.

1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fai clic sull’operatore per modificarlo in O.

1. Segui i passaggi seguenti per configurare la sezione **Impostazioni gruppo di espansione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Impostazioni gruppo** ![Impostazioni gruppo](assets/drilldown-group-icon.png).

   1. Fare clic sul pulsante **Aggiungi raggruppamento** e quindi selezionare il campo da creare come raggruppamento. La colonna di raggruppamento viene visualizzata nella sezione di anteprima a destra.

1. Fai clic su **Salva** per creare il report e aggiungerlo al dashboard.

## Creare un esempio di rapporto di tabella

In questa sezione verranno descritti i passaggi necessari per creare un report di tabella che visualizzi le approvazioni di documenti in sospeso.

Per ulteriori informazioni sugli esempi di report di tabella, vedere [Creare un dashboard di report per la revisione e le approvazioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo superiore destro.

1. Nella casella **Crea dashboard** immettere il **Nome** e la **Descrizione** del dashboard.

1. Fai clic su **Crea**.

1. Nella casella **Aggiungi report** selezionare **Crea report**.

1. Sul lato sinistro, selezionare **Tabella**.

1. Nell&#39;angolo superiore destro fare clic su **Crea report**.

1. Segui i passaggi seguenti per configurare la sezione **Dettagli**:

   1. Digitare _Approvazioni in sospeso_ nel campo **Nome**.
   1. Digitare una descrizione nel campo **Descrizione**. Questo testo viene visualizzato come descrizione accanto al nome del grafico.

1. Segui i passaggi seguenti per configurare la sezione **Tabella di compilazione**:

   1. Nel pannello a sinistra, fai clic sull&#39;icona **Colonne tabella** ![Colonne tabella](assets/drilldown-column.png).
   1. Fare clic su **Aggiungi colonna**.
   1. Scorri verso il basso e seleziona **Approvazioni documenti** > **Stato**.
   1. Aggiungi le seguenti colonne:

   <table>
    <tr>
    <td><strong>Nome progetto</strong></td>
    <td>Versione documento &gt; Documento &gt; Progetto &gt; Nome</td>
    </tr>
    <tr>
    <td><strong>Nome documento</strong></td>
    <td>Document Version &gt; Document &gt; type <em>Name</em> nella casella di ricerca.</td>
    </tr>
    <tr>
    <td><strong>Versione documento</strong></td>
    <td>Versione documento &gt; Documento &gt; Versione</td>
    </tr>
    <tr>
    <td><strong>Scadenza</strong></td>
    <td>Approvazione documento &gt; Fase approvazione &gt; Scadenza</td>
    </tr>
    <tr>
    <td><strong>Richiesta di</strong></td>
    <td>Approvazione documento &gt; Fase approvazione &gt; Partecipanti fase approvazione* &gt; Richiedente &gt; digita <em>Nome</em> nella casella di ricerca.</td>
    </tr>
    <tr>
    <td><strong>Data richiesta</strong></td>
    <td>Documento Approvazione &gt; Fase di approvazione &gt; Partecipanti fase di approvazione* &gt; Creato in</td>
    </tr>
    <tr>
    <td><strong>Approvatore</strong></td>
    <td>Approvazione documento &gt; Fase approvazione &gt; Partecipanti fase approvazione* &gt; Utente partecipante &gt; digitare <em>Nome</em> nella casella di ricerca.</td>
    </tr>
    </table>


   *I partecipanti alla fase di approvazione sono troncati a _Pa fase di approvazione_


1. Segui i passaggi seguenti per configurare la sezione **Filtro**:
   1. Nel pannello a sinistra, fai clic sull&#39;icona **Filtro** ![scheda filtro](assets/filter-tab.png).
   1. Fai clic su **Modifica filtro**, quindi su **Aggiungi condizione**.
   1. Fai clic sul filtro delle condizioni vuoto, quindi fai clic su **Scegli un campo**.
   1. Seleziona **Stato**.
   1. Cambia l&#39;operatore in **Equal**, quindi digita _in attesa di approvazione_ nella casella di testo.
      ![esempio di filtro della tabella di approvazione in sospeso](assets/pending-approval-table-filter.png)
   1. (Facoltativo) Aggiungi altri filtri come descritto nella sezione **Filtri opzionali** di seguito.
1. Fai clic su **Salva** nell&#39;angolo in alto a destra dello schermo.

## Considerazioni durante la creazione di un rapporto di tabella

### Rapporti con dati finanziari

Gli utenti con l’accesso Visualizzazione o Modifica dei dati finanziari nel loro livello di accesso continueranno a visualizzare i dati finanziari nelle visualizzazioni del dashboard di Canvas, anche se l’autorizzazione Visualizza dati finanziari viene rimossa a livello di task o progetto.

* Gli utenti che non dispongono dei diritti relativi ai dati finanziari a livello di accesso non visualizzeranno i dati finanziari nei rapporti.
* Gli utenti che visualizzano i dati finanziari sono limitati ai record per i quali dispongono già delle autorizzazioni di visualizzazione (progetti, attività, problemi, ecc.). Non vedranno i valori finanziari per i record a cui non possono accedere.
* I creatori dei rapporti devono essere cauti nell’includere dati finanziari nelle dashboard e devono prestare attenzione a chi condividono le dashboard per evitare accessi involontari.

Si tratta di un limite noto e prevediamo di affrontarlo il più rapidamente possibile.

### Utilizzo del selettore di campo

L&#39;elenco a discesa **Sezioni** nella sezione **Tabella di compilazione** è progettato per limitare le scelte in un selettore di campi in modo da semplificare la ricerca di un oggetto durante la creazione di un report di tabella. Per iniziare, selezionate un oggetto entità di base.

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
