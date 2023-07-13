---
title: Copiare e inviare richieste
description: Quando invii spesso richieste simili, puoi copiare una richiesta già inviata. In questo caso, puoi copiare una richiesta esistente, apportarvi modifiche minime e inviarla nuovamente come nuova richiesta.
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 2%

---

# Copiare e inviare richieste

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Quando invii spesso richieste simili, puoi copiare una richiesta già inviata. In questo caso, puoi copiare una richiesta esistente, apportarvi modifiche minime e inviarla nuovamente come nuova richiesta.

## Requisiti di accesso

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso per aggiungere richieste a una coda di richieste</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda di richieste, vedi <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richieste</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre di una richiesta inviata in precedenza da te o da un utente dell’organizzazione per poterla copiare e inviare nuovamente. Se la richiesta appartiene a un altro utente, è necessario disporre almeno dell&#39;accesso alla visualizzazione per poterla copiare e inviare come nuova richiesta.

## Considerazioni sulla copia e l’invio delle richieste come nuove

* Puoi solo copiare e inviare richieste inviate. Non è possibile copiare richieste bozze.
* È possibile copiare e inviare le richieste inviate in origine o quelle inviate da altri utenti e a cui si ha accesso almeno alla visualizzazione.
* Puoi sempre accedere a copiare e inviare una copia delle tue richieste, a meno che qualcuno non rimuova le tue autorizzazioni per esse.
* L’accesso per copiare e inviare le richieste originariamente inviate da altri può essere concesso automaticamente alle persone nella stessa società quando l’autore della coda di richieste abilita **Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste** nelle aree Dettagli coda o Modifica progetto. La disattivazione di questa impostazione consente solo al richiedente originale di visualizzare le proprie richieste.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md)

* È possibile aggiornare la copia della richiesta originale prima di inviarla nuovamente come nuova richiesta.
* Se le seguenti modifiche si verificano dopo l&#39;invio della richiesta originale, non è più possibile copiarla e inviarla di nuovo:

   * La coda richieste è stata eliminata.
   * L&#39;argomento della coda è stato eliminato.

     >[!TIP]
     >
     >Se l’argomento della coda era l’unico presente nella coda richieste, puoi comunque copiare e inviare la richiesta, che verrà salvata nella coda richieste stessa.

   * La coda di richieste non viene più pubblicata come coda di richieste di aiuto. Per informazioni, consulta [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Se la coda di richieste non ha un argomento di coda e la richiesta originale è stata inviata prima di gennaio 2022.

   * Lo stato del progetto associato alla coda di richieste non è più Corrente.

* È possibile copiare e inviare una copia di una richiesta convertita se la richiesta è stata mantenuta nel processo di conversione. Per ulteriori informazioni, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >La richiesta copiata non è collegata a un oggetto di risoluzione.

## Copiare e inviare richieste

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Richieste**.
1. (Condizionale) Se la sezione Inviata non viene visualizzata per impostazione predefinita, fai clic su **Inviato** nel pannello a sinistra.
1. Individuare la richiesta che si desidera copiare e inviare come nuova ed effettuare una delle seguenti operazioni:

   * Selezionala, quindi fai clic su **Copia** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) nell’angolo superiore sinistro dell’elenco Richieste inviate.

   >[!TIP]
   >
   > Se non hai selezionato prima una richiesta, l’icona Copia non è attiva.

   * Fai clic su **Altro** menu ![](assets/more-icon.png) a destra del nome della richiesta, quindi fai clic su **Copia e invia come nuovo**

     Oppure

     Fare clic con il pulsante destro del mouse sulla richiesta selezionata, quindi scegliere **Copia e invia come nuovo**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Se non disponi dell’accesso per la creazione di problemi, ricevi un avviso che informa che l’amministratore non ti ha consentito di creare richieste.

1. (Facoltativo) Se necessario, aggiorna le seguenti informazioni:

   * **Tipo di richiesta**: la coda di richieste in cui viene salvata la richiesta copiata. Per impostazione predefinita, la richiesta copiata viene salvata nella coda richieste della richiesta originale.
   * **Gruppi di argomenti** e **Argomenti Coda**, se sono selezionati. I nomi o i gruppi di argomenti e gli argomenti della coda vengono personalizzati per l&#39;ambiente in uso. Per impostazione predefinita, la richiesta copiata viene salvata nei gruppi di argomenti e negli argomenti della coda della richiesta originale.

     >[!TIP]
     >
     >Se il percorso cambia rispetto a quello della richiesta originale, l’autore della coda di richieste ha modificato la coda.

