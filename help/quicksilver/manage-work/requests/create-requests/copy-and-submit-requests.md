---
title: Copia e invia richieste
description: Copia e invia richieste
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Copia e invia richieste

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

Quando si inviano spesso richieste simili, è possibile copiare una richiesta inviata esistente. In questo caso, puoi copiare una richiesta esistente, apportarvi modifiche minime e inviarla nuovamente come nuova richiesta.

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
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso all’aggiunta di richieste a una coda di richiesta</p> <p>Visualizza o autorizzazioni superiori per la richiesta esistente</p> <p>Per informazioni sulla configurazione di una coda di richiesta, vedi <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Devi ricevere una richiesta inviata in precedenza da te o da un utente dell’organizzazione per poterla copiare e inviare nuovamente. Se la richiesta appartiene a un altro utente, è necessario disporre almeno dell’accesso a Visualizza per poterlo copiare e inviare come nuovo.

## Considerazioni sulla copia e l’invio delle richieste come nuove

* È possibile solo copiare e inviare le richieste inviate. Non è possibile copiare le richieste di bozza.
* È possibile copiare e inviare le richieste inviate originariamente, o le richieste inviate da altri utenti e a cui si ha accesso almeno a Visualizza.
* Puoi sempre accedere a copiare e inviare una copia delle tue richieste, a meno che qualcuno non abbia rimosso le tue autorizzazioni.
* L’accesso alle richieste di copia e invio originariamente inviate da altri potrebbe essere concesso automaticamente alle persone della stessa azienda quando l’autore della coda di richiesta abilita **Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste** nelle aree Dettagli coda o Modifica progetto. La disattivazione di questa impostazione consente solo al richiedente originale di visualizzare le proprie richieste.

   Per ulteriori informazioni, consulta i seguenti articoli:

   * [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md)

* È possibile aggiornare la copia della richiesta originale prima di inviarla nuovamente come nuova richiesta.
* Se dopo l’invio della richiesta originale si verificano le seguenti modifiche, non è più possibile copiarla e inviarla nuovamente:

   * La coda di richiesta è stata eliminata.
   * L&#39;argomento della coda è stato eliminato.

      >[!TIP]
      >
      >Se l’argomento della coda era l’unico nella coda delle richieste, è comunque possibile copiare e inviare la richiesta e verrà salvato nella coda delle richieste stessa.

   * La coda di richiesta non viene più pubblicata come coda di richiesta della Guida in linea. Per informazioni, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Se la coda di richiesta non ha un argomento della coda e la richiesta originale è stata inviata prima di gennaio 2022.

   * Lo stato del progetto associato alla coda di richiesta non è più Corrente.

