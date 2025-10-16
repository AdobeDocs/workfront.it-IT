---
product-area: requests
navigation-topic: create-requests
title: Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste
description: Puoi configurare un progetto per consentire agli utenti di aggiungere problemi al progetto tramite e-mail.
author: Becky
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puoi configurare un progetto per consentire agli utenti di aggiungere problemi al progetto tramite e-mail. Puoi consentire l’invio di e-mail di problemi a un progetto solo se il progetto è designato come coda di richieste. Per ulteriori informazioni sulla creazione di un progetto di coda richieste, vedere [Creare una coda richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Prodotto</td> 
   <td> <ul><li>Adobe Workfront</li><li>È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per configurare un progetto in modo che gli utenti possano aggiungere problemi al progetto tramite e-mail, sono necessarie le seguenti condizioni:

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
>  &#x200B;>È consigliabile che il progetto configurato per la ricezione di richieste tramite e-mail non contenga più di un argomento della coda. Se le richieste inviate sono destinate a risorse o progetti diversi, è necessario indirizzarle o spostarle manualmente, dopo l’invio.

1. Vai al progetto che desideri abilitare per ricevere i problemi tramite e-mail.
1. Fai clic su **Dettagli coda** nel pannello a sinistra.
1. Nell&#39;area **Tipo coda**, selezionare **Pubblica come coda richieste di aiuto**.

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

  >[!NOTE]
  >
  > I file MSG non sono supportati e non verranno allegati al problema in Workfront.

* L’utente che invia l’e-mail diventa il contatto principale del nuovo problema in Workfront.
* Il corpo del testo dell’e-mail non può superare i 4.000 caratteri.
* Gli allegati e-mail non possono superare i 7 MB in totale.
