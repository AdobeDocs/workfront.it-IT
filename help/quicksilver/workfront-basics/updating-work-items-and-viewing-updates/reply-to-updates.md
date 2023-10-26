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
source-git-commit: 97a89293989fd5dcc3ba40dd12ad0e1cf97d69ff
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# Rispondi agli aggiornamenti

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

>[!IMPORTANT]
>
>Attualmente stiamo riprogettando l’esperienza di aggiunta di commenti in Adobe Workfront.
>
>A seconda degli oggetti per i quali accedi all’esperienza di commento, per la sezione Aggiornamenti potresti visualizzare le seguenti funzionalità:
>* La nuova esperienza
>* L’esperienza legacy
>* La nuova esperienza e quella legacy
>
>Per ulteriori informazioni sulla nuova esperienza di commento e sulla sua disponibilità, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nuova esperienza di aggiunta di commenti è disponibile solo per la sezione Aggiornamenti degli oggetti di Workfront e non è disponibile quando si accede agli oggetti dalle aree seguenti:
>
> * Home
> * Pannello Riepilogo negli elenchi
> * Pannello Riepilogo nelle schede orario

Quando qualcuno risponde a un commento o a un aggiornamento di sistema su un oggetto di lavoro, la risposta viene visualizzata nel thread di comunicazione nella sezione Aggiornamenti dell’oggetto.

>[!IMPORTANT]
>
>Nella nuova esperienza di inserimento di commenti non è possibile rispondere agli aggiornamenti di sistema. Per ulteriori informazioni, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

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

### Rispondere a un commento quando si utilizza la nuova esperienza di commento

Per informazioni sulle funzioni disponibili nella nuova esperienza di commento e sugli oggetti, consulta [Nuova esperienza di commento](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Passare all&#39;oggetto a cui si desidera aggiungere una risposta.
1. Clic **Aggiornamenti**, quindi fare clic su **Commenti** e trovare il commento o la risposta a cui si desidera rispondere.
1. (Facoltativo) Per includere nella risposta il testo di un aggiornamento precedente, fare clic sul pulsante **Altro** nell’angolo superiore destro del commento a cui desideri rispondere, quindi fai clic su **Risposta preventivo**. Il testo dell&#39;aggiornamento precedente viene visualizzato nell&#39;area di input, contrassegnato da una linea grigia verticale.
1. Clic **Rispondi**.

   ![](assets/reply-to-update-empty-box.png)

   Puoi vedere gli utenti attivamente coinvolti nella conversazione nella parte inferiore della sezione **Aggiungi risposta...** e puoi aggiungerne altre o rimuovere quelle che non sono più pertinenti. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto. Puoi anche assegnare tag a più utenti per includerli nella risposta.  Per assegnare tag a più utenti, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   Per aggiungere ulteriori risposte a una risposta esistente, puoi iniziare a digitare nella **Aggiungi risposta...** o fai clic su **Rispondi** sul commento originale. La risposta viene aggiunta alla fine del thread.

1. Inizia a digitare la risposta e utilizza eventuali opzioni aggiuntive dalla barra degli strumenti Testo formattato. Per informazioni sull’utilizzo di Rich Text o di altre funzionalità di aggiornamento, consulta [Aggiorna lavoro](../updating-work-items-and-viewing-updates/update-work.md).

1. Clic **Invia** per salvare la risposta.

1. (Facoltativo) Fai clic su **Altro** menu ![](assets/more-menu.png) nell’angolo superiore destro del commento a cui desideri rispondere per ulteriori opzioni di gestione della risposta. Per ulteriori informazioni, consulta [Aggiorna lavoro](../updating-work-items-and-viewing-updates/update-work.md).

### Rispondi a un aggiornamento o rispondi nella sezione Aggiornamenti legacy

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

## Rispondere a un aggiornamento da una notifica e-mail

A seconda della configurazione delle notifiche e-mail, potresti ricevere una notifica e-mail quando viene effettuato un aggiornamento a determinati oggetti a cui hai accesso.

È possibile rispondere a un aggiornamento da una notifica e-mail nei modi seguenti:

* Rispondi all’e-mail ricevuta. L’e-mail di risposta viene aggiunta come risposta di Workfront al commento originale.
* Utilizza il pulsante Commento all’interno dell’e-mail per tornare a Workfront e rispondere all’aggiornamento nell’area Aggiornamenti.

Di seguito è riportato un esempio di notifica e-mail attivata in seguito a un aggiornamento effettuato nella scheda Aggiornamenti di un’attività:

![email.png](assets/email-350x202.png)

Per informazioni, consulta [Rispondi alle notifiche e-mail](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






