---
product-area: projects
navigation-topic: use-the-home-area
title: Visualizza elementi in [!UICONTROL Elenco lavori] nell'area Home
description: L'[!UICONTROL Elenco lavori] nell'area [!UICONTROL Home] visualizza tutti gli elementi di lavoro assegnati all'utente. Puoi controllare quali elementi vengono visualizzati nel [!UICONTROL Elenco lavori], utilizzando i filtri e raggruppando e ordinando gli elementi di lavoro.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1840'
ht-degree: 0%

---

# Visualizza gli elementi in [!UICONTROL Elenco lavori] nell&#39;area [!UICONTROL Home]

<!-- Audited: 1/2024 -->


L&#39;[!UICONTROL Elenco lavori] nell&#39;area [!UICONTROL Home] visualizza tutti gli elementi di lavoro assegnati all&#39;utente. Puoi controllare quali elementi vengono visualizzati nel [!UICONTROL Elenco lavori], utilizzando i filtri e raggruppando e ordinando gli elementi di lavoro.

>[!NOTE]
>
>* Quando si converte un problema in un’attività o un progetto, il problema viene rimosso dall’area Home dell’utente assegnato al problema.
>
>* Quando si converte un’attività in un progetto, l’attività viene eliminata e rimossa dall’area Home dell’utente assegnato all’attività.


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
   <td> <p>Autorizzazioni Contribute o superiori per le attività e i problemi su cui devi lavorare</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtra [!UICONTROL Elenco lavori]

È possibile filtrare gli elementi nel [!UICONTROL Elenco lavori] per visualizzare solo tipi specifici di elementi. Ad esempio, puoi filtrare [!UICONTROL Elenco lavori] per visualizzare solo problemi o richieste.

>[!NOTE]
>
>Le opzioni del filtro sono memorizzate nel browser. Se utilizzi sempre lo stesso browser sullo stesso computer (e non cancelli i dati del sito), i filtri selezionati non cambiano. Se si cambia browser o computer, i filtri tornano all&#39;opzione predefinita, con tutti i filtri deselezionati.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic sul menu a discesa **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png). Se hai selezionato dei filtri, al posto dell’icona viene visualizzato il numero di filtri selezionati.
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
         <li> <p>Tutte le attività predecessore sono state completate.</p> </li> 
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
      <td>Visualizza solo le attività personali. Queste attività vengono create come attività [!UICONTROL To Do], come descritto nella sezione <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Creare un'attività personale</a> nell'articolo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Creare elementi di lavoro dalla home page [!UICONTROL]</a>.</td> 
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
        <p>Per ulteriori informazioni sulla delega di attività, vedere <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delegare attività e problemi</a>.
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
   >* Le attività e i problemi sono ulteriormente filtrati in base al loro stato in relazione alla nostra disponibilità a lavorarci ([!UICONTROL Lavorando il], [!UICONTROL Pronto per iniziare], [!UICONTROL Non pronto] per le attività e [!UICONTROL Lavorando il] e [!UICONTROL Richiesto] per i problemi). È possibile scegliere di visualizzare le attività o i problemi in uno stato specifico oppure fare clic su Attività o Problemi per selezionare e visualizzare tutti gli stati.
   >* Esiste un filtro separato per gli elementi completati che include sia attività che problemi. Non sono incluse le approvazioni. Il filtro [!UICONTROL Completed] include le attività personali.
   >* È possibile scegliere di visualizzare un solo stato alla volta. Ad esempio, puoi visualizzare solo [!UICONTROL Attività in corso] e solo [!UICONTROL Richiesti] problemi. È inoltre possibile selezionare più stati alla volta.
   >* Non è possibile applicare filtri per gli elementi assegnati a uno dei team e le assegnazioni dei team non sono incluse negli elementi assegnati direttamente all&#39;utente.


