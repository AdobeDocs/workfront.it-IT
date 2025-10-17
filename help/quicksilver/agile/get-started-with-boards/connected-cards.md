---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Usa schede collegate sulle bacheche
description: È possibile aggiungere alla bacheca una scheda connessa alle attività e ai problemi esistenti in Workfront.
author: Jenny
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 1%

---

# Utilizzare le schede collegate sulle bacheche

<!-- Audited: 2/2024 -->

È possibile aggiungere alla bacheca una scheda connessa ad attività e problemi esistenti in [!DNL Workfront].

Quando uno qualsiasi dei seguenti dettagli viene aggiornato per la scheda in una posizione, viene automaticamente aggiornato nell’altra posizione:

* [!UICONTROL Nome]
* [!UICONTROL Descrizione]
* [!UICONTROL Assegnatari]
* [!UICONTROL Stato]
* [!UICONTROL Data di completamento pianificata]
* [!UICONTROL Stima] / [!UICONTROL Punti Storia]
* [!UICONTROL Attività secondarie]
* [!UICONTROL Documenti]

Per sincronizzare le schede collegate con Workfront, fai clic sul menu **[!UICONTROL Altro]** ![[!UICONTROL Altro menu]](assets/more-icon-spectrum.png) accanto al nome della bacheca e seleziona **[!UICONTROL Sincronizza elementi connessi]**. Le schede archiviate non vengono sincronizzate con attività e problemi di Workfront. Se una scheda viene ripristinata, questa verrà nuovamente sincronizzata.

>[!NOTE]
>
>È possibile aggiungere una sola attività o un singolo problema collegato una sola volta per bacheca. La stessa attività o lo stesso problema può essere collegato a più bacheche.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader">Configurazioni del livello di accesso</td>
   <td><p>Visualizzare o accedere più facilmente ad attività e problemi</p></td>
  </tr>
  <tr>
   <td role="rowheader">Autorizzazioni oggetto</td>
   <td><p>Visualizza o autorizzazioni superiori per l’attività o il problema di Workfront</p>
</td>
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere una scheda collegata

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Aggiungi scheda] > [!UICONTROL Scheda connessa]**.
1. Scegli un progetto, quindi scegli un’attività o un problema da aggiungere come scheda sulla bacheca.

   È possibile selezionare più oggetti che verranno aggiunti come schede separate.

   >[!NOTE]
   >
   >* Nei risultati della ricerca sono disponibili solo gli oggetti per i quali si dispone di autorizzazioni. Se un elemento viene oscurato, è già stato aggiunto alla bacheca.
   >* Quando si filtra in base a **[!UICONTROL Progetti di mia proprietà]** o **[!UICONTROL Progetti in corso]**, i progetti con stato Completato, Inattivo o Rifiutato non vengono inclusi. Puoi comunque cercare questi progetti con il filtro **[!UICONTROL All]**.

1. Fai clic su **[!UICONTROL Aggiungi]**.

   ![Cerca l&#39;attività o il problema da connettere](assets/boards-tasksissues-350x94.png)

   La scheda viene aggiunta nella parte inferiore della colonna più a sinistra. L&#39;oggetto [!DNL Workfront] connesso e i relativi assegnatari vengono visualizzati sulla scheda.

   ![Scheda connessa](assets/boards-connected-card-first-added.png)

1. Fai clic su ![Apri attività o problema](assets/boards-launch-icon.png) per aprire l&#39;attività o il problema [!DNL Workfront] in una nuova scheda del browser.
1. Per modificare i dettagli della scheda, fai clic sulla scheda (non nel nome della scheda).

   Oppure

   Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Modifica]**.

