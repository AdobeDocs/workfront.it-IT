---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gestire le notifiche per i commenti e le decisioni relativi alle bozze
description: Quando lavori su una bozza, che tu sia un utente di Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere in merito ai commenti e alle decisioni prese sulla bozza. Per ulteriori informazioni, consulta Notifiche per commenti e decisioni relativi alla bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: b3fe63f7a332f50c7bac3bedee5db3bbbabd2b42
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 2%

---

# Gestire le notifiche per i commenti e le decisioni relativi alle bozze

Quando lavori su una bozza, che tu sia un utente di Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere in merito ai commenti e alle decisioni prese sulla bozza. Per ulteriori informazioni, consulta [Notifiche per i commenti della bozza e panoramica delle decisioni](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Queste notifiche sono diverse dagli avvisi e-mail che puoi ricevere sul flusso di una bozza tra i revisori e dalle impostazioni degli avvisi e-mail che puoi configurare in Workfront.

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

1. Apri la bozza per la quale desideri configurare le notifiche.
1. Se la barra degli strumenti sinistra non è visualizzata, fare clic sull&#39;icona **Menu** nell&#39;angolo superiore sinistro del visualizzatore bozze Web.

   ![icona_menu_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Nella barra degli strumenti a sinistra, fai clic sull&#39;icona **Impostazioni** ![Impostazioni_icona.png](assets/settings-icon.png) .

1. Nella sezione **Invia notifiche e-mail su**, seleziona l&#39;impostazione di notifica per questa bozza.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutte le attività</td> 
      <td>Viene inviata un’e-mail al revisore ogni volta che si verifica un’attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione.<br><p>Questa impostazione è consigliata alla persona che gestisce il processo di verifica, in quanto consente di visualizzare l’attività nel momento in cui si verifica. Gli utenti non ricevono un avviso e-mail relativo alla propria attività (ad esempio commenti, risposte o decisioni prese).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risposte ai miei commenti</td> 
      <td>Un messaggio e-mail viene inviato al revisore solo se qualcuno risponde direttamente al proprio commento (escludendo le risposte sui propri commenti).<p>Questa impostazione è consigliata per i clienti in modo che ricevano solo le notifiche delle risposte ai propri commenti e non per eventuali altri commenti aggiunti alla bozza, anche se possono ancora visualizzare tutti i commenti nel visualizzatore di bozze.</p>
      <p>Per informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizzare e rispondere ai commenti della bozza</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisioni</td> 
      <td>Un’e-mail viene inviata al revisore solo quando qualcuno prende una decisione.<br><p>Questo avviso e-mail può essere utile alla persona che gestisce il processo di approvazione in quanto consente alla persona che gestisce il processo di approvazione di monitorare lo stato della bozza e vedere quali utenti hanno preso la loro decisione.<br></p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione finale</td> 
      <td>Viene inviata un’e-mail quando viene presa la decisione finale sulla bozza.<br><p>Questo avviso viene spesso utilizzato dalla finestra di progettazione perché la finestra di progettazione non deve partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario</td> 
      <td>Ogni ora viene inviata un’e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nell’ultima ora.<br><p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. Se non è presente alcuna attività da parte di altri utenti, non viene inviata alcuna e-mail.<br></p><p>Questo avviso è un buon modo per visualizzare una panoramica del progetto mentre procede.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero</td> 
      <td>(impostazione predefinita): ogni giorno viene inviata un’e-mail con tutti i commenti, le risposte e le decisioni elencati. Questo messaggio viene inviato solo nei giorni in cui è presente attività oltre alla tua.<br><p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nessuna e-mail</td> 
      <td>Non vengono inviati avvisi e-mail.<br><p>Questa impostazione è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.</p><p>Nota: <p>Questa opzione disattiva solo gli avvisi e-mail relativi a commenti e decisioni relativi alla bozza; non disattiva gli avvisi e-mail che puoi ricevere sul flusso di una bozza, ad esempio l’e-mail Nuova bozza o Bozza tardiva. Per ulteriori informazioni, consulta i seguenti articoli: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">E-mail nuova bozza</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail nuova versione</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail per bozza tardiva</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail Proof Made</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
