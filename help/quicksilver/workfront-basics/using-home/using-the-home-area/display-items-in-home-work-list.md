---
product-area: projects
navigation-topic: use-the-home-area
title: Visualizza gli elementi nel [!UICONTROL Elenco lavori] nell'area Home
description: La [!UICONTROL Elenco lavori] in [!UICONTROL Pagina principale] area visualizza tutti gli elementi di lavoro assegnati all'utente. Puoi controllare quali elementi visualizzare nel [!UICONTROL Lavoro] Elenco come descritto di seguito.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Visualizza gli elementi nel [!UICONTROL Elenco lavori] nell&#39;area Home

La [!UICONTROL Elenco lavori] in [!UICONTROL Pagina principale] area visualizza tutti gli elementi di lavoro assegnati all&#39;utente. Puoi controllare quali elementi visualizzare nel [!UICONTROL Lavoro] Elenco come descritto di seguito.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>Revisione solo per le approvazioni</p> <p>Lavoro o superiore per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Visualizzazione o accesso a progetti, attività, problemi e documenti</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni di Contribute o superiori alle attività e ai problemi su cui lavorare</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Filtrare [!UICONTROL Elenco lavori]

Puoi filtrare gli elementi nella [!UICONTROL Elenco lavori] per visualizzare solo tipi specifici di elementi. Ad esempio, puoi filtrare il [!UICONTROL Elenco lavori] per visualizzare solo i problemi o le richieste.