1. Nella casella **[!UICONTROL Dettagli scheda]**, aggiungi o aggiorna le seguenti informazioni:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>La modifica del nome comporta anche la modifica del nome nell'oggetto [!DNL Workfront] connesso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td> 
      <td>La modifica della descrizione comporta anche la modifica della descrizione dell'oggetto [!DNL Workfront] connesso. Puoi aggiungere gli URL nella descrizione, che diventeranno collegamenti cliccabili al salvataggio della scheda.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Colonna]</strong></td>
      <td>Seleziona la colonna per la scheda.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Stato]</strong></td>
      <td><p>Selezionare uno stato per la scheda. Le impostazioni predefinite sono [!UICONTROL New], [!UICONTROL In corso] e [!UICONTROL Complete], ma sono disponibili anche eventuali stati personalizzati definiti per l'elemento in [!DNL Workfront].</p>
      <p>Se sono stati abilitati i criteri di colonna per l’aggiornamento dei valori dei campi, la modifica dello stato sulla scheda sposta automaticamente la scheda nella colonna corrispondente. Per ulteriori informazioni, vedere "Definire le impostazioni e i criteri delle colonne" nell'articolo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gestione colonne bacheca</a>.</p>
      <p>Se fai clic su <strong>[!UICONTROL Mark Complete]</strong> nella parte superiore della scheda, lo stato cambia automaticamente in Complete.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL completamento pianificato]</strong></td>
      <td>La modifica di questa data determina anche la modifica della data di completamento pianificata per l'oggetto [!DNL Workfront] connesso.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Stima </strong></td>
      <td><p>Il numero di ore per il completamento della scheda.</p><p>La modifica della stima cambia anche il valore dei punti della storia sull'oggetto [!DNL Workfront] connesso.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assegnazioni]</strong></td>
      <td><p>Per assegnare più persone o un team alla scheda, fare clic su <strong>[!UICONTROL Aggiungi assegnazione]</strong> e iniziare a digitare un nome nel campo di ricerca. Quindi, selezionalo quando viene visualizzato nell’elenco dei risultati. Puoi aggiungere sia singoli utenti che team. Su una scheda connessa è consentita una sola assegnazione team.</p>
      <p>Tutti gli assegnatari selezionati vengono assegnati anche all'attività o al problema in [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Cerca e seleziona i tag per la scheda.</p>
      <p>Per informazioni sulla creazione di nuovi tag, vedere <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Aggiungi tag</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campi personalizzati]</strong></td>
      <td><p>Tutti i campi personalizzati aggiunti verranno visualizzati in quest'area.</p>
      <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizzare i campi visualizzati in una scheda</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Sottoattività]</strong></td>
      <td><p>Tutte le sottoattività esistenti per l'attività vengono visualizzate in questa sezione. Fare clic su <strong>[!UICONTROL Aggiungi sottoattività]</strong> per aggiungere una nuova sottoattività.</p>
      <p>Il contatore nella parte superiore della sezione mostra il numero di sottoattività completate e il numero totale di sottoattività.</p>
      <p>Per ulteriori informazioni sulle sottoattività, vedere <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Gestione delle sottoattività nelle bacheche</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>Elenco di controllo di </strong></td>
      <td><p>Fare clic su <strong>[!UICONTROL Add checklist item]</strong>. Digitare quindi il titolo dell'elemento e premere Invio. Un altro elemento viene aggiunto automaticamente. Continua a inserire i titoli per aggiungere altri elementi.</p>
      <p>Il contatore nella parte superiore dell’elenco di controllo mostra il numero di elementi completati e il numero totale di elementi.</p> <p>Per ulteriori informazioni sugli elementi dell'elenco di controllo, vedere <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gestire gli elementi dell'elenco di controllo sulle schede</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documenti]</strong></td>
      <td>Per un documento esistente, passa il cursore sulla miniatura del documento e fai clic su <strong>Anteprima</strong> per visualizzare il file nel browser o su <strong>Scarica</strong> per scaricarlo nel computer. Per un nuovo documento, vedi <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Aggiungi documenti su schede</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Consulta "Registrare le ore su una scheda collegata", di seguito.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Commenti]</strong></td>
      <td><p>Fare clic nel campo <strong>[!UICONTROL Nuovo commento]</strong> e digitare il commento. Utilizza gli strumenti di formattazione per formattare il testo. Per assegnare un tag a una persona o a un team, utilizza la casella di ricerca nella parte inferiore dell’area dei commenti. L’utente non deve essere un membro della bacheca. Gli utenti taggati sulle schede collegate riceveranno notifiche e-mail.</p><p>Fare clic su <strong>[!UICONTROL Submit]</strong> per aggiungere il commento alla scheda.</p>
      <p>Per ulteriori informazioni sui commenti, vedere <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Aggiorna lavoro</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Attività di sistema]</strong></td> 
      <td><p>Se <strong>Attività di sistema</strong> è abilitata come sezione scheda, l'attività viene visualizzata in quest'area.</p> <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizzare i campi visualizzati in una scheda</a> e <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Aggiornamenti rilevati dal sistema</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Utilizza il pannello di navigazione a sinistra per spostarti tra le sezioni dei campi nei dettagli della scheda.

