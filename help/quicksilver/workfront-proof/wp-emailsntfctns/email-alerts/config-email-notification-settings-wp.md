---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configura le impostazioni di notifica e-mail in [!DNL Workfront Proof]
description: Le notifiche e-mail informano i collaboratori sulle recenti attività sulle bozze, ad esempio commenti, risposte, decisioni.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1995'
ht-degree: 0%

---

# Configura le impostazioni di notifica e-mail in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Le notifiche e-mail informano i collaboratori sulle recenti attività sulle bozze, ad esempio commenti, risposte, decisioni.

Le notifiche e-mail per i revisori possono essere impostate nella pagina Nuova bozza , [!UICONTROL Nuova versione] e gestiti nella [!UICONTROL Flusso di lavoro] della sezione [!UICONTROL Dettagli della bozza] pagina. Per ulteriori informazioni, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Ogni utente può anche impostare le proprie impostazioni di avviso e-mail che verranno applicate automaticamente quando una bozza viene condivisa con loro. Se i collaboratori hanno le loro preferenze, o gli amministratori dell&#39;account hanno le loro raccomandazioni sulla frequenza degli avvisi. Può essere impostato come predefinito di bozza nelle pagine dei dettagli degli utenti.

>[!NOTE]
>
>Queste impostazioni vengono suggerite quando gli utenti creano le bozze e aggiungono questi collaboratori. Tuttavia, questi sono solo suggerimenti, in modo che possano essere adeguati in qualsiasi momento durante il processo di revisione e le modifiche si applicano a tutta l&#39;attività effettuata dopo la modifica. Le impostazioni predefinite della bozza vengono sostituite dalle impostazioni a livello di bozza.

Utenti con [!UICONTROL Amministratore] o [!UICONTROL Amministratore fatturazione] i profili possono inoltre impostare le impostazioni predefinite della bozza per altri utenti nel loro account dall’interno delle impostazioni account.