* Puoi copiare e inviare una copia di una richiesta convertita se la richiesta è stata mantenuta nel processo di conversione. Per ulteriori informazioni, consulta [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >La richiesta copiata non è collegata a un oggetto di risoluzione.

## Copia e invia richieste

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Richieste**.
1. (Condizionale) Se la sezione Inviata non viene visualizzata per impostazione predefinita, fare clic su **Inviato** nel pannello a sinistra.
1. Individua la richiesta da copiare e inviare come nuova ed effettua una delle seguenti operazioni:

   * Selezionala, quindi fai clic sul pulsante **Copia e invia come nuovo** icona ![](assets/copy-and-submit-as-new-requests-area-nwe.png) nell’angolo in alto a sinistra dell’elenco Richieste inviate.
   * Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome della richiesta, quindi fai clic su **Copia e invia come nuovo**

      Oppure

      Fai clic con il pulsante destro del mouse sulla richiesta selezionata, quindi fai clic su **Copia e invia come nuovo**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >Se non si dispone dell’accesso per la creazione di problemi, viene visualizzato un avviso che informa che l’amministratore ha impedito la creazione di richieste.

1. (Facoltativo) Se necessario, aggiorna le seguenti informazioni:

   * **Tipo di richiesta**: la coda di richiesta in cui viene salvata la richiesta copiata. Per impostazione predefinita, la richiesta copiata viene salvata nella coda di richiesta della richiesta originale.
   * **Gruppi di argomenti** e **Argomenti coda**, se sono selezionati. I nomi o i gruppi di argomenti e gli argomenti della coda sono personalizzati per il tuo ambiente. Per impostazione predefinita, la richiesta copiata viene salvata nei gruppi di argomenti e negli argomenti della coda della richiesta originale.

      >[!TIP]
      >
      >Se il percorso cambia dal percorso della richiesta originale, l&#39;autore della coda di richiesta ha modificato la coda.

1. (Facoltativo) Aggiorna tutte le informazioni dalla richiesta copiata. A seconda dei campi abilitati dall’autore della coda di richiesta in **Nuovi campi problema** della sezione **Dettagli coda** nella sottoscheda del progetto è possibile trovare uno dei campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Oggetto</strong> </td> 
      <td>Visualizza il nome della richiesta originale. Se necessario, aggiornalo. In caso contrario, Workfront assegna un nome alla richiesta copiata <b>Copia di &lt;name of="" original="" request=""&gt;</b>. Questo campo è obbligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Visualizza la descrizione della richiesta originale. Se necessario, aggiornalo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Visualizza l’URL della richiesta originale. Se necessario, aggiornalo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorità</strong> </td> 
      <td> <p>Specifica la priorità della richiesta. La priorità dovrebbe definire la velocità con cui si ritiene che questa richiesta debba essere risolta. Le opzioni predefinite sono:</p> 
       <ul> 
        <li>Nessuno</li> 
        <li>Basso</li> 
        <li>Normal</li> 
        <li>Alta</li> 
        <li>Urgente</li> 
       </ul> <p>Il tuo amministratore Workfront può modificare i nomi delle priorità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravità</strong> </td> 
      <td> <p>Specifica la gravità della richiesta. La gravità deve definire l'impatto che questa richiesta ha sul tuo lavoro se non viene risolta in tempo. Le opzioni predefinite sono:</p> 
       <ul> 
        <li>Cosmetico</li> 
        <li>Causa Confusione</li> 
        <li>Bug con workaround</li> 
        <li>Bug senza workaround</li> 
        <li>Errore Fatale</li> 
       </ul> <p>L’amministratore di Workfront può modificare i nomi delle severità.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contatto principale</strong> </td> 
      <td>Per impostazione predefinita, il contatto principale di una richiesta viene contattato automaticamente, in quanto tu sei la persona che punta a rispondere a qualsiasi domanda relativa alla richiesta. Tuttavia, è possibile modificare questo valore in qualsiasi altro utente Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Assegnazioni</strong></span> </td> 
      <td> <p>Indicare il nome di un utente attivo, di un ruolo o di un team a cui deve essere assegnata la richiesta. </p> <p> È possibile specificare più di un utente, un ruolo o un team. </p> <p>A seconda della configurazione della coda di richiesta, è possibile assegnare la richiesta a uno o due tipi di risorse, anziché a tutti e tre. </p> <p>È consigliabile utilizzare le regole di routing per le code di richieste in modo che possano essere instradate automaticamente alle risorse appropriate. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">A seconda della configurazione della coda di richiesta, potrebbe essere possibile assegnare alla richiesta un solo tipo di risorsa (ad esempio, utenti). Se una regola di instradamento è associata anche alla coda di richiesta e instrada automaticamente la richiesta a un tipo diverso di risorsa (ad esempio, un team), la richiesta viene assegnata sia all'entità specificata manualmente durante l'invio della richiesta (utenti) sia alla risorsa specificata nella regola di instradamento (team).</p> <p style="font-weight: normal;">Per ulteriori informazioni, consulta i seguenti articoli:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di routing</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Lavoro Necessario</strong> </td> 
      <td> <p>Stimare quante ore sono necessarie per il completamento della richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di inizio pianificata</strong> </td> 
      <td> <p>Data di inizio del lavoro su questa richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data di completamento Pianificata</strong> </td> 
      <td>Data in cui si desidera risolvere la richiesta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Stato</strong> </td> 
      <td>Lo stato predefinito di una nuova richiesta è "Nuovo". Il nome di questo stato potrebbe essere stato modificato dall’amministratore di Workfront. È inoltre possibile modificare lo stato impostandolo su un'altra opzione nel menu a discesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documenti</strong> </td> 
      <td> <p>Aggiungi i documenti alla tua richiesta. I documenti allegati alla richiesta originale non vengono trasferiti alla richiesta copiata.</p> <p><b>SUGGERIMENTO</b>

   A seconda di come è stata impostata la coda di richiesta, la sezione Documenti potrebbe essere visualizzata prima o dopo i campi personalizzati.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Se necessario, è possibile aggiornare le informazioni contenute nei moduli personalizzati allegati.

   >[!TIP]
   >
   >* Tutti i moduli personalizzati allegati alla richiesta originale e i valori inclusi nei campi personalizzati vengono trasferiti alla richiesta copiata. Sono inclusi i campi che contengono logica.
   >* Non è possibile rimuovere moduli personalizzati dalla richiesta copiata.


1. Fai clic su **Invia**.

   La richiesta copiata viene inviata come nuova richiesta nella coda di richiesta specificata.
