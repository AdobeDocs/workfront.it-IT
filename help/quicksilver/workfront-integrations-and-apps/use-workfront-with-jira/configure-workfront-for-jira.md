---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configura [!DNL Adobe Workfront for Jira]
description: Puoi utilizzare  [!DNL Adobe Workfront for Jira] per integrare i tuoi [!DNL Jira] e [!DNL Workfront] sistemi.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '2470'
ht-degree: 0%

---

# Configura [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, l&#39;integrazione Workfront for Jira non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Jira.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Jira, vedere [Moduli software Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

È possibile utilizzare [!DNL Adobe Workfront for Jira] per integrare i sistemi [!DNL Jira] e [!DNL Workfront].

Dopo aver installato il componente aggiuntivo, è possibile definire flussi di lavoro che creano automaticamente [!DNL Jira] problemi alla creazione di [!DNL Workfront] elementi di lavoro. Gli elementi di entrambe le applicazioni vengono collegati e alcune delle relative informazioni vengono aggiornate automaticamente in entrambi i sistemi.

Tutti gli utenti in [!DNL Workfront] e [!DNL Jira] possono beneficiare di questa integrazione. È sufficiente una licenza per il sistema in cui operano maggiormente e non per entrambi i sistemi.

Questo componente aggiuntivo è disponibile per entrambe le versioni [!UICONTROL Server] e [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software [!DNL Jira].

Per un elenco di [!DNL Jira] versioni attualmente supportate da [!DNL Workfront for Jira], vedere [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) in [!DNL Atlassian Marketplace].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] piano]</td> 
   <td><p>Nuovo: Qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: [!UICONTROL Pro] o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard] </p>
       <p>oppure</p> 
       <p>Corrente: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di configurare [!DNL Workfront for Jira], è necessario:

* Installa [!DNL Workfront for Jira].
Per istruzioni sull&#39;installazione di [!DNL Workfront for Jira], vedere [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configura [!DNL Workfront for Jira]

Configurando [!DNL Workfront for Jira], è possibile:

* Definisci i trigger che creeranno [!DNL Jira] elementi quando vengono creati [!DNL Workfront] elementi.
* Specificare i campi da sincronizzare tra gli elementi collegati tra [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Dopo aver configurato [!DNL Workfront for Jira] nell&#39;ambiente [!DNL Jira], tutti gli utenti [!DNL Jira] visualizzano un pannello destro [!DNL Workfront] su tutti gli elementi [!DNL Jira]. Il pannello contiene informazioni sugli elementi che potrebbero essere collegati da [!DNL Workfront] o specifica che nessun elemento [!DNL Workfront] è collegato a [!DNL Jira] elementi.
>* Quando si utilizza l&#39;installazione di [!DNL Jira Server], nel pannello Workfront vengono visualizzati solo i problemi associati ai progetti identificati come attivatori per l&#39;integrazione di Workfront. Per ulteriori informazioni sulla configurazione dei trigger per il flusso di lavoro [!DNL Workfront to Jira], vedere [Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Per configurare [!DNL Workfront for Jira]:

1. Accedere a [!DNL Jira] come amministratore [!DNL Jira].
1. Fare clic su **[!UICONTROL Impostazioni]** nel menu principale di [!DNL Jira].
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi fai clic su **[!UICONTROL Gestisci componenti aggiuntivi]**.

1. Espandere il componente aggiuntivo **[!DNL Workfront]**.
1. Fare clic su **[!UICONTROL Configura]**.
1. Seguire le istruzioni per accedere a [!DNL Workfront].

   >[!NOTE]
   >
   >L&#39;utente deve avere un `apiKey` valido in [!UICONTROL Workfront] per creare una connessione riuscita.

   Per continuare la configurazione, è necessario accedere a [!DNL Workfront] come amministratore [!DNL Workfront].

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] si connette a [!DNL Jira] utilizzando OAuth 2.0, uno standard utilizzato dalla maggior parte delle integrazioni basate sul Web per l&#39;autenticazione e l&#39;autorizzazione degli utenti.
   >* Quando viene richiesto di immettere il dominio dell&#39;account [!DNL Workfront], digitarlo in questo formato: *yourCompany&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L&#39;autenticazione avanzata non è disponibile finché non viene abilitata da un amministratore [!DNL Workfront] per questa integrazione.