1. (Facoltativo) Organizzare ulteriormente [!UICONTROL Elenco lavori], come descritto nella sezione [Raggruppa e ordina per data, progetto e priorità](#group-and-sort-by-date-project-and-priority) in questo articolo.

## Raggruppa e ordina per [!UICONTROL Data], [!UICONTROL Progetto] e [!UICONTROL Priorità]

Puoi raggruppare e ordinare l&#39;[!UICONTROL Elenco lavori] per [!UICONTROL Data completamento Pianificata], [!UICONTROL Data impegno], [!UICONTROL Progetto] o [!UICONTROL Mia Priorità]. L&#39;opzione scelta determina il modo in cui gli elementi vengono raggruppati in [!UICONTROL Elenco lavori].

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic sul menu a discesa **[!UICONTROL Raggruppa per]** ![Raggruppa per](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

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
      <td>Gli articoli vengono visualizzati nell'ordine scelto. Per ulteriori informazioni, vedere <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Assegnare priorità al lavoro nell'area [!UICONTROL Home]</a>.</td> 
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
* **Schede orario**: [!UICONTROL Data invio]
* **Approvazioni**: [!UICONTROL Data invio]
* **Approvazioni bozza**: [!UICONTROL Scadenza bozza]

## Cerca in [!UICONTROL Elenco lavori]

Durante la ricerca in [!UICONTROL Elenco lavori], vengono restituiti tutti gli elementi assegnati all&#39;utente (anche quelli non attualmente caricati sullo schermo). Se l&#39;opzione [!UICONTROL Mostra completato] è selezionata, verranno restituiti anche tutti gli elementi contrassegnati come completati nelle ultime due settimane.

Inoltre, vengono cercati solo i nomi degli elementi di lavoro (le informazioni all’interno dell’elemento di lavoro non vengono cercate, né i nomi dei progetti in cui risiede l’elemento di lavoro).

Per eseguire una ricerca in [!UICONTROL Elenco lavori]:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. (Facoltativo) Filtrare e raggruppare l&#39;[!UICONTROL Elenco lavori], come descritto in [Filtrare l&#39;[!UICONTROL Elenco lavori]](#filter-the-work-list) e [Raggruppare e ordinare per Data, Progetto e Priorità](#group-and-sort-by-date-project-and-priority).

1. (Facoltativo) Se stai cercando un elemento di lavoro già completato, devi configurare [!UICONTROL Elenco di lavoro] per visualizzare gli elementi completati prima di eseguire la ricerca.

1. Fare clic sull&#39;icona di ricerca ![Ricerca](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Inizia a digitare il nome del nome dell&#39;elemento che stai cercando.\
   L&#39;[!UICONTROL Elenco lavori] viene filtrato automaticamente in modo da includere elementi con un nome corrispondente.

## Modificare le dimensioni dell’elenco di lavoro

È possibile modificare le dimensioni dell&#39;[!UICONTROL Elenco lavori] in modo che occupi un&#39;area compresa tra circa un quarto dell&#39;area Home e circa la metà dell&#39;area [!UICONTROL Home].

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Passa il puntatore del mouse sul bordo destro di [!UICONTROL Elenco lavori], quindi trascina a sinistra o a destra fino a ottenere le dimensioni desiderate per l&#39;elenco lavori.

## Comprimi ed espandi raggruppamenti

Gli elementi in [!UICONTROL Elenco lavori] sono visualizzati all&#39;interno di raggruppamenti. È possibile comprimere ed espandere i raggruppamenti per controllare la quantità di informazioni visualizzate sulla pagina in un determinato momento.

È possibile comprimere ed espandere i raggruppamenti all&#39;interno di [!UICONTROL Elenco lavori] per controllare meglio quali informazioni sono visibili.\
Per impostazione predefinita, il raggruppamento [!UICONTROL Questa settimana] è espanso e tutti gli altri raggruppamenti sono compressi. Tutte le modifiche apportate vengono memorizzate al successivo accesso all&#39;area Home.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. Fare clic sulla freccia **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** accanto ai raggruppamenti che si desidera espandere o comprimere.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Oppure\
   Per espandere o comprimere tutti i raggruppamenti contemporaneamente, fare clic sulla freccia **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** accanto a qualsiasi raggruppamento tenendo premuto il tasto [!UICONTROL Maiusc].
