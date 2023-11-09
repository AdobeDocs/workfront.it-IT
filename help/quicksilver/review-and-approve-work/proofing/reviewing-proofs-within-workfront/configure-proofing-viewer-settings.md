---
product-area: documents;setup
navigation-topic: review-a-proof
title: Configurare le impostazioni del visualizzatore di verifica
description: È possibile configurare le impostazioni sia per Web Proofing Viewer che per Desktop Proofing Viewer.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 0%

---

# Configurare le impostazioni del visualizzatore di verifica

È possibile configurare le impostazioni seguenti sia per il visualizzatore bozze Web che per il visualizzatore bozze desktop:

* Indica se le marcature e i pin dei commenti vengono visualizzati sulle bozze.
* Indica se gli strumenti di markup vengono visualizzati nella parte superiore del visualizzatore di bozze o in un menu a discesa.
* Quali notifiche e-mail ricevi come revisore sulla bozza aperta.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

È possibile configurare le seguenti impostazioni per il Visualizzatore bozze desktop:

* Come desideri che i collegamenti all’interno del contenuto del sito web vengano aperti nel Visualizzatore.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Che cosa accade quando si fa clic su un collegamento impostato per l&#39;apertura in una nuova scheda o finestra del browser?
* Cancella i dati della cache che potrebbero essere salvati con la bozza che stai visualizzando per consentire la visualizzazione nel Visualizzatore di contenuto come i pop-up (che possono essere bloccati dai dati della cache del browser).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza disponibile, contattare l&#39;amministratore Workfront o Workfront Proof.

## Configurare le impostazioni del visualizzatore di verifica

Per configurare le impostazioni del visualizzatore di verifica:

1. Aprire il visualizzatore bozze Web o il visualizzatore bozze desktop in uno dei modi seguenti:

   * Se esegui una bozza in Adobe Workfront, passa a un elenco di documenti contenente la bozza che desideri visualizzare, passa il puntatore del mouse sul documento e fai clic su **Apri bozza**.
   * Se utilizzi Workfront Proof, fai clic su **Vai alla bozza** icona per la bozza nel dashboard o in un elenco delle visualizzazioni ![](assets/go-to-proof-blue-icon.png).

1. Se la barra degli strumenti a sinistra non è visualizzata, fare clic su **Menu** nell&#39;angolo superiore sinistro del visualizzatore bozze Web.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Nella barra degli strumenti a sinistra, fai clic su **Impostazioni** icona ![](assets/settings-icon-in-pv.png).

1. Configura uno dei seguenti elementi **Impostazioni** quella visualizzazione.

   Le impostazioni disponibili possono variare a seconda del tipo di bozza aperto.

   * **Mostra markup** (sempre disponibile in Web Proofing Viewer e Desktop Proofing Viewer): questi sono i segni di commento aggiunti dai revisori alle bozze quando utilizzano gli strumenti di markup. Se li disattivate, potete comunque visualizzarli quando fate clic su un commento nell&#39;elenco dei commenti.

     Questa impostazione ha effetto su tutte le bozze aperte.

   * **Mostra pin** (sempre disponibile in Web Proofing Viewer e Desktop Proofing Viewer): si tratta dei pin numerati che i revisori aggiungono alle bozze quando utilizzano gli strumenti di markup. Indicano dove e in quale ordine il revisore ha aggiunto i commenti. Se li disattivate, potete comunque visualizzarli quando fate clic su un commento nell&#39;elenco dei commenti.

     Questa impostazione ha effetto su tutte le bozze aperte.

   * **Utilizzare strumenti di markup espansi** (sempre disponibile in Web Proofing Viewer e Desktop Proofing Viewer): per impostazione predefinita, le opzioni dello strumento di markup vengono visualizzate nella parte superiore del visualizzatore di bozze. È possibile configurarli per la visualizzazione in un menu verticale che si apre solo quando si fa clic su di esso.

     Questa impostazione è attiva per tutte le bozze aperte.

   * **Inviami notifiche e-mail su** (sempre disponibile in Web Proofing Viewer e Desktop Proofing Viewer): fare clic su una delle opzioni seguenti. Questa impostazione ha effetto solo sulla bozza aperta. Per ulteriori informazioni, consulta [Panoramica delle notifiche per commenti e decisioni relativi alla bozza](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Tutte le attività</td> 
        <td>Workfront invia un’e-mail al revisore ogni volta che si verifica un’attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione. <p>Si tratta di un'ottima opzione per la persona che gestisce il processo di verifica, in quanto consente di visualizzare l'attività nel momento in cui si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Risposte ai miei commenti</td> 
        <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.</p><p>Per informazioni sui commenti, vedi <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e rispondi ai commenti della bozza</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisioni</td> 
        <td>Workfront invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio, un project manager) e che deve monitorare i progressi sulla bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisione finale</td> 
        <td>Workfront invia un’e-mail quando l’ultimo approvatore della bozza prende la sua decisione.<p>Questo avviso viene spesso utilizzato dal progettista, che di solito non ha bisogno di partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve ricevere una notifica solo al termine del processo di revisione.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Riepilogo orario</td> 
        <td>Workfront invia ogni ora un messaggio e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nel corso dell’ora.<p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. </p><p>Questo avviso è utile per avere una panoramica del progetto.</p><p>Un caso d’uso di esempio per questo riepilogo è un revisore senior che ha bisogno di una panoramica del progetto ma non ha bisogno di essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Riepilogo giornaliero</td> 
        <td>Workfront invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.</p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestire le notifiche per i commenti e le decisioni relativi alle bozze</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nessuna e-mail</td> 
        <td>Workfront non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.<p>L'impostazione predefinita del sistema è Riepilogo giornaliero (visualizzato anche come Non impostato). Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Quando si fa clic sui collegamenti ipertestuali all’interno di una bozza** (disponibile solo nel Visualizzatore bozze desktop): selezionare un&#39;opzione per specificare cosa accade nel Visualizzatore bozze desktop quando si fa clic su un collegamento impostato per l&#39;apertura in una nuova scheda o finestra del browser.

     Questa impostazione è attiva per tutte le bozze interattive aperte.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Apri nel visualizzatore di bozze</td> 
        <td>I collegamenti si aprono sempre all’interno del Visualizzatore bozze desktop e puoi verificare il contenuto collegato. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Apri nel browser</td> 
        <td>I collegamenti si aprono sempre nel browser, non in un visualizzatore di bozze. Impossibile verificare il contenuto collegato.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Chiedi ogni volta</td> 
        <td> <p>Ogni volta viene richiesto se si desidera aprire il collegamento nel Visualizzatore bozze desktop o nel browser. Se apri il collegamento all’interno del Visualizzatore bozze desktop, puoi verificare il contenuto collegato. Se apri il collegamento nel browser, non potrai verificare il contenuto collegato.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_always_ask.png" style="width: 350;height: 243;"> </p> <p>Questa impostazione ha effetto solo sulla bozza aperta.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Cancella cache**: cancella i dati della cache del browser che potrebbero essere salvati con una bozza interattiva che stai visualizzando. In questo modo, nel Visualizzatore bozze desktop è possibile visualizzare contenuti quali i popup (che possono essere bloccati dai dati della cache del browser).

     I dati cancellati includono la cache HTTP (ad esempio le immagini da riutilizzare dopo il prossimo aggiornamento della pagina) e la cache dei dati di archiviazione web (ad esempio i cookie e i dati che identificano gli utenti).

     Questa impostazione ha effetto solo sulla bozza aperta.
