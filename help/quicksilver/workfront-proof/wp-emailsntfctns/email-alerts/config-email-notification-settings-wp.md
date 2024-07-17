---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configura le impostazioni delle notifiche e-mail in [!DNL Workfront Proof]
description: Le notifiche e-mail generate da Workfront Proof informano i collaboratori sulle recenti attività su bozze, ad esempio commenti, risposte o decisioni.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2049'
ht-degree: 0%

---

# Configura le impostazioni delle notifiche e-mail in [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Le notifiche e-mail informano i collaboratori sulle attività recenti relative alle bozze, ad esempio commenti, risposte o decisioni.

Puoi impostare le notifiche e-mail per i revisori nelle seguenti aree:

Le notifiche e-mail per i revisori possono essere impostate sulla pagina Nuova bozza, [!UICONTROL Nuova versione], e gestite nella sezione [!UICONTROL Flusso di lavoro] della pagina [!UICONTROL Dettagli bozza]. Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* Pagina Nuova bozza
* Pagina [!UICONTROL Nuova versione]
* La sezione [!UICONTROL Workflow] della pagina [!UICONTROL Dettagli bozza].

Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Ogni utente può anche impostare le proprie impostazioni di avviso e-mail, che vengono applicate automaticamente quando viene condivisa una bozza con lui, nel caso in cui i collaboratori abbiano le loro preferenze o gli amministratori dell’account abbiano i loro consigli sulla frequenza degli avvisi. Questo può essere impostato come valore predefinito della bozza nelle pagine dei dettagli degli utenti.

Ogni utente può anche impostare le proprie impostazioni di avviso e-mail, che verranno applicate automaticamente quando viene condivisa una bozza. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Queste impostazioni vengono consigliate quando gli utenti creano le bozze e aggiungono questi collaboratori. Tuttavia, si tratta solo di suggerimenti, che possono essere modificati in qualsiasi momento durante il processo di revisione e le modifiche si applicano a tutte le attività effettuate dopo la modifica. Le impostazioni predefinite della bozza vengono ignorate dalle impostazioni a livello di bozza.

Gli utenti con i profili [!UICONTROL Amministratore] o [!UICONTROL Amministratore fatturazione] possono impostare le impostazioni predefinite della bozza per altri utenti nel proprio account dall&#39;interno delle impostazioni account.

Per informazioni sui profili, consulta [Profili autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Standalone Workfront Proof</td> 
  </tr> 
</table>

+++

## Configura impostazioni bozza predefinite in impostazioni personali ([!DNL Workfront Proof] utenti)

È possibile configurare le impostazioni della bozza per le bozze create.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Fare clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni personali]**.

1. Fare clic sulla scheda **[!UICONTROL Impostazioni predefinite bozza]**.
1. Fare clic su **[!UICONTROL Impostazioni notifiche e-mail predefinite]** per espanderle.
1. Nell’elenco a discesa a destra delle due impostazioni seguenti, seleziona una delle opzioni illustrate nella tabella seguente.

   * **[!UICONTROL Avviso e-mail predefinito]**: influisce su ogni bozza condivisa con te. Questa impostazione può essere ignorata a livello di bozza.
   * **[!UICONTROL Avviso e-mail predefinito per i nuovi revisori ospiti]**: influisce sui revisori che non esistevano in precedenza come contatti nel tuo account.

   >[!NOTE]
   >
   >Se non si sceglie una delle opzioni seguenti, [!DNL Workfront Proof] invia un riepilogo giornaliero dell&#39;attività nelle bozze.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tutte le attività]</td> 
      <td>[!UICONTROL Workfront] invia un'e-mail al revisore ogni volta che viene eseguita un'attività sulla bozza, ad esempio un nuovo commento, una risposta o una nuova decisione. <p>Si tratta di un'ottima opzione per la persona che gestisce il processo di verifica, in quanto consente di visualizzare l'attività nel momento in cui si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Risponde ai miei commenti]</td> 
      <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.</p><p>Per informazioni sui commenti, vedere <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizzare e rispondere ai commenti della bozza</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio, un project manager) e che deve monitorare i progressi sulla bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisione finale]</td> 
      <td>[!DNL Workfront] invia un’e-mail quando l’ultimo approvatore sulla bozza ha preso la sua decisione.<p>Questo avviso viene spesso utilizzato dal progettista, che di solito non ha bisogno di partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve ricevere una notifica solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario [!UICONTROL]</td> 
      <td>[!DNL Workfront] invia ogni ora un'e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nel corso dell'ora.<p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. </p><p>Questo avviso è utile per avere una panoramica del progetto.</p><p>Un caso d’uso di esempio per questo riepilogo è un revisore senior che ha bisogno di una panoramica del progetto ma non ha bisogno di essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero di [!UICONTROL]</td> 
      <td>[!DNL Workfront] invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.</p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestire le notifiche per i commenti e le decisioni relative alle bozze</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.<p>L'impostazione predefinita del sistema è [!UICONTROL Riepilogo giornaliero], ovvero [!UICONTROL Non impostato]. Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Modificare uno dei seguenti elementi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Conferma e-mail quando le bozze sono pronte]</td> 
      <td>Specifica se desideri ricevere un’e-mail di [!UICONTROL Proof made] quando crei una bozza. Per ulteriori informazioni, vedere <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato delle e-mail inviate all'utente] </td> 
      <td> <p>Scegli tra e-mail in stile HTML ed e-mail in testo normale. </p> <p><b>NOTA</b></p>
      <p>Le impostazioni predefinite della bozza vengono sostituite dalle impostazioni a livello di bozza. Tuttavia, se le notifiche e-mail delle bozze sono disabilitate per l'intero account nelle impostazioni dell'account [!UICONTROL], nessun avviso e-mail verrà inviato ai collaboratori anche se l'avviso e-mail [!UICONTROL Disabled] non è selezionato nelle bozze.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **[!UICONTROL Impostazioni messaggio]**, modificare una delle impostazioni seguenti:

   | Modello di bozza | Descrizione |
   |---|---|
   | **[!UICONTROL Modello oggetto bozza]** | Vengono visualizzate le pagine Nuova bozza, Nuova versione, Messaggio e Promemoria. Può essere modificato prima dell’invio. |
   | **[!UICONTROL Modello di messaggio bozza]** | Vengono visualizzate le pagine Nuova bozza, Nuova versione, Messaggio e Promemoria. Può essere modificato prima dell’invio. |

