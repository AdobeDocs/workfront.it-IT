---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gestione delle notifiche per commenti e decisioni di bozza
description: Quando lavori su una bozza, che tu sia un utente Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere sui commenti e sulle decisioni prese sulla bozza. Per ulteriori informazioni, consulta Notifiche per i commenti e le decisioni della bozza Panoramica.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# Gestione delle notifiche per commenti e decisioni di bozza

Quando lavori su una bozza, che tu sia un utente Adobe Workfront o un collaboratore esterno, puoi specificare quali notifiche e-mail desideri ricevere sui commenti e sulle decisioni prese sulla bozza. Per ulteriori informazioni, consulta [Panoramica delle notifiche per commenti e decisioni di prova](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Queste notifiche sono diverse dagli avvisi e-mail che puoi ricevere sul flusso di una bozza tra i revisori. Sono inoltre diverse dalle impostazioni di avviso e-mail che puoi configurare in Workfront. 

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Gestione delle notifiche per commenti e decisioni di bozza

1. Apri la bozza per la quale vuoi configurare le notifiche che riceverai.
1. Se la barra degli strumenti a sinistra non viene visualizzata, fai clic sul pulsante **Menu** nell’angolo in alto a sinistra del visualizzatore per correzione Web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Nella barra degli strumenti a sinistra, fai clic sul pulsante **Impostazioni** icona. ![Settings_icon.png](assets/settings-icon.png)

1. Sotto **Inviami notifiche e-mail su**, fai clic sull’impostazione desiderata per la bozza.

   L’impostazione selezionata rimane attiva solo per la bozza aperta.

   Il valore predefinito del sistema è **Riepilogo giornaliero**. Se tu o i tuoi revisori non apporti altre modifiche, tutte le tue bozze avranno questa impostazione.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutte le attività</td> 
      <td>Un messaggio e-mail viene inviato al revisore ogni volta che vi è attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione.<br><p>Questa è una grande opzione per la persona che gestisce il processo di correzione perché consente loro di vedere l'attività mentre si verifica. Gli utenti non ricevono un avviso e-mail relativo alla propria attività (ad esempio, commenti, risposte e decisioni prese).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risposte ai miei commenti</td> 
      <td>Un’e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte dai propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non viene informato.<p>Questa impostazione è consigliata per i clienti sulla prova in modo che non siano informati di altri commenti sulla prova e siano informati solo delle risposte alle proprie osservazioni.</p><p>Sebbene i revisori con questa impostazione di avviso e-mail non siano informati di altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di correzione.<br></p><p>Per informazioni consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e risponde ai commenti di prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisioni</td> 
      <td>Un messaggio e-mail viene inviato al revisore solo quando qualcuno prende una decisione.<br><p>Questo avviso e-mail può essere utile per la persona che gestisce il processo di approvazione (ad esempio un project manager) perché consente alla persona che gestisce il processo di approvazione di monitorare l’avanzamento della bozza e di vedere quali utenti hanno preso la loro decisione.<br></p><p>Non riceverai una notifica della tua decisione a meno che non selezioni un’opzione di conferma e-mail quando invii la tua decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione finale</td> 
      <td>Viene inviata un'e-mail quando viene presa la decisione finale sulla prova (quando l'ultimo approvatore sulla prova ha preso la sua decisione).<br><p>Questo avviso viene spesso utilizzato dal designer perché il designer non deve partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista viene informato e può quindi intervenire su eventuali modifiche necessarie.<br></p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve essere informato solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario</td> 
      <td>Ogni ora viene inviata un’e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nell’ultima ora.<br><p>L’e-mail viene inviata solo quando l’attività oltre alla tua si verifica entro l’ora passata. Se non esiste alcuna attività da parte di altri utenti, non viene inviata alcuna e-mail.<br></p><p>Questo avviso è un buon modo per vedere una panoramica del progetto.<br></p><p>Un esempio di utilizzo per questo riepilogo è un revisore senior che necessita di una panoramica del progetto ma non deve essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero</td> 
      <td>(Impostazione predefinita): Viene inviata ogni giorno un’e-mail con tutti i commenti, le risposte e le decisioni elencate. Un’e-mail viene inviata solo nei giorni in cui è presente un’attività oltre alla tua.<br><p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sopraffatto da numerosi aggiornamenti durante tutto il giorno.<br></p><p>Un esempio di utilizzo per questo riepilogo è un responsabile del reparto che desidera monitorare l'avanzamento complessivo del progetto.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nessuna e-mail</td> 
      <td>Non vengono inviati avvisi e-mail.<br><p>Questa impostazione è utile per una persona che viene aggiunta a una prova solo a scopo di riferimento e non deve essere informata di eventuali modifiche.</p><p>Nota: <p>Questa opzione disattiva solo gli avvisi e-mail che possono essere ricevuti su commenti e decisioni di bozza. Non disattiva gli avvisi e-mail che puoi ricevere sul flusso di una bozza, ad esempio Nuova bozza o Prova in ritardo. Per ulteriori informazioni sugli avvisi e-mail relativi al flusso di una bozza, vedi i seguenti articoli: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nuova e-mail a prova di</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail sulla nuova versione</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail a prova di ritardo</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail di bozza creata</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
