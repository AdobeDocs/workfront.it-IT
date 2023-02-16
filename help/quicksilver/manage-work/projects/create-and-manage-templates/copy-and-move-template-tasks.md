---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copia e sposta le attività del modello
description: È possibile copiare o spostare un'attività modello nello stesso modello o in un altro modello.
author: Alina
feature: Work Management
source-git-commit: 4a33d72e234ff812a72d7d7a382226697f858df6
workflow-type: tm+mt
source-wordcount: '2101'
ht-degree: 3%

---


# Copia e sposta le attività del modello

<span class="preview">L’operazione Copia e spostamento di un’attività modello è disponibile nell’ambiente di produzione. Tuttavia, i passaggi descritti in questa pagina fanno riferimento alla funzionalità solo nell’ambiente di anteprima. Questa funzionalità sarà disponibile in Produzione il 2 marzo 2023.</span>

È possibile copiare un&#39;attività modello da un modello a un altro modello oppure spostarla in un altro modello o in un&#39;altra posizione nello stesso modello.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per un modello e per l'attività modello </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sulla copia o lo spostamento delle attività dei modelli

Quando si copia un&#39;attività modello, tenere presente quanto segue:

* Le attività cardine non vengono trasferite all&#39;attività del modello copiata o spostata.

* Puoi copiare un’attività modello nelle seguenti aree dell’applicazione Web Adobe Workfront:

   * A livello di task del modello, dal **Icona Altro** ![](assets/more-icon.png) a destra del nome dell&#39;attività del modello.

   * In un elenco di attività del modello.
* È possibile copiare o spostare le attività del modello una alla volta oppure selezionando più attività del modello.

## Copia attività modello

1. Passare al modello che contiene l&#39;attività modello o le attività modello che si desidera copiare.
1. Fai clic su **Attività dei modelli** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:
   * Fare clic sul nome di un&#39;attività modello per aprirla.
   * Selezionare una o più attività del modello nell&#39;elenco.
1. (Condizionale) Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) nella parte superiore dell&#39;elenco delle attività del modello o a destra del nome dell&#39;attività del modello se l&#39;attività è stata aperta, quindi fare clic su **Copia in** o **Copia**, a seconda della posizione di accesso all’opzione Copia da.
Viene visualizzata la casella Copia attività modello.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Facoltativo) Rinomina l’attività del modello nel **Nome attività modello** campo .

   >[!TIP]
   >
   >Questo campo è oscurato e non modificabile quando si seleziona per copiare più attività di modello in un elenco. Passa il puntatore del mouse sul campo Nome attività modello per visualizzare un elenco di tutte le attività del modello selezionate.

1. Inizia a digitare il nome della **Modello di destinazione** in cui si desidera copiare l&#39;attività del modello nel **Seleziona modello di destinazione** , quindi selezionalo quando viene visualizzato nell’elenco.

   Per impostazione predefinita viene visualizzato il nome del modello corrente. Se si desidera copiare l&#39;attività del modello all&#39;interno dello stesso modello, lasciare invariato questo campo.

   >[!TIP]
   >
   >Puoi anche iniziare a digitare il numero di riferimento o l’ID del modello. Questo potrebbe essere utile per distinguere tra modelli con nomi identici.

1. (Condizionale) Fai clic su **richiesta di accesso** per richiedere l’accesso al modello di destinazione, se non si dispone dell’accesso al modello selezionato.
1. (Condizionale) Continua a copiare l&#39;attività del modello nel modello di destinazione selezionato senza richiedere l&#39;accesso se hai accesso per aggiungere attività del modello a uno dei task del modello nel modello di destinazione.

