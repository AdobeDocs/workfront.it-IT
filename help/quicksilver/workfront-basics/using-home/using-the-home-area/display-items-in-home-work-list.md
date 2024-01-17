---
product-area: projects
navigation-topic: use-the-home-area
title: Visualizzare gli elementi in [!UICONTROL Elenco lavori] nell’area Home
description: Il [!UICONTROL Elenco lavori] nel [!UICONTROL Home] In quest'area vengono visualizzati tutti gli elementi di lavoro assegnati all'utente. Puoi controllare quali elementi visualizzare nel tuo [!UICONTROL Elenco lavori], utilizzando i filtri e raggruppando e ordinando gli elementi di lavoro.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '1826'
ht-degree: 0%

---

# Visualizzare gli elementi in [!UICONTROL Elenco lavori] nel [!UICONTROL Home] area

<!-- Audited: 1/2024 -->


Il [!UICONTROL Elenco lavori] nel [!UICONTROL Home] In quest&#39;area vengono visualizzati tutti gli elementi di lavoro assegnati all&#39;utente. Puoi controllare quali elementi visualizzare nel tuo [!UICONTROL Elenco lavori], utilizzando i filtri e raggruppando e ordinando gli elementi di lavoro.

>[!NOTE]
>
>* Quando si converte un problema in un’attività o un progetto, il problema viene rimosso dall’area Home dell’utente assegnato al problema.
>
>* Quando si converte un’attività in un progetto, l’attività viene eliminata e rimossa dall’area Home dell’utente assegnato all’attività.


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Nuovo:</p><ul><li>[!UICONTROL Contributor] solo per le approvazioni</li> <li>[!UICONTROL Standard] o versione successiva per tutti gli altri oggetti</li> <p>Oppure</p> 
  </ul><p>Corrente:</p><ul><li>[!UICONTROL Revisione] solo per le approvazioni</li> <li>[!UICONTROL Work] o versione successiva per tutti gli altri oggetti</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti, attività, problemi e documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni per contribuire o superiore alle attività e ai problemi su cui devi lavorare</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Filtra il [!UICONTROL Elenco lavori]

È possibile filtrare gli elementi in [!UICONTROL Elenco lavori] per visualizzare solo tipi specifici di elementi. Ad esempio, puoi filtrare i [!UICONTROL Elenco lavori] per visualizzare solo i problemi o le richieste.

