---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Esplorare il bilanciamento dei carichi di lavoro
description: Utilizza il Bilanciatore dei carichi di lavoro per comprendere la disponibilità delle risorse e per assegnare lavoro agli utenti. Questo articolo illustra come utilizzare le icone e le impostazioni disponibili per aggiornare la visualizzazione e navigare nel Bilanciatore dei carichi di lavoro.
author: Lisa
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8bwTS-3UaNbMLtyx8yEmH7zF5vMYaWP1nedWaGP4UJE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d3382524-5489-431b-bde9-271ab257bc37
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66c43904a7f5d937cba61b6e3da5adeb3a6c0c8c
workflow-type: tm+mt
source-wordcount: 4457
ht-degree: 2%

---

# Esplorare il bilanciamento dei carichi di lavoro

<!--Audited: 12/2024-->

Utilizza il Bilanciatore dei carichi di lavoro in Adobe Workfront per assegnare il lavoro agli utenti in base alla loro disponibilità. Questo articolo descrive come utilizzare le impostazioni e le opzioni per navigare nel Bilanciatore dei carichi di lavoro e visualizzare le informazioni pertinenti. Gli articoli aggiuntivi elencati di seguito descrivono come utilizzare il Bilanciatore dei carichi di lavoro per gestire le risorse e la relativa allocazione al lavoro.

Il Bilanciatore dei carichi di lavoro è disponibile in più aree di Adobe Workfront. La navigazione è simile in tutte le aree.

