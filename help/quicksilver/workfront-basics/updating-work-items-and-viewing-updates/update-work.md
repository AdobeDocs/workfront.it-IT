---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Aggiorna lavoro
description: È possibile aggiungere un aggiornamento su un oggetto Adobe Workfront (progetto, attività o problema) per comunicare l’avanzamento dell’oggetto. Gli utenti assegnati o abbonati all’oggetto possono visualizzare l’aggiornamento. Puoi anche assegnare tag agli utenti per attirare la loro attenzione sull’aggiornamento.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 77a489455b0d058bc53fbb87ffd219cf7b50a213
workflow-type: tm+mt
source-wordcount: '3153'
ht-degree: 1%

---

# Aggiorna lavoro

<!--take "Beta" references out when we remove the beta-->

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

>[!NOTE]
>
>Stiamo riprogettando l’esperienza di commento in Adobe Workfront.
>
>Per ulteriori informazioni sulla nuova esperienza di commento, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Puoi accedere alla nuova esperienza per i seguenti oggetti:
> * Problemi relativi all’abilitazione della funzione di commento Beta.
   >
   >     Questa funzionalità è disponibile solo per la sezione Aggiornamenti dei problemi e non è disponibile per le seguenti aree:
   >
   >     * Home
   >     * Pannello di riepilogo negli elenchi
   >     * Pannello Riepilogo nei fogli presenze
