---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Aggiorna lavoro
description: È possibile aggiungere un aggiornamento su un oggetto Adobe Workfront (progetto, attività o problema) per comunicare l’avanzamento dell’oggetto. Gli utenti assegnati o abbonati all’oggetto possono visualizzare l’aggiornamento. Puoi anche assegnare tag agli utenti per attirare la loro attenzione sull’aggiornamento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 1%

---

# Aggiorna lavoro

<!-- Drafted for commenting experience: 

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the way you update work when using the Updates section of an object. 
>You can access the new design by enabling the commenting Beta. 
>Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

Puoi aggiungere commenti alla maggior parte degli oggetti in Adobe Workfront nella sezione Aggiornamenti . Per ulteriori informazioni sugli oggetti che visualizzano la sezione Aggiornamenti, consulta [Panoramica della sezione Aggiornamenti](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

È possibile aggiungere un aggiornamento a un oggetto Workfront (progetto, attività o problema) per comunicare l’avanzamento dell’oggetto, mentre si commenta l’oggetto. Gli utenti assegnati o abbonati all’oggetto possono visualizzare l’aggiornamento. Puoi anche assegnare tag agli utenti per attirare la loro attenzione sull’aggiornamento. Gli utenti con tag riceveranno una notifica in-app e un messaggio e-mail sull’aggiornamento.

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

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects

Adding an update to a work item differs depending on what version of the Updates section and what object you choose. 

### Add an update to a work item in the current Updates section

>[!NOTE]
>
>The following functionality is available for all objects except for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. Passare all&#39;elemento di lavoro per il quale si desidera fornire un aggiornamento (ad esempio un progetto, un&#39;attività o un problema).
1. Fai clic sul pulsante **Aggiornamenti** sezione .
1. Fai clic su **Avvia un nuovo aggiornamento,** quindi digita l&#39;aggiornamento.
1. (Facoltativo) Utilizza Rich Text o aggiungi emoticon, collegamenti o immagini al tuo aggiornamento per migliorare i contenuti. Per ulteriori informazioni, consulta la sezione &quot;Utilizzare il testo RTF in un aggiornamento Workfront&quot; in questo articolo
1. (Facoltativo) Aggiornare una delle seguenti informazioni sull&#39;elemento di lavoro:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notifica</strong></td> 
      <td>Identifica gli utenti a cui è necessario notificare l’aggiornamento. Gli utenti assegnati o abbonati all’oggetto ricevono automaticamente la notifica quando viene effettuato un aggiornamento.<br><p>Per informazioni su come includere altri in un aggiornamento, vedi <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Assegnare tag agli altri utenti in caso di aggiornamenti</a>.</p></td> 
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
      <td>Fai clic sulla freccia accanto allo stato corrente, quindi seleziona lo stato desiderato dal menu a discesa. Per informazioni sull'impostazione di uno stato, consulta <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiorna stato attività</a>.<p>L'aggiornamento dello stato di un elemento di lavoro non modifica automaticamente lo stato di un progetto. A seconda della configurazione del progetto, potrebbe essere necessario eseguire separatamente gli aggiornamenti allo stato del progetto. Per ulteriori informazioni sui vari tipi di aggiornamento dei progetti, consulta <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p><p><b>NOTA</b>

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

<!--

### Add an update to a work item using the commenting Beta experience


>[!NOTE]
>
>The functionality described in this section is available for the following objects:
>
>* <span class="preview">Issues, when you enable the commenting Beta experience.</span>
>
>   <span class="preview">This functionality is available only for the Updates section of issues, and it is not available for the following areas:</span>
>
>   * <span class="preview">Home</span>
>   * <span class="preview">Summary panel in lists</span>
>   * <span class="preview">Summary panel in timesheets</span>
>* Goals
>
>   The commenting experience Beta is the default current experience for goals.
>   You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


1. Locate the object you want to update, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Click **Try out the commenting Beta** button in the lower-right corner of the Updates area, then click **Agree** on the Beta agreement. This switches the Updates area to the commenting Beta experience. 
   The **Comments** tab is selected by default. 
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any of the following options from the **Rich Text** toolbar to enhance your text: 

   * Bold
   * Italics
   * Underline
   * Link
   * Bulleted List
   * Numbered List
   * Add attachment (mark this parenthesis as draft: ************ this might be renamed)
   
   For more information, see the "Use Rich Text in a Workfront update" section in this article.

   >[!TIP]
   >
   >   If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
   >
   > ![](assets/real-time-new-red-indicator-unified-commenting.png)



1. Click **Submit** to add the update to the Workfront object. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment, or remove any of the tagged users. 
   You can edit your comment within 15 from submitting it. An "Edited" indicator is added to the left of the date stamp that displays when the comment was updated. 

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********). For information about replying to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Click the **Like** icon![](assets/like-icon.png). The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When the object or any of its children are updated, Workfront generates a note about that update and displays it in the System Activity tab. 

   For more information see [Updates section  overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >You cannot add a comment to a system update.
-->


## Utilizzare Rich Text in un aggiornamento di Workfront

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.

>[!NOTE]
>
>Some of the options in the Rich Text toolbar are not available for the commenting Beta experience.-->


Puoi migliorare gli aggiornamenti utilizzando Rich Text o aggiungendo vari elementi, come emoticon, collegamenti o immagini.

1. Vai all’area Aggiornamenti e inizia a digitare un commento.
1. (Facoltativo) Per aggiungere formattazione RTF all&#39;aggiornamento, utilizzare qualsiasi attributo **Rich Text** durante la digitazione.

   | **Attributo** | **Pulsante della barra degli strumenti** | **Tasti di scelta rapida Mac** | **Tasti di scelta rapida PC** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png) | inta+b | Ctrl+B |
   | Corsivo | ![mceclip9.png](assets/mceclip9.png) | +i | Ctrl+I |
   | Sottolinea | ![mceclip8.png](assets/mceclip8.png) | +u | Ctrl+U |
   | Collegamento ipertestuale | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | Elenco puntato | ![mceclip6.png](assets/mceclip6.png) | +Maiusc+8 | Ctrl+Maiusc+8 |
   | Elenco numerato | ![mceclip5.png](assets/mceclip5.png) | +Maiusc+7 | Ctrl+Maiusc+7 |
   | Citazione | ![](assets/block-quote-icon-large.png) | +Maiusc+9 | Ctrl+Maiusc+9 |

   Per interrompere la formattazione del testo, deselezionare l&#39;attributo **Rich Text** barra degli strumenti.

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