Per informazioni sui profili, consulta [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Configura le impostazioni predefinite della bozza nelle impostazioni personali ([!DNL Workfront Proof] solo utenti)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Modificare gli avvisi e-mail per un destinatario](#change-email-alerts-for-a-recipient)
* [Configurare i valori predefiniti della bozza per un utente](#configure-proof-defaults-for-a-user)

## Configura le impostazioni predefinite della bozza nelle impostazioni personali ([!DNL Workfront Proof] solo utenti)

Puoi configurare le impostazioni di bozza per le bozze create.

Per informazioni sulle impostazioni di bozza, consulta [!DNL Workfront] amministratore o [!DNL Workfront Proof] l’amministratore può effettuare la configurazione, consulta .

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni personali]**.

1. Fai clic sul pulsante **[!UICONTROL Valori predefiniti di correzione]** scheda .
1. Fai clic su **[!UICONTROL Impostazioni predefinite delle notifiche e-mail]** per espanderlo.
1. Nell’elenco a discesa a destra delle due impostazioni seguenti, selezionare una delle opzioni illustrate nella tabella seguente.

   * **[!UICONTROL Avviso e-mail predefinito]**: Influisce su ogni prova condivisa con te. È possibile ignorare questa impostazione a livello di bozza.
   * **[!UICONTROL Avviso e-mail predefinito per i nuovi revisori ospiti]**: Influisce sui revisori che non esistevano in precedenza come contatti nel tuo account.

   >[!NOTE]
   >
   >Se non si sceglie una delle seguenti opzioni, [!DNL Workfront Proof] invia un riepilogo giornaliero dell’attività sulle bozze.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tutte le attività]</td> 
      <td>[!UICONTROL Workfront] invia un’e-mail al revisore ogni volta che vi è attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione. <p>Questa è una grande opzione per la persona che gestisce il processo di correzione perché consente loro di vedere l'attività mentre si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Risposte ai miei commenti]</td> 
      <td>Un’e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte dai propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non viene informato.<p>Questa impostazione è consigliata per i clienti sulla prova in modo che non siano informati di altri commenti sulla prova e siano informati solo delle risposte alle proprie osservazioni.</p><p>Sebbene i revisori con questa impostazione di avviso e-mail non siano informati di altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di correzione.</p><p>Per informazioni sui commenti, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e risponde ai commenti di prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisioni]</td> 
      <td>[!DNL Workfront] invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio un project manager) e deve monitorare l’avanzamento della bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che non selezioni un’opzione di conferma e-mail quando invii la tua decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisione finale]</td> 
      <td>[!DNL Workfront] invia un'e-mail quando l'ultimo approvatore della bozza ha preso la sua decisione.<p>Questo avviso viene spesso utilizzato dal designer, che di solito non deve prendere parte alla discussione di revisione effettiva. Al momento della decisione finale, il progettista viene informato e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve essere informato solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Riepilogo orario]</td> 
      <td>[!DNL Workfront] invia un'e-mail al revisore ogni ora con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificate nell'ora.<p>L’e-mail viene inviata solo quando l’attività oltre alla tua si verifica entro l’ora passata. </p><p>Questo avviso è un buon modo per vedere una panoramica del progetto.</p><p>Un esempio di utilizzo per questo riepilogo è un revisore senior che necessita di una panoramica del progetto ma non deve essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Riepilogo giornaliero]</td> 
      <td>[!DNL Workfront] invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sopraffatto da numerosi aggiornamenti durante tutto il giorno.</p><p>Un esempio di utilizzo per questo riepilogo è un responsabile del reparto che desidera monitorare l'avanzamento complessivo del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestione delle notifiche per commenti e decisioni di bozza</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Nessun messaggio e-mail]</td> 
      <td>[!DNL Workfront] non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una prova solo a scopo di riferimento e non deve essere informata di eventuali modifiche.<p>L’impostazione predefinita del sistema è [!UICONTROL Daily summary] (visto anche come [!UICONTROL Not Set]). Se tu o i tuoi revisori non apporti altre modifiche, tutte le tue bozze avranno questa impostazione.</p></td> 
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
      <td>Specifica se desideri ricevere un messaggio e-mail [!UICONTROL Proof made] al momento di creare una bozza. Per ulteriori informazioni, consulta <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail di [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato delle e-mail inviate all’utente]</strong> </td> 
      <td> <p>Scegli tra e-mail di stile HTML ed e-mail di testo normale. </p> <p>Nota:  Le impostazioni predefinite per la correzione dei dati vengono sostituite dalle impostazioni a livello di bozza. Tuttavia, se le notifiche e-mail di bozza sono disabilitate per l’intero account nelle impostazioni dell’account , non verranno inviati avvisi e-mail ai collaboratori anche se l’avviso e-mail Disabilitato non è selezionato nelle bozze.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Sotto **[!UICONTROL Impostazioni messaggio]**, modifica uno dei seguenti elementi:

   | **[!UICONTROL Modello del soggetto di prova]** | Viene visualizzata nella pagina Nuova bozza, Nuova versione, Messaggio e Promemoria . Può essere modificato prima dell’invio. |
   |---|---|
   | **[!UICONTROL Modello di messaggio di bozza]** | Viene visualizzata nella pagina Nuova bozza, Nuova versione, Messaggio e Promemoria . Può essere modificato prima dell’invio. |

   {style="table-layout:auto"}

## Modificare gli avvisi e-mail per un destinatario

Puoi modificare gli avvisi e-mail per un particolare destinatario in un’azione batch.

1. Fai clic su **[!UICONTROL Contatti]** nel pannello di navigazione a sinistra.
1. Fai clic sul pulsante **[!UICONTROL Altro]** (tre punti) menu per il destinatario, quindi fai clic su **[!UICONTROL Visualizza dettagli membro]** nel menu a discesa .

1. Apri **[!UICONTROL Elementi condivisi]** sezione .
1. Seleziona la casella di controllo a sinistra di ogni elemento per il quale desideri modificare l’avviso e-mail.
1. Fai clic su **[!UICONTROL Altro]** sopra l&#39;elenco degli elementi condivisi, quindi fai clic su **[!UICONTROL Modifica avviso e-mail]** nel menu a discesa .

1. Modifica l’avviso e-mail, quindi fai clic su **[!UICONTROL Invia]**.

## Configurare i valori predefiniti della bozza per un utente

Se sei un [!DNL Workfront Proof] amministratore, puoi impostare le impostazioni predefinite della bozza per gli utenti nel tuo account.

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**.

1. Apri **[!UICONTROL Utenti]** scheda .
1. Apri **[!UICONTROL Altro]** a destra del nome dell&#39;utente. ![Altro_pulsante_piccolo.png](assets/more-button-small.png)

1. Fai clic su **[!UICONTROL Visualizzare i dettagli degli utenti]** nel menu a discesa .
1. Sotto **[!UICONTROL Impostazioni]**, fai clic su **[!UICONTROL Impostazioni predefinite avvisi e-mail]** per espanderlo.

