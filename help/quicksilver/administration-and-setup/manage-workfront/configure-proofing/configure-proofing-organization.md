---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare le impostazioni di bozza per l’organizzazione
description: In qualità di amministratore di Adobe Workfront o di Workfront Proof, puoi personalizzare le impostazioni predefinite della bozza per la tua organizzazione. Queste impostazioni includono opzioni di condivisione predefinite, branding e altro ancora.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# Configurare le impostazioni della bozza per l’organizzazione

In qualità di amministratore di Adobe Workfront o di Workfront Proof, puoi personalizzare le impostazioni predefinite della bozza per la tua organizzazione. Queste impostazioni includono opzioni di condivisione predefinite, branding e altro ancora.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium o Select</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Nel profilo di autorizzazione bozza deve essere selezionato Amministratore. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurare l'accesso di verifica di un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Configurare le azioni

Per informazioni sull&#39;utilizzo delle azioni nel visualizzatore di bozze, vedere [Utilizzare azioni sui commenti della bozza](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

Puoi configurare le azioni per la tua organizzazione nei seguenti modi:

* [Aggiungere o rinominare un&#39;azione](#add-or-rename-an-action)
* [Disattivare o riattivare un&#39;azione](#deactivate-or-reactivate-an-action)
* [Riordina azioni](#reorder-actions)

### Aggiungere o rinominare un’azione {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Fai clic su **Impostazioni** > **Impostazioni account** nell&#39;angolo superiore destro dell&#39;interfaccia di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. Effettuare una delle seguenti operazioni:

   * Per creare una nuova azione, nella sezione **Azioni** fare clic su **Nuova azione**.

     Non esiste alcun limite al numero di azioni che è possibile impostare nel proprio account.

   * Per rinominare un&#39;azione esistente, fare clic su **Configurazione** accanto all&#39;azione.

1. Digita un nome per l&#39;azione, quindi fai clic su **Salva**.
1. Fai clic su **Salva.**

### Disattivare o riattivare un&#39;azione {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Fai clic su **Impostazioni** > **Impostazioni account** nell&#39;angolo superiore destro dell&#39;interfaccia di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. Fai clic su **Configurazione** accanto all&#39;azione da disattivare o riattivare.
1. Seleziona **Attiva** o **Disattiva**, quindi fai clic su **Salva**.

### Riordina azioni {#reorder-actions}

{{step1-to-proofing}}

1. Fai clic su **Impostazioni** > **Impostazioni account** nell&#39;angolo superiore destro dell&#39;interfaccia di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. Fai clic sulle frecce blu verso l&#39;alto e verso il basso accanto a **Configurazione** per riordinare le azioni.

   ![Riordina_azioni.png](assets/re-order-actions-350x103.png)

## Configurare dispositivi personalizzati per le bozze

Puoi aggiungere qualsiasi dispositivo personalizzato al sistema, consentendo agli utenti di esaminare i contenuti interattivi e simulare la modalità di visualizzazione del contenuto su un dispositivo specifico.

Per informazioni su come gli utenti possono selezionare i dispositivi durante la revisione del contenuto interattivo, vedi [Modificare la risoluzione della bozza interattiva nel visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

Per aggiungere un dispositivo personalizzato:

{{step1-to-proofing}}

1. Fai clic su **Impostazioni** > **Impostazioni account** nell&#39;angolo superiore destro dell&#39;interfaccia di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. Nella sezione **Dispositivi personalizzati per le bozze** fare clic su **Aggiungi nuovo dispositivo**.

1. Nella casella **Aggiungi nuovo dispositivo** visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Il nome visualizzato dagli utenti durante la selezione del dispositivo nel Visualizzatore bozze desktop, come descritto in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Modificare la risoluzione della bozza interattiva nel visualizzatore bozze</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensioni</td> 
      <td>Specificare le dimensioni da utilizzare per il dispositivo. Gli utenti visualizzano le dimensioni sotto il nome del dispositivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rapporto</td> 
      <td>Specifica la proporzione per il dispositivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td>Seleziona se il dispositivo è un dispositivo mobile, tablet o desktop.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stringa agente utente</td> 
      <td>Immettere l'agente utente per il dispositivo per fornire informazioni che consentano l'esecuzione e la visualizzazione del software come previsto per il dispositivo.<p>È possibile ottenere l'agente utente da <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> dal dispositivo.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disabilitato</td> 
      <td>Se questa opzione è selezionata, il dispositivo non è disponibile per la selezione da parte degli utenti durante la revisione delle bozze interattive.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Crea**.

## Configurare i messaggi popup per le bozze

È possibile configurare messaggi popup sulle bozze per comunicare informazioni generali a tutti i revisori dell’organizzazione.

Puoi configurare i messaggi in modo che vengano visualizzati nelle seguenti situazioni:

* **Messaggio al caricamento**: viene visualizzato la prima volta che si apre la bozza. Utile per spiegare agli utenti come rivedere una bozza o fornire una liberatoria o altro testo legale.
* **Sul messaggio di decisione**: viene visualizzato quando un utente seleziona una decisione su una bozza. Utile per fornire agli utenti liste di controllo per elementi quali la conformità del marchio o alle normative. Per informazioni sulle decisioni, consulta [Decidere su una bozza nel visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Testo pulsante di conferma**: l&#39;etichetta visualizzata sul pulsante nel messaggio popup al caricamento descritto sopra.

Per creare messaggi popup per le bozze:

1. Fai clic su **Modifica** a destra del messaggio che desideri personalizzare.
1. Specifica un messaggio e includi la formattazione appropriata, quindi fai clic su **Salva**.
1. (Facoltativo) Se hai personalizzato il messaggio Al caricamento e desideri personalizzare anche l&#39;etichetta del pulsante di conferma, fai clic su **Modifica** a destra di **Testo pulsante di conferma**, specifica un&#39;etichetta, quindi fai clic su **Salva**.

## Configurare i valori predefiniti per la bozza

Per informazioni sulla configurazione delle impostazioni predefinite della bozza per l&#39;organizzazione, vedere [Configurare le impostazioni predefinite della bozza](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Configurare le impostazioni predefinite di condivisione

Puoi specificare con chi possono essere condivise le bozze della tua organizzazione, quali versioni sono disponibili per i revisori e quando le bozze con un flusso di lavoro automatico sono visibili agli utenti associati a una determinata fase.

Per informazioni più dettagliate sulle impostazioni di condivisione in Workfront Proof, vedere [Configurare le impostazioni di condivisione per gli utenti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Assegna il marchio al sito Workfront Proof

Se utilizzi Workfront Proof, puoi impostare il branding per le seguenti aree del sito:

* Pagina iniziale visualizzata al caricamento della bozza
* Schermate di accesso e disconnessione
* Notifiche e-mail

Per informazioni dettagliate su come aggiungere un marchio al sito Workfront Proof, consulta [Assegnare un marchio al sito Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Configurare le impostazioni avanzate della password

>[!IMPORTANT]
>
>Questa opzione è disponibile solo per i piani Workfront legacy. Se si utilizza un piano Pro, Business o Enterprise Workfront, non è più possibile configurare le impostazioni avanzate della password.

In **Impostazioni password avanzate**, puoi migliorare la sicurezza delle password per i tuoi utenti.

1. Fai clic su **Configurazione** a destra dell&#39;impostazione che desideri configurare:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lunghezza minima password</td> 
      <td>La lunghezza predefinita della password di Workfront Proof è di sei caratteri. Puoi aumentare il numero, a seconda dei criteri della tua organizzazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Combinazione di caratteri</strong> </td> 
      <td>È possibile forzare gli utenti a utilizzare una combinazione di lettere minuscole, lettere maiuscole, numeri e simboli nelle password. È possibile decidere il numero di caratteri che la password deve contenere.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Numero massimo di caratteri ripetuti</strong> </td> 
      <td>È possibile specificare il numero di caratteri che possono essere ripetuti nella password di ogni utente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scadenzario automatico password</td> 
      <td>Obbliga gli utenti a modificare regolarmente la password. Decidi con quale frequenza lo faranno.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Numero di ripetizioni password non consentite</strong> </td> 
      <td>Configura il numero di ripetizioni di password non consentite nel tuo account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Blocco profilo</strong> </td> 
      <td>Blocca gli utenti fuori dall’account dopo una serie di tentativi di accesso non riusciti specificati. Puoi anche specificare per quanto tempo devono attendere prima di poter accedere nuovamente al loro account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca utente se la password non viene reimpostata dopo 30 giorni</td> 
      <td>Se l’utente non modifica la password iniziale entro 30 giorni dall’attivazione del profilo, viene bloccato dall’account.<br><p>Gli amministratori degli account possono sbloccare (riattivare) gli utenti che vengono bloccati automaticamente dal sistema. In questo modo, avranno a disposizione altri sette giorni per cambiare la password.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca account utente se inattivo per 120 giorni</td> 
      <td>Se l’utente non accede a Workfront Proof o a una bozza di accesso richiesta per 120 giorni, viene bloccato l’account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cambia password dopo il primo accesso</strong> </td> 
      <td>Richiede agli utenti di modificare la password temporanea dopo il primo accesso.<p>Gli amministratori degli account possono sbloccare (riattivare) gli utenti che vengono automaticamente bloccati dal sistema.</p><p>Per ulteriori informazioni sulla password, vedere <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Accesso e modifica della password e dell'indirizzo di posta elettronica per Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