>[!NOTE]
>
>Le opzioni del filtro sono memorizzate nel browser. Se utilizzi sempre lo stesso browser sullo stesso computer (e non cancelli i dati del sito) i filtri selezionati non cambiano. Se si passa a un browser o a un computer, i filtri ripristinano l&#39;opzione predefinita, che è con tutti i filtri deselezionati.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. Fai clic sul pulsante **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png) menu a discesa.
1. Seleziona tra le seguenti opzioni filtro per specificare il tipo di elementi da visualizzare:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL ALL]</strong></td> 
      <td>Visualizza e seleziona tutti gli elementi. Ciò include attività, problemi, approvazioni, attività personali e attività e problemi completati. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Attività Su Cui Lavorare]</strong></td> 
      <td> <p>Visualizza solo le attività su cui si sta lavorando attivamente. Si tratta di task assegnati per i quali hai fatto clic sul pulsante [!UICONTROL Work On It].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Attività pronte per l'avvio]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le attività pronte per l'avvio. Entrambe le affermazioni seguenti devono essere vere:</p> 
        <ul> 
         <li> <p>I compiti e i loro genitori non hanno predecessori o vincoli di compito che impediscono loro di lavorare.</p> </li> 
         <li> <p>La [!UICONTROL Pianificazione della data di inizio] delle attività è prevista in passato o fino a due settimane in futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Attività non pronte]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le attività non ancora pronte per l'avvio. Una delle seguenti affermazioni deve essere vera:</p> 
        <ul> 
         <li> <p>I compiti e i loro genitori potrebbero avere predecessori o vincoli di compito che impediscono loro di lavorare.</p> </li> 
         <li> <p>Le attività dispongono di una [!UICONTROL Pianificazione della data di inizio] che sarà superiore a due settimane in futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemi Al Lavoro]</strong></td> 
      <td> <p>Visualizza solo i problemi su cui stai lavorando attivamente. Si tratta di problemi a te assegnati per i quali hai fatto clic sul pulsante [!UICONTROL Work On It] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemi richiesti]</strong></td> 
      <td>Visualizza solo i problemi a cui sei assegnato ma per i quali non hai fatto clic sul pulsante [!UICONTROL Work On It].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personale</strong></td> 
      <td>Visualizza solo le attività personali. Si tratta di attività create come attività da eseguire, come descritto nella sezione <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Creare un’attività personale</a> nell'articolo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Creare elementi di lavoro dall'area [!UICONTROL Home]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Visualizza solo le approvazioni assegnate o delegate all'utente e le approvazioni inviate. Le approvazioni includono le approvazioni su elementi di lavoro (progetti, attività e problemi) e le approvazioni per documenti, bozze, richieste di accesso e fogli ore. Per ulteriori informazioni sulle approvazioni, vedere i seguenti articoli:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visualizza approvazioni</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Approvazione del lavoro</a> </p> </li> 
        </ul> 
        <p>Nota: Le approvazioni inviate e in cui si è anche uno degli approvatori vengono conteggiate due volte.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completato]</strong></td> 
      <td> <p>Visualizza solo le attività, i problemi e le attività personali completate. Il lavoro completato viene visualizzato per le due settimane precedenti e viene raggruppato nell'Elenco di lavoro in base alla settimana in cui è stato completato. Le approvazioni non sono incluse.</p> <p>Il lavoro completato viene nascosto nell’[!UICONTROL Work List] a meno che non selezioni questo filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Le opzioni filtro si basano sugli oggetti (Attività, Problemi, Approvazioni, Attività personali).
   >* Le attività e i problemi vengono ulteriormente filtrati dal loro stato in relazione alla nostra disponibilità a lavorarci su ([!UICONTROL Utilizzo], [!UICONTROL Pronto per l&#39;inizio], [!UICONTROL Non pronto] per i compiti e [!UICONTROL Utilizzo] e [!UICONTROL Richiesto] per questioni). È possibile selezionare per visualizzare attività o problemi in uno stato specifico oppure fare clic su Attività o Problemi per selezionare e visualizzare tutti gli stati.
   >* Esiste un filtro separato per gli elementi completati e include sia attività che problemi. Non sono incluse le approvazioni. La [!UICONTROL Completato] Il filtro include le attività Personali.
   >* È possibile selezionare un solo stato alla volta. Ad esempio, puoi visualizzare solo [!UICONTROL Utilizzo] solo attività [!UICONTROL Richiesto] problemi.
   >* Non puoi applicare filtri per gli elementi assegnati a uno dei tuoi team e non sono inclusi negli elementi che ti vengono assegnati direttamente.



1. (Facoltativo) Organizzare ulteriormente [!UICONTROL Elenco lavori], come descritto nella sezione [Raggruppa e ordina per data, progetto e priorità](#group-and-sort-by-date-project-and-priority) in questo articolo.

## Raggruppa e ordina per [!UICONTROL Data], [!UICONTROL Progetto]e [!UICONTROL Priorità]

Puoi raggruppare e ordinare i [!UICONTROL Elenco lavori] da [!UICONTROL Data completamento pianificata], [!UICONTROL Data impegno], [!UICONTROL Progetto]oppure [!UICONTROL Priorità]. L’opzione selezionata determina il modo in cui gli elementi vengono raggruppati nel gruppo [!UICONTROL Elenco lavori].

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. Fai clic sul pulsante **[!UICONTROL Raggruppa per]** menu a discesa.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Seleziona tra le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completamento pianificato]</strong></td> 
      <td> <p> Gli elementi vengono visualizzati nei raggruppamenti seguenti nell’[!UICONTROL Work List], a seconda della [!UICONTROL Planned Completion Date] (Data completamento pianificata) (il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell’intestazione):</p> 
       <ul> 
        <li> <p>[!UICONTROL in ritardo]</p> </li> 
        <li> <p>[!UICONTROL Nessuna Data Di Completamento Pianificata]</p> </li> 
        <li> <p>[!UICONTROL Questa Settimana]</p> <p>Questo raggruppamento viene espanso per impostazione predefinita.</p> </li> 
        <li> <p>[!UICONTROL Settimana Prossima]</p> </li> 
        <li> <p>[!UICONTROL Pianificato], seguito da vari [!UICONTROL Pianificato date di completamento] (raggruppamenti multipli)</p> </li> 
        <li> <p>[!UICONTROL Completato]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Inizio pianificato]</strong></td> 
      <td> <p>Gli elementi vengono visualizzati nei raggruppamenti seguenti nell’[!UICONTROL Work List], a seconda della [!UICONTROL Planned Start Date] (Data inizio pianificata) (il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell’intestazione):</p> 
       <ul> 
        <li> <p>[!UICONTROL in ritardo]</p> </li> 
        <li> <p>[!UICONTROL Questa Settimana] </p> <p>Questo raggruppamento viene espanso per impostazione predefinita.</p> </li> 
        <li> <p>[!UICONTROL Settimana Prossima]</p> </li> 
        <li> <p>[!UICONTROL Pianificato], seguito da varie [!UICONTROL Date di inizio pianificate] (più raggruppamenti)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data del commit]</strong></td> 
      <td> <p>Gli elementi vengono visualizzati nei raggruppamenti seguenti nell’ [!UICONTROL Work List] (il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell’intestazione):</p> 
       <ul> 
        <li> <p>[!UICONTROL Nessuna data di commit]</p> </li> 
        <li> <p>[!UICONTROL Impegnato la settimana prossima]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Gli elementi vengono raggruppati in base al progetto e i progetti vengono visualizzati in ordine alfabetico nell’ [!UICONTROL Work List]. Il numero di elementi contenuti in ciascun raggruppamento viene visualizzato tra parentesi accanto al titolo dell’intestazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL La mia priorità]</strong></td> 
      <td>Gli elementi vengono visualizzati in un ordine scelto. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Dare priorità al lavoro nell'area [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>L&#39;ordinamento predefinito è crescente. Se l’ordinamento viene modificato in decrescente , le opzioni di ordinamento selezionate vengono memorizzate nel browser. Se si utilizza in modo coerente lo stesso browser sullo stesso computer (e non si cancellano i dati del sito) l&#39;ordinamento non cambia, ma se si cambia browser o computer, l&#39;ordinamento viene modificato in base all&#39;ordinamento predefinito.

