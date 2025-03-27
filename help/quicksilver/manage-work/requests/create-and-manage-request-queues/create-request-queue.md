---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Creare una coda di richieste
description: Puoi impostare una coda di richieste in cui gli utenti possono immettere richieste occasionali che non sono pianificate per lavorare su un progetto. Ad esempio, è possibile impostare una coda di richieste dell'helpdesk per acquisire tutte le richieste degli utenti inviate a un reparto IT.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '5167'
ht-degree: 2%

---


# Creare una coda di richieste

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Puoi impostare una coda di richieste in cui gli utenti possono immettere richieste occasionali che non sono pianificate per lavorare su un progetto. Ad esempio, è possibile impostare una coda di richieste dell&#39;helpdesk per acquisire tutte le richieste degli utenti inviate a un reparto IT.

Le richieste diventano problemi in Adobe Workfront e vengono aggiunte ai progetti.

L’impostazione di una coda di richieste consente di formalizzare le informazioni sui problemi che verranno aggiunti a un progetto. Tutti i problemi inviati al progetto saranno inviati nello stesso modo e seguiranno lo stesso percorso fino al completamento.

È possibile impostare i seguenti oggetti come code di richieste in Workfront:

* Progetti
* Modelli. I progetti creati da modelli impostati come code di richieste diventeranno code di richieste.

Per impostare un progetto o un modello come coda di richieste, è necessario modificare l&#39;area Dettagli coda del progetto o del modello.

Questo articolo descrive come configurare un progetto come coda di richieste in cui gli utenti possono inviare le richieste. L’impostazione dei dettagli della coda per un modello è simile all’impostazione nel progetto.

Per informazioni su come inviare una nuova richiesta a una coda di richieste, vedere [Copia e invia richieste](../create-requests/copy-and-submit-requests.md).

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
   <td> 
   <p>Nuova licenza: Standard </p>
   Oppure
   <p>Licenza corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestire le autorizzazioni per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica delle code di richieste

Puoi impostare una coda di richieste come progetto. Quando si designa il progetto come Coda richieste, la coda diventa accessibile dall&#39;area Richieste di Adobe Workfront. Quando personalizzi la Coda richieste, puoi anche personalizzare il modulo che gli utenti compilano quando inviano le richieste.

Questo articolo descrive come creare una coda di richieste da un progetto esistente. Tuttavia, per garantire la coerenza del processo di acquisizione delle richieste o per aggiungervi più livelli a scopo di reporting e per una migliore gestione, puoi anche configurare blocchi predefiniti aggiuntivi di una coda di richieste, descritti nella tabella seguente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Dettagli coda</td> 
   <td> <p>È necessario impostare un progetto come coda di richieste nell'area Dettagli coda. Questo passaggio è obbligatorio. </p> <p>Per ulteriori informazioni, vedere la sezione <a href="#create-a-request-queue" class="MCXref xref">Creare una coda di richieste</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gruppi di argomenti</td> 
   <td> <p>Si tratta di menu aggiuntivi che classificano le richieste in base alle funzioni comuni. Ad esempio, per una coda di richieste IT, potrebbe essere necessario disporre di gruppi di argomenti "On-Site" e "Remote". </p> <p>Per ulteriori informazioni, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Creare gruppi di argomenti</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Argomenti Coda</td> 
   <td> <p>Si tratta di menu aggiuntivi che classificano le richieste che appartengono allo stesso Gruppo di argomenti in base alle funzioni comuni. Un gruppo di argomenti può contenere diversi argomenti della coda. </p> <p>Ad esempio, il gruppo di argomenti "On-site" per la coda di richieste IT può contenere gli argomenti "Hardware", "Software" e "Rete". </p> <p>Per ulteriori informazioni, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Creare argomenti coda</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regole di instradamento</td> 
   <td> <p>Ti consentono di indirizzare ogni richiesta a un utente, una mansione, un team o a un progetto. </p> <p>Per ulteriori informazioni, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Creare regole di routing</a>. </p> <p>Questo è facoltativo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare una coda di richieste

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

La creazione di una coda di richieste varia a seconda dell’ambiente utilizzato.

### Creare una coda di richieste nell’ambiente di produzione

In questa sezione viene descritto come definire i dettagli della coda per i seguenti oggetti:

* Un progetto nell’ambiente di produzione
* Un modello nell’ambiente di produzione o di anteprima

Quando imposti un progetto come Coda richieste, per poter essere visualizzato nell’area Richieste di Workfront lo stato del progetto deve essere Corrente.