1. Nell’elenco a discesa a destra delle due impostazioni seguenti, seleziona una delle opzioni illustrate nella tabella seguente:

   * **[!UICONTROL Avviso e-mail predefinito]**: Influisce su ogni prova condivisa con te. È possibile ignorare questa impostazione a livello di bozza.
   * **[!UICONTROL Avviso e-mail predefinito per i nuovi revisori ospiti]**: Influisce sui revisori che non esistevano in precedenza come contatti nel tuo account.

   >[!NOTE]
   >
   >Se non scegli una delle seguenti opzioni per un utente, [!DNL Workfront Proof] invia agli utenti un riepilogo giornaliero dell’attività sulle relative bozze.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Tutte le attività]</td>
      <td>[!DNL Workfront] invia un’e-mail al revisore ogni volta che vi è un’attività sulla bozza, ad esempio un nuovo commento, una risposta o una decisione. <p>Questa è una grande opzione per la persona che gestisce il processo di correzione perché consente loro di vedere l'attività mentre si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Risposte ai miei commenti]</td>
      <td>Un’e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte dai propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non viene informato.<p>Questa impostazione è consigliata per i clienti sulla prova in modo che non siano informati di altri commenti sulla prova e siano informati solo delle risposte alle proprie osservazioni.</p><p>Sebbene i revisori con questa impostazione di avviso e-mail non siano informati di altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di correzione.</p><p>Per informazioni sui commenti, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e risponde ai commenti di prova</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisioni]</td>
      <td>[!DNL Workfront] invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio un project manager) e deve monitorare l’avanzamento della bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che non selezioni un’opzione di conferma e-mail quando invii la tua decisione.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisione finale]</td>
      <td>[!DNL Workfront] invia un'e-mail quando l'ultimo approvatore della bozza ha preso la sua decisione.<p>Questo avviso viene spesso utilizzato dal designer, che di solito non deve prendere parte alla discussione di revisione effettiva. Al momento della decisione finale, il progettista viene informato e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve essere informato solo al termine del processo di revisione.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Riepilogo orario]</td>
      <td>[!DNL Workfront] invia un'e-mail al revisore ogni ora con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificate nell'ora.<p>L’e-mail viene inviata solo quando l’attività oltre alla tua si verifica entro l’ora passata. </p><p>Questo avviso è un buon modo per vedere una panoramica del progetto.</p><p>Un esempio di utilizzo per questo riepilogo è un revisore senior che necessita di una panoramica del progetto ma non deve essere informato immediatamente di tutte le attività sulla bozza.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Riepilogo giornaliero]</td>
      <td>[!DNL Workfront] invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sopraffatto da numerosi aggiornamenti durante tutto il giorno.</p><p>Un esempio di utilizzo per questo riepilogo è un responsabile del reparto che desidera monitorare l'avanzamento complessivo del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestione delle notifiche per commenti e decisioni di bozza</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Nessun messaggio e-mail]</td>
      <td>[!DNL Workfront] non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una prova solo a scopo di riferimento e non deve essere informata di eventuali modifiche.<p>L’impostazione predefinita del sistema è [!UICONTROL Daily summary] (visto anche come [!UICONTROL Not Set]). Se tu o i tuoi revisori non apporti altre modifiche, tutte le tue bozze avranno questa impostazione.</p></td>
     </tr>
    </tbody>
   </table>

1. Nel resto **[!UICONTROL Impostazioni predefinite avvisi e-mail]**, modifica uno dei seguenti elementi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Conferma e-mail quando le bozze sono pronte]</td> 
      <td>Specifica se desideri ricevere un messaggio e-mail [!UICONTROL Proof made] al momento di creare una bozza. Per ulteriori informazioni, consulta <a href="https://support.workfront.com/hc/en-us/article">L’E-Mail [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato delle e-mail inviate all’utente]</strong> </td> 
      <td> <p>Scegli tra e-mail di stile HTML ed e-mail di testo normale. </p> <p>Nota:  Le impostazioni predefinite per la correzione dei dati vengono sostituite dalle impostazioni a livello di bozza. Tuttavia, se le notifiche e-mail di bozza sono disabilitate per l’intero account nelle impostazioni dell’account , non verranno inviati avvisi e-mail ai collaboratori anche se l’avviso e-mail Disabilitato non è selezionato nelle bozze.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