## Visualizza elementi in ritardo

[!DNL Adobe Workfront] utilizza le date seguenti per determinare se le richieste di lavoro sono in ritardo:

* **Attività**: [!UICONTROL Data completamento pianificata]
* **Problemi**: [!UICONTROL Data completamento pianificata]
* **Documenti**: [!UICONTROL Data di invio]
* **Schede temporali**: [!UICONTROL Data di invio]
* **Approvazioni**: [!UICONTROL Data di invio]
* **Prove di omologazione**: [!UICONTROL Termine di prova]

## Cerca nel [!UICONTROL Elenco lavori]

Quando esegui una ricerca nel [!UICONTROL Elenco lavori], tutti gli elementi assegnati all’utente vengono restituiti nella ricerca (anche quelli che non sono attualmente caricati sullo schermo). Se la [!UICONTROL Mostra completato] viene selezionata l’opzione , vengono restituiti anche tutti gli elementi contrassegnati come completi nelle ultime due settimane.

Vengono inoltre cercati solo i nomi degli elementi di lavoro (le informazioni all’interno dell’elemento di lavoro non vengono cercate, né i nomi dei progetti in cui risiede l’elemento di lavoro).

Per cercare [!UICONTROL Elenco lavori]:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. (Facoltativo) Filtrare il [!UICONTROL Elenco lavori], come descritto in [Filtrare [!UICONTROL Elenco lavori]](#filter-the-work-list) e [Raggruppa e ordina per data, progetto e priorità](#group-and-sort-by-date-project-and-priority).

1. (Facoltativo) Se stai cercando un elemento di lavoro già completato, devi configurare il [!UICONTROL Elenco lavori] per visualizzare gli elementi completati prima della ricerca.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Inizia a digitare il nome dell’elemento che stai cercando.\
   La [!UICONTROL Elenco lavori] viene filtrato automaticamente in modo da includere elementi con un nome corrispondente.

## Modificare le dimensioni dell&#39;elenco di lavoro

È possibile modificare le dimensioni del [!UICONTROL Elenco lavori] in modo che consuma ovunque tra circa un quarto dell&#39;area Home e circa la metà del [!UICONTROL Pagina principale] area.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. Passa il mouse sul bordo destro del [!UICONTROL Elenco lavori], quindi trascinare a sinistra o a destra finché l’Elenco di lavoro non raggiunge la dimensione desiderata.

## Comprimere ed espandere i raggruppamenti

Elementi nel [!UICONTROL Elenco lavori] vengono visualizzati all’interno dei raggruppamenti. È possibile comprimere ed espandere i raggruppamenti per controllare la quantità di informazioni visualizzate sulla pagina in un dato momento.

È possibile comprimere ed espandere i raggruppamenti all’interno di [!UICONTROL Elenco lavori] per controllare meglio quali informazioni sono visibili.\
Per impostazione predefinita, la [!UICONTROL Questa settimana] Il raggruppamento viene espanso e tutti gli altri raggruppamenti vengono compressi. Tutte le modifiche apportate verranno ricordate al successivo accesso all&#39;area Home.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. Fai clic sul pulsante **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** accanto a un raggruppamento da espandere o comprimere.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Oppure\
   Per espandere o comprimere tutti i raggruppamenti contemporaneamente, fai clic sul pulsante **[!UICONTROL Espandi]** o **[!UICONTROL Comprimi]** freccia accanto a qualsiasi raggruppamento tenendo premuto il tasto [!UICONTROL Maiusc] chiave.