1. In Jira, seleziona la scheda **[!UICONTROL Triggers]** per configurare la creazione automatica di [!DNL Jira] elementi durante la creazione di nuovi [!DNL Workfront] elementi.

   Per ulteriori informazioni sulla configurazione dei trigger per il flusso di lavoro da Workfront a [!DNL Jira], vedere [Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Selezionare la scheda **[!UICONTROL Configurazione]** per configurare la sincronizzazione dei campi tra gli elementi collegati [!DNL Jira] e [!DNL Workfront].

   Per ulteriori informazioni sulla configurazione della sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront], vedere [Configurare la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] Elementi](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Dopo aver definito i trigger e la sincronizzazione dei campi tra le due applicazioni, qualsiasi utente [!DNL Workfront] in grado di creare attività o problemi potrebbe potenzialmente attivare la creazione di un elemento in [!DNL Jira]. L&#39;utente può creare un elemento se i criteri dell&#39;elemento creato corrispondono ai trigger in [!DNL Jira], anche se l&#39;utente non dispone di una licenza di [!DNL Jira]. Inoltre, qualsiasi utente [!DNL Jira] può iniziare immediatamente a lavorare sull&#39;elemento [!DNL Jira] e i relativi aggiornamenti sono visibili in [!DNL Workfront], senza disporre di una licenza [!DNL Workfront]. Eventuali aggiornamenti in [!DNL Workfront] sono visibili anche sugli elementi [!DNL Jira].

1. (Facoltativo) Seleziona la scheda **[!UICONTROL Registro attività]** per esaminare eventuali errori che potrebbero essersi verificati durante l&#39;integrazione.

   Per ulteriori informazioni sul [!UICONTROL registro attività], vedere [Visualizza il [!DNL Jira] [!UICONTROL registro attività]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurare i trigger per il collegamento automatico degli elementi tra [!DNL Jira] e [!DNL Workfront]

In qualità di amministratore di sistema [!DNL Jira], puoi definire trigger che creerebbero automaticamente problemi in [!DNL Jira] quando un elemento in [!DNL Workfront] soddisfa determinati criteri.

>[!NOTE]
>
>La creazione di nuovi problemi in [!DNL Jira] potrebbe richiedere fino a 10 minuti per l&#39;integrazione.

Quando si configura l&#39;attivazione della creazione di [!DNL Jira] elementi durante la creazione di [!DNL Workfront] elementi, tenere presente quanto segue:

* L&#39;integrazione è unidirezionale: è possibile attivare solo gli elementi creati in [!DNL Workfront] per la creazione automatica in [!DNL Jira]. Impossibile attivare la creazione automatica in [!DNL Jira] degli elementi creati in [!DNL Workfront].
* Non esiste alcun limite al numero di attivatori che è possibile avere.
* Se un elemento creato in [!DNL Workfront] corrisponde a più di uno dei trigger, in [!DNL Jira] verrà creato un solo elemento. L&#39;elemento viene creato in [!DNL Jira] in base al primo trigger (nell&#39;ordine in cui sono stati definiti in [!DNL Jira]). Tutti gli altri trigger vengono ignorati.
* È possibile collegare un solo elemento in [!DNL Workfront] a un elemento in Jira. Non puoi collegare un elemento [!DNL Workfront] a più problemi [!DNL Jira] o un problema [!DNL Jira] a più elementi [!DNL Workfront].

Per configurare i trigger per la creazione automatica di elementi in [!DNL Jira]:

1. Accedere a [!DNL Jira] come amministratore di sistema.
1. Fare clic su **[!UICONTROL Impostazioni]** nel menu principale di [!DNL Jira].
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi su **[!UICONTROL Gestisci componenti aggiuntivi]**.
1. Espandere il componente aggiuntivo **[!DNL Workfront]**.
1. Fare clic su **[!UICONTROL Configura]**.
1. Accedere a [!DNL Workfront] come amministratore di sistema.

   La scheda **[!UICONTROL Triggers]** è selezionata per impostazione predefinita in Jira.

1. Fai clic su **[!UICONTROL Aggiungi trigger]** per aggiungere un nuovo trigger.
1. Nel campo **[!UICONTROL Team/utente/ruolo]** di Workfront, specificare il nome di un team, un utente o una mansione [!DNL Workfront], quindi fare clic su di esso per selezionarlo quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Non è possibile avere più trigger per lo stesso team, utente o ruolo.

   Quando un utente crea un&#39;attività o un problema e lo assegna a una di queste entità, viene automaticamente creato un problema in [!DNL [!DNL Jira]].

1. Nel campo **[!UICONTROL [!DNL Jira]progetto]**, inizia a digitare il nome di un progetto [!DNL Jira], quindi fai clic su per selezionarlo quando viene visualizzato nell&#39;elenco.

   Quando viene creato il problema [!DNL Jira], questo viene inserito nel progetto scelto qui.

1. Seleziona un tipo di **I[!UICONTROL problema]** dal menu a discesa.

   Indica il tipo di problema creato in [!DNL Jira] quando vengono soddisfatte le condizioni di questo trigger, in base alle impostazioni per quel progetto specifico in [!DNL Jira].

1. Fai clic su **[!UICONTROL Salva]**.

   Con questa configurazione, ogni volta che un utente di [!DNL Workfront] crea un elemento che corrisponde ai trigger specificati, viene creato un nuovo problema in [!DNL Jira].

## Configura la sincronizzazione dei campi tra [!DNL Jira] e [!DNL Workfront] elementi

In qualità di amministratore [!DNL Jira], puoi definire quali campi devono essere sincronizzati automaticamente sugli elementi collegati tra [!DNL Workfront] e Jira. Alcuni campi possono essere sincronizzati da [!DNL Workfront] all&#39;elemento [!DNL Jira], mentre altri possono essere sincronizzati da Jira a Workfront.

Per definire i campi da sincronizzare automaticamente sugli elementi collegati tra le due applicazioni:

1. Accedi a [!DNL Jira] come amministratore Jira.
1. Fare clic su **[!UICONTROL Impostazioni]** nel menu principale di [!DNL Jira].
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi su **[!UICONTROL Gestisci componenti aggiuntivi]**.
1. Espandere il componente aggiuntivo **[!DNL Workfront]**.
1. Fare clic su **[!UICONTROL Configura]**.
1. Accedere a [!DNL Workfront] come amministratore Workfront.
1. In Jira, fare clic sulla scheda **[!UICONTROL Configurazione]**.
1. Nella sezione **[!UICONTROL Sincronizza da Workfront a Jira]**, seleziona i campi che desideri aggiornare in [!DNL Jira] quando vengono aggiornati in Workfront.

   1. Selezionare una delle seguenti frequenze con cui vengono sincronizzati i campi:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Alla Creazione]</td>
              <td>I campi specificati vengono sincronizzati tra gli elementi Workfront collegati e [!DNL Jira] quando l'elemento viene creato in Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>I campi specificati vengono sincronizzati tra gli elementi Workfront collegati e [!DNL Jira] quando vengono aggiornati in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>I campi specificati non vengono mai sincronizzati tra gli elementi collegati [!DNL Workfront] e [!DNL Jira]. Nessuna indicazione in [!DNL Jira] che il campo sia stato aggiornato in [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selezionare una delle opzioni seguenti per sincronizzare i campi da [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Il nome di un'attività o di un problema in [!DNL Workfront] diventa il nome del problema a cui è collegato in [!DNL Jira].</p><p>Nota: quando vengono creati automaticamente nuovi elementi in [!DNL Jira], il nome [!DNL Workfront] viene sempre aggiornato sull'elemento [!DNL Jira], indipendentemente dal fatto che questo campo sia abilitato o meno. Quando un elemento [!DNL Jira] è collegato manualmente a un elemento [!DNL Workfront], il nome dell'elemento [!DNL Workfront] viene aggiornato solo in [!DNL Jira] quando si seleziona <strong>Sincronizza sempre</strong> questo campo. Per ulteriori informazioni sul collegamento manuale o automatico degli elementi, vedere <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Collegare gli elementi tra [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrizione]</td>
         <td>La descrizione di un'attività o di un problema in [!DNL Workfront] diventa la descrizione del problema a cui è collegata in [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documenti</td>
         <td><p>I documenti allegati a un'attività o a un problema in [!DNL Workfront] sono allegati anche al problema a cui sono collegati in Jira. Le nuove versioni dei documenti da [!DNL Workfront] vengono aggiunte come documenti separati a Jira e sono aggiunte con <i>_v&lt;numero di versione&gt;</i> per indicare la versione numerata in Workfront. </p><p>Se ad esempio il nome di un documento in [!DNL Workfront] è <strong>Annuncio principale</strong> e si aggiunge una nuova versione in [!DNL Workfront], la nuova versione verrà trasferita in [!DNL Jira] come nuovo documento con il nome <strong>Annuncio principale_v2</strong>.</p><p>Importante: <p>Quando si sincronizzano i documenti, tenere presente quanto segue:</p>
           <ul>
            <li><p>I documenti superiori a 5 MB non vengono sincronizzati. Se la sincronizzazione di un documento non riesce perché il documento è troppo grande, nel registro attività viene registrato un errore. </p><p>Per ulteriori informazioni sul registro attività, vedere <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Visualizzare il registro attività Jira</a>.</p></li>
            <li><p>I documenti collegati ad attività e problemi da server esterni non vengono trasferiti agli elementi [!DNL Jira]. Solo i documenti caricati direttamente sull'attività o sul problema in [!DNL Workfront] vengono trasferiti al problema collegato in [!DNL Jira].</p></li>
            <li><p>Per creare una bozza da un documento, è necessario generarla in [!DNL Workfront]. </p><p>Per ulteriori informazioni sulla generazione di una bozza, vedere <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Creare una bozza per un documento esistente </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Creare una bozza per un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td>
         <td><p>La [!UICONTROL Planned Completion Date] (Data di completamento pianificata) di un'attività o di un problema in [!DNL Workfront] diventa la [!UICONTROL Due Date] del problema a cui è collegata in [!DNL Jira].</p><p>Nota: accertati di visualizzare <strong>[!UICONTROL Scadenza]</strong> su [!DNL Jira] problemi, per sincronizzare questo valore.</p></td>
        </tr>
       </tbody>
      </table>

1. Nella sezione **[!UICONTROL Sincronizza da [!DNL Jira] a[!DNL Workfront]]** selezionare i campi che si desidera aggiornare in [!DNL Workfront] quando vengono aggiornati in [!DNL Jira].

   1. Selezionare una delle seguenti frequenze con cui vengono sincronizzati i campi:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>I campi specificati vengono sempre sincronizzati tra gli elementi collegati [!DNL Workfront] e [!DNL Jira] quando vengono aggiornati in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>I campi specificati non vengono mai sincronizzati tra gli elementi collegati [!DNL Workfront] e [!DNL Jira]. Nessuna indicazione in [!DNL Workfront] che il campo sia stato aggiornato in [!DNL Jira]. </p><p>Nota: quando selezioni Mai, i campi [!DNL Workfront] possono ancora essere aggiornati manualmente da [!DNL Jira] nel pannello [!DNL Workfront] a sinistra del problema [!DNL Jira]. Questi aggiornamenti vengono visualizzati solo su [!DNL Workfront] elementi in [!DNL Jira] e [!DNL Workfront] e non su [!DNL Jira] elementi.</p></td>
        </tr>
       </tbody>
      </table>

   1. Selezionare questa opzione per sincronizzare i campi seguenti da [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Stato]</td>
         <td>Lo stato  di un problema in [!DNL Jira] diventa lo stato  dell'attività o del problema a cui è collegato in [!DNL Workfront].<br>Per ulteriori informazioni sugli stati [!DNL Workfront], vedere <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creare o modificare uno stato</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL assegnatario]</td>
         <td><p>Il [!UICONTROL Assignee] di un problema in [!DNL Jira] diventa il [!UICONTROL Assignee] dell'attività o del problema a cui è collegato in [!DNL Workfront].</p><p>Importante: quando si assegna un elemento in [!DNL Jira] a un utente che non dispone di un account [!DNL Workfront], l'integrazione crea un nuovo utente attivo in [!DNL Workfront] solo quando <strong>Crea automaticamente un utente in [!DNL Workfront] se l'utente [!DNL Jira] non dispone di un account [!DNL Workfront]</strong> è impostato su <strong>[!UICONTROL Always]</strong>. Questo utente non occupa una licenza [!DNL Workfront]. Gli utenti attivi possono essere assegnati ad elementi di lavoro in [!DNL Workfront], ma non possono essere inclusi negli aggiornamenti. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Allegati]</td>
         <td>Gli allegati di un problema in [!DNL Jira] sono allegati anche all'attività o al problema a cui è collegato in [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Commenti]</td>
         <td><p>Un commento su un problema di [!DNL Jira] è pubblicato anche sull'elemento [!DNL Workfront] collegato nell'area [!UICONTROL Aggiornamenti]. Al contrario, un commento pubblicato nell'area [!UICONTROL Updates] per un'attività [!DNL Workfront] o un problema si sincronizza con il flusso di commenti nativo di [!DNL Jira] per il problema collegato. </p><p>Impostazione predefinita: <strong>[!UICONTROL Always]</strong>. Se si seleziona <strong>[!UICONTROL Never]</strong> qui, è comunque possibile pubblicare commenti manualmente su un elemento collegato in [!DNL Workfront] o in [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Nella sezione **[!UICONTROL OTHER]**, seleziona i campi aggiuntivi da aggiornare tra gli elementi collegati.

   1. Selezionare un&#39;opzione per determinare se i campi specificati **[!UICONTROL Sempre]** o **[!UICONTROL Mai]** vengono aggiornati in [!DNL Jira] o [!DNL Workfront] quando vengono modificati.

   1. Seleziona uno dei campi e degli aggiornamenti seguenti:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copia [!DNL Workfront] dati personalizzati nel pannello di destra in [!DNL Jira]]</td>
         <td><p>Visualizza i dati personalizzati [!DNL Workfront] di un elemento nel pannello di destra [!DNL Workfront].</p><p>Nota: le sezioni dei moduli personalizzati vengono visualizzate nel pannello destro [!DNL Workfront] con il livello di accesso dell'amministratore di sistema [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copia [!DNL Workfront] Priorità nel pannello di destra in [!DNL Jira]]</td>
         <td>Visualizza la priorità [!DNL Workfront] di un elemento nel pannello di destra [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Aggiungi un aggiornamento nella scheda Aggiornamenti [!DNL Workfront] sulle modifiche alla data di scadenza in [!DNL Jira]]</td>
         <td>Aggiunge un commento nella scheda [!UICONTROL Update] dell'elemento [!DNL Workfront] quando [!UICONTROL Due Date] cambia nell'elemento [!DNL Jira] collegato.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crea automaticamente un utente in [!DNL Workfront] se l'utente [!DNL Jira] non dispone di un account [!DNL Workfront]]</td>
         <td><p>Esistono i seguenti scenari:</p>
          <ul>
           <li>Quando si seleziona <strong>[!UICONTROL Always]</strong>, l'integrazione consente di creare un nuovo utente di Workfront ogni volta che un utente [!DNL Jira] senza un account [!DNL Workfront] esegue le azioni seguenti su un problema [!DNL Jira] collegato:
            <ul>
             <li>È assegnato a un problema [!DNL Jira]</li>
             <li><p>Registra il tempo per un problema [!DNL Jira]</p><p>Questo nuovo utente non occupa una licenza [!DNL Workfront]. L'impostazione predefinita è Always. L'utente creato in questo modo in [!DNL Workfront] ha "[!UICONTROL Jira]" aggiunto al proprio nome.</p></li>
            </ul></li>
           <li>Quando si seleziona <strong>[!UICONTROL Never]</strong>, si verificano le seguenti condizioni:
            <ul>
             <li>Impossibile visualizzare [!DNL Jira] assegnazioni sugli elementi [!DNL Workfront]. In questo caso, solo le assegnazioni effettuate in [!DNL Workfront] vengono visualizzate sugli elementi [!DNL Workfront].</li>
             <li>L'ora registrata per un problema di [!DNL Jira] collegato da un utente senza un account di [!DNL Workfront] non viene trasferita automaticamente all'elemento di [!DNL Workfront] collegato. Puoi comunque registrare l'ora per l'elemento [!DNL Workfront] nel pannello a destra del problema [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Fai clic su **[!UICONTROL Salva]**.

   Ora, ogni volta che un utente aggiorna uno dei campi specificati in questa configurazione su un elemento in [!DNL Jira] o [!DNL Workfront], viene aggiornato anche l&#39;elemento collegato nell&#39;altra applicazione.

## Risoluzione dei problemi

### Impossibile creare elementi in [!DNL Jira] a causa di campi trigger contrassegnati come &quot;[!UICONTROL Impossibile trovare]&quot;

#### Problema

Quando si verifica un errore con l&#39;applicazione [!DNL Workfront for Jira], [!DNL Workfront] disabilita i trigger per evitare ulteriori complicazioni. Quando questi trigger sono disabilitati, vengono visualizzati come &quot;[!UICONTROL Impossibile trovare].&quot;

#### Soluzione

Individua l’errore che ha disabilitato i trigger. È possibile trovare l&#39;errore nel [!DNL Workfront for Jira] [!UICONTROL registro attività].

La causa più comune di questo comportamento è l&#39;errore &quot;[!UICONTROL Impossibile impostare il campo &#39;duedate&#39;. Non si trova nella schermata appropriata o è sconosciuta.]&quot;

Questo errore indica che si sta tentando di sincronizzare &quot;[!UICONTROL Data di completamento Pianificata]&quot; da [!DNL Workfront] a [!DNL Jira]. Per eseguire questa operazione, è necessario assicurarsi che gli oggetti [!DNL Jira] abbiano un campo denominato &quot;[!UICONTROL Scadenza]&quot;. Se non dispongono di questo campo, [!DNL Workfront] non è in grado di sincronizzare la data di completamento pianificata da [!DNL Workfront] e disabilita i trigger.

Per risolvere l&#39;errore, eseguire una delle operazioni seguenti:

* Chiedere all&#39;amministratore di [!DNL Jira] di aggiornare gli oggetti [!DNL Jira] interessati per assicurarsi che abbiano un campo data di scadenza.
* Disattiva la sincronizzazione della data di completamento pianificata di [!DNL Workfront] nella pagina [!UICONTROL Configurazione] di Workfront.
