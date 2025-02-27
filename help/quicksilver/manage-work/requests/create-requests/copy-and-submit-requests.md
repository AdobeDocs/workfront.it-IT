---
title: Copiare e inviare richieste
description: Quando invii spesso richieste simili, puoi copiare una richiesta già inviata. In questo caso, puoi copiare una richiesta esistente, apportarvi modifiche minime e inviarla nuovamente come nuova richiesta.
author: Lisa
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 4ec3732d547cb3976c1376cbd0cf86b44b0e691b
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 1%

---

# Copiare e inviare richieste

Quando invii spesso richieste simili, puoi copiare una richiesta già inviata. In questo caso, puoi copiare una richiesta esistente, apportarvi modifiche minime e inviarla nuovamente come nuova richiesta.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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

Se non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso per aggiungere richieste a una coda di richieste</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda richieste, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda richieste</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   Oppure
   <p>Corrente: richiesta o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  </td> 
  </tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Accesso per aggiungere richieste a una coda di richieste</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda richieste, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda richieste</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario disporre di una richiesta inviata in precedenza da te o da un utente dell’organizzazione per poterla copiare e inviare nuovamente. Se la richiesta appartiene a un altro utente, è necessario disporre almeno dell&#39;accesso alla visualizzazione per poterla copiare e inviare come nuova richiesta.

## Considerazioni sulla copia e l’invio delle richieste come nuove

* Puoi solo copiare e inviare richieste inviate. Non è possibile copiare richieste bozze.
* È possibile copiare e inviare le richieste inviate in origine o quelle inviate da altri utenti e a cui si ha accesso almeno alla visualizzazione.
* Puoi sempre accedere a copiare e inviare una copia delle tue richieste, a meno che qualcuno non rimuova le tue autorizzazioni per esse.
* L&#39;accesso per copiare e inviare le richieste originariamente inviate da altri utenti potrebbe essere concesso automaticamente agli utenti della stessa società quando il creatore della coda di richieste abilita **Gli utenti della stessa società erediteranno le stesse autorizzazioni per tutte le richieste** nelle aree Dettagli coda o Modifica progetto. La disattivazione di questa impostazione consente solo al richiedente originale di visualizzare le proprie richieste.

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

   * La coda di richieste non viene più pubblicata come coda di richieste di aiuto. Per informazioni, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Se la coda di richieste non ha un argomento di coda e la richiesta originale è stata inviata prima di gennaio 2022.

   * Lo stato del progetto associato alla coda di richieste non è più Corrente.

* È possibile copiare e inviare una copia di una richiesta convertita se la richiesta è stata mantenuta nel processo di conversione. Per ulteriori informazioni, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >La richiesta copiata non è collegata a un oggetto di risoluzione.

## Copiare e inviare richieste

{{step1-to-requests}}

1. (Condizionale) Se la sezione Inviata non viene visualizzata per impostazione predefinita, fai clic su **Inviata** nel pannello a sinistra.

   >[!TIP]
   >
   >   L’amministratore del Workfront o del gruppo può personalizzare il modello di layout e rimuovere aree dal menu Principale o dal pannello a sinistra nell’ambiente. In questo caso, potrebbero non essere disponibili.

1. Individuare la richiesta che si desidera copiare e inviare come nuova ed effettuare una delle seguenti operazioni:

   * Selezionala, quindi fai clic su **Copia** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) nell&#39;angolo superiore sinistro dell&#39;elenco Richieste inviate.

   >[!TIP]
   >
   > Se non hai selezionato prima una richiesta, l’icona Copia non è attiva.

   * Fai clic sul menu **Altro** ![](assets/more-icon.png) a destra del nome della richiesta, quindi fai clic su **Copia e invia come nuovo**

     Oppure

     Fare clic con il pulsante destro del mouse sulla richiesta selezionata, quindi scegliere **Copia e invia come nuovo**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Se non disponi dell’accesso per la creazione di problemi, ricevi un avviso che informa che l’amministratore non ti ha consentito di creare richieste.

1. (Facoltativo) Se necessario, aggiorna le seguenti informazioni:

   * **Tipo di richiesta**: la coda di richieste in cui viene salvata la richiesta copiata. Per impostazione predefinita, la richiesta copiata viene salvata nella coda richieste della richiesta originale.
   * **Gruppi di argomenti** e **Argomenti coda**, se selezionati. I nomi o i gruppi di argomenti e gli argomenti della coda vengono personalizzati per l&#39;ambiente in uso. Per impostazione predefinita, la richiesta copiata viene salvata nei gruppi di argomenti e negli argomenti della coda della richiesta originale.

     >[!TIP]
     >
     >Se il percorso cambia rispetto a quello della richiesta originale, l’autore della coda di richieste ha modificato la coda.

1. (Facoltativo) Aggiorna tutte le informazioni della richiesta copiata. A seconda dei campi abilitati dall&#39;autore della coda richieste nella sezione **Nuovi campi problema** della scheda secondaria **Dettagli coda** del progetto, è possibile che siano presenti i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Oggetto</strong> </td> 
      <td>Visualizza il nome della richiesta originale. Se necessario, aggiornala. In caso contrario, Workfront nomina la richiesta copiata <b>Copia di &lt;Nome della richiesta originale&gt;</b>. Questo è un campo obbligatorio.</td> 
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
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crea regole di routing</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ore pianificate</strong> </td> 
      <td> <p>Stimare quante ore occorrerebbe per completare la richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data inizio pianificata</strong> </td> 
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

1. Fai clic su **Invia**.

   La richiesta copiata viene inviata come nuova richiesta nella coda richieste specificata.
