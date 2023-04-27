---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Utilizzare schede collegate sulle bacheche
description: Potete aggiungere una scheda sulla bacheca connessa alle attività e ai problemi esistenti in Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: f6bee61bbfbac98595d737fa002bbe01c0c573dc
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Utilizzare schede collegate sulle bacheche

Potete aggiungere una scheda sulla bacheca connessa alle attività e ai problemi esistenti in [!DNL Workfront].

Quando uno dei seguenti dettagli viene aggiornato per la scheda in una posizione, viene aggiornato automaticamente nell&#39;altra posizione:

* [!UICONTROL Nome]
* [!UICONTROL Descrizione]
* [!UICONTROL Assegnatari]
* [!UICONTROL Stato]
* [!UICONTROL Data di completamento pianificata]
* [!UICONTROL Stima] / [!UICONTROL Punti della storia]

>[!NOTE]
>È possibile aggiungere un&#39;unica attività o un singolo problema collegato una sola volta per ogni bacheca. La stessa attività o problema può essere collegato a più bacheche.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td>
   <td><p>Visualizzazione o accesso a attività e problemi più esteso</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td>
   <td><p>Visualizzazione o autorizzazioni successive per l'attività o il problema Workfront</p></td>
  </tr>
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungi una scheda connessa

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Schede]**.
1. Accedete a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Aggiungi scheda] > [!UICONTROL Scheda collegata]**.
1. Scegliete un progetto, quindi scegliete un&#39;attività o un problema da aggiungere come scheda sulla bacheca.

   È possibile selezionare più oggetti che verranno aggiunti come schede separate.

   >[!NOTE]
   >
   >* Nei risultati della ricerca sono disponibili solo gli oggetti per i quali si dispone delle autorizzazioni. Se un elemento è oscurato, è già stato aggiunto alla bacheca.
   >* Quando si filtra per **[!UICONTROL Progetti di proprietà]** o **[!UICONTROL Progetti in corso]**, i progetti che equivalgono a uno stato Completo, Morto o Rifiutato non sono inclusi. È comunque possibile cercare tali progetti con la **[!UICONTROL Tutto]** filtro.


1. Fai clic su **[!UICONTROL Aggiungi]**.

   ![Cerca attività o problema per la connessione](assets/boards-tasksissues-350x94.png)

   La scheda viene aggiunta nella parte inferiore della colonna più a sinistra. Collegato [!DNL Workfront] sulla scheda vengono visualizzati l&#39;oggetto e i relativi assegnatari.

   >[!NOTE]
   >
   >Se un assegnatario [!DNL Workfront] l&#39;attività o il problema non sono membri della bacheca, non sono assegnati alla scheda.

   ![Scheda connessa](assets/boards-connected-card-first-added.png)

1. Fai clic su ![Apri attività o problema](assets/boards-launch-icon.png) per aprire [!DNL Workfront] attività o problema in una nuova scheda del browser.
1. Per modificare i dettagli della scheda, fate clic sulla scheda (non nel nome della scheda).

   Oppure

   Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Modifica]**.

1. In **[!UICONTROL Dettagli scheda]** aggiungi o aggiorna le seguenti informazioni:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>La modifica del nome comporta anche la modifica del nome sulla connessione [!DNL Workfront] oggetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td> 
      <td>La modifica della descrizione cambia anche la descrizione sulla connessione [!DNL Workfront] oggetto. Nella descrizione puoi aggiungere URL che diventeranno collegamenti cliccabili al momento del salvataggio della scheda.</td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignees]</strong></td>
      <td><p>Per assegnare più persone o un team alla scheda, inizia a digitare un nome nel campo di ricerca, quindi selezionalo quando viene visualizzato nell’elenco. Puoi aggiungere sia singoli che team. Su una scheda connessa è consentita una sola assegnazione di team.</p>
      <p>Gli assegnatari devono essere membri della bacheca o non verranno visualizzati nell'elenco di selezione. Quando un team è membro della bacheca, i singoli membri del team possono essere assegnati alla scheda.</p>
      <p>Gli eventuali assegnatari selezionati vengono inoltre assegnati all'attività o al problema in [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Seleziona la colonna della scheda.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Seleziona uno stato per la scheda. Le impostazioni predefinite sono [!UICONTROL Nuovo], [!UICONTROL In corso] e [!UICONTROL Complete], ma sono stati definiti stati personalizzati per l’elemento in [!DNL Workfront] sono anche disponibili.</p>
      <p>Se i criteri colonna sono abilitati per l’aggiornamento dei valori dei campi, quando si modifica lo stato sulla scheda la scheda viene spostata automaticamente nella colonna corrispondente. Per ulteriori informazioni, consulta "Definire le impostazioni e i criteri delle colonne" nell’articolo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gestire le colonne della bacheca</a>.</p>
      <p>Se fai clic su <strong>[!UICONTROL Mark Complete]</strong> nella parte superiore della scheda, lo stato diventa automaticamente Completa.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Completamento pianificato]</strong></td>
      <td>La modifica di questa data comporta anche la modifica della data di completamento pianificata nella [!DNL Workfront] oggetto.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Numero di ore per il completamento della scheda.</p><p>La modifica della stima cambia anche il valore dei punti della storia sulla connessione [!DNL Workfront] oggetto.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Cerca e seleziona i tag per la scheda.</p>
      <p>Per informazioni sulla creazione di nuovi tag, consulta <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Aggiungi tag</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Elementi della checklist]</strong> </td> 
      <td> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento di checklist]</strong>. Quindi, digitare il titolo dell'elemento e premere Invio. Viene aggiunto automaticamente un altro elemento. Continua a inserire titoli per aggiungere altri elementi.</p> <p>Il contatore nella parte superiore della lista di controllo mostra il numero di elementi completati e il numero totale di elementi.</p> <p>Per ulteriori informazioni sugli elementi della lista di controllo, consulta <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gestione degli elementi delle liste di controllo sulle schede</a>.</p></td>
     </tr>
    </tbody> 
   </table>

   Utilizza il pannello di navigazione a sinistra per spostarsi tra gruppi di campi nei dettagli della scheda.

   >[!NOTE]
   >
   >Il pannello di navigazione a sinistra e la possibilità di aggiungere collegamenti selezionabili nel campo Descrizione sono disponibili solo tramite la funzionalità opt-in iniziale per le schede Workfront.

