---
product-area: requests
navigation-topic: create-requests
title: Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste
description: Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: ca3c28174dca24f14a75869bdc209569d8d8d1a0
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puoi configurare un progetto per consentire agli utenti di aggiungere problemi al progetto tramite e-mail. Puoi consentire l’invio di e-mail dei problemi a un progetto solo se il progetto è designato come coda di richiesta. Per ulteriori informazioni sulla creazione di un progetto di coda richieste, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per configurare un progetto è necessario disporre dei seguenti prerequisiti per consentire agli utenti di aggiungere problemi al progetto tramite e-mail.

Prima di abilitare questa funzione, è necessario soddisfare queste condizioni:

* Gli utenti che inviano problemi a questo account devono essere utenti attivi con una licenza per Workfront.
* Gli utenti esterni non possono inviare problemi tramite e-mail a una coda di richiesta perché non hanno accesso per creare problemi.
* Gli utenti che inviano problemi a questo account devono disporre delle autorizzazioni Aggiungi problema per il progetto.
* Le e-mail provenienti dall’indirizzo e-mail associato a un utente Workfront attivo sono le uniche e-mail consentite per inviare problemi al progetto.
* Il progetto è configurato come coda di richiesta.
* L’account e-mail associato al progetto non è collegato a un account utente Workfront.

## Configurare il progetto in Workfront

>[!NOTE]
>
>Quando abiliti le impostazioni della coda e-mail, tieni presente quanto segue:
>
>* Workfront consente un’e-mail univoca per coda di richiesta in tutti i cluster. Se scegli di disabilitare la coda delle richieste, mantieni l’indirizzo e-mail creato purché sia ancora nella casella Indirizzo e-mail di input. Se scegli di interrompere l’utilizzo dell’e-mail di assunzione, devi eliminarla dal campo e-mail di immissione in modo che possa essere disponibile per un utilizzo futuro.
>
>* Se la coda di richiesta contiene più argomenti o gruppi di argomenti in coda, Workfront selezionerà in modo casuale l’argomento della coda a cui verranno indirizzate le richieste inviate e-mail, rendendo le richieste inviate difficoltose da gestire.
   >È consigliabile che il progetto configurato per la ricezione di richieste tramite e-mail non includa più di un argomento della coda. Se le richieste inviate sono destinate a risorse o progetti diversi, dopo l’invio è necessario instradarle o spostarle manualmente.


1. Vai al progetto che desideri abilitare per ricevere i problemi tramite e-mail.
1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro** prima.
1. In **Tipo di coda** area, selezionare **Pubblica come coda delle richieste di aiuto**.

1. Scorri verso il basso fino a **Impostazioni coda e-mail** area, quindi selezionare **Abilita l’acquisizione della richiesta tramite e-mail**.

1. Immetti l’inizio dell’indirizzo e-mail nel **Indirizzo e-mail di acquisizione** scatola.

   Devi creare un indirizzo e-mail univoco. Si consiglia di utilizzare il nome della società come parte dell&#39;indirizzo e-mail di assunzione.

   >[!CAUTION]
   >
   >* Impossibile recuperare questo indirizzo e-mail dal cestino se il progetto contenente la coda di richiesta viene eliminato.
   >
   >* Poiché questo indirizzo e-mail deve essere univoco, potrebbe non essere disponibile in futuro se eliminato.

   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Facoltativo) Seleziona la **Inoltrare tutti i problemi che non vengono inviati tramite e-mail**, quindi immetti un indirizzo e-mail di inoltro nella casella seguente.

   Questo indirizzo e-mail riceve informazioni sulle e-mail che non sono state inviate al progetto.

1. Fai clic su **Salva**. Ora, quando gli utenti con un account Workfront attivo inviano un’e-mail a questo indirizzo e-mail, viene creato un problema nel progetto Workfront.

   >[!NOTE]
   >
   >Per poter inviare tramite e-mail, gli utenti devono disporre dell’accesso per creare problemi nel progetto. È possibile concedere questo accesso nella finestra di dialogo Condivisione in Impostazioni avanzate.
   >
   >Gli utenti esterni non possono inviare problemi tramite e-mail a una coda di richiesta perché non hanno accesso per creare problemi.

## Ricevere il problema in Workfront

Quando un utente Workfront invia un’e-mail a Workfront, si verificano le seguenti situazioni:

* L’oggetto dell’e-mail diventa il Nome del problema.
* Il corpo dell’e-mail diventa la Descrizione del problema.
* Se sono presenti documenti allegati all’e-mail, tali documenti sono allegati al problema in Workfront.
* L’utente che invia l’e-mail diventa il contatto principale del nuovo problema in Workfront.
* Il testo del corpo dell’e-mail non può superare i 4.000 caratteri.
* Gli allegati e-mail non possono superare i 7 MB totali.
