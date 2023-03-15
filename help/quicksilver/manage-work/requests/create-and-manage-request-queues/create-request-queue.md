---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Creare una coda di richiesta
description: È possibile impostare una coda richieste in cui gli utenti possono immettere richieste occasionali non pianificate per un progetto.
author: Alina
feature: Work Management
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '2545'
ht-degree: 2%

---

# Creare una coda di richiesta

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

È possibile impostare una coda richieste in cui gli utenti possono immettere richieste occasionali non pianificate per un progetto. Ad esempio, è possibile impostare una coda di richiesta dell&#39;help desk per acquisire tutte le richieste degli utenti che arrivano a un reparto IT.

## Requisiti di accesso

<!--drafted for P&P: replace the table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere il piano, il tipo di licenza o l&#39;accesso a cui hai accesso, contatta il tuo amministratore Workfront

## Panoramica sulle code di richiesta

Imposta una coda di richiesta come progetto. Quando si designa il progetto come coda di richiesta, la coda diventa accessibile dall’area Richieste di Adobe Workfront. Quando si personalizza la coda di richiesta, si sta anche personalizzando il modulo che gli utenti compilano quando inviano le richieste.

Questo articolo descrive come creare una coda di richiesta da un progetto esistente. Tuttavia, per creare coerenza per il processo di assunzione delle richieste o per aggiungergli più livelli a scopo di reporting e per una migliore gestione, puoi anche configurare ulteriori blocchi predefiniti di una coda di richieste descritti nella tabella seguente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Dettagli coda</td> 
   <td> <p>È necessario impostare un progetto come coda di richiesta nell’area Dettagli coda. Questo passaggio è obbligatorio. </p> <p>Per ulteriori informazioni, consulta la sezione <a href="#create-a-request-queue" class="MCXref xref">Creare una coda di richiesta</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gruppi di argomenti</td> 
   <td> <p>Si tratta di menu aggiuntivi che classificano le richieste in base a funzionalità comuni. Ad esempio, per una coda di richiesta IT, è possibile che si desideri avere gruppi di argomenti "On-site" e "Remote". </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Crea gruppi di argomenti</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Argomenti Coda</td> 
   <td> <p>Si tratta di menu aggiuntivi che classificano le richieste che appartengono allo stesso gruppo di argomenti in base alle funzioni comuni. Un gruppo di argomenti può contenere diversi argomenti della coda. </p> <p>Ad esempio, il gruppo di argomenti "in loco" per la coda richieste IT può contenere gli argomenti relativi alla coda "Hardware", "Software" e "Rete". </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crea argomenti coda</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regole di instradamento</td> 
   <td> <p>Consentono di indirizzare ogni richiesta a un utente, a un ruolo di lavoro, a un team o a un progetto. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di routing</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare una coda di richiesta

Quando si imposta un progetto come coda richieste, lo stato del progetto deve essere Corrente per essere visualizzato nell’area Richieste di Workfront.

Per creare una coda di richiesta:

1. Passa al progetto da impostare come coda di richiesta.
1. (Facoltativo) Fai clic su **Dettagli progetto** nel pannello a sinistra e aggiungi un **Descrizione** al progetto **Panoramica** area. Queste informazioni vengono visualizzate su tutte le nuove richieste.
1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Dettagli coda**.

   Viene visualizzata la sezione Dettagli coda .

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Specifica le seguenti informazioni:

   * **Pubblica come coda richieste di aiuto:** Seleziona questa opzione per identificare il progetto come coda di richiesta. Tutti i problemi in arrivo sono considerati richieste.\
      Quando questa opzione non è selezionata, il progetto si comporta come un progetto standard in Workfront e tutti i problemi in arrivo sono problemi.

   * **Chi può aggiungere richieste a questa coda:** Seleziona gli utenti che hanno accesso per aggiungere richieste a questa coda. È possibile consentire ai seguenti gruppi di persone di visualizzare la coda richieste nell&#39;area Richieste della barra di navigazione globale:

      | Tutti | Qualsiasi utente Workfront con un account attivo può visualizzare questa coda di richiesta e aggiungerle richieste |
      |---|---|
      | Persone con accesso in visualizzazione al progetto | Gli utenti con autorizzazioni di visualizzazione per il progetto possono visualizzare e aggiungere richieste a questa coda |
      | Persone nella società del progetto | Gli utenti che appartengono alla società associata a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se esiste un’azienda associata al progetto, dopo questa impostazione il nome dell’azienda viene elencato tra parentesi. |
      | Persone nel gruppo del progetto | Gli utenti che appartengono al gruppo associato a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se un gruppo è associato al progetto, dopo questa impostazione il nome del gruppo viene elencato tra parentesi. |

      {style="table-layout:auto"}

   * **Condividi con questi collegamenti:** Le seguenti opzioni consentono di fornire accesso diretto alla coda di richiesta e ai moduli ad essa associati a utenti esterni a Workfront o a utenti Workfront che utilizzano una pagina esterna. Per informazioni su come incorporare una coda di richiesta in un dashboard come pagina esterna, consulta [Incorporare una coda di richiesta in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

      Per poter accedere direttamente, gli utenti devono già disporre dei diritti di accesso alla coda richieste. L’utilizzo di una delle due opzioni qui descritte non concede automaticamente l’accesso agli utenti.

      >[!TIP]
      >
      >Gli utenti devono prima accedere a Workfront prima di accedere alla coda di richiesta quando accedono alla pagina Coda di richiesta da un’altra applicazione.

      * **URL di accesso diretto:** Quando un utente accede a questo URL da un browser, l’utente viene portato direttamente alla sezione Nuova richiesta nell’area Richieste e questa richiesta viene selezionata per impostazione predefinita.

         ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

         >[!NOTE]
         >
         >È possibile visualizzare una coda richieste in un dashboard come pagina esterna. In questo caso, la coda di richiesta è preselezionata, ma puoi selezionare qualsiasi altra coda di richiesta dal campo Tipo di richiesta . Gli utenti possono modificare il tipo di richiesta. Vengono visualizzati anche i componenti di navigazione delle Richieste .

      * **Codice di incorporamento:** Utilizza questo codice HTML per incorporare il modulo della coda di richiesta come iframe in qualsiasi pagina HTML.\
         Se gli utenti non sono già autenticati in Workfront quando visualizzano la pagina in cui è incorporato il codice, viene visualizzata la finestra di dialogo di accesso di Workfront. Dopo l’accesso, viene visualizzato il modulo Coda richieste .

         ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

         >[!NOTE]
         Quando si visualizza una coda richieste in un iframe, viene visualizzato solo il modulo di richiesta, il nome della richiesta viene preselezionato e oscurato. L&#39;utente non può modificare il tipo di richiesta. I componenti di navigazione dell’area Richieste non vengono visualizzati.

         Affinché il modulo della coda di richiesta venga visualizzato quando si utilizza questo codice di incorporamento, è necessario abilitare l’impostazione &quot;Consenti incorporamento di Workfront in un iframe&quot; nella configurazione del sistema. Per ulteriori informazioni sull&#39;abilitazione dell&#39;incorporazione di Workfront in un iframe, vedi [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se questa impostazione non è abilitata, l’iframe viene visualizzato come vuoto.

         È possibile regolare vari aspetti della visualizzazione del modulo incorporato, come segue:

         <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funzionalità</strong> </p> </th> 
           <th> <p><strong>Soluzione</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Regolare le dimensioni del frame</p> </td> 
           <td> <p>Modifica gli attributi "larghezza" e "altezza".</p> <p>Per impostazione predefinita, la larghezza è "500" e l'altezza è "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Indirizza gli utenti a un argomento o gruppo di argomenti della coda specifico</p> </td> 
           <td> <p>Aggiungi il parametro "path" all'URL src. Per trovare il parametro del percorso, passare all'argomento o al gruppo di argomenti della coda desiderato nel modulo non incorporato ed esaminare l'URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostra e consente agli utenti di modificare l’elenco a discesa Gruppo di argomenti preconfigurato</p> </td> 
           <td> <p>Usa il parametro "path" aggiungendo il <code>showPreSelectedOptions=true</code> al <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Rileva quando è stato inviato il modulo</p> </td> 
           <td> <p>Aggiungi un listener di eventi "message" alla finestra della pagina web e controlla se <code>event.data.type</code> è <code>requestSubmitted</code>. <code>event.data.newIssueID</code> sarà impostato sull'ID del problema creato.</p> </td> 
          </tr> 
         </tbody> 
        </table>
   * **Tipi di richieste:** Seleziona tra le opzioni predefinite riportate di seguito.

      L’amministratore di Workfront può rinominare i tipi di richiesta predefiniti. Per ulteriori informazioni sulla ridenominazione dei tipi di richiesta, consulta [Personalizzare i tipi di problemi predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Cambia ordine
      * Problema
      * Richieste
      * Rischio

         Questo campo è obbligatorio ed è necessario selezionare almeno un’opzione.
      >[!NOTE]
      I tipi di richiesta vengono visualizzati come selezione nell&#39;area Richieste solo se il tipo di richiesta è selezionato nelle pagine Dettagli coda e Argomento coda. Per informazioni sulla configurazione dell&#39;area Dettagli coda di un progetto, consulta [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Ogni tipo selezionato sarà disponibile nel modulo (è possibile selezionarne più di uno). Selezionando più di un tipo di dati è possibile organizzare più richieste in arrivo.\
      Ad esempio, se utilizzi il modulo su una coda di richiesta per un progetto IT, i seguenti tipi di richiesta possono entrare nella coda: hardware, software, correzioni di bug e problemi.

   * **Durata predefinita:** La durata predefinita corrisponde al periodo di tempo normalmente necessario per completare un problema. Questo diventa il valore predefinito per tutti i problemi in arrivo e può essere modificato manualmente. La durata è generalmente impostata in ore, giorni o settimane. La durata predefinita di un problema è la stessa delle ore pianificate sul problema. La data di completamento pianificata dell&#39;emissione viene calcolata in base a questo campo.\
      Il valore predefinito per il problema Durata è 1 giorno o 8 ore. Se l’amministratore di Workfront imposta l’orario tipico per giorno lavorativo su meno di 8 ore, la durata predefinita dei problemi è ancora di 8 ore. Ad esempio, se l’opzione Ore tipiche per giorno lavorativo è impostata su 7 ore, la durata predefinita per i problemi è di 1,14 giorni o 8 ore. Per ulteriori informazioni su come impostare il sistema Ore tipiche per giorno di lavoro, consulta la sezione &quot;Calcoli Timeline&quot; nell’articolo [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste.:** Quando questa opzione è selezionata, tutte le richieste inviate alla coda sono visibili per gli utenti della stessa azienda. Gli utenti possono visualizzare queste richieste nella sezione Tutte le richieste , che si trova all’interno dell’area Richieste . Quando questa impostazione è abilitata o disabilitata, influisce su tutte le richieste future; non influisce retroattivamente sulle informazioni.
   * **Quando qualcuno effettua una richiesta, concede automaticamente:** Quando un utente effettua una richiesta alla coda di richiesta, all&#39;utente viene automaticamente concesso il livello di autorizzazione scelto per tale richiesta. Seleziona uno dei seguenti livelli di autorizzazione:\
      **- Visualizza**

      **- contribuire**
      **- Gestisci**

      Per informazioni sul modello di autorizzazioni Workfront, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
      L’impostazione delle autorizzazioni in questo caso consente di risparmiare tempo, anziché concedere autorizzazioni per ogni singola richiesta in arrivo. La scelta di questa opzione interessa tutte le richieste future, ma non influisce retroattivamente sulle richieste esistenti.

   * **Approvazione predefinita**: Associa un processo di approvazione a questa coda di richiesta. Solo i processi di approvazione dei problemi sono visibili in questo menu a discesa. Tutti i problemi inviati a questa coda saranno associati al processo di approvazione. Prima di poter essere associati alle code di richiesta, l’amministratore di Workfront deve definire i processi di approvazione a livello di sistema. Gli utenti con accesso amministrativo ai processi di approvazione possono anche creare processi di approvazione specifici per gruppo.

      >[!IMPORTANT]
      Se il gruppo del progetto cambia, il processo di approvazione specifico per gruppo allegato ai problemi esistenti diventa un processo di approvazione a uso singolo. Per ulteriori informazioni su come le modifiche apportate al gruppo del progetto o al processo di approvazione influiscono sulle impostazioni di approvazione, vedere [Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

      Se a una coda di richiesta sono associati più argomenti della coda, è consigliabile associare i processi di approvazione agli argomenti della coda. Per ulteriori informazioni sulla creazione degli argomenti della coda, vedi [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Quando si aggiungono processi di approvazione alle code di richiesta, tenere presente quanto segue:

      * Nell’elenco vengono visualizzati solo i processi di approvazione attivi.
      * Nell&#39;elenco vengono visualizzati i processi di approvazione a livello di sistema e di gruppo. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.
   * **Percorso predefinito**: Associa una regola di instradamento a questa coda di richiesta. Utilizzare le regole di instradamento per assegnare automaticamente i nuovi problemi inviati a una coda richieste alla risorsa corretta (utente, ruolo o team) e al progetto corretto. Tutti i problemi inviati a questa coda saranno associati a questa regola di routing. È necessario configurare le regole di instradamento prima di poterle associare alla coda di richiesta.\
      Se a una coda di richiesta sono associati più argomenti della coda, è consigliabile associare le regole di routing agli argomenti della coda. Per ulteriori informazioni sulla creazione di regole di routing, vedere [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nuovi campi problema:** Nella sezione Mostra i campi selezionati seguenti a tutti gli utenti , seleziona i campi che desideri rendere visibili a tutti gli utenti che inviano una richiesta al progetto o aggiungono un problema al progetto o alle attività.

      >[!TIP]
      I nuovi campi problema selezionati nella sezione Dettagli coda sono associati anche a qualsiasi nuovo problema aggiunto al progetto o alle attività nella sezione Problemi.

      Quando si abilita uno dei campi Assegnato a, Ruolo lavoro o Team, questi vengono sempre rinominati Assegnazioni nel modulo di richiesta, ma è possibile specificare solo il tipo di assegnazione selezionato qui.

      **Esempio:** Se è stata selezionata l’opzione Assegnato a nell’area Dettagli coda, è possibile immettere solo gli utenti nel campo Assegnazioni del modulo di richiesta. In questo caso, non è possibile inserire ruoli di lavoro o un team.

   * **Documenti**: Se si sceglie di visualizzare la sezione Documenti nel nuovo modulo di richiesta, selezionare il percorso in cui posizionare la sezione di caricamento del documento. Seleziona una delle seguenti opzioni:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Dopo i moduli personalizzati</td> 
        <td><span>La sezione Documenti viene visualizzata nella parte inferiore del modulo di richiesta.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Prima dei moduli personalizzati</td> 
        <td> <p><span>La sezione Documenti viene visualizzata tra i campi Workfront e i campi personalizzati del modulo di richiesta.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

      ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostra tutti i campi selezionati e non selezionati in:** Selezionare gli utenti a cui si desidera visualizzare tutti i campi del modulo. Le opzioni seguenti controllano l’accesso ai campi del modulo.

      | Tutti gli utenti (pianificazione licenze) | Tutti gli utenti con una licenza Plan possono visualizzare i campi selezionati e quelli non selezionati. |
      |---|---|
      | Persone con accesso di visualizzazione al progetto (licenza Pianificazione) | Gli utenti con una licenza di piano che dispongono anche dei diritti di visualizzazione per questo progetto possono visualizzare i campi selezionati e quelli non selezionati. Gli altri utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. |
      | Nessun utente | Nessun utente può visualizzare i campi non selezionati. Tutti gli utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. |

      {style="table-layout:auto"}

   * **Forms personalizzato**: Selezionare un modulo personalizzato da associare alla coda richieste. È disponibile solo Issue Custom Forms da selezionare da questo menu a discesa. A tutti i problemi inviati alla coda di richiesta verranno associati i moduli selezionati.\
      Se a una coda di richieste sono associati più argomenti della coda, è consigliabile associare i moduli personalizzati agli argomenti della coda. Per ulteriori informazioni sulla creazione di sottosezioni per la coda richieste, vedi [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Se sono presenti più moduli personalizzati associati alla coda di richiesta, trascinarli e rilasciarli per ordinarli nell’ordine desiderato nella **Riordina Forms** sezione .

      >[!TIP]
      I moduli personalizzati aggiunti alla sezione Dettagli coda sono associati anche a qualsiasi nuovo problema aggiunto al progetto o alle attività nella sezione Problemi .

   * **Consenti l’aggiunta di problemi tramite e-mail:** Seleziona questa opzione per consentire l’invio delle richieste tramite e-mail.\
      Per ulteriori informazioni, consulta [Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).




1. Fai clic su **Salva**.\
   Il progetto è ora configurato come coda di richiesta e gli utenti possono aggiungere richieste.

1. (Facoltativo) Per migliorare la funzionalità Coda richieste , crea ulteriori sottosezioni per la coda, nonché regole per indirizzare le richieste in arrivo al team, all’assegnatario o al progetto corretti.

   Per informazioni sulla creazione di sottosezioni per la coda richieste, vedere gli articoli [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) e [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).\
   Per informazioni su come indirizzare le richieste all&#39;assegnatario, al team e al progetto appropriato, consulta [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