1. Fai clic su **Opzioni** nel pannello a sinistra, deselezionare gli attributi dell&#39;attività del modello che non si desidera copiare con l&#39;attività del modello. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!TIP]
   >
   >Deselezionare **Seleziona tutto** deseleziona tutte le opzioni.

   Deselezionare le opzioni seguenti per non trasferirle nell&#39;attività modello copiata. La tabella seguente descrive cosa accade quando le opzioni sono deselezionate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionare questa opzione per rimuovere tutte le informazioni dall'attività del modello durante la copia nella nuova posizione. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>Il vincolo dell'attività del modello viene impostato su Il più presto possibile o Il più tardi possibile in base all'impostazione Modalità pianificazione modello.</p> <p> Se selezionata, il vincolo corrente dell'attività modello viene trasferito all'attività modello copiata. </p> 
      <p><b>NOTA</b>

   Quando si copia un&#39;attività modello con vincoli specifici per la data in un altro modello e le date dei vincoli dell&#39;attività modello sono al di fuori delle date del nuovo modello, il vincolo dell&#39;attività modello viene modificato in Non appena possibile o Più tardi possibile oppure le date di inizio pianificato o di completamento pianificato dei modelli vengono modificate.

   Di seguito sono riportati alcuni esempi di vincoli specifici per la data:
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
      <td>Tutti i processi di approvazione vengono rimossi dall'attività del modello.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Ciò significa che le dipendenze non verranno riportate alle attività del modello copiate. </p> <p>Se selezionata, i predecessori all'interno del gruppo di attività modello copiate vengono mantenuti, altri vengono eliminati.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>I valori per i campi personalizzati vengono cancellati e i moduli personalizzati vengono trasferiti all’attività modello copiata. </p> <p>Se questa opzione è selezionata, sia i moduli che i valori dei campi personalizzati vengono trasferiti all’attività modello copiata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazione Finanziaria</td> 
      <td>Le informazioni finanziarie dell'attività modello copiata vengono rimosse e Workfront aggiorna il tipo di costo dell'attività modello su No Cost e il tipo di ricavi dell'attività modello su Non fatturabile.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività modello non vengono trasferiti all'attività modello copiata. Ciò include versioni, bozze e documenti collegati.</p> <p><b>NOTA</b></p>

   <p>Non sono incluse le approvazioni dei documenti. Le approvazioni dei documenti non possono mai essere copiate quando un'attività modello viene copiata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria delle attività del modello non vengono trasferiti all'attività del modello copiata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate nell'attività modello non vengono trasferite all'attività modello copiata. </td> 
     </tr>  
    </tbody> 
   </table>

(RICHIEDENDO L’ULTIMA RIGA: L&#39;ATTIVITÀ DEL MODELLO NON SEMBRA AVERE &quot;CONDIVISIONE&quot;)

1. (Facoltativo) Fai clic su **Seleziona padre** nel pannello a sinistra, selezionare l&#39;attività template nel modello di destinazione che si desidera diventare padre dell&#39;attività template copiata.

   >[!TIP]
   >
   >Quando si seleziona di copiare più attività modello in un elenco, tutte le attività modello selezionate diventano le attività secondarie dell&#39;elemento padre selezionato e vengono aggiunte dopo le attività figlio esistenti.

   Selezionare un padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività del modello, selezionare uno degli elementi principali nel piano del modello.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività modello padre per nome.

   L&#39;attività modello deve essere visualizzata nell&#39;elenco.

1. Selezionare il pulsante di scelta per il padre dopo averlo trovato.

   Se non si seleziona un&#39;attività modello padre, le attività modello vengono copiate come attività modello principale anziché come attività secondarie e vengono posizionate alla fine dell&#39;elenco attività modello nel modello di destinazione.

1. Fai clic su **Copia attività modello**.

   Le attività del modello copiate ora si trovano nel modello specificato e sono sottoattività all&#39;attività del modello principale selezionata o le ultime attività del modello nel modello.


## Spostare le attività dei modelli

Oltre a copiare le attività del modello, è anche possibile spostare un&#39;attività del modello in un&#39;altra attività del modello nello stesso modello o in un altro modello.


1. Passare al modello che contiene l&#39;attività modello o le attività modello che si desidera spostare.
1. Fai clic su **Attività dei modelli** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:
   * Fare clic sul nome di un&#39;attività modello per aprirla.
   * Selezionare una o più attività del modello nell&#39;elenco.
1. (Condizionale) Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) nella parte superiore dell&#39;elenco delle attività del modello o a destra del nome dell&#39;attività del modello se l&#39;attività è stata aperta, quindi fare clic su **Sposta a** o **Sposta**, a seconda della posizione di accesso all’opzione Sposta .
Viene visualizzata la casella Sposta attività modello.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Facoltativo) Rinomina l’attività del modello nel **Nome attività modello** campo .

   >[!TIP]
   >
   >Questo campo è oscurato e non modificabile quando si seleziona per spostare più attività modello in un elenco. È possibile passare il puntatore del mouse sul campo Nome dell&#39;attività del modello e viene visualizzato un elenco di tutte le attività del modello selezionate.

1. Inizia a digitare il nome della **Modello di destinazione** in cui si desidera spostare l&#39;attività del modello nel **Seleziona modello di destinazione** , quindi selezionalo quando viene visualizzato nell’elenco.

   >[!TIP]
   >
   >Puoi anche iniziare a digitare il numero di riferimento o l’ID del modello. Questo potrebbe essere utile per distinguere tra modelli con nomi identici.

1. (Condizionale) Fai clic su **richiesta di accesso** per richiedere l’accesso al modello, se non hai accesso al modello di destinazione.
1. (Condizionale) Continuare a spostare l&#39;attività del modello nel modello di destinazione selezionato senza richiedere l&#39;accesso se si dispone dell&#39;accesso per aggiungere attività del modello a uno dei task del modello nel modello di destinazione.