1. Fai clic su **[!UICONTROL Chiudi]** per tornare al consiglio di amministrazione.
L&#39;oggetto connesso, gli assegnatari, i tag, la data di scadenza, il contatore delle checklist, le ore stimate e lo stato vengono visualizzati sulla scheda.

   ![Scheda aggiunta a bordo](assets/boards-connected-card-details-110922.png)

## Scollegare una scheda connessa

Potete disconnettere una scheda connessa dal suo oggetto Workfront e la scheda rimane sulla bacheca come una scheda ad hoc modificabile.

Per disconnettersi a livello di scheda:

1. Accedete alla bacheca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) sulla scheda connessa e selezionare **[!UICONTROL Disconnetti]**.
1. Fai clic su **[!UICONTROL Disconnetti]** nel messaggio di conferma.

Per disconnettersi a livello di scheda:

1. Accedete alla bacheca e aprite la scheda connessa.
1. Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nell&#39;area Connessione dei dettagli della scheda e selezionare **[!UICONTROL Disconnetti]**.
1. Fai clic su **[!UICONTROL Disconnetti]** nel messaggio di conferma.

## Convertire una scheda ad hoc in una scheda connessa

Dopo aver creato una scheda ad hoc, puoi convertirla in una scheda connessa. Per informazioni dettagliate sulle schede ad hoc, vedi [Aggiunta di una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Accedete alla bacheca e aprite la scheda ad hoc.
1. Verifica il nome e la descrizione sulla scheda. Saranno aggiunti all’attività o al problema creato in [!DNL Workfront].
1. In [!UICONTROL Connessione] area dei dettagli della scheda, fai clic su **[!UICONTROL Connessione con Workfront]**.
1. Sulla [!UICONTROL Scheda di connessione] finestra, seleziona se stai creando un&#39;attività o un problema.
1. Cerca e seleziona un progetto a cui aggiungere l’attività o il problema.

   >[!NOTE]
   >
   >* Nei risultati della ricerca sono disponibili solo gli oggetti per i quali si dispone delle autorizzazioni.
   >* Quando si filtra per **[!UICONTROL Progetti di proprietà]** o **[!UICONTROL Progetti in corso]**, progetti che equivalgono a un [!UICONTROL Completa], [!UICONTROL Morto]oppure [!UICONTROL Rifiutato] lo stato non è incluso. È comunque possibile cercare tali progetti con la **[!UICONTROL Tutto]** filtro.


1. Fai clic su **[!UICONTROL Connetti]**.

   ![Collegare una scheda ad hoc a Workfront](assets/boards-connect-ad-hoc-card.png)

   Il nome del progetto viene visualizzato nell&#39;area Connessione sui dettagli della scheda.

1. Fai clic su **[!UICONTROL Chiudi]** per tornare al consiglio di amministrazione.

## Orari di registrazione su una scheda connessa

È necessario disporre delle autorizzazioni corrette per l&#39;accesso alle ore relative all&#39;attività o al problema connessi.

Per impostazione predefinita, i campi di registrazione dell&#39;ora non vengono visualizzati sulle schede collegate. È necessario attivare [!UICONTROL **Ore**] in [!UICONTROL Configura] zona sotto [!UICONTROL Schede]. Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati su una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Immettere il numero di ore per l&#39;attività o il problema.
1. Seleziona un [!UICONTROL Tipo ora] dal menu a discesa, se è diverso da quello predefinito.
1. Fai clic su [!UICONTROL **Tempo di log**].

   ![Orari di accesso sulla scheda](assets/log-hours-on-card.png)

   Il tempo di accesso alla scheda viene salvato anche sull&#39;attività o sul problema connessi.

Il tempo di registrazione sulla scheda è lo stesso del tempo di registrazione su un&#39;attività o su un problema. Per ulteriori informazioni, consulta &quot;Tempo di log su un progetto, un’attività o un problema&quot; nell’articolo [Tempo di log](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

