---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiare e spostare le attività modello
description: È possibile copiare o spostare un'attività modello nello stesso modello o in un altro modello.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '2127'
ht-degree: 3%

---

# Copiare e spostare le attività modello

È possibile copiare un&#39;attività modello da un modello a un altro modello oppure spostarla in un altro modello o in un&#39;altra posizione nello stesso modello.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un modello e per l’attività modello </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni per la copia o lo spostamento di attività modello

Quando copi le attività modello, tieni presente quanto segue:

* Le seguenti informazioni non vengono trasferite all&#39;attività copiata:

   * Le Milestone

* È possibile selezionare di copiare alcuni elementi associati all&#39;attività modello nell&#39;attività copiata durante il processo di copia. Tuttavia, per impostazione predefinita, i seguenti oggetti non vengono trasferiti all&#39;attività copiata:

   * Commenti utente

* I moduli personalizzati vengono copiati con l&#39;attività modello quando si copia un&#39;attività modello. Le informazioni contenute nei campi personalizzati vengono trasferite alla nuova attività modello solo quando si seleziona di copiare i dati personalizzati.

* Per impostazione predefinita, i seguenti elementi vengono trasferiti all&#39;attività modello copiata:

   * Sottoattività

Quando si spostano le attività modello, considera quanto segue:

* Per impostazione predefinita, le informazioni seguenti vengono trasferite all&#39;attività spostata:

   * Moduli personalizzati e informazioni sui campi personalizzati
   * Sottoattività
   * Commenti utente

* Le seguenti informazioni non vengono trasferite all&#39;attività spostata:

   * Le Milestone.

## Copia attività modello

È possibile copiare una singola attività modello oppure più attività modello in blocco.

1. Passare al modello contenente l&#39;attività modello o le attività modello che si desidera copiare.
1. Clic **Attività modello** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:
   * Fare clic sul nome di un&#39;attività modello per aprirla.
   * Selezionare una o più attività modello nell&#39;elenco.
1. (Condizionale) Fai clic su **Altro** menu ![](assets/more-icon.png) nella parte superiore dell&#39;elenco delle attività modello o a destra del nome dell&#39;attività modello, se l&#39;attività è stata aperta, fare clic su **Copia in** o **Copia**, a seconda di dove si accede all’opzione Copia da.
Viene visualizzata la casella Copia attività modello (Copy Template Task).
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Facoltativo) Rinomina l’attività modello in **Nome Attività Modello** campo.

   >[!TIP]
   >
   >Questo campo è inattivo e non è modificabile quando si seleziona per copiare più attività modello in un elenco. Puoi passare il cursore del mouse sul campo Nome attività modello per visualizzare un elenco di tutte le attività modello selezionate.

1. Inizia a digitare il nome del **Modello di destinazione** dove si desidera copiare l&#39;attività modello in **Seleziona modello di destinazione** , quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   Il nome del modello corrente viene visualizzato per impostazione predefinita. Se si desidera copiare l&#39;attività modello all&#39;interno dello stesso modello, lasciare questo campo invariato.

   >[!TIP]
   >
   >Puoi anche iniziare a digitare il Numero di riferimento o immettere l’ID del modello. Questo potrebbe aiutarti a distinguere tra modelli con nomi identici.

1. (Condizionale) Fai clic su **richiedi accesso** per richiedere l’accesso al modello di destinazione, se non hai accesso al modello selezionato.
1. (Facoltativo) Continua a copiare l’attività modello nel modello di destinazione selezionato senza richiedere l’accesso se disponi dell’accesso per aggiungere attività modello a una delle attività modello nel modello di destinazione.

