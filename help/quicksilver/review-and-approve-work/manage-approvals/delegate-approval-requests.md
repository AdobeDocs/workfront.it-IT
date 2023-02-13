---
product-area: projects
navigation-topic: approvals
title: Delega richiesta di approvazione
description: La delega delle richieste di approvazione ti consente di assegnare a un altro utente il compito di approvare le richieste per un periodo di tempo, ad esempio, nel caso in cui tu sia fuori ufficio in vacanza.
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# Delega richiesta di approvazione

Puoi delegare temporaneamente il lavoro a cui sei assegnato mentre sei fuori ufficio. È possibile delegare le assegnazioni di attività ed emissioni oppure delegare le richieste di approvazione. Questo articolo descrive come delegare le richieste di approvazione. Per informazioni sulla delega delle assegnazioni di task e problemi, vedere [Gestione dell&#39;attività e della delega dei problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>Per evitare incongruenze con le date pianificate per la delega delle approvazioni, è consigliabile che il fuso orario del profilo utente corrisponda a quello della pianificazione. Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>piano Adobe Workfront*</p></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Comprendere l’accesso degli utenti per le approvazioni delegate

Durante il periodo di approvazione designato, l&#39;utente al quale si delega una richiesta di approvazione ha le seguenti capacità:

* Può approvare o rifiutare le richieste di approvazione esistenti in assenza di una decisione
* Può approvare e rifiutare le nuove richieste di approvazione ricevute durante un periodo di tempo specificato
* Accesso alla visualizzazione degli oggetti in attesa di approvazione

   >[!NOTE]
   >
   > L’amministratore di Adobe Workfront può impedire agli utenti di accedere a determinati tipi di oggetti. Quando un utente non ha accesso a un tipo di oggetto e l&#39;approvazione di tale tipo viene delegata all&#39;utente, l&#39;utente non dispone dell&#39;accesso Visualizza all&#39;oggetto. Tuttavia, l’utente può comunque approvare o rifiutare le richieste di approvazione da **Pagina principale** come descritto in [Approvazione del lavoro](../../review-and-approve-work/manage-approvals/approving-work.md).\
   Ad esempio, l&#39;utente A appartiene al gruppo A. L&#39;amministratore di Workfront ha limitato i diritti di accesso del gruppo A in modo che gli utenti di questo gruppo non possano visualizzare le attività all&#39;interno di Workfront. Se una richiesta di approvazione di un&#39;attività viene delegata all&#39;utente A, l&#39;utente A non può visualizzare l&#39;attività a cui è associata l&#39;approvazione. Tuttavia, l’utente A può approvare o rifiutare la richiesta di approvazione dalla home page.

   Per informazioni su come l’amministratore di Workfront può limitare l’accesso ai tipi di oggetto all’interno di Configurazione, consulta  [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Dopo l&#39;arresto o l&#39;annullamento della delega di approvazione, l&#39;utente designato come approvatore:

* Non dispone più dell&#39;accesso per approvare il lavoro per gli articoli che richiedono l&#39;approvazione
* Continua ad avere l&#39;accesso Visualizza agli elementi di lavoro\
   Gli utenti a cui è stato concesso l’accesso Visualizza agli oggetti tramite una delega di approvazione conservano tale accesso Visualizza anche dopo che la delega di approvazione si è arrestata o è richiamata. Per rimuovere l&#39;accesso Visualizza agli oggetti a cui l&#39;utente ha avuto accesso durante il periodo di delega delle approvazioni, è necessario passare all&#39;oggetto e rimuovere i diritti di accesso direttamente dall&#39;oggetto.

## Delega richieste di approvazione nell&#39;area Home

* [Delega le approvazioni a un altro utente](#delegate-your-approvals-to-another-user)
* [Aggiornare o interrompere una delega di approvazione](#update-or-stop-an-approval-delegation)
* [Visualizza approvazioni delegate](#view-delegated-approvals)

### Delega le approvazioni a un altro utente {#delegate-your-approvals-to-another-user}

È possibile delegare i seguenti tipi di approvazioni, indipendentemente da come l&#39;approvazione è stata assegnata all&#39;utente (sia direttamente assegnata all&#39;utente, a un team di cui è membro o al suo ruolo di lavoro):

* Approvazioni dei progetti
* Approvazioni task
* Rilascio delle approvazioni

Non è possibile delegare le approvazioni di schede attività e documenti. 

Quando deleghi le approvazioni, considera quanto segue:

* Quando deleghi le approvazioni, tutte le approvazioni vengono delegate. Non è possibile delegare singole richieste di approvazione.
* Puoi delegare le approvazioni a un solo utente; non è possibile delegare le approvazioni a più utenti contemporaneamente.\
   Tutte le approvazioni per tutti i progetti, le attività e i problemi vengono delegate all&#39;utente designato.
* Un massimo di 5 utenti può delegare le approvazioni allo stesso tempo allo stesso utente. In altre parole, un singolo utente non può essere designato come approvatore temporaneo per più di 5 utenti contemporaneamente.
* L’attività relativa alle approvazioni viene visualizzata nella scheda Aggiornamenti . È necessario che Mostra aggiornamenti di sistema sia abilitato. Sia l’utente che delega l’approvazione che l’utente a cui vengono delegate le approvazioni ricevono una notifica e-mail relativa all’attività di approvazione.

Per delegare le approvazioni a un altro utente:

1. Fai clic sul pulsante **Pagina principale** icona ![](assets/home-icon-30x29.png) nell’angolo in alto a sinistra di Adobe Workfront.

   >[!NOTE]
   L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nell’ambiente:
   * Sostituiscilo con un&#39;immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   * Sostituisci la pagina collegata con una pagina diversa. In questo caso, fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) nell’angolo superiore destro della pagina, quindi fai clic su **Pagina principale**.


   Oppure

   Fai clic sul pulsante **Menu principale** icona > **nome** > **Time Off** nel pannello a sinistra.

1. (Facoltativo e condizionale) Nell’area Home, fai clic sul pulsante **Filtro** menu a discesa, quindi fai clic su **Approvazioni**.

1. (Condizionale) Fai clic su **Delega le mie approvazioni**

   Oppure

   Se l&#39;amministratore di sistema o di gruppo ha abilitato la delega dell&#39;attività e del problema, fare clic su **Delega**, quindi fai clic su **Delega approvazioni**.

   ![](assets/delegate-approvals-nwe.png)

1. Specifica le seguenti informazioni nella sezione Delega approvazioni personali :

   * **Nome**: Inizia a digitare il nome dell&#39;utente a cui desideri delegare le approvazioni, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.
   * **Data di inizio**: Selezionare la data di inizio dell&#39;inoltro delle approvazioni. L&#39;inoltro inizia alle 12:00 alla data selezionata.\
      La data di inizio deve essere la data corrente o una data futura.
   * **Data di fine**:Esegui una delle seguenti operazioni:

      * Selezionare la data per l&#39;interruzione dell&#39;inoltro delle approvazioni. L&#39;inoltro termina alle 23:59 alla data selezionata.
      * Seleziona **Nessuna data di fine** per configurare Workfront per delegare le approvazioni a tempo indeterminato.

1. Fai clic su **Salva**.

### Aggiornare o interrompere una delega di approvazione {#update-or-stop-an-approval-delegation}

1. Fai clic sul pulsante **Pagina principale** icona ![](assets/home-icon-30x29.png) nell’angolo in alto a sinistra di Adobe Workfront.

   >[!NOTE]
   L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nell’ambiente:
   * Sostituiscilo con un&#39;immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   * Sostituisci la pagina collegata con una pagina diversa. In questo caso, fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) nell’angolo superiore destro della pagina, quindi fai clic su **Pagina principale**.


1. Fai clic sul pulsante **Filtro** menu a discesa, quindi fai clic su **Approvazioni**.

1. (Condizionale) Fai clic su **Modifica delega**

   Oppure

   Se l&#39;attività e la delega sono state abilitate dall&#39;amministratore di sistema o di gruppo, fare clic su **Modifica delega**, quindi fai clic su **Delega approvazioni**.

1. (Condizionale) Effettuare una delle seguenti operazioni:

   * Per aggiornare la delega di approvazione esistente: Modifica le informazioni visualizzate, quindi fai clic su **Salva**.

   * Per interrompere la delega esistente: Fai clic su **Interrompi delega**, quindi fai clic su **Interrompi delega** per confermare.

      ![](assets/stop-delegation-nwe.png)

### Visualizza approvazioni delegate {#view-delegated-approvals}

È possibile visualizzare solo i seguenti tipi di delegazioni di approvazione nell&#39;Elenco di lavoro:

* Approvazioni dei progetti
* Approvazioni task
* Rilascio delle approvazioni

Per visualizzare le approvazioni delegate:

1. Fai clic sul pulsante **Pagina principale** icona ![](assets/home-icon-30x29.png) nell’angolo in alto a sinistra di Adobe Workfront.

   >[!NOTE]
   L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nell’ambiente:
   * Sostituiscilo con un&#39;immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   * Sostituisci la pagina collegata con una pagina diversa. In questo caso, fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) nell’angolo superiore destro della pagina, quindi fai clic su **Pagina principale**.


1. Fai clic sul pulsante **Filtro** menu a discesa, quindi fai clic su **Approvazioni**.\
   Tutte le approvazioni vengono visualizzate nell&#39;elenco per impostazione predefinita, incluse le approvazioni assegnate all&#39;utente e le approvazioni delegate all&#39;utente.

   ![](assets/delegated-to-me-nwe-350x93.png)