>[!NOTE]
>
>Le opzioni del filtro sono memorizzate nel browser. Se utilizzi sempre lo stesso browser sullo stesso computer (e non cancelli i dati del sito), i filtri selezionati non cambiano. Se si cambia browser o computer, i filtri tornano all&#39;opzione predefinita, con tutti i filtri deselezionati.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic su **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png) menu a discesa. Se hai selezionato dei filtri, al posto dell’icona viene visualizzato il numero di filtri selezionati.
1. Per specificare il tipo di elementi da visualizzare, seleziona una delle seguenti opzioni di filtro:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tutto]</strong></td> 
      <td>Visualizza e seleziona tutti gli elementi. Ciò include attività, problemi, approvazioni, attività personali e attività e problemi completati. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Working On]</strong></td> 
      <td> <p>Visualizza solo le attività su cui si sta lavorando attivamente. Queste sono attività assegnate all'utente per le quali è stato fatto clic sul pulsante [!UICONTROL Lavoraci].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le attività pronte per l'avvio. Entrambe le istruzioni seguenti devono essere vere:</p> 
        <ul> 
         <li> <p>Le attività e i relativi genitori non hanno predecessori o vincoli di attività che impediscono di lavorarci.</p> </li> 
         <li> <p>La [!UICONTROL Planned Start Date] (Data di inizio pianificata) delle attività è negli ultimi o nel futuro di un massimo di due settimane.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le attività che non sono ancora pronte per l'avvio. Una delle seguenti affermazioni deve essere vera:</p> 
        <ul> 
         <li> <p>Le attività e i relativi genitori potrebbero avere predecessori o vincoli di attività che impediscono di lavorarci.</p> </li> 
         <li> <p>Le attività hanno una [!UICONTROL Planned Start Date] che è più di due settimane nel futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemi: Lavorare]</strong></td> 
      <td> <p>Visualizza solo i problemi su cui si sta lavorando attivamente. Si tratta di problemi assegnati all'utente per i quali si è fatto clic sul pulsante [!UICONTROL Lavoraci].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Requested]</strong></td> 
      <td>Visualizza solo i problemi assegnati a, ma per i quali non è stato fatto clic sul pulsante [!UICONTROL Lavoraci].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personale</strong></td> 
      <td>Visualizza solo le attività personali. Si tratta di attività che vengono create come attività [!UICONTROL Da fare], come descritto nella sezione <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Crea un'attività personale</a> nell’articolo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Crea elementi di lavoro dall'area Home di [!UICONTROL]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le approvazioni assegnate o delegate all'utente e le approvazioni inviate. Le approvazioni includono approvazioni su elementi di lavoro (progetti, attività e problemi) e approvazioni per documenti, bozze, richieste di accesso e schede orario. Per ulteriori informazioni sulle approvazioni, consulta i seguenti articoli:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visualizza approvazioni</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Approvazioni lavoro</a> </p> </li> 
        </ul> 
        <p>Nota: le approvazioni sottomesse e per le quali si è anche uno degli approvatori vengono conteggiate due volte.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegata: delegata da me]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo gli elementi di lavoro delegati a un altro utente.</p> 
        <p>Per ulteriori informazioni sulla delega delle attività, vedere <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delega attività e problemi a un altro utente</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegata: delegata a me]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo gli elementi di lavoro che sono stati temporaneamente delegati da un altro utente.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL completato]</strong></td> 
      <td> <p>Visualizza solo le attività completate, i problemi e le attività personali. Il lavoro completato viene visualizzato per le due settimane precedenti ed è raggruppato in Work List (Elenco di lavoro) in base alla settimana in cui è stato completato. Le approvazioni non sono incluse.</p> <p>Il lavoro completato è nascosto in [!UICONTROL Work List] a meno che non si selezioni questo filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Le opzioni filtro si basano su oggetti (Attività, Problemi, Approvazioni, Attività personali).
   >* I compiti e le questioni sono ulteriormente filtrati dal loro stato in relazione alla nostra disponibilità a lavorare su di essi ([!UICONTROL Lavori in corso], [!UICONTROL Pronto per iniziare], [!UICONTROL Non pronto] per le attività, e [!UICONTROL Lavori in corso] e [!UICONTROL Richiesto] per i problemi). È possibile scegliere di visualizzare le attività o i problemi in uno stato specifico oppure fare clic su Attività o Problemi per selezionare e visualizzare tutti gli stati.
   >* Esiste un filtro separato per gli elementi completati che include sia attività che problemi. Non sono incluse le approvazioni. Il [!UICONTROL Completato] Il filtro include le attività personali.
   >* È possibile scegliere di visualizzare un solo stato alla volta. Ad esempio, puoi visualizzare solo [!UICONTROL Lavori in corso] attività e solo [!UICONTROL Richiesto] problemi. È inoltre possibile selezionare più stati alla volta.
   >* Non è possibile applicare filtri per gli elementi assegnati a uno dei team e le assegnazioni dei team non sono incluse negli elementi assegnati direttamente all&#39;utente.