1. Clic **Opzioni** nel pannello a sinistra, deseleziona gli attributi dell’attività modello che non desideri copiare con l’attività modello. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!TIP]
   >
   >Deselezionare **Seleziona tutto** deseleziona tutte le opzioni.

   Deseleziona tra le seguenti opzioni per non trasferirle all’attività modello copiata. La tabella seguente descrive cosa accade quando le opzioni vengono deselezionate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionare questa opzione per rimuovere tutte le informazioni dall'attività modello quando la si copia nella nuova posizione. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>In base all'impostazione della modalità di pianificazione del modello, il vincolo attività modello viene impostato su Il più presto possibile o Il più tardi possibile.</p> <p> Se questa opzione è selezionata, il vincolo corrente dell'attività modello viene trasferito all'attività modello copiata. </p> 
      <p><b>NOTA</b>

   Quando si copia un&#39;attività modello con vincoli specifici della data in un altro modello e le date dei vincoli dell&#39;attività modello non rientrano nelle date del nuovo modello, l&#39;opzione Vincolo dell&#39;attività modello viene impostata su Il più presto possibile o Il più tardi possibile oppure le date di Inizio pianificato o Completamento pianificato dei modelli vengono modificate.

   Di seguito sono riportati alcuni esempi di vincoli specifici per data:
   <ul>
      <li> Deve ininziare al</li>
      <li> Deve Finire al</li>
      <li> Iniziare non Prima di</li>
      <li> Iniziare non Dopo di</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td> <p>Tutte le assegnazioni vengono rimosse dall'attività modello. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td>Tutti i processi di approvazione vengono rimossi dall'attività modello.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Ciò significa che le dipendenze non verranno riportate nelle attività modello copiate. </p> <p>Se questa opzione è selezionata, i predecessori all'interno del gruppo di attività modello copiate vengono mantenuti, mentre gli altri vengono eliminati.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>I valori dei campi personalizzati vengono cancellati e i moduli personalizzati vengono trasferiti all’attività modello copiata. </p> <p>Se questa opzione è selezionata, sia i moduli che i valori dei campi personalizzati vengono trasferiti all'attività modello copiata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazioni finanziarie</td> 
      <td>Le informazioni finanziarie dell'attività modello copiata vengono rimosse e Workfront aggiorna il tipo di costo dell'attività modello su Nessun costo e il tipo di ricavi dell'attività modello su Non fatturabile.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività modello non vengono trasferiti all'attività modello copiata. Sono inclusi versioni, bozze e documenti collegati.</p> <p><b>NOTA</b></p>

   <p>Non sono incluse le approvazioni di documenti. Le approvazioni dei documenti non possono mai essere copiate quando un'attività modello viene copiata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria delle attività modello non vengono trasferiti all'attività modello copiata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate nell'attività modello non vengono trasferite all'attività modello copiata. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facoltativo) Fai clic su **Seleziona elemento padre** nel pannello a sinistra, seleziona l’attività modello nel modello di destinazione che desideri diventi l’attività padre dell’attività modello copiata.

   >[!TIP]
   >
   >Quando si seleziona di copiare più attività modello in un elenco, tutte le attività modello selezionate diventano gli elementi figlio dell&#39;attività padre selezionata e vengono aggiunte dopo le attività figlio esistenti.

   Selezionare un elemento padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività modello selezionare uno dei padri nel piano modello.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività modello padre per nome.

   L&#39;attività modello dovrebbe essere visualizzata nell&#39;elenco.

1. Dopo averlo trovato, seleziona il pulsante di opzione relativo al genitore.

   Se non si seleziona un&#39;attività modello padre, le attività modello vengono copiate come attività modello principale anziché come attività secondarie e si trovano alla fine dell&#39;elenco delle attività modello nel modello di destinazione.

1. Clic **Copia attività modello**.

   Le attività modello copiate si trovano ora nel modello specificato e sono sottoattività dell&#39;attività modello padre selezionata o delle ultime attività modello nel modello.


## Sposta le attività modello

È possibile spostare un&#39;attività modello in un&#39;altra attività modello nello stesso modello o in un altro modello. È possibile spostare una o più attività modello in blocco.

1. Passare al modello contenente l&#39;attività modello o le attività modello che si desidera spostare.
1. Clic **Attività modello** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:
   * Fare clic sul nome di un&#39;attività modello per aprirla.
   * Selezionare una o più attività modello nell&#39;elenco.
1. (Condizionale) Fai clic su **Altro** menu ![](assets/more-icon.png) nella parte superiore dell&#39;elenco delle attività modello o a destra del nome dell&#39;attività modello, se l&#39;attività è stata aperta, fare clic su **Sposta in** o **Sposta**, a seconda del punto da cui si accede all’opzione Sposta.
Viene visualizzata la casella Sposta attività modello (Move Template Task).
   ![](assets/move-template-task-box-unshimmed.png)

1. (Facoltativo) Rinomina l’attività modello in **Nome Attività Modello** campo.

   >[!TIP]
   >
   >Questo campo è inattivo e non è modificabile quando si seleziona per spostare più attività modello in un elenco. Passa il puntatore del mouse sul campo Nome attività modello per visualizzare un elenco di tutte le attività modello selezionate.

1. Inizia a digitare il nome del **Modello di destinazione** dove si desidera spostare l&#39;attività modello in **Seleziona modello di destinazione** , quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   >[!TIP]
   >
   >Puoi anche iniziare a digitare il Numero di riferimento o immettere l’ID del modello. Questo potrebbe aiutarti a distinguere tra modelli con nomi identici.

1. (Condizionale) Fai clic su **richiedi accesso** per richiedere l’accesso al modello, se non hai accesso al modello di destinazione.
1. (Facoltativo) Continua a spostare l’attività modello nel modello di destinazione selezionato senza richiedere l’accesso, se disponi dell’accesso per aggiungere attività modello a una delle attività modello nel modello di destinazione.