1. Fai clic su **Opzioni** nel pannello a sinistra, deselezionare gli attributi dell&#39;attività del modello che non si desidera copiare con l&#39;attività del modello. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!TIP]
   >
   >* La sezione Opzioni è disponibile solo dopo aver selezionato un modello di destinazione.
   >* Deselezionare **Seleziona tutto** deseleziona tutte le opzioni.


   Deselezionare le opzioni seguenti per non trasferire le informazioni all&#39;attività modello spostata. La tabella seguente descrive cosa accade quando le opzioni sono deselezionate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionare questa opzione per rimuovere tutte le informazioni dall'attività del modello quando lo si sposta nella nuova posizione. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>Il vincolo dell'attività del modello viene impostato su Il più presto possibile o Il più tardi possibile in base all'impostazione Modalità pianificazione modello.</p> <p> Se selezionata, il vincolo corrente dell'attività modello viene trasferito all'attività modello spostata. </p>

   <p><b>NOTA</b>

   Quando si sposta un&#39;attività modello con vincoli specifici per la data in un altro modello e le date dei vincoli dell&#39;attività modello sono al di fuori delle date del nuovo modello, il Vincolo dell&#39;attività del modello viene modificato in Non appena possibile o Più tardi possibile oppure vengono modificate le date di inizio pianificato o di completamento pianificato dei modelli.

   Di seguito sono riportati alcuni esempi di vincoli specifici per la data:
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
      <td>Tutti i processi di approvazione vengono rimossi dall'attività del modello.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Ciò significa che le dipendenze non verranno riportate con le attività del modello spostato. </p> <p>Quando è selezionata questa opzione, i predecessori all'interno del gruppo di attività modello spostate vengono mantenuti, gli altri vengono eliminati.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>I valori per i campi personalizzati vengono cancellati e i moduli personalizzati vengono trasferiti con l’attività modello spostata. </p> <p>Se selezionata, sia i moduli che i valori per i campi personalizzati vengono trasferiti con l’attività modello spostata. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazione Finanziaria</td> 
      <td>Le informazioni finanziarie dell'attività del modello spostata vengono rimosse e Workfront aggiorna il tipo di costo dell'attività del modello su No Cost e il tipo di ricavi dell'attività del modello su Non fatturabile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività modello non vengono trasferiti con l'attività modello spostata. Ciò include versioni, bozze e documenti collegati.</p>

   <p><b>NOTA</b></p>

   <ul><li>
      <p>Non sono incluse le approvazioni dei documenti. Le approvazioni dei documenti non possono mai essere spostate quando un'attività modello viene spostata.</p> </li>
      <li>Se si sceglie di non spostare i documenti con l'attività del modello, i documenti vengono eliminati e inseriti nel Cestino per 30 giorni. Un amministratore può ripristinarli e ripristinarli nell’attività del modello spostato.

   Se l&#39;attività del modello viene eliminata dopo lo spostamento, i documenti ripristinati verranno posizionati nell&#39;area Documenti della pagina utente dell&#39;amministratore che li ripristina. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria delle attività del modello non vengono trasferiti all'attività del modello spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate nell'attività modello non vengono trasferite con l'attività modello spostata. </td> 
     </tr>  
    </tbody> 
   </table>

(RICHIEDENDO L’ULTIMA RIGA: L&#39;ATTIVITÀ DEL MODELLO NON SEMBRA AVERE &quot;CONDIVISIONE&quot;)

1. (Facoltativo) Fai clic su **Seleziona padre** nel pannello a sinistra, selezionare l&#39;attività template nel modello di destinazione che si desidera diventare padre dell&#39;attività template spostata.

   >[!TIP]
   >
   >Quando si seleziona di spostare più attività modello in un elenco, tutte le attività modello selezionate diventano le secondari dell&#39;elemento padre selezionato e vengono aggiunte dopo le attività figlio esistenti.

   Selezionare un padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività del modello, selezionare uno degli elementi principali nel piano del modello.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività modello padre per nome.

   L&#39;attività modello deve essere visualizzata nell&#39;elenco.

1. Selezionare il pulsante di scelta per il padre dopo averlo trovato.

   Se non si seleziona un&#39;attività modello padre, le attività modello vengono spostate come attività modello principale anziché come attività secondarie e vengono posizionate alla fine dell&#39;elenco attività modello nel modello di destinazione.

1. Fai clic su **Sposta attività modello**.

   Le attività del modello spostato ora si trovano nel modello specificato e sono attività secondarie dell&#39;attività del modello principale selezionata oppure le ultime attività del modello nel modello.


