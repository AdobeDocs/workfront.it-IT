---
product-area: projects
navigation-topic: approvals
title: Delega richiesta di approvazione
description: La delega delle richieste di approvazione ti consente di assegnare a un altro utente il compito di approvare le richieste per un determinato periodo di tempo, ad esempio se ti trovi fuori sede in vacanza.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# Delega richiesta di approvazione

Puoi delegare temporaneamente il lavoro che ti è stato assegnato mentre sei fuori sede. Puoi delegare le assegnazioni di attività e problemi, oppure puoi delegare le richieste di approvazione. Questo articolo descrive come delegare le richieste di approvazione. Per informazioni sulla delega delle assegnazioni di attività e problemi, vedere [Delegare attività e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

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

## Delega le tue approvazioni a un altro utente {#delegate-your-approvals-to-another-user}

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

### Delega le approvazioni dall’area Home


Per delegare le approvazioni a un altro utente:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere il widget **Le mie approvazioni**.
1. Vai al widget Le mie approvazioni, quindi fai clic su **Delega le mie approvazioni**.

   >[!NOTE]
   >
   >Gli amministratori di Workfront possono disattivare le deleghe di approvazione dall’area di configurazione. Se le deleghe di approvazione sono disattivate, il pulsante Delega approvazioni non viene visualizzato.

   ![Delega le approvazioni in home](assets/delegate-approvals-home.png)

1. Specifica le seguenti informazioni nella sezione Delegate My Approvals (Delega le mie approvazioni):

   * **Nome**: inizia a digitare il nome dell&#39;utente a cui desideri delegare le approvazioni, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.
   * **Data inizio**: seleziona la data in cui le approvazioni iniziano a essere inoltrate. L’inoltro inizia alle 00:00 del mattino successivo alla data selezionata.\
     La data di inizio deve essere la data corrente o una data futura.
   * **Data di fine**: eseguire una delle operazioni seguenti:
      * Seleziona la data in cui le approvazioni non verranno più inoltrate. L’inoltro termina alle 23:59 della data selezionata.
      * Seleziona **Nessuna data di fine** per configurare Workfront in modo da delegare le approvazioni a tempo indefinito.

1. Fai clic su **Salva**.

### Delegare le approvazioni dal profilo utente

1. Fai clic sull&#39;icona **Main Menu** > **your name** > **Time Off** nel pannello a sinistra.
1. Fai clic su **Delega approvazioni**.

   >[!NOTE]
   >
   >Gli amministratori di Workfront possono disattivare le deleghe di approvazione dall’area di configurazione. Se le deleghe di approvazione sono disattivate, il pulsante Delega approvazioni non viene visualizzato.
1. Specifica le seguenti informazioni nella sezione Delegate My Approvals (Delega le mie approvazioni):

   * **Nome**: inizia a digitare il nome dell&#39;utente a cui desideri delegare le approvazioni, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.
   * **Data inizio**: seleziona la data in cui le approvazioni iniziano a essere inoltrate. L’inoltro inizia alle 00:00 del mattino successivo alla data selezionata.\
     La data di inizio deve essere la data corrente o una data futura.
   * **Data di fine**: eseguire una delle operazioni seguenti:
      * Seleziona la data in cui le approvazioni non verranno più inoltrate. L’inoltro termina alle 23:59 della data selezionata.
      * Seleziona **Nessuna data di fine** per configurare Workfront in modo da delegare le approvazioni a tempo indefinito.

## Aggiornare o interrompere una delega di approvazione {#update-or-stop-an-approval-delegation}

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere il widget **Le mie approvazioni**.

1. Vai al widget Le mie approvazioni, quindi fai clic su **Modifica delega**.
   ![Modifica deleghe](assets/edit-delegations.png)
<!--
   Or

   If your system or group administrator enabled task and issue delegation, click **Edit delegation**, then click **Delegate approvals**.   -->

1. (Condizionale) Effettua una delle seguenti operazioni:

   * Per aggiornare la delega di approvazione esistente: modifica le informazioni visualizzate, quindi fai clic su **Salva**.

   * Per interrompere la delega esistente: fare clic su **Interrompi delega**, quindi fare clic su **Interrompi delega** per confermare.

## Visualizza approvazioni delegate {#view-delegated-approvals}

Nel widget Approvazioni personali è possibile visualizzare solo i seguenti tipi di deleghe di approvazione:

* Approvazioni progetto
* Approvazioni attività
* Approvazioni problemi

Per visualizzare le approvazioni delegate:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere il widget **Le mie approvazioni**.
1. Nel widget **Le mie approvazioni**, fai clic sul menu a discesa **Filtra**, quindi fai clic su **Approvazioni delegate**.\
   Tutte le approvazioni delegate all&#39;utente vengono visualizzate nell&#39;elenco.