1. (Facoltativo) Per allegare un&#39;immagine all&#39;aggiornamento, fai clic sul pulsante **Immagine** icona ![](assets/addimageicon-35x32.png) e passare all&#39;immagine sul computer.\
   Oppure\
   Trascina l’immagine nell’area di aggiornamento.

   >[!NOTE]
   >
   >* Per visualizzare l’icona Immagine, l’amministratore di Workfront deve abilitare l’aggiunta di immagini.
   >* La dimensione massima del file immagine è 7 MB. I tipi di file immagine supportati sono .jpg, .gif e .png.
   >* Le immagini sono accessibili solo dalla scheda Aggiornamenti di un oggetto e non sono disponibili nella scheda Documenti.
   >* Puoi inviare un aggiornamento con un’immagine e senza testo.

1. Fai clic su **Aggiorna**  <!--<span class="preview">or **Submit**</span>, in the commenting Beta experience-->.


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
1. Fai clic sul pulsante **Altro** menu, quindi fai clic su **Copia collegamento thread**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Copia il collegamento di aggiornamento {#copy-the-update-link}

Questa opzione copia un collegamento di aggiornamento specifico negli Appunti. Quando condividi il collegamento di aggiornamento, l’utente che lo segue visualizza un bordo intorno all’aggiornamento.

1. Vai all&#39;aggiornamento o alla risposta che desideri copiare.
1. Fai clic sul pulsante **Altro** accanto al singolo aggiornamento, quindi fai clic su **Collegamento Copia aggiornamento**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Eliminare un aggiornamento o una risposta

A seconda dell’accesso fornito dall’amministratore di Workfront, potrebbe essere possibile eliminare gli aggiornamenti aggiunti nella scheda Aggiornamenti di un oggetto. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) nell&#39;articolo [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Nessun utente Workfront (incluso l’amministratore Workfront) può eliminare gli aggiornamenti effettuati da un altro utente. Tuttavia, se il livello di accesso di un utente consente loro di eliminare i propri aggiornamenti, l&#39;amministratore di Workfront può effettuare l&#39;accesso come tale utente ed eliminare gli aggiornamenti apportati. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) e [Accedi come altro utente](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Passa all&#39;aggiornamento o alla risposta da eliminare.
1. Fai clic sul pulsante **Altro** accanto all&#39;aggiornamento o alla risposta che si desidera eliminare, quindi fare clic su **Elimina**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Nel messaggio visualizzato, fai clic su **Conferma** <!--<span class="preview">or **Delete**</span>, in the commenting Beta experience-->.

>[!NOTE]
>
>Se si elimina un aggiornamento con un&#39;immagine allegata, vengono eliminati sia il commento che l&#39;immagine.

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

<!--remove preview with 23.2 production: 

<div class="preview">
>[!NOTE]
>
>It is not possible to disable system updates when using the Beta commenting experience. 
>The information in this section refers only to functionality available in the current Updtes section. 
>For more information about system updates in the Beta version, see [Updates section overview](../updating-work-items-and-viewing-updates/updates-tab-overview.md) 
</div>
-->

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

