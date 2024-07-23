---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gestire le notifiche per i commenti e le decisioni relativi alle bozze
description: Quando lavori su una bozza, che tu sia un utente di Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere in merito ai commenti e alle decisioni prese sulla bozza. Per ulteriori informazioni, consulta Notifiche per commenti e decisioni relativi alla bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 1%

---

# Gestire le notifiche per i commenti e le decisioni relativi alle bozze

Quando lavori su una bozza, che tu sia un utente di Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere in merito ai commenti e alle decisioni prese sulla bozza. Per ulteriori informazioni, consulta [Notifiche per i commenti della bozza e panoramica delle decisioni](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Queste notifiche sono diverse dagli avvisi e-mail che puoi ricevere sul flusso di una bozza tra i revisori. Sono anche diverse dalle impostazioni degli avvisi e-mail che puoi configurare in Workfront. 

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Gestire le notifiche per i commenti e le decisioni relativi alle bozze

1. Apri la bozza per la quale desideri configurare le notifiche che riceverai.
1. Se la barra degli strumenti a sinistra non è visualizzata, fare clic sull&#39;icona **Menu** nell&#39;angolo superiore sinistro del visualizzatore bozze Web.

   ![icona_menu_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Nella barra degli strumenti a sinistra, fai clic sull&#39;icona **Impostazioni**. ![icona_impostazioni.png](assets/settings-icon.png)

1. In **Invia notifiche e-mail su**, fare clic sull&#39;impostazione desiderata per la bozza.

   L’impostazione selezionata rimane attiva solo per la bozza aperta.

   Il valore predefinito di sistema è **Riepilogo giornaliero**. Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutte le attività</td> 
      <td>Viene inviata un’e-mail al revisore ogni volta che si verifica un’attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione.<br><p>Si tratta di un'ottima opzione per la persona che gestisce il processo di verifica, in quanto consente di visualizzare l'attività nel momento in cui si verifica. Gli utenti non ricevono un avviso e-mail relativo alla propria attività (ad esempio, commenti, risposte e decisioni prese).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risposte ai miei commenti</td> 
      <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.<br></p><p>Per informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizzare e rispondere ai commenti della bozza</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisioni</td> 
      <td>Un’e-mail viene inviata al revisore solo quando qualcuno prende una decisione.<br><p>Questo avviso e-mail può essere utile per la persona che gestisce il processo di approvazione (ad esempio, un project manager) perché consente alla persona che gestisce il processo di approvazione di monitorare lo stato di avanzamento della bozza e di vedere quali utenti hanno preso la loro decisione.<br></p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione finale</td> 
      <td>Viene inviata un’e-mail quando viene presa la decisione finale sulla bozza (quando l’ultimo approvatore ha preso la sua decisione).<br><p>Questo avviso viene spesso utilizzato dalla finestra di progettazione perché la finestra di progettazione non deve partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.<br></p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve ricevere una notifica solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario</td> 
      <td>Ogni ora viene inviata un’e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nell’ultima ora.<br><p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. Se non è presente alcuna attività da parte di altri utenti, non viene inviata alcuna e-mail.<br></p><p>Questo avviso è utile per avere una panoramica del progetto.<br></p><p>Un caso d’uso di esempio per questo riepilogo è un revisore senior che ha bisogno di una panoramica del progetto ma non ha bisogno di essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero</td> 
      <td>(impostazione predefinita): ogni giorno viene inviata un’e-mail con tutti i commenti, le risposte e le decisioni elencati. Un’e-mail viene inviata solo nei giorni in cui è presente attività oltre alla tua.<br><p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.<br></p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nessuna e-mail</td> 
      <td>Non vengono inviati avvisi e-mail.<br><p>Questa impostazione è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere informata di eventuali modifiche.</p><p>Nota: <p>Questa opzione disattiva solo gli avvisi e-mail che puoi ricevere relativamente ai commenti e alle decisioni sulle bozze. Non disattiva gli avvisi e-mail che puoi ricevere sul flusso di una bozza, ad esempio l’e-mail New Proof (Nuova bozza) o Late Proof (Bozza tardiva). Per ulteriori informazioni sugli avvisi e-mail relativi al flusso di una bozza, consulta i seguenti articoli: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">E-mail nuova bozza</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail nuova versione</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail per bozza tardiva</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail Proof Made</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
