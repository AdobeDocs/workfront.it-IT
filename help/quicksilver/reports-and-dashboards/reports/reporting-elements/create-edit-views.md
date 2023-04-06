---
product-area: reporting
navigation-topic: reporting-elements
title: Creare o modificare visualizzazioni in Adobe Workfront
description: Puoi personalizzare il tipo di informazioni da visualizzare sullo schermo utilizzando le visualizzazioni. Puoi utilizzare diversi tipi di visualizzazioni in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Creare o modificare visualizzazioni in Adobe Workfront

Puoi personalizzare il tipo di informazioni da visualizzare sullo schermo utilizzando le visualizzazioni. Puoi utilizzare diversi tipi di visualizzazioni in Adobe Workfront.

Questo articolo descrive come creare e modificare visualizzazioni standard per elenchi e rapporti e come creare visualizzazioni Agile. Per ulteriori informazioni, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per creare una visualizzazione in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per creare o modificare una visualizzazione in un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare o personalizzare una visualizzazione

Il processo di creazione o personalizzazione di una visualizzazione varia a seconda che si stia creando o personalizzando una visualizzazione standard o una visualizzazione agile.

* [Creare o personalizzare una visualizzazione standard](#create-or-customize-a-standard-view)
* [Creare o personalizzare una visualizzazione Agile](#create-or-customize-an-agile-view)

### Creare o personalizzare una visualizzazione standard {#create-or-customize-a-standard-view}

È possibile creare una nuova visualizzazione standard oppure personalizzare una visualizzazione standard esistente creata in precedenza.

1. Fai clic sul pulsante **Visualizza** menu a discesa in qualsiasi elenco in cui si desidera creare o personalizzare una visualizzazione.
1. (Facoltativo) Per personalizzare una visualizzazione esistente, selezionare la visualizzazione standard da personalizzare.\
   Le visualizzazioni standard sono disponibili in qualsiasi tipo di elenco in Workfront, ad esempio un rapporto, un elenco di progetti o un elenco di attività.
1. Fai clic sul pulsante **Visualizza** menu a discesa, quindi fai clic su **Personalizza visualizzazione** o **Nuova vista**.\
   La **Personalizza visualizzazione** viene visualizzata la finestra di dialogo.

1. In **Anteprima a colonne** eseguire una delle operazioni seguenti:

   * Modificare il valore di una colonna facendo clic sul titolo della colonna e quindi selezionando un nuovo campo.
   * Aggiungi una colonna facendo clic su **Aggiungi colonna**, inizia a digitare il nome della colonna che desideri aggiungere, quindi fai clic su di essa quando viene visualizzata nell’elenco a discesa.
   * Per regolare l’ordine di visualizzazione delle colonne, trascinate il titolo della colonna in una nuova posizione.

      * (Facoltativo) In **Impostazioni colonna** fai clic sull’area **Riepiloga questa colonna per** dall’elenco a discesa, quindi seleziona una delle opzioni disponibili per il riepilogo delle informazioni. Quando scegli questa opzione, le informazioni nella colonna vengono aggregate nei raggruppamenti del rapporto.\
         Per i campi data, è possibile riepilogare i valori utilizzando le seguenti opzioni:

         * Massimo
         * Minimo

         Per i campi numero e valuta, è possibile riepilogare i valori utilizzando le opzioni seguenti:

         * Count
         * SOMMA

         * Media
         * Massimo
         * Minimo

         >[!NOTE]
         >
         >Le seguenti eccezioni si applicano agli oggetti principali (ad esempio, le attività principali) quando si aggregano valori per i seguenti campi nei raggruppamenti:
         >   
         >   * Tutti i campi relativi al numero e alla divisa, ad eccezione delle ore effettive (ad esempio, Costo manodopera pianificato/effettivo, Costo spesa pianificato/effettivo, Costo pianificato/effettivo, Ore pianificate) aggregano solo i valori relativi alle attività figlio e alle attività autonome. Non aggregano i valori per le attività principali o le attività principali dei genitori.
         >   * Le ore effettive aggregano i valori per le attività principali e le attività autonome; non aggregano i numeri relativi alle attività principali o alle attività figlio per le attività padre.
         >   * I campi dati personalizzati per i valori di numero e valuta aggregano tutte le attività: genitori, figli, genitori di genitori e compiti autonomi.


         Per ulteriori informazioni sull’utilizzo dei raggruppamenti in un rapporto, consulta l’articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facoltativo) Fai clic su **Opzioni avanzate** per specificare le seguenti informazioni per la colonna:

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etichetta colonna personalizzata</strong></td> 
           <td><p>Specifica un’etichetta personalizzata per la colonna. Questa etichetta sostituisce l’etichetta predefinita.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato campo</strong></td> 
           <td>Selezionare il formato in cui si desidera visualizzare i valori per i campi della colonna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
           <td><p>Seleziona questa opzione per visualizzare questa colonna su un dashboard, quando il rapporto viene visualizzato accanto a un altro rapporto. Se questa opzione non è selezionata, questa colonna non viene visualizzata quando il rapporto viene visualizzato in una dashboard in cui i rapporti vengono visualizzati affiancati.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Regole colonna</strong></td> 
           <td><p>Fai clic su <strong>Aggiungi una regola per questa colonna</strong> per definire una regola per la colonna. Dopo aver aggiunto una regola, puoi definire gli stili di campo e testo per la modalità di visualizzazione dei campi corrispondenti a tale regola. Fai clic su <strong>Aggiungi regola</strong> dopo aver definito la regola.</p></td> 
          </tr> 
         </tbody> 
        </table>

         Per ulteriori informazioni sulla formattazione condizionale delle viste nei rapporti, consulta l’articolo [Utilizzare la formattazione condizionale nella modalità Testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. (Condizionale) Se hai fatto clic su **Opzioni avanzate**, fai clic su **Fine**.

1. Fai clic su **Salva visualizzazione** per creare una nuova visualizzazione o sostituire la visualizzazione corrente con le modifiche apportate.\
   Oppure\
   Fai clic su **Salva come nuova vista** per salvare le modifiche come nuova visualizzazione.

   >[!TIP]
   >
   >La **Salva come nuova vista** è l’unica opzione disponibile per personalizzare una visualizzazione integrata di Workfront.

   L’accesso determina la modalità di salvataggio della visualizzazione. Se la visualizzazione è stata creata in origine, è possibile salvare le modifiche; in caso contrario, viene richiesto di salvare una versione. Le modifiche apportate alla visualizzazione hanno un impatto sugli utenti con i quali la visualizzazione è stata condivisa.

### Creare o personalizzare una visualizzazione Agile {#create-or-customize-an-agile-view}

È possibile creare una nuova visualizzazione Agile o personalizzare una visualizzazione Agile esistente creata in precedenza.

>[!IMPORTANT]
>
>Le visualizzazioni delle linee guida sono disponibili solo quando si visualizza un progetto.

Per ulteriori informazioni sulle visualizzazioni Agile, consulta l’articolo [Gestire un progetto nella vista Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

Per creare o personalizzare una visualizzazione Agile:

1. Passa all’elenco delle attività di un progetto.
1. Fai clic sul pulsante **Storyboard Agile** icona ![](assets/agile-storyboard-nwe.png).

1. (Condizionale) Per personalizzare una visualizzazione Agile esistente:

   1. Fai clic sul pulsante **Visualizza** dal menu a discesa, quindi selezionate la vista Agile da personalizzare.\
      Non è possibile personalizzare la visualizzazione Agile predefinita.

   1. Fai clic sul pulsante **Visualizza** menu a discesa, quindi fare clic **Personalizza visualizzazione**.\
      ![](assets/view-agile-customize.png)

1. (Condizionale) Per creare una nuova visualizzazione Agile, fai clic su **Nuova vista**.\
   La **Personalizzare la visualizzazione degli articoli** viene visualizzata la finestra di dialogo.

1. In **Personalizzare la visualizzazione degli articoli** specificare un nome per la visualizzazione Agile.\
   È consigliabile includere la parola &quot;Agile&quot; nel nome della visualizzazione, in modo che gli utenti sappiano che si tratta di una visualizzazione Agile.\
   Questo nome viene visualizzato nella **Visualizza** menu a discesa quando si seleziona una visualizzazione.

1. Definite le colonne di stato da visualizzare sulla bacheca del racconto nella vista agile. Si tratta degli stati delle attività definiti dall’amministratore Workfront, come descritto in [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Solo gli stati del sistema sono disponibili per l&#39;utilizzo sulla bacheca di Agile. Se uno stato è disponibile solo per un singolo gruppo di cui sei membro, lo stato non è disponibile sulla bacheca di storie agili. Inoltre, le attività che si trovano in uno stato disponibile solo per un gruppo personalizzato non sono visibili quando il progetto viene visualizzato in una visualizzazione Agile.

   Gli utenti possono spostare le storie tra queste colonne di stato sulla bacheca delle storie di Agile.\
   Quando definisci le colonne di stato, puoi effettuare le seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Consente di riordinare le colonne di stato:</strong> </td> 
      <td> Trascina una colonna di stato nell’ordine in cui desideri visualizzarla.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rimuovi colonne di stato:</strong> </td> 
      <td>Fai clic sull’icona (x) nella colonna da rimuovere.<br>Non è possibile rimuovere lo stato "Nuovo" a meno che non sia stato aggiunto uno stato personalizzato alla visualizzazione e che lo stato personalizzato corrisponda a "Nuovo".<br>Per informazioni sulla creazione di uno stato personalizzato, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aggiungi colonne di stato:</strong> </td> 
      <td> <p>Fai clic sul pulsante <strong>Plus</strong> , quindi seleziona lo stato da aggiungere.<br>Vengono visualizzati tutti gli stati di sistema predefiniti, nonché tutti gli stati personalizzati condivisi con l’utente.<br>Puoi configurare fino a 10 stati da visualizzare.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. In **Associa colore scheda a** seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Storia:</strong> </td> 
      <td>Tutte le sottoattività corrispondono al colore dell'attività padre, in modo che i colori di tutte le storie in una determinata corsia da bagno siano gli stessi.<br>I colori vengono assegnati in modo casuale alle attività quando vengono create se l’attività non dispone di attività secondarie o se non dispone di un’attività padre.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modulo libero:</strong> </td> 
      <td> Tutte le schede sono visualizzate in blu per impostazione predefinita finché un utente non modifica manualmente il colore, come descritto nell’articolo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorizzare le storie per colore sulla scheda Scrum</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorità:</strong> </td> 
      <td> <p> I colori sono associati alla priorità della storia, come segue:</p> 
       <ul> 
        <li>Alto = Rosso</li> 
        <li>Media = Giallo</li> 
        <li>Bassa = Verde<br>Se l’amministratore di Workfront ha configurato priorità personalizzate per il sistema Workfront, la priorità più alta è rossa, la seconda più alta è gialla e la restante è verde.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Proprietario attività:</strong> </td> 
      <td> Tutte le storie con lo stesso assegnatario primario sono dello stesso colore.<br>L’assegnatario principale è l’utente che è stato assegnato per la prima volta all’attività. </td> 
     </tr> 
    </tbody> 
   </table>

1. In **Agile** nella sezione **Campi aggiuntivi** area, fai clic su **Aggiungi campo**, quindi selezionate il campo da aggiungere alle schede delle storie. Si tratta degli stessi campi che è possibile aggiungere quando si crea una visualizzazione o si creano colonne per un rapporto.\
   Ripeti questo processo per aggiungere fino a tre campi aggiuntivi alle schede delle storie.\
   Quando si aggiungono campi alle schede dei brani, i campi sono di sola visualizzazione e vengono visualizzati solo quando il campo è compilato.

   Per impostazione predefinita, sulla scheda del brano vengono visualizzati i seguenti tipi di dati:

   * Nome della storia con un collegamento direttamente all’attività
   * Nome del progetto con un collegamento diretto al progetto\
      Questo collegamento viene visualizzato solo quando si utilizza la visualizzazione agile su un&#39;iterazione; non viene visualizzato quando si utilizza una visualizzazione Agile in un progetto.
   * Descrizione attività
   * Impegno attuale
   * Visualizza e modifica la percentuale di completamento regolando la percentuale di completamento oppure regolando il numero di punti o ore di completamento
   * Utenti assegnati

   È possibile visualizzare dati aggiuntivi (inclusi dati personalizzati) sulle schede delle storie. È possibile visualizzare campi aggiuntivi sulle schede delle storie per diversi motivi. Ad esempio, potrebbe essere utile visualizzare l&#39;ID cliente se si stanno lavorando a storie per più clienti all&#39;interno del progetto o se si desidera visualizzare la data di inizio attività.

1. Fai clic su **Salva**.\
   L’accesso determina la modalità di salvataggio della visualizzazione. Se la visualizzazione è stata creata in origine, è possibile salvare le modifiche; in caso contrario, viene richiesto di salvare una versione. Le modifiche apportate alla visualizzazione hanno un impatto sugli utenti con i quali la visualizzazione è stata condivisa.

1. (Facoltativo) Fai clic sul pulsante **Vista a elenco** icona ![](assets/list-view-in-agile-view-for-tasks.png) per tornare all&#39;elenco delle attività.
