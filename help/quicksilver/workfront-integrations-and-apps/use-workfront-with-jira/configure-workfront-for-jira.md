---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configura [!DNL Adobe Workfront for Jira]
description: È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 9ff647ba4eca31e6d2d06a8c9b787badaf965477
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 0%

---

# Configura [!DNL Adobe Workfront for Jira]

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare [!DNL Jira] e [!DNL Workfront] sistemi.

Dopo aver installato il componente aggiuntivo, è possibile definire i flussi di lavoro che creano [!DNL Jira] problemi automaticamente quando [!DNL Workfront] vengono creati elementi di lavoro. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni vengono aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] può trarre vantaggio da questa integrazione. È sufficiente una licenza per il sistema in cui operano maggiormente e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile sia per [!UICONTROL Server] e [!UICONTROL On demand] (o [!UICONTROL Cloud]) versioni di [!DNL Jira] Software.

Per un elenco di [!DNL Jira] versioni che [!DNL Workfront for Jira] attualmente supporta, vedi [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) alla [!DNL Atlassian Marketplace].

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] piano]*</td> 
   <td><p>Nuovo piano: [!UICONTROL Prime] o versione successiva</p>
       <p>oppure</p>
       <p>Piano corrente: [!UICONTROL Pro] o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td><p>Nuovo piano: [!UICONTROL Standard] </p>
       <p>oppure</p> 
       <p>Piano corrente: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

Prima di configurare [!DNL Workfront for Jira], è necessario:

* Installa [!DNL Workfront for Jira].
Per istruzioni sull&#39;installazione [!DNL Workfront for Jira], vedi [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configura [!DNL Workfront for Jira]

Configurando [!DNL Workfront for Jira], è possibile:

* Definisci i trigger che creeranno [!DNL Jira] elementi quando [!DNL Workfront] vengono creati.
* Specificare i campi da sincronizzare tra gli elementi collegati [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Dopo aver configurato [!DNL Workfront for Jira] sul tuo [!DNL Jira] ambiente, tutti [!DNL Jira] gli utenti visualizzano un [!DNL Workfront] pannello destro su tutti [!DNL Jira] elementi. Il pannello contiene informazioni sugli elementi che potrebbero essere collegati da [!DNL Workfront] o specifica che no [!DNL Workfront] elementi collegati a [!DNL Jira] elementi.
>* Quando si utilizza [!DNL Jira Server] durante l’installazione, nel pannello Workfront vengono visualizzati solo i problemi associati ai progetti identificati come attivatori per l’integrazione di Workfront. Per ulteriori informazioni sulla configurazione dei trigger per [!DNL Workfront to Jira] flusso di lavoro, vedi [Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Per configurare [!DNL Workfront for Jira]:

1. Accedi a [!DNL Jira] as a [!DNL Jira] amministratore.
1. Clic **[!UICONTROL Impostazioni]** nell&#39;area [!DNL Jira] menu.
1. Clic **[!UICONTROL Componenti aggiuntivi]**, quindi fai clic su **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. Espandi **[!DNL Workfront]** componente aggiuntivo.
1. Clic **[!UICONTROL Configura]**.
1. Segui le istruzioni per accedere a [!DNL Workfront].

   >[!NOTE]
   >
   >L&#39;utente deve disporre di un `apiKey` in [!UICONTROL Workfront] per creare una connessione riuscita.

   Devi accedere a [!DNL Workfront] as a [!DNL Workfront] per continuare la configurazione.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] si connette a [!DNL Jira] con OAuth 2.0, uno standard utilizzato dalla maggior parte delle integrazioni basate sul web per l’autenticazione e l’autorizzazione degli utenti.
   >* Quando viene richiesto di immettere il dominio del [!DNL Workfront] account, digitalo utilizzando questo formato: *yourCompany&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L’autenticazione avanzata non è disponibile fino a quando non viene [!DNL Workfront] l&#39;amministratore consente questa integrazione.

1. In Jira, seleziona la **[!UICONTROL Triggers]** per configurare la creazione automatica di [!DNL Jira] elementi come nuovi [!DNL Workfront] vengono creati.

   Per ulteriori informazioni sulla configurazione dei trigger per Workfront per [!DNL Jira] flusso di lavoro, vedi [Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleziona la **[!UICONTROL Configurazione]** per configurare la sincronizzazione dei campi tra i campi collegati [!DNL Jira] e [!DNL Workfront] elementi.

   Per ulteriori informazioni sulla configurazione della sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront], vedi [Configurare la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Dopo aver definito i trigger e la sincronizzazione dei campi tra le due applicazioni, qualsiasi [!DNL Workfront] utente che può creare attività o problemi potrebbe potenzialmente attivare la creazione di un elemento in [!DNL Jira]. L’utente può creare un elemento se i criteri dell’elemento che crea corrispondono ai trigger in [!DNL Jira], anche se l’utente non dispone di un [!DNL Jira] licenza. Inoltre, qualsiasi [!DNL Jira] l&#39;utente può iniziare immediatamente a lavorare sul [!DNL Jira] e i relativi aggiornamenti sono visibili in [!DNL Workfront], senza che abbiano un [!DNL Workfront] licenza. Qualsiasi aggiornamento in [!DNL Workfront] sono visibili anche sul [!DNL Jira] elementi.

1. (Facoltativo) Seleziona la **[!UICONTROL Registro attività]** per esaminare eventuali errori che potrebbero essersi verificati durante l’integrazione.

   Per ulteriori informazioni su [!UICONTROL Registro attività], vedi [Visualizza [!DNL Jira] [!UICONTROL Registro attività]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]

Come [!DNL Jira] dell&#39;amministratore di sistema, è possibile definire trigger che creerebbero automaticamente problemi in [!DNL Jira] quando un elemento [!DNL Workfront] soddisfa determinati criteri.

>[!NOTE]
>
>Potrebbero essere necessari fino a 10 minuti perché l’integrazione crei nuovi problemi in [!DNL Jira].

Quando configuri l’attivazione della creazione di, tieni presente quanto segue [!DNL Jira] elementi come [!DNL Workfront] gli elementi vengono creati:

* L’integrazione è unidirezionale: puoi attivare solo gli elementi creati in [!DNL Workfront] da creare automaticamente in [!DNL Jira]. Non è possibile attivare gli elementi creati in [!DNL Jira] da creare automaticamente in [!DNL Workfront].
* Non esiste alcun limite al numero di attivatori che è possibile avere.
* Se un elemento creato in [!DNL Workfront] corrisponde a più di uno dei trigger, viene creato un solo elemento in [!DNL Jira]. L&#39;elemento viene creato in [!DNL Jira] in base al primo trigger (nell&#39;ordine in cui sono stati definiti in [!DNL Jira]). Tutti gli altri trigger vengono ignorati.
* Solo un elemento in [!DNL Workfront] può essere collegato a un elemento in Jira. Non puoi mai collegarne uno [!DNL Workfront] elemento su più [!DNL Jira] problemi, o uno [!DNL Jira] problema a più [!DNL Workfront] elementi.

Per configurare i trigger per la creazione automatica di elementi in [!DNL Jira]:

1. Accedi a [!DNL Jira] come amministratore di sistema.
1. Clic **[!UICONTROL Impostazioni]** nell&#39;area [!DNL Jira] menu.
1. Clic **[!UICONTROL Componenti aggiuntivi]**, quindi **[!UICONTROL Gestire i componenti aggiuntivi]**.
1. Espandi **[!DNL Workfront]** componente aggiuntivo.
1. Clic **[!UICONTROL Configura]**.
1. Accedi a [!DNL Workfront] come amministratore di sistema.

   Il **[!UICONTROL Triggers]** è selezionata per impostazione predefinita in Jira.

1. Clic **[!UICONTROL Aggiungi trigger]** per aggiungere un nuovo trigger.
1. In **[!UICONTROL team/utente/ruolo Workfront]** , specificare il nome di un [!DNL Workfront] team, utente o mansione, quindi fai clic su per selezionarlo quando viene visualizzato nell’elenco.

   >[!NOTE]
   >
   >Non è possibile avere più trigger per lo stesso team, utente o ruolo.

   Quando un utente crea un&#39;attività o un problema e lo assegna a una di queste entità, viene automaticamente creato un problema in [!DNL [!DNL Jira]].

1. In **[!UICONTROL [!DNL Jira]progetto]** , inizia a digitare il nome di un [!DNL Jira] , quindi fare clic su per selezionarlo quando viene visualizzato nell&#39;elenco.

   Quando [!DNL Jira] viene creato, viene inserito nel progetto scelto qui.

1. Seleziona un **I[!UICONTROL tipo di problema]** dal menu a discesa.

   Indica il tipo di problema creato in [!DNL Jira] quando le condizioni di questo attivatore sono soddisfatte, in base alle impostazioni per quel progetto specifico in [!DNL Jira].

1. Fai clic su **[!UICONTROL Salva]**.

   Con questa configurazione, ogni volta [!DNL Workfront] l’utente crea un elemento che corrisponde ai trigger specificati; viene creato un nuovo problema in [!DNL Jira].

## Configurare la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi

Come [!DNL Jira] amministratore, puoi definire quali campi devono essere sincronizzati automaticamente sugli elementi collegati tra [!DNL Workfront] e Jira. Alcuni campi possono essere sincronizzati dal [!DNL Workfront] al [!DNL Jira] e altri sincronizzano da Jira a Workfront.

Per definire i campi da sincronizzare automaticamente sugli elementi collegati tra le due applicazioni:

1. Accedi a [!DNL Jira] in qualità di amministratore Jira.
1. Clic **[!UICONTROL Impostazioni]** nell&#39;area [!DNL Jira] menu.
1. Clic **[!UICONTROL Componenti aggiuntivi]**, quindi **[!UICONTROL Gestire i componenti aggiuntivi]**.
1. Espandi **[!DNL Workfront]** componente aggiuntivo.
1. Clic **[!UICONTROL Configura]**.
1. Accedi a [!DNL Workfront] come amministratore di Workfront.
1. In Jira, fai clic su **[!UICONTROL Configurazione]** scheda.
1. In **[!UICONTROL Sincronizzare da Workfront a Jira]** , selezionare i campi che si desidera aggiornare [!DNL Jira] quando vengono aggiornati in Workfront.

   1. Selezionare una delle seguenti frequenze con cui vengono sincronizzati i campi:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Alla Creazione]</td>
              <td>I campi specificati vengono sincronizzati tra il Workfront collegato e [!DNL Jira] elementi quando l'elemento viene creato in Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>I campi specificati vengono sincronizzati tra il Workfront collegato e [!DNL Jira] elementi quando i campi vengono aggiornati in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>I campi specificati non vengono mai sincronizzati tra i campi collegati [!DNL Workfront] e [!DNL Jira] elementi. Non vi è alcuna indicazione in [!DNL Jira] il campo è stato aggiornato in [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selezionare una delle opzioni seguenti da cui sincronizzare i campi [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Nome di un’attività o di un problema in [!DNL Workfront] diventa il nome del problema a cui è collegato [!DNL Jira].</p><p>Nota: quando vengono creati nuovi elementi in [!DNL Jira] automaticamente, [!DNL Workfront] Il nome viene sempre aggiornato in [!DNL Jira] elemento, indipendentemente dal fatto che questo campo sia abilitato o meno in questo punto. Quando un [!DNL Jira] l'elemento è collegato manualmente a un [!DNL Workfront] elemento, il nome del [!DNL Workfront] aggiornamenti solo elemento in [!DNL Jira] quando si seleziona per <strong>Sempre</strong> sincronizza questo campo. Per ulteriori informazioni sul collegamento manuale o automatico degli elementi, vedere <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Collega elementi tra [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrizione]</td>
         <td>Descrizione di un’attività o di un problema in [!DNL Workfront] diventa la descrizione del problema a cui è collegato [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documenti</td>
         <td><p>Documenti allegati a un’attività o a un problema in [!DNL Workfront] sono anche collegate alla questione a cui sono collegate in Jira. Nuove versioni di documenti da [!DNL Workfront] sono aggiunti come documenti separati a Jira e sono aggiunti con <i>_v&lt;version number=""&gt;</i> per indicare la versione numerata in Workfront. </p><p>Ad esempio, se il nome di un documento in [!DNL Workfront] è <strong>Annuncio principale</strong>e aggiungi una nuova versione in [!DNL Workfront], la nuova versione viene trasferita a [!DNL Jira] come nuovo documento con il nome <strong>Ad_v2 principale</strong>.</p><p>Importante: <p>Quando si sincronizzano i documenti, tenere presente quanto segue:</p>
           <ul>
            <li><p>I documenti superiori a 5 MB non vengono sincronizzati. Se la sincronizzazione di un documento non riesce perché il documento è troppo grande, nel registro attività viene registrato un errore. </p><p>Per ulteriori informazioni sul registro attività, consulta <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Visualizzare il registro attività Jira</a>.</p></li>
            <li><p>I documenti collegati ad attività e problemi da server esterni non vengono trasferiti al [!DNL Jira] elementi. Solo i documenti caricati direttamente sull’attività o sul problema in [!DNL Workfront] vengono trasferiti al problema collegato in [!DNL Jira].</p></li>
            <li><p>Per creare una bozza da un documento, è necessario generarla in [!DNL Workfront]. </p><p>Per ulteriori informazioni sulla generazione di una bozza, consulta <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Creare una bozza per un documento esistente </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Creare una bozza per un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td>
         <td><p>[!UICONTROL Planned Completion Date] (Data di completamento pianificata) di un’attività o di un problema in [!DNL Workfront] diventa [!UICONTROL Scadenza] del problema a cui è collegato [!DNL Jira].</p><p>Nota: assicurarsi di visualizzare <strong>[!UICONTROL Scadenza]</strong> il [!DNL Jira] problemi, affinché questo valore venga sincronizzato.</p></td>
        </tr>
       </tbody>
      </table>

1. In **[!UICONTROL Sincronizza da [!DNL Jira] a[!DNL Workfront]]** , selezionare i campi che si desidera aggiornare [!DNL Workfront] quando vengono aggiornati in [!DNL Jira].

   1. Selezionare una delle seguenti frequenze con cui vengono sincronizzati i campi:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>I campi specificati vengono sempre sincronizzati tra i [!DNL Workfront] e [!DNL Jira] elementi quando i campi vengono aggiornati in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>I campi specificati non vengono mai sincronizzati tra i campi collegati [!DNL Workfront] e [!DNL Jira] elementi. Non vi è alcuna indicazione in [!DNL Workfront] il campo è stato aggiornato in [!DNL Jira]. </p><p>Nota: quando si seleziona Mai, [!DNL Workfront] I campi possono ancora essere aggiornati manualmente da [!DNL Jira] a sinistra [!DNL Workfront] pannello del [!DNL Jira] problema. Questi aggiornamenti vengono visualizzati solo in data [!DNL Workfront] elementi in [!DNL Jira] e [!DNL Workfront] e non il [!DNL Jira] elementi.</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleziona questa opzione per sincronizzare uno dei seguenti campi [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Stato]</td>
         <td>Lo stato [!UICONTROL] di un problema in [!DNL Jira] diventa lo [!UICONTROL Status] dell'attività o del problema a cui è collegato [!DNL Workfront].<br>Per ulteriori informazioni su [!DNL Workfront] stati, vedere <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL assegnatario]</td>
         <td><p>[!UICONTROL Assegnatario] di un problema in [!DNL Jira] diventa l'[!UICONTROL Assegnatario] dell'attività o del problema a cui è collegato [!DNL Workfront].</p><p>Importante: quando si assegna un elemento in [!DNL Jira] a un utente che non dispone di un [!DNL Workfront] , l’integrazione crea un nuovo utente attivo in [!DNL Workfront] solo quando <strong>Crea automaticamente un utente in [!DNL Workfront] se [!DNL Jira] l’utente non dispone di un [!DNL Workfront] account</strong> è impostato su <strong>[!UICONTROL Always]</strong>. Questo utente non occupa un [!DNL Workfront] licenza. Gli utenti attivi possono essere assegnati ad elementi di lavoro in [!DNL Workfront], ma non può essere incluso negli aggiornamenti. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Allegati]</td>
         <td>Allegati di un problema in [!DNL Jira] sono anche collegate all’attività o al problema a cui sono collegate [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Commenti]</td>
         <td><p>Un commento su un [!DNL Jira] problema è pubblicato anche sul [!DNL Workfront] nell'area [!UICONTROL Aggiornamenti]. Al contrario, un commento pubblicato nell'area [!UICONTROL Aggiornamenti] per un [!DNL Workfront] sincronizzazioni di attività o problemi con [!DNL Jira]Flusso di commenti nativo di per il problema collegato. </p><p>Questo è impostato su <strong>[!UICONTROL Always]</strong> per impostazione predefinita. Se si seleziona <strong>[!UICONTROL Never]</strong> qui è ancora possibile pubblicare commenti manualmente su un elemento collegato in [!DNL Workfront] o in [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. In **[!UICONTROL ALTRO]** , seleziona i campi aggiuntivi da aggiornare tra gli elementi collegati.

   1. Selezionare un&#39;opzione per determinare se i campi specificati **[!UICONTROL Sempre]** o **[!UICONTROL Mai]** aggiorna in [!DNL Jira] o [!DNL Workfront] quando vengono modificati.

   1. Seleziona uno dei campi e degli aggiornamenti seguenti:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Dati personalizzati nel pannello a destra in [!DNL Jira]]</td>
         <td><p>Visualizza la [!DNL Workfront] Dati personalizzati di un elemento in [!DNL Workfront] pannello a destra.</p><p>Nota: le sezioni del modulo personalizzato vengono visualizzate nel [!DNL Workfront] con il livello di accesso del [!DNL Workfront] Amministratore di sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priorità nel pannello a destra in [!DNL Jira]]</td>
         <td>Visualizza la [!DNL Workfront] Priorità di un elemento in [!DNL Workfront] pannello a destra.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Aggiungi un aggiornamento in [!DNL Workfront] Scheda Aggiornamenti sulle modifiche della data di scadenza in [!DNL Jira]]</td>
         <td>Aggiunge un commento nella scheda [!UICONTROL Update] del [!DNL Workfront] elemento quando [!UICONTROL Scadenza] cambia in collegato [!DNL Jira] elemento.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crea automaticamente un utente in [!DNL Workfront] se [!DNL Jira] l’utente non dispone di un [!DNL Workfront] account]</td>
         <td><p>Esistono i seguenti scenari:</p>
          <ul>
           <li>Quando selezioni <strong>[!UICONTROL Always]</strong>, l’integrazione consente di creare un nuovo utente Workfront ogni volta che [!DNL Jira] utente senza un [!DNL Workfront] l'account esegue le azioni seguenti su un [!DNL Jira] problema:
            <ul>
             <li>È assegnato a un [!DNL Jira] problema</li>
             <li><p>Registra il tempo su un [!DNL Jira] problema</p><p>Questo nuovo utente non occupa un [!DNL Workfront] licenza. L'impostazione predefinita è Always. L’utente ha creato in questo modo in [!DNL Workfront] ha "[!UICONTROL Jira]" aggiunto al nome.</p></li>
            </ul></li>
           <li>Quando selezioni <strong>[!UICONTROL Never]</strong>, si verificano le seguenti situazioni:
            <ul>
             <li>Non sei in grado di visualizzare [!DNL Jira] assegnazioni sul [!DNL Workfront] elementi. In questo caso, solo le assegnazioni effettuate in [!DNL Workfront] visualizzare sul [!DNL Workfront] elementi.</li>
             <li>Ora di accesso a un oggetto collegato [!DNL Jira] problema da parte di un utente senza [!DNL Workfront] l'account non viene trasferito automaticamente al [!DNL Workfront] elemento. È comunque possibile accedere al [!DNL Workfront] elemento nel pannello a destra della [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Fai clic su **[!UICONTROL Salva]**.

   Ora, ogni volta che un utente aggiorna uno qualsiasi dei campi specificati in questa configurazione su un elemento in [!DNL Jira] o [!DNL Workfront], viene aggiornato anche l’elemento collegato nell’altra applicazione.