1. Clic **Opzioni** nel pannello a sinistra, deseleziona gli attributi dell’attività modello che non desideri copiare con l’attività modello. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!TIP]
   >
   >* La sezione Opzioni è disponibile solo dopo aver selezionato un modello di destinazione.
   >* Deselezionare **Seleziona tutto** deseleziona tutte le opzioni.

   Deseleziona tra le seguenti opzioni per non trasferire le informazioni all’attività modello spostata. La tabella seguente descrive cosa accade quando le opzioni vengono deselezionate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionate questa opzione per rimuovere tutte le informazioni dall'attività modello quando la spostate nella nuova posizione. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>In base all'impostazione della modalità di pianificazione del modello, il vincolo attività modello viene impostato su Il più presto possibile o Il più tardi possibile.</p> <p> Se questa opzione è selezionata, il vincolo corrente dell'attività modello viene trasferito all'attività modello spostata. </p>

   <p><b>NOTA</b>

   Quando si sposta un&#39;attività modello con vincoli specifici della data in un altro modello e le date dei vincoli dell&#39;attività modello non rientrano nelle date del nuovo modello, l&#39;attività modello Vincolo viene modificata in Il più presto possibile o Il più tardi possibile oppure vengono modificate le date di Inizio pianificato o Completamento pianificato dei modelli.

   Di seguito sono riportati alcuni esempi di vincoli specifici per data:
   <ul>
      <li> Inizia il</li>
      <li> Deve Finire al</li>
      <li> Iniziare non Prima di</li>
      <li> Iniziare non Dopo di</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td> <p>Tutte le assegnazioni vengono rimosse dall'attività modello. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td>Tutti i processi di approvazione vengono rimossi dall'attività modello.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Ciò significa che le dipendenze non verranno riportate con le attività modello spostate. </p> <p>Se questa opzione è selezionata, i predecessori all'interno del gruppo di attività modello spostate vengono mantenuti, mentre gli altri vengono eliminati.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>I valori dei campi personalizzati vengono cancellati e i moduli personalizzati vengono trasferiti con l’attività modello spostata. </p> <p>Se questa opzione è selezionata, i moduli e i valori per i campi personalizzati vengono trasferiti con l'attività modello spostata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazioni finanziarie</td> 
      <td>Le informazioni finanziarie dell'attività modello spostata vengono rimosse e Workfront aggiorna il tipo di costo dell'attività modello su Nessun costo e il tipo di ricavi dell'attività modello su Non fatturabile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività modello non vengono trasferiti con l'attività modello spostata. Sono inclusi versioni, bozze e documenti collegati.</p>

   <p><b>NOTA</b></p>

   <ul><li>
      <p>Non sono incluse le approvazioni di documenti. Le approvazioni dei documenti non possono mai essere spostate quando si sposta un'attività modello.</p> </li>
      <li>Se si sceglie di non spostare i documenti con l'attività modello, i documenti vengono eliminati e posizionati nel Cestino per 30 giorni. Un amministratore può ripristinarli e verranno ripristinati durante l’attività modello spostata.

   Se l&#39;attività modello viene eliminata dopo essere stata spostata, i documenti ripristinati verranno posizionati nell&#39;area Documenti della pagina utente dell&#39;amministratore che li ripristina. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria delle attività modello non vengono trasferiti all'attività modello spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate nell'attività modello non vengono trasferite con l'attività modello spostata. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facoltativo) Fai clic su **Seleziona elemento padre** nel pannello a sinistra, seleziona l’attività modello nel modello di destinazione che desideri diventi l’attività padre dell’attività modello spostata.

   >[!TIP]
   >
   >Quando si seleziona per spostare più attività modello in un elenco, tutte le attività modello selezionate diventano gli elementi figlio dell&#39;attività padre selezionata e vengono aggiunte dopo le attività figlio esistenti.

   Selezionare un elemento padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività modello selezionare uno dei padri nel piano modello.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività modello padre per nome.

   L&#39;attività modello dovrebbe essere visualizzata nell&#39;elenco.

1. Dopo averlo trovato, seleziona il pulsante di opzione relativo al genitore.

   Se non si seleziona un&#39;attività modello padre, le attività modello vengono spostate come attività modello principale anziché come attività secondarie e si trovano alla fine dell&#39;elenco delle attività modello nel modello di destinazione.

1. Clic **Sposta attività modello**.

   Le attività modello spostate si trovano ora nel modello specificato e sono sottoattività dell&#39;attività modello padre selezionata o delle ultime attività modello nel modello.