1. Fai clic su **[!UICONTROL Chiudi]** per tornare alla bacheca.
L’oggetto connesso, gli assegnatari, i tag, la data di scadenza, il contatore della lista di controllo, le ore stimate e lo stato vengono visualizzati sulla scheda.

   ![Scheda aggiunta alla bacheca](assets/boards-connected-card-details-110922.png)

## Scollegare una scheda collegata

È possibile scollegare una scheda collegata dal relativo oggetto Workfront e la scheda rimane sulla scheda come scheda ad hoc modificabile.

Per disconnettersi a livello di scheda:

1. Accedi alla bacheca.
1. Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) sulla scheda connessa e seleziona **[!UICONTROL Disconnetti]**.
1. Fai clic su **[!UICONTROL Disconnetti]** nel messaggio di conferma.

Per disconnettersi a livello di scheda:

1. Accedere alla scheda e aprire la scheda collegata.
1. Fare clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) nell&#39;area Connessione dei dettagli della scheda e selezionare **[!UICONTROL Disconnetti]**.
1. Fai clic su **[!UICONTROL Disconnetti]** nel messaggio di conferma.

## Convertire una scheda ad hoc in una scheda collegata

Dopo aver creato una scheda ad hoc, è possibile convertirla in una scheda collegata. Per informazioni dettagliate sulle schede ad hoc, vedere [Aggiungere una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Accedi alla bacheca e apri la scheda ad hoc.
1. Verifica il nome e la descrizione sulla scheda. Verranno aggiunti all&#39;attività o al problema creato in [!DNL Workfront].
1. Nell&#39;area [!UICONTROL Connessione] dei dettagli della scheda, fare clic su **[!UICONTROL Connetti a Workfront]**.
1. Nella finestra [!UICONTROL Scheda di connessione], seleziona se stai creando un&#39;attività o un problema.
1. Cerca e seleziona un progetto a cui aggiungere l’attività o il problema.

   >[!NOTE]
   >
   >* Nei risultati della ricerca sono disponibili solo gli oggetti per i quali si dispone di autorizzazioni.
   >* Quando si filtra in base a **[!UICONTROL Progetti di mia proprietà]** o **[!UICONTROL Progetti che mi interessano]**, i progetti con stato [!UICONTROL Completo], [!UICONTROL Inattivo] o [!UICONTROL Rifiutato] non sono inclusi. Puoi comunque cercare questi progetti con il filtro **[!UICONTROL All]**.

1. Fai clic su **[!UICONTROL Connetti]**.

   ![Connetti scheda ad hoc a Workfront](assets/boards-connect-ad-hoc-card.png)

   Il nome del progetto viene visualizzato nell’area Connessione sui dettagli della scheda.

1. Fai clic su **[!UICONTROL Chiudi]** per tornare alla bacheca.

## Registra ore su una scheda collegata

È necessario disporre delle autorizzazioni corrette per registrare le ore per l’attività o il problema connesso.

Per impostazione predefinita, i campi di registrazione ora non vengono visualizzati sulle schede collegate. Devi abilitare [!UICONTROL **Ore**] nell&#39;area [!UICONTROL Configura] in [!UICONTROL Schede]. Per ulteriori informazioni, vedere [Personalizzare i campi visualizzati in una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Immetti il numero di ore per l’attività o il problema.
1. Selezionare un Tipo di [!UICONTROL Ora] dal menu a discesa, se diverso dal valore predefinito.
1. Fare clic su [!UICONTROL **Tempo di registrazione**].

   ![Registra ore sulla scheda](assets/log-hours-on-card.png)

   L’ora registrata sulla scheda viene salvata anche sull’attività o sul problema connesso.

Il tempo di registrazione sulla scheda è lo stesso di quello su un’attività o un problema. Per ulteriori informazioni, vedere &quot;Log time on a project, task, or issue&quot; nell&#39;articolo [Log time](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

