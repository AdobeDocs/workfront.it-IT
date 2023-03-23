---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configura [!DNL Adobe Workfront for Jira]
description: È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: d2c366a69b986bd8d559a18994810011c6d33441
workflow-type: tm+mt
source-wordcount: '2413'
ht-degree: 0%

---

# Configura [!DNL Adobe Workfront for Jira]

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.

Dopo aver installato il componente aggiuntivo, puoi definire i flussi di lavoro che creano [!DNL Jira] si verifica automaticamente quando [!DNL Workfront] gli elementi di lavoro vengono creati. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni vengono aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] può trarre vantaggio da questa integrazione. Hanno solo bisogno di una licenza per il sistema in cui funzionano di più, e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile sia per [!UICONTROL Server] e [!UICONTROL OnDemand] o [!UICONTROL Cloud]) versioni di [!DNL Jira] Software.

Per un elenco di [!DNL Jira] versioni [!DNL Workfront for Jira] supporta attualmente, vedi [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) a [!DNL Atlassian Marketplace].

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] panoramica delle licenze</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: È consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicare a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Prima di configurare [!DNL Workfront for Jira], devi

* Installa [!DNL Workfront for Jira]\
   Per istruzioni sull’installazione [!DNL Workfront for Jira], vedi [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configura [!DNL Workfront for Jira]

Configurazione [!DNL Workfront for Jira] puoi:

* Definire i trigger che creeranno [!DNL Jira] quando [!DNL Workfront] gli elementi vengono creati.
* Specificare i campi da sincronizzare tra gli elementi collegati tra di essi [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Dopo aver configurato [!DNL Workfront for Jira] sul tuo [!DNL Jira] ambiente, tutti [!DNL Jira] gli utenti visualizzano [!DNL Workfront] pannello destro su tutti [!DNL Jira] oggetti. Il pannello contiene informazioni sugli elementi da cui è possibile collegare [!DNL Workfront] o specifica che no [!DNL Workfront] gli elementi sono collegati a [!DNL Jira] oggetti.
>* Quando utilizzi [!DNL Jira Server] Solo i problemi associati ai progetti identificati come trigger per l’integrazione Workfront visualizzano il pannello Workfront. Per ulteriori informazioni sulla configurazione dei trigger per [!DNL Workfront to Jira] flusso di lavoro, vedi [Configura i trigger per il collegamento automatico di elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




Per configurare [!DNL Workfront for Jira]:

1. Accedi a [!DNL Jira] come [!DNL Jira] amministratore.
1. Fai clic su **[!UICONTROL Impostazioni]** nella [!DNL Jira] menu.
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi fai clic su **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. Espandi la **[!DNL Workfront]** add-on.
1. Fai clic su **[!UICONTROL Configura]**.
1. Segui le istruzioni per accedere a [!DNL Workfront].

   >[!NOTE]
   >
   >L&#39;utente deve avere una `apiKey` in [!UICONTROL Workfront] per creare una connessione corretta.

   Devi effettuare l&#39;accesso a [!DNL Workfront] come [!DNL Workfront] per continuare la configurazione.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] si connette a [!DNL Jira] utilizzando OAuth 2.0, uno standard utilizzato dalla maggior parte delle integrazioni basate su web per l’autenticazione e l’autorizzazione degli utenti.
   >* Quando viene richiesto di accedere al dominio del [!DNL Workfront] account, digitare il formato: *la tua azienda&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L’autenticazione avanzata non è disponibile finché non viene [!DNL Workfront] l&#39;amministratore lo abilita per questa integrazione.



1. Seleziona la **[!UICONTROL Triggers]** per configurare la creazione automatica di [!DNL Jira] elementi nuovi [!DNL Workfront] gli elementi vengono creati.

   Per ulteriori informazioni sulla configurazione dei trigger per Workfront su [!DNL Jira] flusso di lavoro, vedi [Configura i trigger per il collegamento automatico di elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleziona la **[!UICONTROL Configurazione]** scheda per configurare la sincronizzazione dei campi tra collegati [!DNL Jira] e [!DNL Workfront] oggetti.

   Per ulteriori informazioni sulla configurazione della sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront], vedi [Configura la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Dopo aver definito i trigger e la sincronizzazione dei campi tra le due applicazioni, qualsiasi [!DNL Workfront] l&#39;utente che può creare attività o problemi potrebbe potenzialmente attivare la creazione di un elemento in [!DNL Jira]. L&#39;utente può creare un elemento se i criteri dell&#39;elemento creato corrispondono ai trigger in [!DNL Jira], anche se l’utente non dispone di un [!DNL Jira] licenza. Inoltre, qualsiasi [!DNL Jira] l&#39;utente può iniziare immediatamente a lavorare [!DNL Jira] e i relativi aggiornamenti sono visibili in [!DNL Workfront]senza che abbiano [!DNL Workfront] licenza. Qualsiasi aggiornamento in [!DNL Workfront] sono visibili anche sul [!DNL Jira] oggetti.

1. (Facoltativo) Seleziona la **[!UICONTROL Registro attività]** per esaminare eventuali errori verificatisi durante l’integrazione.

   Per ulteriori informazioni sulla [!UICONTROL Registro attività], vedi [Visualizza la [!DNL Jira] [!UICONTROL Registro attività]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configura i trigger per il collegamento automatico di elementi tra [!DNL Jira] e [!DNL Workfront]

Come [!DNL Jira] amministratore di sistema, puoi definire i trigger che creerebbero automaticamente problemi in [!DNL Jira] quando un elemento in [!DNL Workfront] soddisfa determinati criteri.

>[!NOTE]
>
>L&#39;integrazione potrebbe richiedere fino a 10 minuti per creare nuovi problemi in [!DNL Jira].

Quando configuri l’attivazione della creazione di [!DNL Jira] elementi come [!DNL Workfront] gli elementi vengono creati:

* L&#39;integrazione è unidirezionale: Puoi attivare solo gli elementi creati in [!DNL Workfront] da creare automaticamente in [!DNL Jira]. Non è possibile attivare gli elementi creati in [!DNL Jira] per creare automaticamente in [!DNL Workfront].
* Non esiste alcun limite al numero di attivatori disponibili.
* Se un elemento creato in [!DNL Workfront] corrisponde a più di un trigger, viene creato un solo elemento in [!DNL Jira]. L’elemento viene creato in [!DNL Jira] in base al primo attivatore (nell&#39;ordine in cui sono stati definiti [!DNL Jira]). Tutti gli altri trigger vengono ignorati.
* Un solo elemento in [!DNL Workfront] può essere collegato a un elemento in Jira. Non puoi mai collegarne uno [!DNL Workfront] elemento a più [!DNL Jira] problemi o uno [!DNL Jira] problema a più [!DNL Workfront] oggetti.

Per configurare i trigger per la creazione automatica di elementi in [!DNL Jira]:

1. Accedi a [!DNL Jira] come amministratore di sistema.
1. Fai clic su **[!UICONTROL Impostazioni]** nella [!DNL Jira] menu.
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. Espandi la **[!DNL Workfront]** add-on.
1. Fai clic su **[!UICONTROL Configura]**.
1. Accedi a [!DNL Workfront] come amministratore di sistema.

   La **[!UICONTROL Triggers]** è selezionata per impostazione predefinita.

1. Fai clic su **[!UICONTROL Aggiungi trigger]** per aggiungere un nuovo trigger.
1. In **[!UICONTROL Team/utente/ruolo di Workfront]** campo , specifica il nome di un [!DNL Workfront] ruolo team, utente o processo, quindi fare clic per selezionarlo quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Non puoi avere più trigger per lo stesso team, utente o ruolo.

   Quando un utente crea un’attività o un problema e la assegna a una di queste entità, viene automaticamente creato un problema in [!DNL [!DNL Jira]].

1. In **[!UICONTROL [!DNL Jira]progetto]** campo, inizia a digitare il nome di un [!DNL Jira] , quindi fai clic su per selezionarlo quando viene visualizzato nell’elenco.

   Quando il [!DNL Jira] Il problema viene creato e posizionato sul progetto qui specificato.

1. Seleziona un **I[!UICONTROL tipo di problema]** dal menu a discesa.

   Indica il tipo di problema creato in [!DNL Jira] quando vengono soddisfatte le condizioni di questo trigger, in base alle impostazioni per quel progetto specifico in [!DNL Jira].

1. Fai clic su **[!UICONTROL Salva]**.

   Con questa configurazione, ogni volta [!DNL Workfront] l&#39;utente crea un elemento che corrisponde ai trigger specificati, viene creato un nuovo problema in [!DNL Jira].

## Configura la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi

Come [!DNL Jira] amministratore, puoi definire quali campi devono essere sincronizzati automaticamente sugli elementi collegati tra [!DNL Workfront] e Jira. Alcuni campi possono essere sincronizzati dalla [!DNL Workfront] al [!DNL Jira] e altri sono sincronizzati da Jira a Workfront.

Per definire quali campi devono essere sincronizzati automaticamente sugli elementi collegati tra le due applicazioni:

1. Accedi a [!DNL Jira] come amministratore Jira.
1. Fai clic su **[!UICONTROL Impostazioni]** nella [!DNL Jira] menu.
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. Espandi la **[!DNL Workfront]** add-on.
1. Fai clic su **[!UICONTROL Configura]**.
1. Accedi a [!DNL Workfront] come amministratore Workfront.
1. Fai clic sul pulsante **[!UICONTROL Configurazione]** scheda .

1. In **[!UICONTROL Sincronizzazione da Jira a Workfront]** seleziona i campi in cui desideri eseguire l’aggiornamento [!DNL Jira] quando vengono aggiornate in Workfront.

   1. Selezionare una delle seguenti frequenze con cui i campi sono sincronizzati:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Alla Creazione]</td>
              <td>I campi specificati vengono sincronizzati tra Workfront collegato e [!DNL Jira] elementi quando l’elemento viene creato in Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>I campi specificati vengono sincronizzati tra Workfront collegato e [!DNL Jira] elementi quando i campi vengono aggiornati in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Mai]</td>
              <td>I campi specificati non vengono mai sincronizzati tra quelli collegati [!DNL Workfront] e [!DNL Jira] oggetti. Nessuna indicazione in [!DNL Jira] che il campo è stato aggiornato in [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Seleziona per sincronizzare uno dei campi seguenti da [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Nome di un'attività o di un problema in [!DNL Workfront] diventa il nome del problema a cui è collegato [!DNL Jira].</p><p>Nota: Quando vengono creati nuovi elementi in [!DNL Jira] automaticamente, [!DNL Workfront] Il nome viene sempre aggiornato [!DNL Jira] , indipendentemente dal fatto che questo campo sia abilitato o meno. Quando un [!DNL Jira] elemento collegato manualmente a un [!DNL Workfront] l'elemento, il nome della [!DNL Workfront] aggiornamenti solo degli elementi in [!DNL Jira] quando si seleziona <strong>Sempre</strong> sincronizza questo campo. Per ulteriori informazioni sul collegamento manuale o automatico degli elementi, consulta <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrizione]</td>
         <td>La descrizione di un'attività o di un problema in [!DNL Workfront] diventa la descrizione del problema a cui è collegato [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documenti</td>
         <td><p>Documenti allegati a un’attività o a un problema in [!DNL Workfront] sono altresì allegati alla questione alla quale è collegata a Jira. Nuove versioni di documenti da [!DNL Workfront] sono aggiunti come documenti separati a Jira e sono aggiunti con <i>_v&lt;version number=""&gt;</i> per indicare la versione numerata in Workfront. </p><p>Ad esempio, se il nome di un documento in [!DNL Workfront] è <strong>Annuncio principale</strong>e aggiungi una nuova versione in [!DNL Workfront], la nuova versione viene trasferita a [!DNL Jira] come nuovo documento con il nome <strong>Ad_v2 principale</strong>.</p><p>Importante: <p>Quando si sincronizzano i documenti, tenere presente quanto segue:</p>
           <ul>
            <li><p>I documenti di dimensioni superiori a 5 MB non vengono sincronizzati. Se la sincronizzazione di un documento non riesce perché il documento è troppo grande, viene registrato un errore nel registro attività, </p><p>Per ulteriori informazioni sul registro attività, vedi <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Visualizza il registro delle attività di Jira</a>.</p></li>
            <li><p>I documenti collegati a attività e problemi dei server esterni non vengono trasferiti al [!DNL Jira] oggetti. Solo documenti caricati direttamente sull'attività o sul problema in [!DNL Workfront] vengono trasferiti al problema collegato in [!DNL Jira].</p></li>
            <li><p>Per creare una bozza da un documento, è necessario generare la bozza in [!DNL Workfront]. </p><p>Per ulteriori informazioni sulla generazione di una bozza, consulta <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">Crea una bozza per un documento esistente </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Crea una bozza per un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data di completamento pianificata]</td>
         <td><p>Data di completamento pianificata di un'attività o di un problema in [!DNL Workfront] diventa la [!UICONTROL Due Date] del problema a cui è collegato [!DNL Jira].</p><p>Nota: Assicurati di visualizzare <strong>[!UICONTROL Data di scadenza]</strong> su [!DNL Jira] problemi, per sincronizzare questo valore.</p></td>
        </tr>
       </tbody>
      </table>

1. In **[!UICONTROL Sincronizza da [!DNL Jira] a[!DNL Workfront]]** seleziona i campi in cui desideri eseguire l’aggiornamento [!DNL Workfront] quando vengono aggiornati in [!DNL Jira].

   1. Selezionare una delle seguenti frequenze con cui i campi sono sincronizzati:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>I campi specificati vengono sempre sincronizzati tra i campi collegati [!DNL Workfront] e [!DNL Jira] elementi quando i campi vengono aggiornati in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Mai]</td>
         <td><p>I campi specificati non vengono mai sincronizzati tra quelli collegati [!DNL Workfront] e [!DNL Jira] oggetti. Nessuna indicazione in [!DNL Workfront] che il campo è stato aggiornato in [!DNL Jira]. </p><p>Nota: Quando si seleziona Mai, [!DNL Workfront] i campi possono ancora essere aggiornati manualmente da [!DNL Jira] a sinistra [!DNL Workfront] pannello [!DNL Jira] problema. Tali aggiornamenti vengono visualizzati solo su [!DNL Workfront] elementi in [!DNL Jira] e [!DNL Workfront] e non [!DNL Jira] oggetti.</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleziona per sincronizzare uno dei campi seguenti da [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>Lo [!UICONTROL Status] di un problema in [!DNL Jira] diventa lo [!UICONTROL Status] dell'attività o del problema a cui è collegato [!DNL Workfront].<br>Per ulteriori informazioni [!DNL Workfront] stati, vedi <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assegnatario]</td>
         <td><p>L’[!UICONTROL Assegnatario] di un problema in [!DNL Jira] diventa l’ [!UICONTROL Assegnatario] dell’attività o del problema a cui è collegato [!DNL Workfront].</p><p>Importante: Quando si assegna un elemento in [!DNL Jira] a un utente che non ha [!DNL Workfront] l'integrazione crea un nuovo utente attivo in [!DNL Workfront] solo quando <strong>Crea automaticamente un utente in [!DNL Workfront] se [!DNL Jira] l'utente non ha un [!DNL Workfront] account</strong> è impostato su <strong>[!UICONTROL Always]</strong>. Questo utente non occupa un [!DNL Workfront] licenza. Gli utenti attivi possono essere assegnati agli elementi di lavoro in [!DNL Workfront], ma non può essere incluso negli aggiornamenti. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Allegati]</td>
         <td>Allegati di un problema in [!DNL Jira] sono anche collegati all'attività o al problema a cui è collegato [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Commenti]</td>
         <td><p>Un commento su un [!DNL Jira] il problema è anche pubblicato sul link [!DNL Workfront] nell’area [!UICONTROL Updates]. Viceversa, un commento pubblicato nell'area [!UICONTROL Updates] per un [!DNL Workfront] attività o problemi di sincronizzazione con [!DNL Jira]Flusso di commenti nativo per il problema collegato. </p><p>È impostato su <strong>[!UICONTROL Always]</strong> per impostazione predefinita. Se si seleziona <strong>[!UICONTROL Mai]</strong> in questo caso, è comunque possibile pubblicare manualmente i commenti su un elemento collegato in [!DNL Workfront] o [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. In **[!UICONTROL ALTRO]** seleziona i campi aggiuntivi da aggiornare tra gli elementi collegati.

   1. Selezionare un’opzione per determinare se i campi specificati **[!UICONTROL Sempre]** o **[!UICONTROL Mai]** aggiorna in [!DNL Jira] o [!DNL Workfront] quando vengono modificati.

   1. Seleziona dai campi e dagli aggiornamenti seguenti:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copia [!DNL Workfront] Dati personalizzati nel pannello di destra in [!DNL Jira]]</td>
         <td><p>Visualizza la [!DNL Workfront] Dati personalizzati di un elemento nel [!DNL Workfront] pannello a destra.</p><p>Nota: Le sezioni del modulo personalizzato vengono visualizzate nel [!DNL Workfront] pannello a destra con il livello di accesso [!DNL Workfront] Amministratore di sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copia [!DNL Workfront] Priorità nel pannello di destra in [!DNL Jira]]</td>
         <td>Visualizza la [!DNL Workfront] Priorità di un elemento nel [!DNL Workfront] pannello a destra.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Aggiungi un aggiornamento nel [!DNL Workfront] Scheda Aggiornamenti sulle modifiche alla data di scadenza in [!DNL Jira]]</td>
         <td>Aggiunge un commento nella scheda [!UICONTROL Update] del [!DNL Workfront] elemento quando la [!UICONTROL Due Date] cambia in collegata [!DNL Jira] oggetto.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crea automaticamente un utente in [!DNL Workfront] se [!DNL Jira] l'utente non ha un [!DNL Workfront] account]</td>
         <td><p>Esistono i seguenti scenari:</p>
          <ul>
           <li>Quando selezioni <strong>[!UICONTROL Always]</strong> consente di abilitare l’integrazione per creare un nuovo utente Workfront ogni volta che [!DNL Jira] utente senza [!DNL Workfront] l'account esegue le seguenti azioni su un [!DNL Jira] problema:
            <ul>
             <li>È assegnato a un [!DNL Jira] problema</li>
             <li><p>Registrazione del tempo su un [!DNL Jira] problema</p><p>Questo nuovo utente non occupa un [!DNL Workfront] licenza. L'impostazione predefinita è Sempre. L’utente ha creato in questo modo [!DNL Workfront] ha aggiunto "[!UICONTROL Jira]" al loro nome.</p></li>
            </ul></li>
           <li>Quando selezioni <strong>[!UICONTROL Mai]</strong>, si verificano le seguenti situazioni:
            <ul>
             <li>Non puoi vedere nessuna [!DNL Jira] assegnazioni [!DNL Workfront] oggetti. In questo caso, solo le assegnazioni effettuate in [!DNL Workfront] sul display [!DNL Workfront] oggetti.</li>
             <li>L'ora di accesso a un collegamento [!DNL Jira] problema di un utente senza un [!DNL Workfront] l'account non viene trasferito automaticamente al link [!DNL Workfront] oggetto. È comunque possibile eseguire l'accesso al [!DNL Workfront] nel pannello di destra della [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Fai clic su **[!UICONTROL Salva]**.

   Ora, ogni volta che un utente aggiorna uno dei campi specificati in questa configurazione su un elemento in [!DNL Jira] o [!DNL Workfront], viene aggiornato anche l’elemento collegato nell’altra applicazione.

## Risoluzione dei problemi

### Impossibile creare gli elementi in [!DNL Jira] a causa dei campi di attivazione contrassegnati &quot;[!UICONTROL Impossibile trovare]&quot;

#### Problema

Quando si verifica un errore con la [!DNL Workfront for Jira] domanda, [!DNL Workfront] disabilita i trigger per evitare ulteriori complicazioni. Quando tali attivatori sono disabilitati, vengono visualizzati come &quot;[!UICONTROL Impossibile trovare]&quot;.

#### Soluzione

Individua l&#39;errore che ha disabilitato i trigger. Puoi trovare l’errore nella [!DNL Workfront for Jira] &quot;[!UICONTROL Registro attività]&quot;.

La causa più comune di questo comportamento è l&#39;errore &quot;[!UICONTROL Impossibile impostare il campo &#39;duedate&#39;. Non si trova nella schermata appropriata o sconosciuta.]&quot;

Questo errore significa che si sta tentando di sincronizzare il &quot;[!UICONTROL Data completamento pianificata]&quot; [!DNL Workfront] a [!DNL Jira]. Per fare questo, devi assicurarti che il tuo [!DNL Jira] gli oggetti hanno un campo denominato &quot;[!UICONTROL Data di scadenza]&quot;. Se non dispongono di questo campo, [!DNL Workfront] non è in grado di sincronizzare la data di completamento pianificata da [!DNL Workfront] e disabilita i trigger.

Per risolvere questo errore, provare una delle seguenti operazioni:

* Chiedi a [!DNL Jira] amministratore per aggiornare la [!DNL Jira] per garantire che abbiano un campo di scadenza.
* Disattiva la sincronizzazione di [!DNL Workfront]Data di completamento prevista in Workfront &quot;[!UICONTROL Configurazione]&quot; pagina
