---
product-area: requests
navigation-topic: create-requests
title: Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste
description: Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puoi configurare un progetto per consentire agli utenti di aggiungere problemi al progetto tramite e-mail. Puoi consentire l’invio di e-mail di problemi in un progetto solo se il progetto è designato come coda di richieste. Per ulteriori informazioni sulla creazione di un progetto di coda richieste, vedere [Creare una coda richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Per configurare un progetto in modo che gli utenti possano aggiungere problemi al progetto tramite e-mail, sono necessari i seguenti prerequisiti.

Prima di abilitare questa funzione è necessario soddisfare le seguenti condizioni:

* Gli utenti che inviano problemi a questo account tramite e-mail devono essere utenti attivi con una licenza per Workfront.
* Gli utenti che inviano problemi a questo account devono disporre delle autorizzazioni Aggiungi problema per il progetto.
* Gli utenti esterni non possono inviare problemi via e-mail a una coda di richieste perché non hanno accesso alla creazione dei problemi.
* Solo le e-mail provenienti da un indirizzo e-mail associato a un utente Workfront attivo possono inviare problemi al progetto. Le e-mail inoltrate a un utente Workfront attivo da un indirizzo e-mail non associato a un account Workfront non sono in grado di creare problemi nel progetto, in quanto l’indirizzo e-mail del mittente originale deve essere associato a un account Workfront attivo.
* Il progetto è impostato come coda di richieste.
* L’account e-mail associato al progetto non è collegato a un account utente di Workfront.

## Configurare il progetto in Workfront

>[!NOTE]
>
>Quando abiliti le impostazioni della coda e-mail, tieni presente quanto segue:
>
>* Workfront consente di inviare un messaggio e-mail univoco per ogni coda di richieste in tutti i cluster. Se scegli di disabilitare la coda di richieste, mantieni l’indirizzo e-mail creato finché è ancora nella casella Indirizzo e-mail di assegnazione. Se scegli di interrompere l’uso dell’e-mail di assegnazione, devi eliminarla dal campo E-mail di assegnazione in modo che possa essere utilizzata in futuro.
>
>* Se la coda di richieste ha più argomenti della coda o gruppi di argomenti, Workfront selezionerà in modo casuale l’argomento della coda a cui andranno le richieste inviate via e-mail, rendendo difficile la gestione di queste ultime.
>È consigliabile che il progetto configurato per la ricezione di richieste tramite e-mail non contenga più di un argomento della coda. Se le richieste inviate sono destinate a risorse o progetti diversi, è necessario indirizzarle o spostarle manualmente, dopo l’invio.

1. Vai al progetto che desideri abilitare per ricevere i problemi tramite e-mail.
1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**.
1. Nell&#39;area **Tipo coda**, selezionare **Publish come Coda richieste della Guida**.

1. Scorri verso il basso fino all&#39;area **Impostazioni coda e-mail**, quindi seleziona **Abilita acquisizione richieste tramite e-mail**.

1. Immettere l&#39;inizio dell&#39;indirizzo e-mail nella casella **Indirizzo e-mail assegnazione**.

   Devi creare un indirizzo e-mail univoco. È consigliabile utilizzare il nome della società come parte dell’indirizzo e-mail di assegnazione.

   >[!CAUTION]
   >
   >* Non è possibile recuperare questo indirizzo e-mail dal Cestino se il progetto contenente la coda di richieste viene eliminato.
   >
   >* Poiché questo indirizzo e-mail deve essere univoco, potrebbe non essere disponibile in futuro se viene eliminato.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Facoltativo) Seleziona **Inoltra tutti i problemi che non vengono inviati tramite e-mail**, quindi inserisci un indirizzo e-mail di inoltro nella casella qui sotto.

   Questo indirizzo e-mail riceve informazioni sulle e-mail che non sono state inviate al progetto.

1. Fai clic su **Salva**. Ora, quando gli utenti con un account Workfront attivo inviano un’e-mail a questo indirizzo e-mail, nel progetto Workfront viene creato un problema.

   >[!NOTE]
   >
   >Per poter inviare l’e-mail, gli utenti devono avere accesso per creare i problemi nel progetto. È possibile concedere questo accesso nella finestra di dialogo Condivisione in Impostazioni avanzate.
   >
   >Gli utenti esterni non possono inviare problemi via e-mail a una coda di richieste perché non hanno accesso alla creazione dei problemi.

## Ricevi il problema in Workfront

Quando un utente di Workfront invia un’e-mail a Workfront, si verificano le seguenti situazioni:

* La riga Oggetto dell’e-mail diventa il Nome del problema.
* Il corpo dell’e-mail diventa la Descrizione del problema.
* Se all’e-mail sono allegati dei documenti, questi saranno allegati al problema in Workfront.
* L’utente che invia l’e-mail diventa il contatto principale del nuovo problema in Workfront.
* Il corpo del testo dell’e-mail non può superare i 4.000 caratteri.
* Gli allegati e-mail non possono superare i 7 MB in totale.