>
> * Obiettivi

   >
   >   La nuova esperienza di commento è l’impostazione predefinita per gli obiettivi. Devi disporre di una licenza aggiuntiva per accedere agli obiettivi di Workfront. Per ulteriori informazioni, consulta [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Per informazioni sui commenti sugli obiettivi, consulta [Gestire i commenti sull’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).


Puoi aggiungere commenti alla maggior parte degli oggetti in Adobe Workfront nella sezione Aggiornamenti . Per ulteriori informazioni sugli oggetti che visualizzano la sezione Aggiornamenti, consulta [Panoramica della sezione Aggiornamenti](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

È possibile aggiungere un aggiornamento a un oggetto Workfront (progetto, attività o problema) per comunicare l’avanzamento dell’oggetto, mentre si commenta l’oggetto. Gli utenti assegnati o abbonati all’oggetto possono visualizzare l’aggiornamento. Puoi anche assegnare tag agli utenti per attirare la loro attenzione sull’aggiornamento. Gli utenti con tag ricevono una notifica in-app e un messaggio e-mail sull’aggiornamento.

Le informazioni contenute in questa pagina descrivono come è possibile commentare gli oggetti Workfront e come aggiornare progetti, attività e problemi. Per informazioni sui commenti sugli obiettivi, consulta [Gestire i commenti sull’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md). Devi disporre di una licenza aggiuntiva per accedere agli obiettivi di Workfront.


Puoi aggiungere un aggiornamento a progetti, attività e problemi nelle seguenti aree di Workfront:

* Da un oggetto Workfront, nella sezione Aggiornamenti
* Dall&#39;area Home (per attività e problemi)
* Dal pannello Riepilogo in un elenco di oggetti (per attività e problemi)
* Dalla scheda attività (per attività e problemi)

## Requisiti di accesso

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiesta o superiore di problemi e documenti; Revisione o superiore per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Visualizza o modifica l'accesso per l'oggetto su cui si trova l'aggiornamento</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizza l’accesso all’oggetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiungere un aggiornamento a un elemento di lavoro

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

L’aggiunta di un aggiornamento a un elemento di lavoro varia a seconda della versione della sezione Aggiornamenti e dell’oggetto scelto.

### Aggiungere un aggiornamento a un elemento di lavoro nella sezione Aggiornamenti correnti

>[!NOTE]
>
>La seguente funzionalità è disponibile per tutti gli oggetti ad eccezione degli obiettivi. Devi disporre di una licenza aggiuntiva per accedere agli obiettivi di Workfront. Per informazioni sui commenti sugli obiettivi, consulta [Gestire i commenti sull’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md)

1. Passare all&#39;elemento di lavoro per il quale si desidera fornire un aggiornamento (ad esempio un progetto, un&#39;attività o un problema).
1. Fai clic sul pulsante **Aggiornamenti** sezione .
1. Fai clic su **Avvia un nuovo aggiornamento,** quindi digita l&#39;aggiornamento.
1. (Facoltativo) Utilizza Rich Text o aggiungi emoticon, collegamenti o immagini al tuo aggiornamento per migliorare i contenuti. Per ulteriori informazioni, consulta la sezione [Utilizzare Rich Text in un aggiornamento di Workfront](#use-rich-text-in-a-workfront-update) sezione del presente articolo
1. (Facoltativo) Aggiornare una delle seguenti informazioni sull&#39;elemento di lavoro:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notifica</strong></td> 
      <td>Identifica gli utenti a cui deve essere notificato l’aggiornamento. Gli utenti assegnati o abbonati all’oggetto ricevono automaticamente la notifica quando viene effettuato un aggiornamento.<br><p>Per informazioni su come includere altri in un aggiornamento, vedi <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag agli altri utenti in caso di aggiornamenti</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Conferma data</strong></td> 
      <td>Nel selettore data, selezionare la data in cui si effettua il commit per completare l'elemento di lavoro. Per informazioni sulla data di commit, vedi <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data del commit</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condizione</strong></td> 
      <td>Selezionare una nuova condizione per l'attività o il problema. Per informazioni sulla selezione di una condizione, consulta <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aggiorna condizione per attività e problemi</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Stato</strong></td> 
      <td>Fai clic sulla freccia accanto allo stato corrente, quindi seleziona lo stato desiderato dal menu a discesa. Per informazioni sull'impostazione di uno stato, consulta <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiorna stato attività</a>.<p>L'aggiornamento dello stato di un elemento di lavoro non modifica automaticamente lo stato di un progetto. A seconda della configurazione del progetto, è possibile che sia necessario eseguire separatamente gli aggiornamenti allo stato del progetto. Per ulteriori informazioni sui vari tipi di aggiornamento dei progetti, consulta <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p><p><b>NOTA</b>

   Non è possibile modificare lo stato di un elemento di lavoro in attesa di approvazione.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Barra di completamento</strong></td> 
      <td>(Disponibile solo per le attività) Indica la percentuale di lavoro completato portando la barra di avanzamento alla percentuale desiderata. È inoltre possibile fare doppio clic sulla barra di completamento e immettere la percentuale di completamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Privato per la mia azienda</strong></td> 
      <td> <p>Disattiva questa opzione per impedire agli utenti esterni all’azienda di accedere per visualizzare questo aggiornamento.</p> 
      <p><b>NOTA</b></p>
      <p>Questa opzione viene visualizzata solo quando l'utente è associato a un'azienda.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiorna** per aggiungere l’aggiornamento all’oggetto Workfront.

   >[!NOTE]
   >
   >Una piccola finestra pop-up apparirà per sette secondi dopo aver fatto clic su **Aggiorna**, che consente di annullare l’aggiornamento e tornare al riquadro di modifica prima della pubblicazione dell’aggiornamento. L’aggiornamento viene pubblicato se si chiude il pop-up Annulla, se si attende che scompaia o si esce dalla pagina.
   >
   >Se l’amministratore di Workfront seleziona l’impostazione &quot;Non consentire mai agli utenti di eliminare commenti&quot; nel livello di accesso, non è possibile annullare un commento. Per ulteriori informazioni, consulta [Creare e modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Per rispondere a un aggiornamento, vedi [Risposta agli aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Aggiungere un aggiornamento a un elemento di lavoro utilizzando l’esperienza di creazione dei commenti Beta

1. Individuare l’oggetto che si desidera aggiornare, quindi fare clic sul suo nome per aprire la pagina dell’oggetto.
1. Fai clic su  **Aggiornamenti** nel pannello a sinistra.
1. Abilita la **Versione beta dei commenti** seleziona l’angolo superiore destro dell’area Aggiornamenti , quindi fai clic su **Accetto** sull&#39;accordo Beta. In questo modo l’area Aggiornamenti passa all’esperienza di creazione dei commenti Beta.
La **Commenti** è selezionata per impostazione predefinita.
1. Inizia a inserire un commento in **Nuovo commento** scatola.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Se passi dalla sezione Aggiornamenti prima di terminare la digitazione e l’invio di un commento, il commento viene mantenuto in modalità bozza anche dopo la disconnessione e il successivo accesso. Anche le immagini aggiunte al commento vengono salvate nella bozza. Le bozze vengono salvate per 7 giorni dopo i quali vengono scartate e non possono essere recuperate. I commenti creati sono visibili solo all’utente che li inserisce.

1. (Facoltativo) In **Assegnare tag a persone o team** area, inizia a digitare il nome o l’e-mail di un utente o di un team che desideri includere in questo commento, quindi selezionalo quando viene visualizzato nell’elenco.
1. (Facoltativo) Per aggiungere formattazione RTF all&#39;aggiornamento, utilizzare una delle opzioni seguenti nella sezione **Rich Text** barra degli strumenti per migliorare il testo:

   * Bold
   * Corsivo
   * Sottolinea
   * Link
   * Elenco puntato
   * Elenco numerato
   * Aggiungi allegato <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   Per ulteriori informazioni, consulta la sezione [Utilizzare Rich Text in un aggiornamento di Workfront](#use-rich-text-in-a-workfront-update) in questo articolo. <!--remove this list, above, when we get to parity for Rich Text-->

   >[!TIP]
   >
   >Se un altro utente invia un commento allo stesso elemento che stai aggiornando, ci sarà una linea rossa con un indicatore &quot;Nuovo&quot; per informarti dei commenti più recenti.
   >
   >L&#39;indicatore viene visualizzato solo dopo che il commento è stato inviato sull&#39;elemento e non quando il commento è ancora composto.
   >
   >L’indicatore &quot;Nuovo&quot; viene visualizzato solo quando l’utente che ha inserito un nuovo aggiornamento e l’utente che sta attualmente inserendo un aggiornamento utilizzano la nuova esperienza di commento.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)


1. Fai clic su **Invia** per aggiungere l’aggiornamento all’oggetto Workfront.
1. (Facoltativo) Per modificare un commento, fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) a destra dell&#39;icona Mi piace, quindi fai clic su **Modifica**.
1. Modifica le informazioni nel commento, aggiungi o rimuovi immagini o rimuovi uno degli utenti con tag.
È possibile modificare il commento entro 15 dall’invio. Un indicatore &quot;Modificato&quot; viene aggiunto a sinistra del timbro data che viene visualizzato quando il commento è stato aggiornato.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   Viene generato un messaggio e-mail per avvisare gli utenti dell’aggiornamento solo quando si invia l’aggiornamento originale. Dopo aver modificato l’aggiornamento non viene generato alcun messaggio e-mail.

1. (Facoltativo) Fai clic su **Rispondi** per rispondere a un commento esistente, segui i passaggi 4-7 di cui sopra. <!--(**************insure this stays accurate***********)-->. Per informazioni sulla risposta a un aggiornamento, consulta [Risposta agli aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Condizionale e facoltativo) Se altri utenti hanno aggiunto commenti visualizzati al di fuori dell’area visibile nella sezione Aggiornamenti , fai clic su **Visualizza** in blu **nuovo banner commenti** nella parte inferiore dello schermo per visualizzare questi commenti.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Ulteriori commenti vengono visualizzati nella parte inferiore dello schermo.

   >[!NOTE]
   >
   >   L’indicatore &quot;nuovi commenti&quot; e il pulsante &quot;Visualizza&quot; vengono visualizzati solo quando gli utenti che hanno inserito i nuovi aggiornamenti e l’utente che sta guardando la sezione Aggiornamenti stanno utilizzando la nuova esperienza di commento.


1. (Facoltativo) Fai clic sul pulsante **Simile** icona![](assets/like-icon.png). L’icona si aggiorna con il numero di Mi piace.
1. (Condizionale e Facoltativo) Se hai incluso altre persone nel commento, fai clic sul numero di membri inclusi nell’aggiornamento per visualizzare un elenco di entità con cui è condiviso il commento immesso.

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Facoltativo) Fai clic sul pulsante **Attività di sistema** per visualizzare gli aggiornamenti registrati dal sistema. Quando l’oggetto o uno dei relativi elementi figlio viene aggiornato, Workfront genera una nota relativa a tale aggiornamento e la visualizza nella scheda Attività di sistema.

   Per ulteriori informazioni consulta [Panoramica della sezione Aggiornamenti](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Non è possibile aggiungere un commento a un aggiornamento del sistema.


## Utilizzare Rich Text in un aggiornamento di Workfront{#use-rich-text-in-a-workfront-update}

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Alcune delle opzioni nella barra degli strumenti Rich Text potrebbero non essere disponibili per l’esperienza di commento Beta.

Puoi migliorare gli aggiornamenti utilizzando Rich Text o aggiungendo vari elementi, come emoticon, collegamenti o immagini.

1. Vai all’area Aggiornamenti e inizia a digitare un commento.
1. (Facoltativo) Per aggiungere formattazione RTF all&#39;aggiornamento, utilizzare qualsiasi attributo **Rich Text** durante la digitazione.

   | **Attributo** | **Pulsante Barra degli strumenti** | **Tasti di scelta rapida Mac** | **Tasti di scelta rapida di Windows** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png) | inta+b | Ctrl+B |
   | Corsivo | ![mceclip9.png](assets/mceclip9.png) | +i | Ctrl+I |
   | Sottolinea | ![mceclip8.png](assets/mceclip8.png) | +u | Ctrl+U |
   | Collegamento ipertestuale | ![mceclip7.png](assets/mceclip7.png) | <br>Per aprire la casella Crea collegamenti o Aggiungi collegamenti : ALT+K</br> <br><span class="preview">Nell’esperienza beta dei commenti, per incollare un collegamento sul testo selezionato: +V</span></br> | <br>Per aprire la casella Crea collegamenti o Aggiungi collegamenti : Ctrl+K</br> <br><span class="preview">Nell’esperienza beta dei commenti, per incollare un collegamento sul testo selezionato: Ctrl+V</span></br> |
   | Elenco puntato | ![mceclip6.png](assets/mceclip6.png) | +Maiusc+8 | Ctrl+Maiusc+8 |
   | Elenco numerato | ![mceclip5.png](assets/mceclip5.png) | +Maiusc+7 | Ctrl+Maiusc+7 |
   | Citazione | ![](assets/block-quote-icon-large.png) | +Maiusc+9 | Ctrl+Maiusc+9 |

   Per interrompere la formattazione del testo, deselezionare l&#39;attributo **Rich Text** barra degli strumenti.

   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment-->

   >[!NOTE]
   >
   >* La formattazione viene visualizzata anche in qualsiasi notifica e-mail che gli utenti ricevono contenente il tuo aggiornamento.
   >* La formattazione RTF applicata a un aggiornamento in un messaggio e-mail non viene visualizzata nell’aggiornamento quando viene visualizzata nella scheda Aggiornamenti.
   >* Se l’organizzazione utilizza Workfront con Internet Explorer, qualsiasi testo formattato incollato in un aggiornamento perde la formattazione RTF e viene visualizzato come testo normale. È possibile riformattare il testo utilizzando gli attributi nella barra degli strumenti RTF.
   >* La formattazione RTF non è disponibile per gli aggiornamenti apportati nell’area Foglio presenze o per gli oggetti Nota e Ultima condizione visualizzati in un rapporto.


1. (Facoltativo) Se desideri includere testo da aggiornamenti precedenti o da altre fonti e distinguerlo dall’aggiornamento, puoi contrassegnarlo come preventivo di blocco. Fai clic sul pulsante **Preventivo** icona ![](assets/block-quote-small.png) e digitare il testo che si desidera citare. Il testo tra virgolette viene contrassegnato da una linea grigia verticale. Fai clic sul pulsante **Preventivo** per tornare alla formattazione normale.

   ![](assets/block-quote-marked-350x144.png)

1. (Facoltativo) Aggiungi gli emoticon al tuo aggiornamento.

   >[!NOTE]
   >
   >* Workfront non sostituisce gli emoticon di punteggiatura come :) con gli emoticon.
   >* Le emoticon non sono disponibili per gli aggiornamenti effettuati nell’area Timesheets o per gli oggetti Note e Last Condition visualizzati in un rapporto.
   >* La funzione emoji in Workfront utilizza caratteri Unicode e, come tale, viene visualizzata solo sui browser e sui sistemi operativi che supportano i punti di codice Unicode. Gli utenti di una versione di piattaforma, browser o sistema operativo diversa dalla tua potrebbero non avere accesso agli stessi emoticon.
   >* Un’emoji non supportata è rappresentata da una casella bianca o nera.
   >* Windows 7 supporta solo le emoticon in bianco e nero.
   >* Le emoticon applicate a un aggiornamento effettuato tramite e-mail non vengono visualizzate sull’aggiornamento quando visualizzate nell’area Aggiornamenti .


1. (Facoltativo) Per aggiungere un collegamento URL a ulteriori origini di informazioni:

   1. Fai clic nell’aggiornamento in cui desideri inserire un collegamento.
   1. Sulla **Rich Text** barra degli strumenti, fai clic su **Collegamento ipertestuale** icona. ![](assets/link-icon.png)

   1. In **Crea collegamento** casella visualizzata, sotto **URL**, digita o incolla l’URL dell’origine a cui desideri collegare.

   1. Sotto **Testo da visualizzare**, digita o incolla il testo del collegamento.
   1. Fai clic su **Salva**.

1. (Facoltativo) Per allegare un&#39;immagine all&#39;aggiornamento, effettua una delle seguenti operazioni, a seconda dell&#39;ambiente utilizzato:

   * Fai clic sul pulsante **Immagine** icona ![](assets/addimageicon-35x32.png) e sfogliare l&#39;immagine sul computer o trascinare l&#39;immagine nell&#39;area di aggiornamento, quando si utilizza l&#39;esperienza di aggiornamento corrente

   Oppure

   Fai clic sul pulsante **Aggiungi allegato** icona ![](assets/add-image-paperclip-icon.png) e sfogliare l&#39;immagine sul computer, quando si utilizza l&#39;esperienza di commento Beta. <!--the name of the icon and the icon for it might change-->

   >[!NOTE]
   >
   >* Per poter visualizzare le icone Immagine o Aggiungi allegato, l’amministratore di Workfront deve abilitare l’aggiunta di immagini nella sezione Preferenze feed aggiornamento dell’area Interfaccia Workfront . Per informazioni, consulta [Configurare le preferenze per gli aggiornamenti utente](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* La dimensione massima del file immagine è 7 MB. I tipi di file immagine supportati sono .jpg, .gif e .png.
   >* Le immagini sono accessibili dalla sezione Aggiornamenti di un oggetto e sono disponibili anche nell’area Documenti.
   >* Puoi inviare un aggiornamento con un’immagine e senza testo.
   >* Quando elimini un commento che contiene un’immagine, esistono i seguenti scenari a seconda dell’esperienza scelta:
      >
      >     * Nell’esperienza di commento corrente, l’immagine rimane nell’area Documenti ma non è più visibile nella sezione Aggiornamenti .
      >     * Nella nuova esperienza di commento, l’immagine viene rimossa dalla sezione Aggiornamenti e dall’area Documenti. L’immagine viene inoltre eliminata dall’area Documenti quando si modifica un commento ed elimina l’immagine.
   >* Quando un utente elimina un&#39;immagine associata a un commento dall&#39;area Documenti, viene rimossa anche dal commento.


1. Fai clic su **Aggiorna**  o **Invia**, quando si utilizza l’esperienza di creazione di commenti Beta.


## Copia informazioni di aggiornamento

<!--drafted for beta release toggle - remove when copying an update will be available:

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

Esistono diversi modi per copiare un aggiornamento. Dopo aver copiato un collegamento, puoi condividerlo con altri per indirizzarlo all’aggiornamento.

* [Copia l&#39;aggiornamento](#copy-the-update)
* [Copia il collegamento del thread](#copy-the-thread-link)
* [Copia il collegamento di aggiornamento](#copy-the-update-link)

### Copia l&#39;aggiornamento {#copy-the-update}

Questa opzione copia il testo da un aggiornamento specifico negli Appunti.

1. Vai all&#39;aggiornamento o alla risposta che desideri copiare.
1. Fai clic sul pulsante **Altro** menu, quindi fai clic su **Copia testo corpo**.

   ![Seleziona Copia testo corpo](assets/update-stream-copy-body-text-350x152.png)

### Copia il collegamento del thread {#copy-the-thread-link}

Questa opzione copia il collegamento del thread completo negli Appunti in modo da poter condividere il thread con altri utenti.

1. Passa al thread di aggiornamento da copiare.

1. Fai clic sul pulsante **Altro** menu, quindi fai clic su **Copia collegamento thread** o **Copia collegamento**, quando utilizzi l’esperienza Beta.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Copia il collegamento di aggiornamento {#copy-the-update-link}

Questa opzione copia un collegamento di aggiornamento specifico negli Appunti. Quando condividi il collegamento di aggiornamento, l’utente che lo segue visualizza un bordo intorno all’aggiornamento.

1. Vai all&#39;aggiornamento o alla risposta che desideri copiare.
1. Fai clic sul pulsante **Altro** accanto al singolo aggiornamento, quindi fai clic su **Collegamento Copia aggiornamento** o **Copia collegamento**, quando utilizzi l’esperienza Beta.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Eliminare un aggiornamento o una risposta

A seconda dell’accesso fornito dall’amministratore di Workfront, potrebbe essere possibile eliminare gli aggiornamenti aggiunti nella scheda Aggiornamenti di un oggetto. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) nell&#39;articolo [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Nessun utente Workfront (incluso l’amministratore Workfront) può eliminare gli aggiornamenti effettuati da un altro utente. Tuttavia, se il livello di accesso di un utente consente loro di eliminare i propri aggiornamenti, l&#39;amministratore di Workfront può effettuare l&#39;accesso come tale utente ed eliminare gli aggiornamenti apportati. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) e [Accedi come altro utente](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Passa all&#39;aggiornamento o alla risposta da eliminare.
1. Fai clic sul pulsante **Altro** accanto all&#39;aggiornamento o alla risposta che si desidera eliminare, quindi fare clic su **Elimina**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Nel messaggio visualizzato, fai clic su **Conferma** o fai clic su **Elimina**, quando si utilizza l’esperienza di creazione di commenti Beta.

   >[!NOTE]
   >
   >Se si elimina un aggiornamento con un&#39;immagine allegata, vengono eliminati sia il commento che l&#39;immagine. Per ulteriori informazioni, consulta la sezione [Utilizzare testo RTF in un aggiornamento Workfront](#use-rich-text-in-a-workfront-update) in questo articolo.

   Quando al commento eliminato sono associate delle risposte, è presente un&#39;indicazione che il commento è stato rimosso con il nome dell&#39;utente che lo ha rimosso.

   ![](assets/removed-comment-indicator-new-experience.png)

   Quando si utilizza l’esperienza di commento Beta, i commenti eliminati vengono rimossi immediatamente da Workfront. Un utente che utilizza la sezione Aggiornamenti vede un commento eliminato da un altro utente in tempo reale.

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

## Aggiungere un aggiornamento in una scheda attività

1. Passare a una scheda attività in cui si desidera eseguire un aggiornamento.
1. Fare clic sulla scheda attività per aprirla.
1. Nella parte inferiore della scheda attività fare clic su **Includi un commento**.
1. Nella casella visualizzata nella parte inferiore della scheda attività, digitare un aggiornamento.

   ![scheda_aggiornamento_flusso.png](assets/timesheet-update-stream-350x50.png)

1. (Condizionale) Per salvare l&#39;aggiornamento senza inviare la scheda attività per l&#39;approvazione, fare clic su **Salva per più tardi**.

   Oppure

   Per salvare l&#39;aggiornamento e inviare la scheda attività per l&#39;approvazione, fare clic su **Invia per approvazione**.

   Oppure

   Se la scheda attività non è impostata con un approvatore, fare clic su **Salva e chiudi scheda attività** per salvare l&#39;aggiornamento.

## Attiva o disattiva gli aggiornamenti del sistema

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->

>[!NOTE]
>
>Non è possibile disabilitare gli aggiornamenti di sistema quando si utilizza l&#39;esperienza di commento Beta.
>Le informazioni presenti in questa sezione si riferiscono solo alle funzionalità disponibili nella sezione Aggiornamenti correnti.
>Per ulteriori informazioni sugli aggiornamenti di sistema nella versione Beta, consulta [Panoramica della sezione Aggiornamenti](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


Nella sezione Aggiornamenti di un oggetto Workfront sono visualizzati due tipi di informazioni:

* **Aggiornamenti utente:** Gli aggiornamenti utente sono commenti inseriti dall&#39;utente e da altri utenti nel sistema.

   ![](assets/user-update-cl-350x277.png)

* **Aggiornamenti di sistema:** Gli aggiornamenti di sistema registrano la rimozione delle risorse, l&#39;aggiunta o l&#39;eliminazione di versioni, l&#39;aggiunta o la rimozione di una richiesta di approvazione, nonché di eventuali modifiche o modifiche apportate ai documenti sull&#39;oggetto.

   ![](assets/system-updates-cl-350x277.png)

A seconda della licenza Workfront, gli aggiornamenti di sistema potrebbero essere attivati per impostazione predefinita. Gli amministratori di Workfront possono determinare cosa viene tracciato negli aggiornamenti di sistema, come spiegato in [Aggiornamenti tracciati dal sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). È inoltre possibile filtrare gli aggiornamenti di sistema o le attività in modo da visualizzare solo gli aggiornamenti utente per tutti gli oggetti.

Per ulteriori informazioni sulla differenza tra gli aggiornamenti utente e di sistema, consulta [Aggiornamenti tracciati dal sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Per attivare o disattivare gli aggiornamenti di sistema:

1. Fai clic sul pulsante **Aggiornamenti** su un oggetto.
1. Fai clic su **Mostra aggiornamenti di sistema** per far scorrere l&#39;interruttore a sinistra (disattivato) o a destra (attivato).

   ![](assets/show-system-updates-qs-350x55.png)

   Questa opzione è persistente in tutti gli oggetti in Workfront e rimane nella posizione selezionata, anche se si disconnette da Workfront.