## Modificare gli avvisi e-mail per un destinatario

È possibile modificare gli avvisi e-mail per un destinatario specifico in un&#39;azione batch.

1. Fai clic su **[!UICONTROL Contatti]** nel pannello di navigazione a sinistra.
1. Fai clic sul menu **[!UICONTROL Altro]** ![](assets/more-button-small.png) per il destinatario, quindi fai clic su **[!UICONTROL Visualizza dettagli membro]** nel menu a discesa.

1. Apri la sezione **[!UICONTROL Elementi condivisi]**.
1. Seleziona la casella di controllo a sinistra di ogni elemento per il quale desideri modificare l’avviso e-mail.
1. Fai clic su **[!UICONTROL Altro]** sopra l&#39;elenco degli elementi condivisi, quindi fai clic su **[!UICONTROL Modifica avviso e-mail]** nel menu a discesa.

1. Modifica l&#39;avviso e-mail, quindi fai clic su **[!UICONTROL Invia]**.

## Configurare le impostazioni predefinite della bozza per un utente

Se sei un amministratore di [!DNL Workfront Proof], puoi impostare le impostazioni predefinite della bozza per gli utenti nel tuo account.

1. Fare clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri la scheda **[!UICONTROL Utenti]**.
1. Apri il menu **[!UICONTROL Altro]** ![Altro_button_small.png](assets/more-button-small.png) a destra del nome dell&#39;utente.

1. Fare clic su **[!UICONTROL Visualizza dettagli utenti]** nel menu a discesa.
1. In **[!UICONTROL Impostazioni]**, fai clic su **[!UICONTROL Impostazioni predefinite avvisi e-mail]** per espanderlo.

1. Nell’elenco a discesa a destra delle due impostazioni seguenti, seleziona una delle opzioni illustrate nella tabella seguente:

   * **[!UICONTROL Avviso e-mail predefinito]**: influisce su ogni bozza condivisa con te. Questa impostazione può essere ignorata a livello di bozza.
   * **[!UICONTROL Avviso e-mail predefinito per i nuovi revisori ospiti]**: influisce sui revisori che non esistevano in precedenza come contatti nel tuo account.

   >[!NOTE]
   >
   >Se non scegli una delle seguenti opzioni per un utente, [!DNL Workfront Proof] invia agli utenti un riepilogo giornaliero sull&#39;attività nelle bozze.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Tutte le attività]</td>
      <td>[!DNL Workfront] invia un’e-mail al revisore ogni volta che si verifica un’attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione. <p>Si tratta di un'ottima opzione per la persona che gestisce il processo di verifica, in quanto consente di visualizzare l'attività nel momento in cui si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Risponde ai miei commenti]</td>
      <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.</p><p>Per informazioni sui commenti, vedere <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizzare e rispondere ai commenti della bozza</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio, un project manager) e che deve monitorare i progressi sulla bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisione finale]</td>
      <td>[!DNL Workfront] invia un’e-mail quando l’ultimo approvatore sulla bozza ha preso la sua decisione.<p>Questo avviso viene spesso utilizzato dal progettista, che di solito non ha bisogno di partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve ricevere una notifica solo al termine del processo di revisione.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Riepilogo orario [!UICONTROL]</td>
      <td>[!DNL Workfront] invia ogni ora un'e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nel corso dell'ora.<p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. </p><p>Questo avviso è utile per avere una panoramica del progetto.</p><p>Un caso d’uso di esempio per questo riepilogo è un revisore senior che ha bisogno di una panoramica del progetto ma non ha bisogno di essere informato immediatamente di tutte le attività sulla bozza.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Riepilogo giornaliero di [!UICONTROL]</td>
      <td>[!DNL Workfront] invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.</p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestire le notifiche per i commenti e le decisioni relative alle bozze</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.<p>L'impostazione predefinita del sistema è [!UICONTROL Riepilogo giornaliero], ovvero [!UICONTROL Non impostato]. Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.</p></td>
     </tr>
    </tbody>
   </table>

1. Nelle **[!UICONTROL impostazioni predefinite per gli avvisi e-mail]** rimanenti, modificare una delle seguenti impostazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Conferma e-mail quando le bozze sono pronte]</td> 
      <td>Specifica se desideri ricevere un’e-mail di [!UICONTROL Proof made] quando crei una bozza. Per ulteriori informazioni, vedere <a href="https://support.workfront.com/hc/en-us/article">E-mail [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato delle e-mail inviate all'utente] </td> 
      <td> <p>Scegli tra e-mail in stile HTML ed e-mail in testo normale. </p> <p><b>NOTA</b></p> <p>Le impostazioni predefinite della bozza vengono sostituite dalle impostazioni a livello di bozza. Tuttavia, se le notifiche e-mail delle bozze sono disabilitate per l'intero account nelle impostazioni dell'account [!UICONTROL], nessun avviso e-mail verrà inviato ai collaboratori anche se l'avviso e-mail [!UICONTROL Disabled] non è selezionato nelle bozze.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
