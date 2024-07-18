---
product-area: projects
navigation-topic: approvals
title: Delega richiesta di approvazione
description: La delega delle richieste di approvazione ti consente di assegnare a un altro utente il compito di approvare le richieste per un determinato periodo di tempo, ad esempio se ti trovi fuori sede in vacanza.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 0%

---

# Delega richiesta di approvazione

Puoi delegare temporaneamente il lavoro che ti è stato assegnato mentre sei fuori sede. Puoi delegare le assegnazioni di attività e problemi oppure puoi delegare le richieste di approvazione. Questo articolo descrive come delegare le richieste di approvazione. Per informazioni sulla delega delle assegnazioni di attività e problemi, vedere [Gestire la delega di attività e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

Puoi delegare i seguenti tipi di approvazione, indipendentemente da come ti è stata assegnata l’approvazione (sia che sia assegnata direttamente a te, a un team di cui sei membro o al tuo ruolo lavorativo):

* Approvazioni progetto
* Approvazioni attività
* Approvazioni problemi

Non puoi delegare le approvazioni di schede orario, documenti o bozze.

>[!NOTE]
>
>Per evitare incoerenze con le date pianificate per la delega delle approvazioni, è consigliabile che il fuso orario del profilo utente corrisponda a quello della pianificazione. Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Crea una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modifica il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Comprendere l’accesso degli utenti per le approvazioni delegate

Durante il periodo di approvazione designato, l’utente a cui deleghi una richiesta di approvazione dispone delle seguenti capacità:

* Può approvare o rifiutare le richieste di approvazione esistenti se non è stata presa alcuna decisione
* Può approvare e rifiutare nuove richieste di approvazione ricevute durante un periodo di tempo specificato
* È concesso l’accesso di visualizzazione agli oggetti in attesa di approvazione

  >[!NOTE]
  >
  > L’amministratore Adobe Workfront può impedire agli utenti di accedere a determinati tipi di oggetti. Quando un utente non ha accesso a un tipo di oggetto e all’utente viene delegata un’approvazione di tale tipo, l’utente non ha accesso alla visualizzazione dell’oggetto. Tuttavia, l&#39;utente può ancora approvare o rifiutare le richieste di approvazione dalla **Home** pagina, come descritto in [Approvazione del lavoro](../../review-and-approve-work/manage-approvals/approving-work.md).\
  >Ad esempio, l&#39;utente A appartiene al gruppo A. L&#39;amministratore di Workfront ha limitato i diritti di accesso del Gruppo A in modo che gli utenti di questo gruppo non possano visualizzare le attività all&#39;interno di Workfront. Se una richiesta di approvazione di un’attività è delegata all’Utente A, quest’ultimo non può visualizzare l’attività a cui è associata l’approvazione. Tuttavia, l’utente A può approvare o rifiutare la richiesta di approvazione dalla home page.

  Per informazioni su come l&#39;amministratore di Workfront può limitare l&#39;accesso ai tipi di oggetto in Configurazione, vedere  [Crea o modifica livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Dopo l&#39;interruzione o l&#39;annullamento della delega di approvazione, l&#39;utente designato come approvatore:

* Non dispone più dell&#39;accesso per approvare il lavoro per gli elementi che richiedono l&#39;approvazione
* Continua ad avere accesso in visualizzazione agli elementi di lavoro\
  Gli utenti a cui è stato concesso l’accesso di visualizzazione agli oggetti tramite una delega di approvazione conservano tale accesso anche dopo l’interruzione o il richiamo della delega di approvazione. Per rimuovere l’accesso in visualizzazione a qualsiasi oggetto a cui l’utente aveva accesso durante il periodo di delega delle approvazioni, devi passare all’oggetto e rimuovere i diritti di accesso direttamente dall’oggetto.

## Delegare le richieste di approvazione nell’area Home

Puoi delegare le richieste di approvazione dall’area Home.

### Delega le tue approvazioni a un altro utente {#delegate-your-approvals-to-another-user}

Puoi delegare i seguenti tipi di approvazione, indipendentemente da come ti è stata assegnata l’approvazione (sia che sia assegnata direttamente a te, a un team di cui sei membro o al tuo ruolo lavorativo):

* Approvazioni progetto
* Approvazioni attività
* Approvazioni problemi

Non puoi delegare le approvazioni di schede orario, documenti o bozze.

Quando deleghi le approvazioni, tieni presente quanto segue:

* Quando deleghi le approvazioni, tutte le tue approvazioni vengono delegate. Non è possibile delegare singole richieste di approvazione.
* È possibile delegare le approvazioni a un solo utente; non è possibile delegare le approvazioni a più utenti contemporaneamente.\
  Tutte le approvazioni per tutti i progetti, le attività e i problemi vengono delegate all&#39;utente designato.
* Un massimo di 5 utenti può delegare le approvazioni allo stesso utente contemporaneamente. In altre parole, un singolo utente non può essere designato come approvatore temporaneo per più di 5 utenti contemporaneamente.
* L’attività relativa alle approvazioni viene visualizzata nella scheda Aggiornamenti. È necessario che l&#39;opzione Mostra aggiornamenti di sistema sia abilitata. Sia l’utente che delega l’approvazione sia l’utente a cui vengono delegate le approvazioni ricevono una notifica e-mail relativa all’attività di approvazione.

Per delegare le approvazioni a un altro utente:

1. Fai clic sull&#39;icona **Home** ![](assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro della pagina, quindi fai clic su **Home**.

   Oppure

   Fai clic sull&#39;icona **Main Menu** > **your name** > **Time Off** nel pannello a sinistra.

1. (Facoltativo e condizionale) Nell&#39;area Home, fare clic sul menu a discesa **Filtro**, quindi su **Approvazioni**.

1. (Condizionale) Fai clic su **Delega le mie approvazioni**

   Oppure

   Se l&#39;amministratore del sistema o del gruppo ha abilitato la delega di attività e problemi, fai clic su **Delega**, quindi su **Delega approvazioni**.

   ![](assets/delegate-approvals-nwe.png)

1. Specifica le seguenti informazioni nella sezione Delegate My Approvals (Delega le mie approvazioni):

   * **Nome**: inizia a digitare il nome dell&#39;utente a cui desideri delegare le approvazioni, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.
   * **Data inizio**: seleziona la data in cui le approvazioni iniziano a essere inoltrate. L’inoltro inizia alle 00:00 del mattino successivo alla data selezionata.\
     La data di inizio deve essere la data corrente o una data futura.
   * **Data di fine**:Effettuare una delle operazioni seguenti:

      * Seleziona la data in cui le approvazioni non verranno più inoltrate. L’inoltro termina alle 23:59 della data selezionata.
      * Seleziona **Nessuna data di fine** per configurare Workfront in modo da delegare le approvazioni a tempo indefinito.

1. Fai clic su **Salva**.

### Aggiornare o interrompere una delega di approvazione {#update-or-stop-an-approval-delegation}

1. Fai clic sull&#39;icona **Home** ![](assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro della pagina, quindi fai clic su **Home**.

1. Fai clic sul menu a discesa **Filtro**, quindi fai clic su **Approvazioni**.

1. (Condizionale) Fai clic su **Modifica delega**

   Oppure

   Se l&#39;amministratore del sistema o del gruppo ha abilitato la delega di attività e problemi, fare clic su **Modifica delega**, quindi su **Delega approvazioni**.

1. (Condizionale) Effettua una delle seguenti operazioni:

   * Per aggiornare la delega di approvazione esistente: modifica le informazioni visualizzate, quindi fai clic su **Salva**.

   * Per interrompere la delega esistente: fare clic su **Interrompi delega**, quindi fare clic su **Interrompi delega** per confermare.

     ![](assets/stop-delegation-nwe.png)

### Visualizza approvazioni delegate {#view-delegated-approvals}

In Elenco lavori è possibile visualizzare solo i tipi di deleghe di approvazione seguenti:

* Approvazioni progetto
* Approvazioni attività
* Approvazioni problemi

Per visualizzare le approvazioni delegate:

1. Fai clic sull&#39;icona **Home** ![](assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro della pagina, quindi fai clic su **Home**.

1. Fai clic sul menu a discesa **Filtro**, quindi fai clic su **Approvazioni**.\
   Tutte le approvazioni vengono visualizzate nell’elenco per impostazione predefinita, incluse le approvazioni assegnate all’utente e quelle delegate all’utente.

   ![](assets/delegated-to-me-nwe-350x93.png)