>[!TIP]
>
>L&#39;amministratore del Workfront o del gruppo potrebbe assegnare l&#39;utente a un modello di layout personalizzato che potrebbe non includere alcune delle sezioni descritte nei passaggi seguenti.


Per creare una coda di richieste:

1. Passare al progetto che si desidera impostare come coda di richieste.
1. (Facoltativo) Fai clic su **Dettagli progetto** nel pannello a sinistra e aggiungi una **Descrizione** al progetto nell&#39;area **Panoramica**. Queste informazioni vengono visualizzate in tutte le nuove richieste.
1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Dettagli coda**.

   Verrà aperta la sezione Dettagli coda.

   ![Dettagli coda nella parte superiore della sezione](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Specifica le seguenti informazioni:

   * **Pubblica come coda di richieste della Guida:** Selezionare questa opzione per identificare il progetto come coda di richieste. Tutti i problemi in arrivo vengono considerati richieste.\
     Se questa opzione non è selezionata, il progetto si comporta come un progetto standard in Workfront e tutti i problemi in arrivo sono problemi.

   * **Utenti autorizzati ad aggiungere richieste alla coda:** Selezionare gli utenti autorizzati ad aggiungere richieste alla coda. Puoi consentire ai seguenti gruppi di persone di visualizzare la Coda richieste nell’area Richieste della barra di navigazione globale quando aggiungono una nuova richiesta:

     | Chi può inserire le richieste | Descrizione |
     |---|---|
     | Tutti | Qualsiasi utente di Workfront con un account attivo può visualizzare questa coda di richieste e aggiungervi richieste |
     | Persone con accesso in visualizzazione al progetto | Gli utenti con autorizzazioni di visualizzazione per il progetto possono visualizzare e aggiungere richieste a questa coda |
     | Persone nella società del progetto | Gli utenti che appartengono alla società associata a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se al progetto è associata una società, il nome della società viene elencato tra parentesi dopo questa impostazione. |
     | Persone nel gruppo del progetto | Gli utenti che appartengono al gruppo associato a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se al progetto è associato un gruppo, dopo questa impostazione il nome del gruppo viene elencato tra parentesi, in caratteri grigi. |

     {style="table-layout:auto"}

   * **Condividi con questi collegamenti:** Le opzioni seguenti consentono di fornire l&#39;accesso diretto alla coda richieste e ai moduli ad essa associati a utenti esterni a Workfront o a utenti Workfront che utilizzano una pagina esterna. Per informazioni sull&#39;incorporamento di una coda richieste in un dashboard come pagina esterna, vedere [Incorporare una coda richieste in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Per poter accedere direttamente, gli utenti devono già disporre dei diritti di accesso alla coda richieste. L’utilizzo di una delle opzioni descritte qui non concede automaticamente l’accesso agli utenti.

     >[!TIP]
     >
     >Gli utenti devono prima accedere a Workfront prima di poter accedere alla coda richieste quando accedono alla pagina Coda richieste da un’altra applicazione.

      * **URL di accesso diretto:** Quando un utente accede a questo URL da un browser, viene reindirizzato direttamente alla sezione Nuova richiesta nell&#39;area Richieste e questa richiesta viene selezionata per impostazione predefinita.

        ![Condividi coda richieste con URL diretto incorporato nel dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >È possibile visualizzare una coda di richieste in un dashboard come pagina esterna. In questo caso, la coda di richieste è preselezionata, ma puoi selezionare qualsiasi altra coda di richieste dal campo Tipo di richiesta. Gli utenti possono modificare il Tipo di richiesta. Vengono visualizzati anche i componenti Navigazione delle richieste.

      * **Codice di incorporamento:** Utilizza questo codice HTML per incorporare il modulo della coda di richieste come iframe in qualsiasi pagina HTML.\
        Se gli utenti non sono già autenticati in Workfront quando visualizzano la pagina in cui è incorporato il codice, viene visualizzata la finestra di dialogo Accesso a Workfront. Dopo che gli utenti effettuano l&#39;accesso, viene visualizzato il modulo Coda richieste.

        >[!NOTE]
        >
        >Quando si visualizza una coda di richieste in un iframe, viene visualizzato solo il modulo di richiesta e il nome della richiesta viene preselezionato e oscurato. L’utente non può modificare il tipo di richiesta. I componenti di navigazione dell’area Richieste non vengono visualizzati.

        Per poter visualizzare il modulo della coda di richieste quando si utilizza questo codice di incorporamento, è necessario abilitare l’impostazione &quot;Consenti incorporamento di Workfront in un iframe&quot; nella configurazione del sistema. Per ulteriori informazioni sull&#39;abilitazione dell&#39;incorporamento di Workfront in un iframe, vedere [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se questa impostazione non è abilitata, l’iframe viene visualizzato come vuoto.

        È possibile regolare vari aspetti della visualizzazione del modulo incorporato, come indicato di seguito:

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
           <td> <p>Regola le dimensioni del frame</p> </td> 
           <td> <p>Modificate gli attributi "width" e "height".</p> <p>Per impostazione predefinita, la larghezza è "500" e l’altezza è "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Indirizza gli utenti a un argomento della coda o a un gruppo di argomenti specifico</p> </td> 
           <td> <p>Aggiungi il parametro "path" all’URL src. Per trovare il parametro path, vai all’argomento della coda o al gruppo di argomenti desiderati nel modulo non incorporato e controlla l’URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostra e consenti agli utenti di modificare l'elenco a discesa Gruppo di argomenti preconfigurato</p> </td> 
           <td> <p>Utilizzare il parametro "path" aggiungendo il parametro <code>showPreSelectedOptions=true</code> a <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Rileva quando il modulo è stato inviato</p> </td> 
           <td> <p>Aggiungere un listener di eventi "message" alla finestra della pagina Web e verificare se <code>event.data.type</code> è <code>requestSubmitted</code>. <code>event.data.newIssueID</code> verrà impostato sull'ID del problema creato.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Tipi di richiesta:** Selezionare una delle opzioni predefinite seguenti.

     L’amministratore di Workfront può rinominare i tipi di richiesta predefiniti. Per ulteriori informazioni sulla ridenominazione dei tipi di richiesta, vedere [Personalizzare i tipi di problemi predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Segnalazione Bug
      * Richiesta di Modifica
      * Problema
      * Richiesta

        Questo campo è obbligatorio ed è necessario selezionare almeno un&#39;opzione.

     >[!NOTE]
     >
     >I Tipi di richiesta vengono visualizzati come selezione nell&#39;area Richieste solo se il Tipo di richiesta è selezionato sia nelle pagine Dettagli coda che Argomento coda. Per informazioni sulla configurazione dell&#39;area Dettagli coda di un progetto, vedere [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Ogni tipo selezionato qui sarà disponibile nel modulo (è possibile selezionarne più di uno). Selezionando più di un tipo è possibile organizzare più richieste in arrivo.\
     Ad esempio, se utilizzi il modulo in una coda di richieste per un progetto IT, possono essere messi in coda i seguenti tipi di richieste: hardware, software, correzioni di bug e problemi.

   * **Durata predefinita:** La durata predefinita corrisponde al tempo necessario per completare un problema. Questa impostazione diventa predefinita per tutti i problemi in arrivo e può essere modificata manualmente. La durata è generalmente impostata in ore, giorni o settimane. La durata predefinita di un problema è la stessa delle ore pianificate sul problema. La Data di completamento pianificata del problema viene calcolata in base a questo campo.\
     Il valore predefinito per la Durata del problema è 1 giorno o 8 ore. Se l’amministratore di Workfront ha impostato le ore tipiche per giornata lavorativa su meno di 8 ore, la durata predefinita dei problemi è ancora di 8 ore. Ad esempio, se l’opzione Ore tipiche per giorno lavorativo è impostata su 7 ore, la durata predefinita per i problemi è 1,14 giorni o 8 ore. Per ulteriori informazioni su come impostare il sistema Ore tipiche per giorno lavorativo, vedere la sezione &quot;Calcoli sequenza temporale&quot; nell&#39;articolo [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste.:** Se selezionata, tutte le richieste inviate alla coda sono visibili per gli utenti della stessa società. Gli utenti possono visualizzare queste richieste nella sezione Tutte le richieste , che si trova nell’area Richieste. Quando questa impostazione viene abilitata o disabilitata, influisce su tutte le richieste future; non influisce retroattivamente sulle informazioni.
   * **Quando un utente effettua una richiesta, concede automaticamente:** Quando un utente effettua una richiesta alla coda richieste, all&#39;utente viene concesso automaticamente il livello di autorizzazione scelto per tale richiesta. Seleziona tra i seguenti livelli di autorizzazione:

      * **Accesso visualizzazione**
      * **Accesso a Contribute**. Questa è la selezione predefinita.
      * **Gestisci accesso**

     Per informazioni sul modello di autorizzazioni di Workfront, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     L’impostazione delle autorizzazioni qui consente di risparmiare tempo, anziché dover concedere le autorizzazioni per ogni singola richiesta in ingresso. La scelta di questa opzione influisce su tutte le richieste future, ma non su quelle esistenti in modo retroattivo.

   * **Approvazione predefinita**: associa un processo di approvazione a questa coda di richieste. In questo menu a discesa sono visibili solo i processi di approvazione del problema. Tutti i problemi inviati a questa coda saranno associati a questo processo di approvazione. Prima di poter associare i processi di approvazione a livello di sistema alle code di richieste, l&#39;amministratore di Workfront deve definirli. Gli utenti con accesso amministrativo ai processi di approvazione possono inoltre creare processi di approvazione specifici per il gruppo.

     >[!IMPORTANT]
     >
     >Se il gruppo del progetto cambia, il processo di approvazione specifico del gruppo associato ai problemi esistenti diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche al processo di approvazione influiscono sulle impostazioni di approvazione, vedere [Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Se a una coda di richieste sono associati più argomenti della coda, è consigliabile associare i processi di approvazione agli argomenti della coda. Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Creare argomenti della coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Quando si aggiungono processi di approvazione alle code di richieste, tenere presente quanto segue:

      * Nell&#39;elenco vengono visualizzati solo i processi di approvazione attivi.
      * I processi di approvazione a livello di sistema e di gruppo vengono visualizzati nell’elenco. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.

   * **Route predefinita**: associa una regola di routing a questa coda di richieste. Utilizzare le regole di instradamento per assegnare automaticamente i nuovi problemi inviati a una coda richieste alla risorsa corretta (utente, mansione o team) e al progetto corretto. Tutti i problemi inviati a questa coda saranno associati a questa regola di indirizzamento. È necessario configurare le Regole di routing prima che vengano visualizzate nella sezione Dettagli coda e prima di associarle alla coda di richieste.\
     Se a una coda di richieste sono associati più argomenti della coda, è consigliabile associare le regole di routing agli argomenti della coda. Per ulteriori informazioni sulla creazione di regole di routing, vedere [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nuovi campi problema:** Nella sezione **Mostra i campi selezionati seguenti a tutti gli utenti**, seleziona i campi che desideri rendere visibili a tutti gli utenti che inviano una richiesta al progetto o aggiungono un problema al progetto o alle attività.

     >[!TIP]
     >
     >I campi dei nuovi problemi selezionati nella sezione Dettagli coda sono associati anche a qualsiasi nuovo problema aggiunto al progetto <!--this is confusing: or to the tasks in the Issues section-->.

     Quando si abilita uno dei campi Assegnato a, Mansione o Team, questi vengono sempre rinominati in Assegnazioni nel modulo di richiesta, ma è possibile specificare solo il tipo di assegnazione selezionato qui.

     >[!NOTE]
     >
     >Se è stata selezionata l&#39;opzione Assegnato a nell&#39;area Dettagli coda, è possibile immettere solo gli utenti nel campo Assegnazioni del modulo di richiesta. In questo caso, non è possibile immettere mansioni o un team.

   * **Documenti**: se si sceglie di visualizzare la sezione Documenti nel nuovo modulo di richiesta, selezionare la posizione della sezione di caricamento del documento. Selezionare una delle opzioni seguenti:

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
        <td> <p><span>La sezione Documenti viene visualizzata tra i campi di Workfront e i campi personalizzati del modulo di richiesta.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Area nuovi campi problema con documenti](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostra tutti i campi selezionati e non selezionati in:** Selezionare gli utenti che si desidera visualizzare tutti i campi nel nuovo modulo di richiesta. Le opzioni seguenti controllano l&#39;accesso ai campi del modulo.

     | Quali utenti possono visualizzare tutti i campi nel modulo di richiesta | Descrizione |
     |---|---| 
     | Tutti gli utenti (Full License) | Tutti gli utenti che dispongono di una licenza Pianificazione possono visualizzare i campi selezionati e non selezionati. |
     | Persone con accesso di visualizzazione al progetto (licenza Pianificazione) | Gli utenti con una licenza Pianificazione che dispongono anche dei diritti di visualizzazione per questo progetto possono visualizzare i campi selezionati e non selezionati. Gli altri utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. |
     | Nessun utente | Nessun utente può visualizzare i campi non selezionati. Tutti gli utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. |

   * **Forms personalizzato**: selezionare un modulo personalizzato da associare alla coda richieste. Da questo menu a discesa è disponibile solo Issue Custom Forms (Problema personalizzato). A tutti i problemi inviati alla coda richieste verranno associati i moduli selezionati. È necessario creare moduli personalizzati per problemi prima di visualizzarli nella sezione Dettagli coda.
Se a una coda di richieste sono associati più argomenti coda, è consigliabile associare i moduli personalizzati agli argomenti coda. Per ulteriori informazioni sulla creazione di sottosezioni per la coda richieste, vedere [Creare argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Moduli personalizzati nei dettagli coda](assets/custom-forms-on-queue-details.png)

     Se alla coda richieste sono associati più moduli personalizzati, trascinarli e rilasciarli per ordinarli nell&#39;ordine desiderato nella sezione **Riordina Forms**.

     >[!TIP]
     >
     >I moduli personalizzati aggiunti alla sezione Dettagli coda sono associati anche a qualsiasi nuovo problema aggiunto al progetto <!--this is confusiong: or the tasks in the Issues  section-->.

1. Continua a selezionare le informazioni per le impostazioni nell&#39;area **Impostazioni coda e-mail**, per consentire agli utenti di inviare richieste e-mail al progetto della coda richieste.

   Per ulteriori informazioni, vedere [Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Fai clic su **Salva**.\
   Il progetto è ora configurato come coda di richieste e gli utenti possono aggiungervi richieste.

1. (Facoltativo) Per migliorare la funzionalità Coda richieste, crea sottosezioni aggiuntive per la coda, nonché regole per instradare le richieste in arrivo al team, all’assegnatario o al progetto corretto.

   * Per informazioni sulla creazione di sottosezioni per la coda richieste, vedere gli articoli [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) e [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Per informazioni sull&#39;instradamento delle richieste all&#39;assegnatario, al team e al progetto appropriati, vedere [Creare regole di instradamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

<div class="preview">

### Creare una coda di richieste nell’ambiente di anteprima

Quando imposti un progetto come Coda richieste, per poter essere visualizzato nell’area Richieste di Workfront lo stato del progetto deve essere Corrente.

>[!TIP]
>
>L&#39;amministratore del Workfront o del gruppo potrebbe assegnare l&#39;utente a un modello di layout personalizzato che potrebbe non includere alcune delle sezioni descritte nei passaggi seguenti.

Per creare una coda di richieste:

1. Passare al progetto che si desidera impostare come coda di richieste.
1. (Facoltativo) Fai clic su **Dettagli progetto** nel pannello a sinistra e aggiungi una **Descrizione** al progetto nell&#39;area **Panoramica**. Queste informazioni vengono visualizzate in tutte le nuove richieste.
1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Dettagli coda**.

   Verrà aperta la sezione Dettagli coda.

   ![Sezione Tipo di coda nell&#39;area Dettagli coda](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Specifica le seguenti informazioni:

   * **Pubblica come coda di richieste della Guida**: selezionare questa opzione per identificare il progetto come coda di richieste. Tutti i problemi in arrivo vengono considerati richieste.\
     Se questa opzione non è selezionata, il progetto si comporta come un progetto standard in Workfront e tutti i problemi in arrivo sono problemi.

   * **Chi può aggiungere richieste a questa coda?**: selezionare gli utenti autorizzati ad aggiungere richieste a questa coda. Puoi consentire ai seguenti gruppi di persone di visualizzare la Coda richieste nell’area Richieste della barra di navigazione globale quando aggiungono una nuova richiesta:

     | Chi può inserire le richieste | Descrizione |
     |---|---|
     | Tutti | Qualsiasi utente di Workfront con un account attivo può visualizzare questa coda di richieste e aggiungervi richieste |
     | Persone con accesso in visualizzazione al progetto | Gli utenti con autorizzazioni di visualizzazione per il progetto possono visualizzare e aggiungere richieste a questa coda |
     | Persone nella società del progetto | Gli utenti che appartengono alla società associata a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se al progetto è associata una società, il nome della società viene elencato tra parentesi dopo questa impostazione. |
     | Persone nel gruppo del progetto | Gli utenti che appartengono al gruppo associato a questo progetto possono visualizzare e aggiungere richieste a questa coda. Se al progetto è associato un gruppo, dopo questa impostazione il nome del gruppo viene elencato tra parentesi, in caratteri grigi. |

     {style="table-layout:auto"}

   * Utilizza le seguenti opzioni per fornire accesso diretto alla coda richieste e ai moduli ad essa associati a utenti al di fuori di Workfront o a utenti di Workfront che utilizzano una pagina esterna incorporata.

   Per informazioni sull&#39;incorporamento di una coda richieste in un dashboard come pagina esterna, vedere [Incorporare una coda richieste in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

   Per ottenere l’accesso diretto, gli utenti devono prima disporre delle autorizzazioni per la coda richieste. L’utilizzo di una delle opzioni descritte qui non concede automaticamente l’accesso agli utenti.

   >[!TIP]
   >
   >Gli utenti devono prima accedere a Workfront prima di poter accedere alla coda richieste quando accedono alla pagina Coda richieste da un’altra applicazione.

   * **URL di accesso diretto:** Quando un utente accede a questo URL da un browser, viene reindirizzato direttamente alla sezione Nuova richiesta nell&#39;area Richieste e questa richiesta viene selezionata per impostazione predefinita.

     ![Nuova casella di richiesta dalla condivisione URL diretta](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >È possibile visualizzare una coda di richieste in un dashboard come pagina esterna. In questo caso, la coda di richieste è preselezionata, ma puoi selezionare qualsiasi altra coda di richieste dal campo Tipo di richiesta. Gli utenti che inviano la richiesta possono selezionare un altro tipo di richiesta. Vengono visualizzati anche i gruppi di argomenti e gli argomenti della coda.

   * **Codice di incorporamento:** Utilizza questo codice HTML per incorporare il modulo della coda di richieste come iframe in qualsiasi pagina HTML.\
     Se gli utenti non sono già autenticati in Workfront quando visualizzano la pagina in cui è incorporato il codice, viene visualizzata la finestra di dialogo Accesso a Workfront. Dopo che gli utenti effettuano l&#39;accesso, viene visualizzato il modulo Coda richieste.

     >[!NOTE]
     >
     >Quando si visualizza una coda di richieste in un iframe, viene visualizzato solo il modulo di richiesta e il nome della richiesta viene preselezionato e oscurato. L’utente non può modificare il tipo di richiesta. I componenti di navigazione dell’area Richieste non vengono visualizzati.

     Affinché il modulo della coda di richieste possa essere visualizzato quando si utilizza questo codice di incorporamento, l’amministratore di Workfront deve abilitare l’impostazione &quot;Consenti incorporamento di Workfront in un iframe&quot; nell’area di configurazione del sistema.

     Per ulteriori informazioni sull&#39;abilitazione dell&#39;incorporamento di Workfront in un iframe, vedere [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se questa impostazione non è abilitata, l’iframe viene visualizzato come vuoto.

     È possibile regolare vari aspetti della visualizzazione del modulo incorporato, come indicato di seguito:

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
           <td> <p>Regola le dimensioni del frame</p> </td> 
           <td> <p>Modificate gli attributi "width" e "height".</p> <p>Per impostazione predefinita, la larghezza è "500" e l’altezza è "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Indirizza gli utenti a un argomento della coda o a un gruppo di argomenti specifico</p> </td> 
           <td> <p>Aggiungi il parametro "path" all’URL src. Per trovare il parametro path, vai all’argomento della coda o al gruppo di argomenti desiderati nel modulo non incorporato e controlla l’URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostra e consenti agli utenti di modificare l'elenco a discesa Gruppo di argomenti preconfigurato</p> </td> 
           <td> <p>Utilizzare il parametro "path" aggiungendo il parametro <code>showPreSelectedOptions=true</code> a <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Rileva quando il modulo è stato inviato</p> </td> 
           <td> <p>Aggiungere un listener di eventi "message" alla finestra della pagina Web e verificare se <code>event.data.type</code> è <code>requestSubmitted</code>. <code>event.data.newIssueID</code> verrà impostato sull'ID del problema creato.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Tipi di richiesta:** Nella sezione **Proprietà coda**, selezionare una delle opzioni seguenti:

   * Segnalazione Bug
   * Richiesta di Modifica
   * Problema
   * Richiesta

   Questo campo è obbligatorio ed è necessario selezionare almeno un&#39;opzione.

   L’amministratore di Workfront può rinominare i tipi di richiesta predefiniti. Per ulteriori informazioni sulla ridenominazione dei tipi di richiesta, vedere [Personalizzare i tipi di problemi predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

   >[!NOTE]
   >
   >Quando gli utenti accedono alla coda richieste dall’area Richieste, i Tipi di richiesta vengono visualizzati come selezione solo se il Tipo di richiesta è selezionato sia nella pagina Dettagli coda che in Argomento coda.
   >
   >Per informazioni sulla configurazione dell&#39;area Argomenti coda di un progetto, vedere [Creare argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   Ogni tipo selezionato qui sarà disponibile nel modulo (è possibile selezionarne più di uno). Selezionando più di un tipo è possibile organizzare più richieste in arrivo.\
   Ad esempio, se utilizzi il modulo in una coda di richieste per un progetto IT, possono essere messi in coda i seguenti tipi di richieste: hardware, software, correzioni di bug e problemi.

   * **Durata predefinita:** Immettere un numero per la durata, quindi selezionare dal menu a discesa una delle seguenti unità di durata:

      * Giorni
      * Ore
      * Minuti
      * Settimane

   La durata predefinita è il tempo necessario in genere per completare un problema inviato a questa coda di richieste. Questa impostazione diventa predefinita per tutti i problemi in arrivo e può essere modificata manualmente.
La durata predefinita di un problema è la stessa delle ore pianificate sul problema. La Data di completamento pianificata del problema viene calcolata in base a questo campo.\
   Se non viene modificata, la durata predefinita del problema è di 1 giorno o 8 ore.
Se l’amministratore di Workfront ha impostato le ore tipiche per giornata di lavoro su meno di 8 ore nell’area Configura, la durata predefinita per i problemi è ancora di 8 ore.
Ad esempio, se l’opzione Ore tipiche per giorno lavorativo è impostata su 7 ore nell’area Configurazione di Workfront, la durata predefinita per i problemi è 1,14 giorni o 8 ore.
Per ulteriori informazioni su come impostare il sistema Ore tipiche per giorno lavorativo, vedere la sezione &quot;Calcoli sequenza temporale&quot; nell&#39;articolo [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste.**: se selezionata, tutte le richieste inviate alla coda sono visibili per gli utenti della stessa società. Gli utenti possono visualizzare queste richieste nella sezione Tutte le richieste , che si trova nell’area Richieste. Quando questa impostazione viene abilitata o disabilitata, influisce su tutte le richieste future; non influisce retroattivamente sulle informazioni.
   * **Quando un utente effettua una richiesta, concede automaticamente...:** Quando un utente effettua una richiesta alla coda richieste, all&#39;utente viene concesso automaticamente il livello di autorizzazione scelto per tale richiesta. Fai clic sul pulsante Accesso per selezionare tra i seguenti livelli di autorizzazione:

      * **Accesso visualizzazione**
      * **Accesso a Contribute**. Questa è la selezione predefinita e il nome del pulsante di accesso.
      * **Gestisci accesso**

     Per informazioni sul modello di autorizzazioni di Workfront, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     L’impostazione delle autorizzazioni qui consente di risparmiare tempo, anziché concedere le autorizzazioni singolarmente, per ogni richiesta in ingresso. La scelta di questa opzione influisce su tutte le richieste future, ma non su quelle esistenti in modo retroattivo.

   * **Approvazione predefinita**: fare clic sul menu a discesa per selezionare un processo di approvazione per questa coda di richieste. In questo menu a discesa sono visibili solo i processi di approvazione del problema. Tutti i problemi inviati a questa coda saranno associati a questo processo di approvazione. Prima di poter associare i processi di approvazione a livello di sistema alle code di richieste, l&#39;amministratore di Workfront deve definirli. Gli utenti con accesso amministrativo ai processi di approvazione possono inoltre creare processi di approvazione specifici per il gruppo.

     >[!IMPORTANT]
     >
     >Se il gruppo del progetto cambia, il processo di approvazione specifico del gruppo associato ai problemi esistenti diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche al processo di approvazione influiscono sulle impostazioni di approvazione, vedere [Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Se a una coda di richieste sono associati più argomenti della coda, è consigliabile associare i processi di approvazione agli argomenti della coda.

     Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Creare argomenti della coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Quando si aggiungono processi di approvazione alle code di richieste, tenere presente quanto segue:

      * Nell’elenco vengono visualizzati solo i processi di approvazione dei problemi attivi.
      * I processi di approvazione dei problemi a livello di sistema e di gruppo vengono visualizzati nell’elenco. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.

   * **Route predefinita**: fai clic sul menu a discesa per selezionare una regola di routing per questa coda di richieste. Le regole di instradamento assegnano automaticamente i nuovi problemi inviati a una coda di richieste alla risorsa corretta (utente, mansione o team) e al progetto corretto. Tutti i problemi inviati a questa coda saranno associati a questa regola di routing. È necessario configurare le Regole di routing prima che vengano visualizzate nella sezione Dettagli coda e prima di associarle alla coda di richieste.\
     Se a una coda di richieste sono associati più argomenti della coda, è consigliabile associare le regole di routing agli argomenti della coda. Per ulteriori informazioni sulla creazione di regole di routing, vedere [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nuovi campi problema:** Nella sezione **Mostra i campi selezionati seguenti a tutti gli utenti**, seleziona i campi che desideri rendere visibili a tutti gli utenti che inviano una richiesta al progetto o aggiungono un problema a questo progetto o alle attività del progetto.

     >[!NOTE]
     >
     >* Quando si abilita uno dei campi Assegnato a, Mansione o Team, questi vengono sempre rinominati in Assegnazioni nel modulo di richiesta quando gli utenti inviano la richiesta. È possibile specificare solo il tipo di assegnazione nell&#39;area Dettagli coda.
     >
     >* Se è stata selezionata l&#39;opzione Assegnato a nell&#39;area Dettagli coda, è possibile immettere solo gli utenti nel campo Assegnazioni del modulo di richiesta. In questo caso, non è possibile immettere mansioni o un team.

   * **Documenti**: selezionare questa opzione per visualizzare la sezione Documenti nel nuovo modulo di richiesta, quindi selezionare la posizione della sezione di caricamento del documento. Selezionare una delle opzioni seguenti:

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
        <td> <p><span>La sezione Documenti viene visualizzata tra i campi di Workfront e i campi personalizzati del modulo di richiesta.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Nuovi campi problema e documenti in Dettagli coda](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Mostra tutti i campi selezionati e non selezionati in:** Selezionare gli utenti che dovranno visualizzare tutti i campi nel nuovo modulo di richiesta. Le opzioni seguenti controllano l&#39;accesso ai campi del modulo.

     | Quali utenti possono visualizzare tutti i campi nel modulo di richiesta | Descrizione |
     |---|---| 
     | Tutti gli utenti (Full License) | Tutti gli utenti che dispongono di una licenza Pianificazione possono visualizzare i campi selezionati e non selezionati. |
     | Persone con accesso di visualizzazione al progetto (licenza Pianificazione) | Gli utenti con una licenza Pianificazione che dispongono anche dei diritti di visualizzazione per questo progetto possono visualizzare i campi selezionati e non selezionati. Gli altri utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. |
     | Nessun utente | Nessun utente può visualizzare i campi non selezionati. Tutti gli utenti che possono inviare richieste a questo progetto possono visualizzare solo i campi selezionati. Questa è la selezione predefinita. |

   * **Forms personalizzato**: selezionare un modulo personalizzato da associare alla coda richieste dal menu a discesa. È possibile selezionare più moduli, quindi trascinarli e rilasciarli nell&#39;ordine in cui si desidera che vengano visualizzati nel modulo di richiesta.
Da questo menu a discesa sono disponibili solo i moduli personalizzati del problema. A tutti i problemi inviati a questa coda di richieste, aggiunti al progetto o alle sue attività verranno associati i moduli selezionati.
È necessario creare moduli personalizzati per problemi prima di visualizzarli nella sezione Dettagli coda.
Se a una coda di richieste sono associati più argomenti, è consigliabile associare i moduli personalizzati agli argomenti della coda.
Per ulteriori informazioni, vedere [Creare argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Casella Moduli personalizzati nei dettagli coda](assets/custom-forms-box-on-queue-details.png)

1. Continua a selezionare le informazioni per le impostazioni nell&#39;area **Impostazioni coda e-mail**, per consentire agli utenti di inviare richieste e-mail al progetto della coda richieste.

   Per ulteriori informazioni, vedere [Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Fai clic su **Salva**.\
   Il progetto è ora configurato come coda di richieste e gli utenti possono aggiungervi richieste.

1. (Facoltativo) Per migliorare la funzionalità Coda richieste, crea sottosezioni aggiuntive per la coda, nonché regole per instradare le richieste in arrivo al team, all’assegnatario o al progetto corretto.

   * Per informazioni sulla creazione di sottosezioni per la coda richieste, vedere gli articoli seguenti
   * [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Per informazioni sull&#39;instradamento delle richieste all&#39;assegnatario, al team e al progetto appropriati, vedere [Creare regole di instradamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

</div>