Per ulteriori informazioni sulla posizione del Bilanciatore dei carichi di lavoro, vedere [Individuare il Bilanciatore dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td>
  </tr>
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Pianificare, quando si utilizza il Bilanciatore dei carichi di lavoro nell'area Risorse; lavorare, quando si utilizza il Bilanciatore dei carichi di lavoro di un team o progetto</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore ai seguenti elementi:</p> 
    <ul> 
     <li>Gestione risorse</li> 
     <li>Progetti</li> 
     <li>Tasks</li> 
     <li>Problemi</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Visualizza o autorizzazioni superiori per i progetti, le attività e i problemi</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per la visualizzazione degli elementi nel Bilanciatore dei carichi di lavoro

Quando visualizzi il Bilanciatore dei carichi di lavoro, considera quanto segue:

* Il Bilanciatore dei carichi di lavoro visualizza gli elementi di lavoro in due aree separate, a seconda delle assegnazioni. Gli elementi di lavoro e gli utenti vengono visualizzati nelle seguenti aree:

  * **Lavoro non assegnato**: elementi che non hanno assegnazioni o che sono assegnati solo a mansioni o team.
  * **Lavoro assegnato**: elementi assegnati ad almeno un utente. Gli elementi assegnati vengono visualizzati sotto il nome dell&#39;utente assegnato.

  >[!NOTE]
  >
  >* Gli elementi di lavoro assegnati a una mansione o a un team e assegnati a un utente vengono visualizzati sia nell&#39;area Lavoro non assegnato che sotto il nome dell&#39;utente assegnato nell&#39;area Lavoro assegnato.
  >* Gli elementi di lavoro assegnati a un utente e una mansione, in cui la mansione è selezionata come assegnataria principale dell’elemento, vengono visualizzati nell’area Lavoro non assegnato.
  >* Gli elementi di lavoro assegnati a più utenti vengono visualizzati sotto tutti i nomi degli utenti assegnati nell’area Lavoro assegnato.
  >* Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata. Per informazioni, vedere la sezione [Personalizzare la visualizzazione](#customize-the-view) in questo articolo.

  Per ulteriori informazioni, vedere [Aree di assegnazione nel Bilanciatore dei carichi di lavoro](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md#assignment-areas-in-the-workload-balancer) in [Panoramica sull&#39;assegnazione di lavoro nel Bilanciatore dei carichi di lavoro](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

* Quando un progetto non ha attività in un determinato periodo di tempo, la barra a livello di progetto è vuota per quel periodo di tempo.

  ![Progetto senza attività durante un periodo di tempo](assets/wb-no-tasks-in-time-period.png)

* Se non disponi delle autorizzazioni necessarie per visualizzare alcuni elementi, questi verranno visualizzati come **elementi di lavoro non accessibili** o **progetti non accessibili**.

  ![Elementi di lavoro non accessibili](assets/wb-inaccessible-work-items.png)

* I nomi degli elementi di lavoro vengono visualizzati a sinistra, mentre la sequenza temporale a destra.
* Il totale delle ore pianificate per ogni elemento di lavoro viene visualizzato a destra del nome dell&#39;elemento di lavoro e a sinistra della barra che rappresenta la sequenza temporale dell&#39;elemento di lavoro.
* Il totale delle ore pianificate per ciascun progetto viene visualizzato a destra del nome del progetto e a sinistra della barra che rappresenta la timeline del progetto.

  Le informazioni sulle ore pianificate per il progetto corrispondono al totale delle ore pianificate per tutti gli elementi elencati nel Bilanciatore dei carichi di lavoro e non al totale delle ore pianificate per il progetto.

Per ulteriori informazioni sulla visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro, vedi anche i seguenti articoli:

* [Individuare il bilanciamento dei carichi di lavoro](../workload-balancer/locate-workload-balancer.md)
* [Filtrare le informazioni nel bilanciamento dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md)
* [Condividere il bilanciamento dei carichi di lavoro con un collegamento](../workload-balancer/share-link-for-workload-balancer.md)
* [Aggiorna elementi di lavoro nel Bilanciatore dei carichi di lavoro utilizzando il Riepilogo](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

Per informazioni sulla gestione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedi anche i seguenti articoli:

* [Panoramica sull’assegnazione del lavoro nel bilanciamento dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer)
* [Gestire le allocazioni degli utenti nel bilanciamento dei carichi di lavoro](https://experienceleague.adobe.com/it/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer)

## Navigare nel Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse

La navigazione nel Bilanciatore dei carichi di lavoro è simile in tutte le aree da cui è possibile accedervi.

Le sottosezioni seguenti descrivono come visualizzare le informazioni nel Bilanciatore dei carichi di lavoro per più progetti.

È possibile regolare una serie di impostazioni e opzioni nel Bilanciatore dei carichi di lavoro per visualizzare le informazioni su cui è necessario concentrarsi nell’intervallo di tempo che ha più senso per te.

Dopo aver selezionato le impostazioni da applicare alla vista, il Bilanciatore dei carichi di lavoro memorizza tali impostazioni ogni volta che vi si accede da un browser o dispositivo.

### Accesso al Bilanciatore dei carichi di lavoro per più progetti nell’area Risorse

Per navigare nel Bilanciatore dei carichi di lavoro per più progetti:

{{step1-to-resourcing}}

1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   ![Bilanciamento del carico di lavoro](assets/wb-in-res-mgmt.png)

   Il Bilanciatore dei carichi di lavoro visualizza le informazioni sull’assegnazione del lavoro a partire dalla settimana corrente nelle due aree seguenti:

   * Nell&#39;area **Lavoro non assegnato** sono visualizzati i seguenti elementi di lavoro:

     * Gli elementi di lavoro (attività e problemi) assegnati a ruoli, team o a cui non è stato assegnato vengono visualizzati dopo l’applicazione dei filtri.
       Nell&#39;area Lavoro non assegnato non viene visualizzato alcun elemento di lavoro per impostazione predefinita. È consigliabile utilizzare i filtri per visualizzare informazioni rilevanti per l&#39;utente in quest&#39;area.

       Per informazioni sull&#39;utilizzo dei filtri, vedere [Informazioni sui filtri nel Bilanciatore dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md).

     * Le assegnazioni di ruolo in elementi di lavoro vengono visualizzate solo quando si abilita l&#39;impostazione Mostra assegnazioni di ruolo. Per informazioni, vedere la sezione [Personalizzare la visualizzazione](#customize-the-view) in questo articolo.

     * I progetti vengono visualizzati solo se si abilita l&#39;impostazione Raggruppa per progetto. Per informazioni, vedere la sezione [Personalizzare la visualizzazione](#customize-the-view) in questo articolo.

   * Nell&#39;area **Lavoro assegnato** sono visualizzati i seguenti elementi di lavoro:

     * Per impostazione predefinita, tutti gli utenti attivi nel sistema vengono visualizzati in quest&#39;area. È consigliabile utilizzare i filtri per limitare la quantità di informazioni in quest’area. Se gli utenti sono assegnati agli elementi, anche gli elementi di lavoro vengono visualizzati sotto il loro nome.

     * Le attività e i problemi assegnati ad almeno un utente vengono visualizzati sotto il nome dell&#39;utente.

       Gli elementi di lavoro sotto i nomi degli utenti nell’area Lavoro assegnato sono ordinati in base ai seguenti criteri, in questo ordine:

       1. Data inizio pianificata (prima la meno recente)
       1. Data di completamento pianificata (prima la meno recente)
       1. Alfabetico per progetto (solo quando i primi due criteri sono identici per più elementi di lavoro)

          >[!TIP]
          >
          >* Puoi personalizzare l’ordinamento dei progetti selezionando un’opzione dall’impostazione &quot;Ordina progetti per&quot;.
          >
          >* I progetti vengono visualizzati solo quando si abilita l&#39;impostazione &quot;Raggruppa per progetto&quot;.
          > 
          >Per informazioni sulla personalizzazione delle impostazioni, vedere la sezione [Personalizzare la visualizzazione](#customize-the-view) in questo articolo.

1. (Facoltativo) Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) nell&#39;area **Lavoro assegnato**, quindi seleziona il **Filtro predefinito** nell&#39;area **Suggested** della casella del filtro.

   Quando si applica il filtro Predefinito, vengono visualizzati gli utenti che appartengono a uno dei team e i relativi elementi di lavoro. Puoi modificare una copia di questo filtro.

   >[!TIP]
   >
   >Il filtro Predefinito è disponibile solo nel Bilanciatore dei carichi di lavoro nell’area Risorse.

1. Per navigare nel Bilanciatore dei carichi di lavoro, procedi come segue:

   * [Selezionare un intervallo di tempo nel Bilanciatore dei carichi di lavoro](#select-a-time-frame-in-the-workload-balancer)
   * [Personalizzare la visualizzazione](#customize-the-view)
   * [Assegnazione di elementi di lavoro e adeguamento delle allocazioni utente](#assign-work-items-and-adjust-user-allocations)
   * [Visualizzare le allocazioni in un grafico](#view-allocations-in-a-chart)

### Selezionare un intervallo di tempo nel Bilanciatore dei carichi di lavoro

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area **Risorse**, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.

   Il Bilanciatore dei carichi di lavoro visualizza le informazioni sull’assegnazione del lavoro a partire dalla settimana corrente.

1. Utilizzare lo scorrimento orizzontale per visualizzare la sequenza temporale degli elementi di lavoro che si estendono oltre i limiti dello schermo.
1. Fai clic sulle icone **avanti o indietro** ![Indietro e avanti](assets/back-and-forward-icons.png) nell&#39;angolo superiore sinistro per spostarti nella timeline, quindi fai clic su **Oggi** per tornare alla settimana corrente.
1. Fare clic sul menu a discesa dell&#39;intervallo di tempo **&#x200B;**&#x200B;sulla barra degli strumenti, quindi fare clic sulla data di inizio del periodo che si desidera visualizzare. Per impostazione predefinita, la prima settimana selezionata nel calendario è quella a cui si è passati.

   ![Selezione calendario](assets/calendar-date-picker-wb.png)

1. Seleziona il numero di settimane da visualizzare contemporaneamente nel Bilanciatore dei carichi di lavoro tra le seguenti opzioni:
   * 1 settimana
   * 2 settimane
   * 4 settimane. Questa è l&#39;impostazione predefinita.
   * 6 settimane
   * 3 mesi

   ![Seleziona settimane](assets/3-months-12-weeks-drop-down-wb.png)

1. Fai clic su una delle seguenti opzioni nella barra degli strumenti per visualizzare le informazioni in base a diversi intervalli di tempo:
   * **Giorno**: visualizza le informazioni per giorno per quattro settimane a partire dalla data odierna, per impostazione predefinita.
   * **Settimana**: visualizza le informazioni per settimana per quattro settimane.
   * **Mese**: visualizza le informazioni per mese per tre mesi.

1. Continua a navigare nel Bilanciatore dei carichi di lavoro come descritto nelle sezioni seguenti.

### Personalizzare la visualizzazione

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area **Risorse**, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.

   I nomi degli elementi di lavoro sono elencati a sinistra e sono rappresentati da barre sul lato destro del Bilanciatore dei carichi di lavoro. La lunghezza della barra rappresenta la timeline di un elemento di lavoro.

1. (Facoltativo e consigliato) Utilizzare i filtri nelle aree Lavoro non assegnato e Lavoro assegnato per visualizzare solo gli elementi di lavoro o gli utenti rilevanti.

   Per ulteriori informazioni, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md).

   Per impostazione predefinita, le barre blu rappresentano le timeline dei progetti e delle attività, mentre le barre laterali rappresentano i problemi.

   È possibile modificare il colore delle barre per i progetti e le attività quando si seleziona il tema del colore in modo che corrisponda al progetto. Per ulteriori informazioni, continuare a leggere questa procedura.

   Gli elementi di lavoro nell’area Lavoro assegnato sono ordinati per progetti in base ai seguenti criteri, in questo ordine:
   1. Data inizio pianificata (prima la meno recente)
   1. Data di completamento pianificata (prima la meno recente)
   1. Alfabetico per progetto (solo quando i primi due criteri sono identici per più elementi di lavoro)

1. Fare clic sulla **freccia rivolta verso destra** a sinistra delle aree Non assegnato o Assegnato per espandere tutti gli elementi sotto i nomi di progetto (nell&#39;area Non assegnato) e sotto i nomi utente (nell&#39;area Assegnato).

   >[!TIP]
   >
   >Gli elementi di lavoro vengono elencati sotto i nomi dei progetti nell&#39;area Non assegnato solo quando si abilita l&#39;impostazione &quot;Raggruppa per progetto&quot;.

1. Fare clic sulla **freccia rivolta verso il basso** a sinistra delle aree Non assegnato o Assegnato per comprimere tutti gli elementi sotto i nomi di progetto (nell&#39;area Non assegnato) e sotto i nomi utente (nell&#39;area Assegnato).

1. Passa il puntatore del mouse, quindi trascina e rilascia la **linea di separazione** tra il pannello sinistro e l&#39;area della timeline per modificare le dimensioni del pannello sinistro.

   ![Riga di separazione](assets/wb-adjust-panel-size.png)

1. Fare clic sull&#39;icona **Impostazioni** ![Impostazioni](assets/settings-gear-icon.png).

   Il pannello Impostazioni viene visualizzato a destra.

   ![Pannello Impostazioni del Bilanciatore dei carichi di lavoro](assets/workload-balancer-settings.png)

   Seleziona tra le opzioni elencate di seguito per aggiornare le informazioni visualizzate nel Bilanciatore dei carichi di lavoro, quindi fai clic sull&#39;icona **X** in alto a destra nella casella Impostazioni per chiuderla.

   * **Raggruppa per progetto**: quando questa opzione è selezionata, gli elementi nelle aree Lavoro non assegnato e Lavoro assegnato sono raggruppati per progetto. Questa opzione è selezionata per impostazione predefinita.

   * **Includi ore da problemi**: quando questa opzione è selezionata, i problemi assegnati agli utenti vengono visualizzati con il nome dell&#39;utente nell&#39;area Lavoro assegnato e i problemi non assegnati agli utenti vengono visualizzati nell&#39;area Lavoro non assegnato. Le ore pianificate conteggiate dai problemi vengono conteggiate in base alle ore pianificate per il progetto e per l’utente nell’area Lavoro assegnato.
   * **Mostra date previste**: se selezionata, oltre alla sequenza temporale pianificata viene visualizzata la sequenza temporale prevista degli elementi di lavoro. Osserva quanto segue:
     * La timeline prevista di progetto, attività e problemi viene visualizzata come una linea blu scuro sopra le barre delle attività, dei problemi e dei progetti.
     * La timeline proiettata che si trova al di fuori della timeline pianificata viene visualizzata in blu chiaro, anche quando si aggiorna il tema colore, come descritto di seguito.
     * La timeline proiettata per gli elementi ai quali non hai accesso alla visualizzazione viene visualizzata in grigio chiaro con una linea al di sotto.
     * Quando un&#39;attività o un problema viene completato prima della data di completamento pianificata, i numeri di allocazione per i giorni rimanenti vengono cancellati e non vengono conteggiati per l&#39;allocazione dell&#39;utente. Questa opzione viene visualizzata solo quando sono abilitate sia l’impostazione Mostra date previste che l’icona Mostra allocazione.

     >[!TIP]
     >
     >Si noti che gli elementi di lavoro vengono visualizzati nel Bilanciatore dei carichi di lavoro quando le timeline pianificate o previste (non necessariamente entrambe nello stesso momento) si verificano durante l’intervallo di tempo selezionato.

   * **Mostra lavoro completato**: quando questa opzione è attivata, le attività e i problemi completati vengono visualizzati nell&#39;area Lavoro assegnato. Questa opzione è attivata per impostazione predefinita.

     Al termine dell’operazione, nell’angolo superiore destro della barra delle attività o dei problemi viene visualizzata un’icona di spunta verde. La stessa icona viene visualizzata per un progetto quando vengono completate le attività o i problemi per l’intervallo di tempo selezionato.

     >[!NOTE]
     >
     >La visibilità delle attività nel Bilanciatore dei carichi di lavoro è determinata dal completamento a livello di attività e non dal completamento a livello di assegnazione. Se un&#39;attività ha più assegnatari e uno o più assegnatari selezionano &quot;Completata con la parte&quot; ma lo stato generale dell&#39;attività non è Completo, l&#39;attività viene considerata come lavoro non completato. Quando l&#39;opzione **Mostra lavoro completato** è disattivata, l&#39;attività viene comunque visualizzata perché non è stata completata.

   * **Mostra tempo rimanente**: quando questa opzione è attivata, in Workfront viene visualizzata la differenza tra il tempo giornaliero per il quale l&#39;utente è disponibile a lavorare in base alle proprie pianificazioni e le ore per le quali è allocato nell&#39;area Lavoro assegnato per gli utenti. Questa funzione è disabilitata per impostazione predefinita e il tempo allocato viene visualizzato per impostazione predefinita.
   * **Mostra assegnazioni ruolo**: quando questa opzione è attivata, le assegnazioni ruolo vengono visualizzate nell&#39;area Lavoro non assegnato sotto gli elementi di lavoro assegnati. Questa opzione è attivata per impostazione predefinita.

   * Nella sezione **Seleziona tema colore** selezionare il colore desiderato per le barre del progetto e dell&#39;attività.

     >[!TIP]
     >
     >L&#39;impostazione per la selezione del tema colore non influisce sul colore delle barre dei problemi. I problemi vengono sempre visualizzati in una barra con colori campione.

     Selezionare una delle opzioni seguenti:
     * **Predefinito**: le barre di tutti i progetti e dei relativi elementi di lavoro vengono visualizzate in blu.
     * **Progetto**: le barre associate a ciascun progetto e alle relative attività cambiano in base al nome del progetto. Tutte le attività appartenenti al progetto vengono visualizzate in barre di colore corrispondente al progetto. Le barre del progetto vengono visualizzate in una tonalità più chiara per distinguerle dalle attività. Le barre del progetto includono anche l’icona di un progetto quando si sceglie di non visualizzare le allocazioni.
     * **Stato progetto**: le barre associate a ciascun progetto e ai relativi elementi di lavoro cambiano in base al colore dello stato del progetto.

       Lo stato del progetto è quello associato al gruppo del progetto. Se il gruppo non dispone di stati specifici, il colore delle barre degli elementi di lavoro è quello dello stato del progetto a livello di sistema. Vengono visualizzati sia gli stati di sistema che quelli personalizzati. Per informazioni sugli stati dei gruppi, vedere [Creare o modificare lo stato di un gruppo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

   * Nella sezione **Visualizzazione dell&#39;allocazione utente in** selezionare una delle opzioni seguenti:
     * **Ore**: visualizza il tempo allocato come ore. Questa è l&#39;impostazione predefinita.
     * **Percentuale**: visualizza il tempo allocato come percentuale del tempo totale disponibile
   * Nella sezione **Preferenze di ordinamento**, seleziona la modalità di ordinamento degli elementi nel Bilanciatore dei carichi di lavoro. Selezionare una delle opzioni seguenti:
     * **Ordina utenti per ruolo principale**: gli utenti vengono visualizzati in ordine alfabetico dei ruoli principali nell&#39;area Lavoro assegnato.
     * **Ordinare gli utenti in ordine alfabetico**: gli utenti vengono visualizzati in ordine alfabetico in base al nome nell&#39;area Lavoro assegnato.
     * **Ordina progetti per**: selezionare un campo del progetto dal menu a discesa per ordinare alfabeticamente i progetti in base a tale campo nelle aree Lavoro non assegnato o Assegnato.

   >[!TIP]
   >
   >È possibile ordinare per progetti solo quando l&#39;impostazione Raggruppa per progetto è abilitata. In caso contrario, l&#39;impostazione è inattiva.

1. (Facoltativo e condizionale) Quando modifichi il tema colore in Stato progetto, passa il puntatore del mouse sul nome di un progetto a sinistra per visualizzarne lo stato.

   ![Descrizione comando stato progetto](assets/hover-over-project-status-tooltip-350x115.png)

### Assegnazione di elementi di lavoro e adeguamento delle allocazioni utente

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area Risorse, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.
1. Fai clic sull&#39;icona **Mostra allocazioni** ![Mostra icona allocazioni](assets/show-allocations-icon-small.png) per visualizzare le ore pianificate giornaliere o settimanali per gli elementi di lavoro.

   Questo sostituisce il nome nelle barre degli elementi di lavoro con la quantità di ore pianificate giornaliere o settimanali nelle aree Lavoro non assegnato e Lavoro assegnato. Questa impostazione è disabilitata per impostazione predefinita.

   I giorni che mostrano le sovrassegnazioni vengono visualizzati in rosso.

   >[!TIP]
   >
   >* L’opzione Mostra allocazioni ha effetto solo sulle visualizzazioni per progetti, attività, problemi ed elementi inaccessibili. Le ore pianificate giornaliere per gli utenti vengono visualizzate per impostazione predefinita e non possono essere nascoste.
   >* Per visualizzare le ore pianificate giornaliere per i progetti, è necessario abilitare l&#39;impostazione Raggruppa per progetto.
   >* Quando visualizzi il Bilanciatore dei carichi di lavoro per settimana, le ore visualizzate corrispondono alle ore pianificate settimanali.

1. (Facoltativo) Passa il cursore del mouse sul tempo allocato nella linea utente per comprendere la capacità e l’allocazione dell’utente. La capacità è la disponibilità dell&#39;utente in base alla sua pianificazione.

   ![Dettagli tempo assegnato](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Facoltativo) Fai clic sull&#39;icona **Nascondi allocazioni** ![Mostra icona allocazioni](assets/show-allocations-icon-small.png) per visualizzare il nome delle attività e dei problemi nelle barre degli elementi di lavoro.
1. Fai clic sull&#39;icona **Altro menu** ![Altro icona](assets/more-icon.png) a destra del nome di un&#39;attività, un problema o un ruolo, quindi fai clic su una delle opzioni seguenti.

   ![Altro menu](assets/more-menu-right-of-task-350x104.png)

   * **Assegna a**, quindi inizia a digitare il nome di un utente, una mansione o un team a cui assegnare l&#39;elemento di lavoro nel campo **Cerca persone, mansione o team**.

     Fare clic su **Avanzate** per accedere alla schermata Assegnazioni avanzate per l&#39;elemento di lavoro. Per ulteriori informazioni, vedere [Creare assegnazioni avanzate](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     Per assegnare attività o problemi, è inoltre possibile utilizzare le seguenti scelte rapide:

     * In Windows: CTRL+clic sulla barra delle attività o dei problemi.
     * In Mac: CMD+fai clic sulla barra delle attività o dei problemi.

     Per ulteriori informazioni sull&#39;assegnazione di elementi di lavoro agli utenti nel Bilanciatore dei carichi di lavoro, vedere [Panoramica sull&#39;assegnazione di lavoro nel Bilanciatore dei carichi di lavoro](../workload-balancer/assign-work-in-workload-balancer.md).

     >[!NOTE]
     >
     >Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato solo quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata. Per informazioni, vedere la sezione [Personalizzare la visualizzazione](#customize-the-view) in questo articolo. Per le assegnazioni di ruolo è disponibile solo l&#39;opzione **Assegna a** nel **menu Altro**.

     >[!TIP]
     >
     >Se l’amministratore di Workfront o di gruppo ha abilitato le deleghe nell’ambiente, utilizza la scheda Assegnazioni per assegnare gli utenti all’attività o al problema. Per informazioni sulla delega del lavoro, vedere [Delegare attività e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Modifica allocazioni**, quindi modifica le allocazioni giornaliere o settimanali per l&#39;utente. Per informazioni sulla gestione delle allocazioni utente, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../workload-balancer/manage-user-allocations-workload-balancer.md).

   * **Apri riepilogo**. Il pannello Riepilogo si apre a destra, quindi fai clic sul campo Assegnazioni e inizia a digitare il nome di un utente, ruolo o team nel campo **Cerca persone, ruolo o team** per assegnare l&#39;elemento. Per ulteriori informazioni, vedere la sezione [Visualizzare ulteriori informazioni sulle attività e sui problemi](#display-more-information-about-tasks-and-issues) in questo articolo.

1. (Facoltativo) Fai doppio clic su un&#39;allocazione giornaliera o settimanale per un utente nella barra di un elemento di lavoro per modificare il numero di ore allocate, quindi fai clic sull&#39;icona **Salva** ![Icona Salva](assets/save-allocations-wb.png) per salvare le allocazioni oppure sull&#39;icona **Annulla** ![Icona Annulla](assets/cancel-allocations-wb.png) per rimuovere le allocazioni corrette.

   >[!TIP]
   >
   >Le icone Salva e Annulla vengono visualizzate verso la fine di un’attività o della barra della timeline di un problema.
   >
   >![Salvare o annullare le allocazioni manuali](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   Per informazioni sulla gestione delle allocazioni utente, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Fai clic su **Assegnazioni in blocco** per assegnare elementi di lavoro in blocco.

   Per ulteriori informazioni, consulta [Assegnare il lavoro in blocco utilizzando il bilanciamento dei carichi di lavoro](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md).
1. Trascina gli elementi dall&#39;area **Lavoro non assegnato** o da un utente e rilasciali su un altro utente per assegnarli.

   Per ulteriori informazioni, consulta [Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

### Visualizzare le allocazioni in un grafico

Anziché visualizzare le allocazioni in numeri giornalieri o settimanali, è possibile visualizzarle in un grafico.

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area Risorse, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.
1. Fai clic sull&#39;icona **Grafico** ![Grafico](assets/user-allocation-chart-icon.png) per visualizzare l&#39;allocazione utente in un formato grafico.

   I giorni in cui l’utente è sovrassegnato vengono visualizzati come blocchi rossi e i giorni in cui l’utente è sottoassegnato o alla capacità come blocchi blu.

   Le dimensioni dei blocchi indicano la quantità di allocazione: più grande è la casella, maggiore è il tempo che l’utente viene assegnato agli elementi di lavoro per quel giorno o quella settimana.

   ![Allocazione utente come grafico](assets/wb-allocation-as-chart.png)

### Visualizza ulteriori informazioni su attività e problemi

Puoi visualizzare ulteriori informazioni sulle attività e sui problemi nel Bilanciatore dei carichi di lavoro.

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area Risorse, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.
1. Per visualizzare ulteriori informazioni nel pannello Riepilogo, effettuate una delle seguenti operazioni:

   * Fai clic sulla barra di un’attività o di un problema per aprire il pannello Riepilogo a destra.
   * Fai clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/summary-panel-icon.png), quindi fai clic sulla barra di un&#39;attività o di un problema per aprire il pannello Riepilogo.
   * Fai clic sul menu **Altro** a destra di un&#39;attività o di un problema, quindi fai clic su **Apri riepilogo**.

   Per informazioni sull&#39;aggiornamento delle informazioni sulle attività nel Riepilogo nel Bilanciatore dei carichi di lavoro, vedere [Aggiornare gli elementi di lavoro nel Bilanciatore dei carichi di lavoro utilizzando il Riepilogo](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

1. Passa il puntatore del mouse sul nome di un’attività o di un problema per visualizzare ulteriori informazioni. Sopra l’attività o il problema viene visualizzata una casella con le seguenti informazioni:

   * Nome dell’attività o del problema.
   * Nome del progetto.
   * Le date di inizio e di completamento pianificate.
   * Il numero di ore pianificate.
   * Per le attività, il numero del predecessore.
   * Per le attività, un indicatore nell&#39;angolo superiore della casella che indica se l&#39;attività è pronta per essere lavorata o meno.

   ![Dettagli attività](assets/task-bar-hover-over-detail-wb.png)

1. Fare clic sul nome di un elemento di lavoro a sinistra per accedervi. L’elemento di lavoro viene aperto in una nuova scheda del browser.

### Visualizzare il Bilanciatore dei carichi di lavoro a schermo intero

1. Accedere al Bilanciatore dei carichi di lavoro nell&#39;area Risorse, come descritto nella sezione [Accedere al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.

1. Fai clic sull&#39;icona **Schermo intero** ![Icona Schermo intero](assets/full-screen.png) per visualizzare il Bilanciatore dei carichi di lavoro a schermo intero.

   Il Bilanciatore dei carichi di lavoro occupa l’intera schermata. Le finestre e le schede del browser sono escluse dalla visualizzazione.

1. Fai clic sull&#39;icona **Esci da schermo intero** ![Esci da icona a schermo intero](assets/exit-full-screen.png) per tornare alla schermata predefinita e visualizzare il Bilanciatore dei carichi di lavoro nella scheda del browser.

## Navigare nel Bilanciatore dei carichi di lavoro di un team

La navigazione nel Bilanciatore dei carichi di lavoro di un team è simile alla navigazione nel Bilanciatore dei carichi di lavoro per più progetti. Per informazioni, vedere la sezione [Navigare nel Bilanciatore dei carichi di lavoro per più progetti](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) in questo articolo.

{{step1-to-team}}

Per impostazione predefinita, viene visualizzata la pagina del team predefinito.

1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   ![Bilanciatore dei carichi di lavoro di un team](assets/wb-on-team.png)

   Il Bilanciatore dei carichi di lavoro di un team visualizza le seguenti informazioni, per impostazione predefinita:

   * Nell&#39;area **Lavoro non assegnato**: elementi di lavoro assegnati al team o al team e ai ruoli e che non sono assegnati agli utenti. Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata.
   * Nell&#39;area **Lavoro assegnato**: gli elementi di lavoro assegnati agli utenti vengono visualizzati sotto i nomi degli utenti.

1. Continuare a navigare nel Bilanciatore dei carichi di lavoro di un team come descritto in [Passare al Bilanciatore dei carichi di lavoro per più progetti nell&#39;area Risorse](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) di questo articolo.

## Navigare nel Bilanciatore dei carichi di lavoro di un singolo progetto

{{step1-to-projects}}

1. Fai clic sul nome di un progetto per aprire la pagina del progetto.
1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   ![Bilanciatore dei carichi di lavoro di un progetto](assets/wb-on-project.png)

   Il Bilanciatore dei carichi di lavoro per il progetto visualizza le seguenti informazioni, per impostazione predefinita:

   * Nell&#39;area **Lavoro non assegnato**: elementi di lavoro del progetto assegnati a ruoli o team e non assegnati a utenti. Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata.
   * Nell&#39;area **Lavoro assegnato**: elementi di lavoro del progetto assegnati ad almeno un utente.

   È consigliabile utilizzare i filtri per mostrare solo gli utenti che sono importanti per te.

   Ad esempio, puoi considerare la possibilità di visualizzare solo gli utenti che appartengono ai tuoi team o gruppi. Per ulteriori informazioni, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md).

1. (Facoltativo) Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) nell&#39;area Lavoro assegnato e seleziona l&#39;opzione **Elementi di lavoro del progetto** nell&#39;area **Suggested** del pannello dei filtri. Questo filtro è deselezionato per impostazione predefinita.

   Quando questa opzione è selezionata, vengono visualizzati solo gli elementi assegnati agli utenti del progetto selezionato.

   Quando l’opzione non è selezionata, vengono visualizzati tutti gli elementi assegnati agli utenti del progetto, indipendentemente dai progetti a cui appartengono gli elementi.

1. (Facoltativo e consigliato) Applica un filtro nell&#39;area Lavoro assegnato per visualizzare gli utenti importanti ma che potrebbero non essere assegnati agli elementi del progetto, quindi fai clic sull&#39;icona **Mostra tutti gli utenti** ![Mostra tutti gli utenti icona](assets/show-all-users-icon-project-workload-balancer.png).

   Visualizzando tutti gli utenti, è possibile visualizzare tutti gli utenti di Workfront non ancora assegnati al lavoro o ad altri ruoli nel progetto.

   Puoi applicare prima un filtro per ridurre il numero di utenti visualizzati.

   Ad esempio, potrebbe essere utile filtrare prima per gli utenti che appartengono ai team o ai gruppi, quindi visualizzare tutti gli utenti.

   Per informazioni su come creare un filtro, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md).

   >[!NOTE]
   >
   > L’opzione Mostra tutti gli utenti è disponibile solo per il Bilanciatore dei carichi di lavoro di un progetto.

1. (Facoltativo) Fai clic sull&#39;icona **Mostra allocazioni ruolo** ![Mostra icona allocazioni ruolo](assets/show-role-allocation-icon.png).

   Viene visualizzato il pannello Allocazione ruoli.

   Dalla Pianificazione scenario è possibile visualizzare informazioni sulle ore pianificate associate alle mansioni sul progetto e alle mansioni associate alle iniziative collegate ai progetti.

   Per ulteriori informazioni, vedere [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!NOTE]
   >
   >Non è possibile visualizzare le informazioni sulle mansioni dell&#39;iniziativa se l&#39;organizzazione non ha acquistato una licenza per Workfront Scenario Planner. In questo caso, puoi visualizzare solo le ore pianificate associate alle mansioni sul progetto. Per ulteriori informazioni, vedere [Accesso necessario per utilizzare la Pianificazione scenario](../../scenario-planner/access-needed-to-use-sp.md).

1. Continuare a navigare nel Bilanciatore dei carichi di lavoro di un progetto come descritto nella sezione [Passare al Bilanciatore dei carichi di lavoro per più progetti](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) di questo articolo.

## Navigare nel Bilanciatore dei carichi di lavoro di un utente

Puoi accedere al Bilanciatore dei carichi di lavoro sul tuo profilo utente.

{{step1-click-profile-pic}}

1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   Viene visualizzato il Bilanciatore dei carichi di lavoro per l’utente.

   ![Bilanciatore dei carichi di lavoro di un utente](assets/workload-balancer-user.png)

   Il Bilanciatore dei carichi di lavoro di un utente visualizza quanto segue per impostazione predefinita:

   * **Lavoro assegnato**: le attività e i problemi assegnati all&#39;utente specifico.

   >[!NOTE]
   >
   >Il Bilanciatore dei carichi di lavoro in un profilo utente è di sola lettura e non è possibile modificare assegnazioni e allocazioni.

1. Continuare a navigare nel Bilanciatore dei carichi di lavoro di un utente come descritto nella sezione [Passare al Bilanciatore dei carichi di lavoro per più progetti](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) di questo articolo.