## Risoluzione dei problemi

### Impossibile creare elementi in [!DNL Jira] a causa di campi trigger contrassegnati &quot;[!UICONTROL Impossibile trovare]&quot;

#### Problema

Quando si verifica un errore con [!DNL Workfront for Jira] applicazione, [!DNL Workfront] disabilita i trigger per prevenire ulteriori complicazioni. Quando questi trigger sono disabilitati, vengono visualizzati come &quot;[!UICONTROL Impossibile trovare].&quot;

#### Soluzione

Individua l’errore che ha disabilitato i trigger. L’errore si trova nella sezione [!DNL Workfront for Jira] [!UICONTROL Registro attività].

La causa più comune di questo comportamento è l’errore &quot;[!UICONTROL Impossibile impostare il campo &#39;duedate&#39;. Non si trova nella schermata appropriata o è sconosciuta.]&quot;

Questo errore indica che si sta tentando di sincronizzare &quot;[!UICONTROL Data di completamento Pianificata]&quot; da [!DNL Workfront] a [!DNL Jira]. A questo scopo, assicurati che il tuo [!DNL Jira] Gli oggetti hanno un campo denominato &quot;[!UICONTROL Data di scadenza].&quot; Se non hanno questo campo, [!DNL Workfront] non è in grado di sincronizzare la data di completamento pianificata da [!DNL Workfront] e disattiva i trigger.

Per risolvere l&#39;errore, eseguire una delle operazioni seguenti:

* Chiedi [!DNL Jira] l&#39;amministratore per aggiornare il [!DNL Jira] per garantire che abbiano un campo data di scadenza.
* Disattiva la sincronizzazione di [!DNL Workfront]data di completamento pianificata in Workfront [!UICONTROL Configurazione] pagina.