1. (Facoltativo) Organizza ulteriormente il [!UICONTROL Elenco lavori], come descritto nella sezione [Raggruppa e ordina per data, progetto e priorità](#group-and-sort-by-date-project-and-priority) in questo articolo.

## Raggruppa e ordina per [!UICONTROL Data], [!UICONTROL Progetto], e [!UICONTROL Priorità]

Puoi raggruppare e ordinare i [!UICONTROL Elenco lavori] da [!UICONTROL Data di completamento Pianificata], [!UICONTROL Conferma data], [!UICONTROL Progetto], o [!UICONTROL La mia priorità]. L&#39;opzione scelta determina il modo in cui gli elementi vengono raggruppati nel [!UICONTROL Elenco lavori].

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic su **[!UICONTROL Raggruppa per]** ![Raggruppa per](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) menu a discesa.

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL completamento pianificato]</strong></td> 
      <td> <p> Gli elementi vengono visualizzati nei seguenti raggruppamenti in [!UICONTROL Work List], a seconda della [!UICONTROL Planned Completion Date] (data di completamento pianificata). Il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell'intestazione:</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Nessuna data di completamento pianificata]</p> </li> 
        <li> <p>[!UICONTROL Questa Settimana]</p> <p>Questo raggruppamento viene espanso per impostazione predefinita.</p> </li> 
        <li> <p>[!UICONTROL settimana prossima]</p> </li> 
        <li> <p>[!UICONTROL Planned], seguito da vari [!UICONTROL Planned Completion Dates] (più raggruppamenti)</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Pianificato - Inizio]</strong></td> 
      <td> <p>Gli elementi vengono visualizzati nei seguenti raggruppamenti in [!UICONTROL Work List], a seconda del relativo [!UICONTROL Planned Start Date] (Data di inizio pianificata) (il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell'intestazione):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Questa Settimana] </p> <p>Questo raggruppamento viene espanso per impostazione predefinita.</p> </li> 
        <li> <p>[!UICONTROL settimana prossima]</p> </li> 
        <li> <p>[!UICONTROL Pianificato], seguito da vari [!UICONTROL Pianificato Date Inizio] (più raggruppamenti)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>Gli elementi vengono visualizzati nei seguenti raggruppamenti in [!UICONTROL Work List] (il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell'intestazione):</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Eseguito La Settimana Prossima]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Progetto [!UICONTROL]</strong></td> 
      <td>Gli elementi vengono raggruppati in base al progetto e i progetti vengono visualizzati in ordine alfabetico in [!UICONTROL Work List]. Il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell’intestazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Mia Priorità]</strong></td> 
      <td>Gli articoli vengono visualizzati nell'ordine scelto. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Assegna priorità al lavoro nell'area [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>L&#39;ordinamento predefinito è crescente. Se si modifica l&#39;ordinamento in decrescente, le opzioni di ordinamento selezionate vengono memorizzate nel browser. Se si utilizza sempre lo stesso browser nello stesso computer e non si cancellano i dati del sito, l&#39;ordinamento non cambia, ma se si cambia browser o computer, l&#39;ordinamento diventa quello predefinito.

## Visualizza elementi in ritardo

[!DNL Adobe Workfront] utilizza le date seguenti per determinare se le richieste di lavoro sono in ritardo:

* **Attività**: [!UICONTROL Data di completamento Pianificata]
* **Problemi**: [!UICONTROL Data di completamento Pianificata]
* **Documenti**: [!UICONTROL Data di invio]
* **Schede orario**: [!UICONTROL Data di invio]
* **Approvazioni**: [!UICONTROL Data di invio]
* **Approvazioni bozza**: [!UICONTROL Scadenza bozza]

## Cerca in [!UICONTROL Elenco lavori]

Quando esegui una ricerca nel [!UICONTROL Elenco lavori], tutti gli elementi a te assegnati vengono restituiti nella ricerca (anche quelli che non sono attualmente caricati sullo schermo). Se il [!UICONTROL Mostra completato] è selezionata, verranno restituiti anche tutti gli elementi contrassegnati come completati nelle ultime due settimane.

Inoltre, vengono cercati solo i nomi degli elementi di lavoro (le informazioni all’interno dell’elemento di lavoro non vengono cercate, né i nomi dei progetti in cui risiede l’elemento di lavoro).

Per eseguire ricerche in [!UICONTROL Elenco lavori]:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. (Facoltativo) Filtra e raggruppa i [!UICONTROL Elenco lavori], come descritto in [Filtra il [!UICONTROL Elenco lavori]](#filter-the-work-list) e [Raggruppa e ordina per data, progetto e priorità](#group-and-sort-by-date-project-and-priority).

1. (Facoltativo) Se stai cercando un elemento di lavoro già completo, devi configurare il [!UICONTROL Elenco lavori] per visualizzare gli elementi completati prima della ricerca.

1. Fai clic sull’icona Ricerca ![Ricerca](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Inizia a digitare il nome del nome dell&#39;elemento che stai cercando.\
   Il [!UICONTROL Elenco lavori] viene filtrato automaticamente in modo da includere gli elementi con un nome corrispondente.

## Modificare le dimensioni dell’elenco di lavoro

È possibile modificare le dimensioni del [!UICONTROL Elenco lavori] in modo da consumare da un quarto all&#39;altro dell&#39;area Home a circa la metà [!UICONTROL Home] area.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Passa il puntatore del mouse sul bordo destro [!UICONTROL Elenco lavori], quindi trascina a sinistra o a destra fino a ottenere la dimensione desiderata per Work List (Elenco di lavoro).

## Comprimi ed espandi raggruppamenti

Elementi in [!UICONTROL Elenco lavori] sono visualizzate all’interno di raggruppamenti. È possibile comprimere ed espandere i raggruppamenti per controllare la quantità di informazioni visualizzate sulla pagina in un determinato momento.

È possibile comprimere ed espandere i raggruppamenti all&#39;interno di [!UICONTROL Elenco lavori] per controllare meglio quali informazioni sono visibili.\
Per impostazione predefinita, il [!UICONTROL Questa settimana] Il raggruppamento è espanso e tutti gli altri raggruppamenti sono compressi. Tutte le modifiche apportate vengono memorizzate al successivo accesso all&#39;area Home.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic su **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** accanto a qualsiasi raggruppamento che si desidera espandere o comprimere.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Oppure\
   Per espandere o comprimere tutti i raggruppamenti contemporaneamente, fare clic sul pulsante **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** freccia accanto a qualsiasi raggruppamento tenendo premuto il tasto [!UICONTROL Maiusc] chiave.