1. (Facoltativo) Aggiorna tutte le informazioni della richiesta copiata. A seconda dei campi abilitati dal creatore della coda di richieste in **Campi delle Nuove Issues** sezione del **Dettagli coda** scheda secondaria del progetto, è possibile che siano presenti i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Oggetto</strong> </td> 
      <td>Visualizza il nome della richiesta originale. Se necessario, aggiornala. In caso contrario, Workfront nomina la richiesta copiata <b>Copia di &lt;name of="" original="" request=""&gt;</b>. Questo è un campo obbligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Visualizza la descrizione della richiesta originale. Se necessario, aggiornala.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Visualizza l’URL della richiesta originale. Se necessario, aggiornala.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorità</strong> </td> 
      <td> <p>Specifica la priorità della richiesta. La priorità deve definire la velocità con cui pensi che questa richiesta debba essere risolta. Le opzioni predefinite sono:</p> 
       <ul> 
        <li>Nessuno</li> 
        <li>Basso</li> 
        <li>Normal</li> 
        <li>Alta</li> 
        <li>Urgente</li> 
       </ul> <p>L’amministratore di Workfront può modificare i nomi delle priorità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravità</strong> </td> 
      <td> <p>Specifica la gravità della richiesta. La gravità deve definire l’impatto di questa richiesta sul lavoro nel caso non venga risolta in tempo. Le opzioni predefinite sono:</p> 
       <ul> 
        <li>Cosmetico</li> 
        <li>Causa Confusione</li> 
        <li>Bug con workaround</li> 
        <li>Bug senza workaround</li> 
        <li>Errore Fatale</li> 
       </ul> <p>L’amministratore di Workfront può modificare i nomi delle gravità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contatto principale</strong> </td> 
      <td>Il contatto principale di una richiesta viene impostato automaticamente su di te, in quanto sei la persona che risponde a tutte le domande relative alla richiesta. Tuttavia, puoi modificarlo in qualsiasi altro utente di Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Assegnazioni</strong></span> </td> 
      <td> <p>Indica il nome di un utente attivo, una mansione o un team a cui assegnare la richiesta. </p> <p> È possibile specificare più utenti, mansioni o team. </p> <p>A seconda di come è stata impostata la coda di richieste, potresti essere in grado di assegnare la richiesta solo a uno o due tipi di risorse, anziché a tutti e tre. </p> <p>È consigliabile utilizzare le regole di instradamento per le code di richieste in modo che possano essere instradate automaticamente alle risorse appropriate. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">A seconda di come è stata impostata la coda di richieste, potresti essere in grado di assegnare alla richiesta un solo tipo di risorsa (ad esempio, utenti). Se alla coda di richieste è associata anche una regola di instradamento che instrada automaticamente la richiesta a un tipo diverso di risorsa (ad esempio, un team), la richiesta viene assegnata sia all'entità specificata manualmente durante l'invio della richiesta (utenti) sia alla risorsa specificata nella regola di instradamento (team).</p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta i seguenti articoli:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richieste</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di instradamento</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Lavoro Necessario</strong> </td> 
      <td> <p>Stimare quante ore occorrerebbe per completare la richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di inizio pianificata</strong> </td> 
      <td> <p>La data in cui dovrebbero iniziare i lavori per questa richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di completamento Pianificata</strong> </td> 
      <td>La data in cui desideri che questa richiesta sia risolta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Stato</strong> </td> 
      <td>Lo stato predefinito di una nuova richiesta è "Nuovo". È possibile che il nome dello stato sia stato modificato dall'amministratore di Workfront. Puoi anche cambiare lo stato da questo menu a discesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documenti</strong> </td> 
      <td> <p>Aggiungi documenti alla tua richiesta. I documenti allegati alla richiesta originale non vengono trasferiti alla richiesta copiata.</p> <p><b>SUGGERIMENTO</b>

   A seconda della configurazione della coda di richieste, la sezione Documenti potrebbe essere visualizzata prima o dopo i campi personalizzati.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Se necessario, aggiorna le informazioni nei moduli personalizzati allegati.

   >[!TIP]
   >
   >* Tutti i moduli personalizzati allegati alla richiesta originale e i valori inclusi nei campi personalizzati vengono trasferiti alla richiesta copiata. Sono inclusi i campi che contengono logica.
   >* Non è possibile rimuovere i moduli personalizzati dalla richiesta copiata.

1. Clic **Invia**.

   La richiesta copiata viene inviata come nuova richiesta nella coda richieste specificata.
