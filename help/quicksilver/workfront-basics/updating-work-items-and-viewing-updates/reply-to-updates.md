---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Rispondi agli aggiornamenti
description: Quando qualcuno aggiunge o risponde a un aggiornamento su un oggetto di lavoro, la risposta viene visualizzata nel thread di comunicazione nella sezione Aggiornamenti dell’oggetto. È possibile aggiungere una risposta a un aggiornamento o aggiungerla come se si disponesse dell'accesso di visualizzazione all'oggetto.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Rispondi agli aggiornamenti

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

>[!NOTE]
>
>Attualmente stiamo riprogettando l’esperienza di aggiunta di commenti in Adobe Workfront.
>
>Per ulteriori informazioni sulla nuova esperienza di aggiunta di commenti, vedi [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Puoi accedere alla nuova esperienza per i seguenti oggetti:
> * Problemi, progetti, attività e documenti.
>
>     Questa funzione è disponibile quando abiliti l’esperienza Beta di commento.
>
>     Questa funzionalità è disponibile solo per la sezione Aggiornamenti e non per le aree seguenti:
>
>     * Home
>     * Pannello Riepilogo negli elenchi
>     * Pannello Riepilogo nelle schede orario
>
> * Obiettivi, carte nell’area Bacheche
>
>   La nuova esperienza di commento è l’unica per obiettivi e carte. È necessaria un&#39;ulteriore licenza per accedere a Workfront Goals. Per ulteriori informazioni, consulta [Requisiti per l’utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     È possibile aggiungere e visualizzare aggiornamenti alle schede nell&#39;area Bacheche quando si abilitano le sezioni Commenti e Attività di sistema su una scheda. Per ulteriori informazioni, consulta [Aggiungere una scheda ad hoc a una bacheca](../../agile/get-started-with-boards/add-card-to-board.md).


Quando qualcuno risponde a un commento o a un aggiornamento di sistema su un oggetto di lavoro, la risposta viene visualizzata nel thread di comunicazione nella sezione Aggiornamenti dell’oggetto.

>[!IMPORTANT]
>
>Nella nuova esperienza di inserimento di commenti non è possibile rispondere agli aggiornamenti di sistema. Per ulteriori informazioni, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiedi o superiore per problemi e documenti; rivedi o superiore per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Richiedente o superiore per problemi e documenti; revisore o superiore per tutti gli altri oggetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso di visualizzazione all'oggetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Rispondere a un aggiornamento o a una risposta in Workfront

È possibile rispondere a un commento nel thread di un oggetto che è possibile visualizzare oppure accedere come amministratore di Workfront o di gruppo e rispondere a un commento per conto di un altro utente. Per ulteriori informazioni, consulta [Accedi come altro utente](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

La risposta a un commento o a una risposta varia a seconda dell’esperienza e dell’oggetto selezionato.

### Rispondi a un aggiornamento o rispondi alla sezione Aggiornamenti correnti

1. Passare all&#39;oggetto a cui si desidera aggiungere una risposta.
1. Il giorno **Aggiornamenti** per l&#39;oggetto, trovare l&#39;aggiornamento o la risposta a cui si desidera rispondere.

1. (Facoltativo) Per visualizzare un&#39;immagine nell&#39;aggiornamento esistente, effettuate una delle seguenti operazioni:

   * Fai clic su **Anteprima** icona ![](assets/previewimageicon-31x31.png) sulla miniatura dell’immagine per aprire l’immagine a dimensione intera in una nuova scheda del browser.
   * Fai clic su **Scarica** icona ![](assets/downloadimageicon.png) sulla miniatura dell&#39;immagine per scaricare l&#39;immagine.

1. Clic **Rispondi** nell’aggiornamento, digita una risposta nella casella che viene visualizzata.

   Puoi vedere gli utenti attivamente coinvolti nella conversazione o taggati in ogni risposta nella parte superiore del thread di aggiornamento. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto. Puoi anche assegnare tag a più utenti per includerli nella risposta.  Per assegnare tag a più utenti, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Facoltativo) Per includere nella risposta il testo di un aggiornamento precedente, fare clic sul pulsante **Altro** accanto all&#39;aggiornamento o alla risposta che si desidera citare, quindi fare clic su **Risposta preventivo**. Il testo dell&#39;aggiornamento precedente viene visualizzato nell&#39;area di input, contrassegnato da una linea grigia verticale.
1. (Facoltativo) Utilizza la formattazione, le emoticon, i collegamenti o le immagini come spiegato nella sezione &quot;Utilizzare il testo RTF in un aggiornamento di Workfront&quot; nell’articolo [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Clic **Rispondi** per salvare la risposta.

### Rispondere a un commento quando si utilizza la nuova esperienza di commento

Per informazioni sulle funzioni disponibili nella nuova esperienza di commento e sugli oggetti, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Passare all&#39;oggetto a cui si desidera aggiungere una risposta.
1. Clic **Aggiornamenti**, quindi fare clic su **Commenti** e trovare il commento o la risposta a cui si desidera rispondere.
1. (Facoltativo) Per includere nella risposta il testo di un aggiornamento precedente, fare clic sul pulsante **Altro** menu accanto all&#39;aggiornamento o alla risposta che si desidera citare <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>-->, quindi fai clic su **Risposta preventivo**. Il testo dell&#39;aggiornamento precedente viene visualizzato nell&#39;area di input, contrassegnato da una linea grigia verticale.
1. Clic **Rispondi**.

   Puoi vedere gli utenti attivamente coinvolti nella conversazione nella parte inferiore della sezione **Nuovo commento** e puoi aggiungerne altre o rimuovere quelle che non sono più pertinenti. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto. Puoi anche assegnare tag a più utenti per includerli nella risposta.  Per assegnare tag a più utenti, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Inizia a digitare la risposta e utilizza eventuali opzioni aggiuntive dalla barra degli strumenti Testo formattato. Per informazioni sull’utilizzo di Rich Text o di altre funzionalità di aggiornamento, consulta [Aggiorna lavoro](../updating-work-items-and-viewing-updates/update-work.md).

1. Clic **Invia** per salvare la risposta.

1. (Facoltativo) Fai clic su **Altro** menu ![](assets/more-menu.png) accanto all’aggiornamento <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>--> per ulteriori opzioni per gestire la risposta. Per ulteriori informazioni, consulta [Aggiorna lavoro](../updating-work-items-and-viewing-updates/update-work.md).


## Rispondere a un aggiornamento da una notifica e-mail

A seconda della configurazione delle notifiche e-mail, potresti ricevere una notifica e-mail quando viene effettuato un aggiornamento a determinati oggetti a cui hai accesso.

È possibile rispondere a un aggiornamento da una notifica e-mail nei modi seguenti:

* Rispondi all’e-mail ricevuta. L’e-mail di risposta viene aggiunta come risposta di Workfront al commento originale.
* Utilizza il pulsante Commento all’interno dell’e-mail per tornare a Workfront e rispondere all’aggiornamento nell’area Aggiornamenti.

Di seguito è riportato un esempio di notifica e-mail attivata in seguito a un aggiornamento effettuato nella scheda Aggiornamenti di un’attività:

![email.png](assets/email-350x202.png)

Per informazioni, consulta [Rispondi alle notifiche e-mail](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






