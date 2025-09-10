---
title: Guida introduttiva all'integrazione di Workfront Planning e GenStudio for Performance Marketing
description: L’area di lavoro GenStudio for Performance Marketing è disponibile in Adobe Workfront Planning quando la tua azienda ha acquistato entrambi i prodotti. Scopri alcune delle nozioni di base su come semplificare i flussi di lavoro utilizzando questa integrazione.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1906'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Guida introduttiva all’integrazione di Adobe Workfront Planning ed Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Le organizzazioni che utilizzano sia Adobe Workfront Planning che Adobe GenStudio for Performance Marketing spesso definiscono concetti di marketing come campagne, prodotti, attivazioni e utenti tipo in modo più dettagliato rispetto a quello supportato da GenStudio per impostazione predefinita.

Esiste un&#39;integrazione nativa tra GenStudio for Performance Marketing e Workfront Planning. Questa integrazione consente agli utenti di Workfront Planning di gestire Campagne, Prodotti, Utenti tipo, Attivazioni, Canali e Aree geografiche utilizzati in GenStudio. Consente inoltre di configurare GenStudio per fare riferimento ai tipi di record esistenti di Workfront Planning, creando un flusso di lavoro di marketing più connesso e coerente.

L’area di lavoro GenStudio for Performance Marketing è disponibile in Adobe Workfront Planning quando la tua azienda ha acquistato entrambi i prodotti.

## Vantaggi dell’integrazione

Con l&#39;integrazione tra Workfront Planning e GenStudio for Performance Marketing, è possibile:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Visualizzare l&#39;area di lavoro di GenStudio in Workfront Planning.
* Modifica campagne, prodotti, utenti tipo e attivazioni in GenStudio for Performance Marketing e ottieni aggiornamenti in tempo reale delle stesse informazioni in Workfront Planning.
* Modifica campagne, prodotti, utenti tipo e attivazioni in Workfront Planning e ottieni aggiornamenti in tempo reale delle stesse informazioni in GenStudio for Performance Marketing.
* Evita la duplicazione dei dati.
* Mantenere l&#39;allineamento tra le attività di pianificazione e attivazione.

## Requisiti di integrazione

Affinché l&#39;integrazione tra Workfront Planning e GenStudio for Performance Marketing possa esistere, l&#39;organizzazione deve soddisfare i seguenti requisiti:

* Workfront e GenStudio for Performance Marketing devono essere abilitati nella stessa organizzazione.

  Per ulteriori informazioni su GenStudio, consulta [Guida utente di Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* La tua istanza di Workfront fa parte di Adobe Unified Experience, incluso l’utilizzo di Identity Management System (IMS).

  Per informazioni, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Gli utenti che utilizzano sia Workfront Planning che GenStudio for Performance Marketing devono appartenere a una sola istanza di Workfront all’interno dell’organizzazione IMS.

  Gli utenti solo Workfront possono visualizzare l’area di lavoro di GenStudio, anche se non sono utenti GenStudio for Performance Marketing.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Requisiti di accesso

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront</p>
<p>Qualsiasi pacchetto Planning</p>

</td> </tr>
   <tr> 
<td> 
   <p> Prodotti aggiuntivi</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Ruoli utente di Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualsiasi ruolo utente di GenStudio per accedere a Campagne, Prodotti e Utenti tipo</li>
   <li>GenSudio System Manager per accedere alle attivazioni <!--and Events--></li></ul>
   Per informazioni, vedere <a href="https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Ruoli utente e autorizzazioni</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Gestisci le autorizzazioni per l’area di lavoro di GenStudio per aggiungere nuovi campi o tipi di record all’area di lavoro di GenStudio</p></li>
   <li><p>Autorizzazioni di Contribute all'area di lavoro di GenStudio per aggiungere, aggiornare o eliminare record nell'area di lavoro di GenStudio</p> </li>  
   </ul>
   <p>Nessun utente può rimuovere tipi di record o campi GenStudio for Performance Marketing dall'area di lavoro di GenStudio in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Qualsiasi autorizzazione in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Creare le autorizzazioni in Adobe GenStudio for Performance Marketing per creare elementi</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Per informazioni sull&#39;accesso ad Adobe Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Per ulteriori informazioni su Adobe GenStudio for Performance Marketing, consulta [Guida utente di Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/home).


## Panoramica delle funzionalità di integrazione di Workfront Planning e GenStudio for Performance Marketing

A seconda del numero di istanze di Workfront dell&#39;organizzazione, si dispone automaticamente delle seguenti autorizzazioni per l&#39;area di lavoro di GenStudio in Planning:

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Un’istanza di Workfront</p></td> 
   <td> 
<p>L'area di lavoro di GenStudio è visibile nell'istanza di Workfront Planning</p>
<p>Per impostazione predefinita, tutti gli utenti, inclusi gli amministratori di Workfront, hanno accesso all'area di lavoro di GenStudio in Planning</p>
<p>Gli amministratori di Workfront possono modificare e concedere a chiunque le autorizzazioni Gestione nell’area di lavoro di GenStudio</p>
</td> </tr>
   <tr> 
<td> 
   <p> Più istanze di Workfront</p> </td> 
   <td> 
   <p>L’area di lavoro di GenStudio è visibile da tutte le istanze di Workfront</p>
<p>Per impostazione predefinita, tutti gli utenti con accesso a GenStudio for Performance Marketing e Workfront Planning dispongono delle autorizzazioni Contribute per GenStudio in Planning</p> 
<p>Gli amministratori di Workfront non possono concedere a nessuno le autorizzazioni di gestione per l’area di lavoro di GenStudio</p>

</td> 
  </tr>
   </tbody> 
</table>

Per informazioni sulle autorizzazioni di Workfront Planning, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Le sezioni seguenti descrivono:

* Funzionalità per l&#39;aggiornamento delle informazioni di Workfront Planning da GenStudio for Performance Marketing
* Funzionalità per l&#39;aggiornamento delle informazioni di GenStudio for Performance Marketing da Workfront Planning
* Limitazioni di ciò che è possibile e non è possibile gestire in un&#39;area di lavoro di GenStudio da Workfront Planning.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Area di lavoro GenStudio in Workfront Planning

* Nell&#39;area di lavoro di GenStudio viene visualizzato un indicatore visivo in Workfront Planning per identificarlo come rappresentante l&#39;area di lavoro di GenStudio for Performance Marketing.

  ![Scheda GenStudio in Planning](assets/genstudio-card-with-tag-highlighted.png)

  Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Quando si dispone delle autorizzazioni Gestione per l&#39;area di lavoro di GenStudio in Planning, è possibile:

   * Aggiornare l&#39;area di lavoro di GenStudio in Planning (nome, descrizione, icona)
   * Creare sezioni
   * Aggiungi tipi di record
   * Condividi con altri

     Puoi condividere l’area di lavoro di GenStudio con altri utenti che non dispongono di un account GenStudio. Puoi condividerlo solo con gli utenti disponibili nel sistema Identity Management (IMS) della tua organizzazione. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Se si dispone delle autorizzazioni Contribute per l&#39;area di lavoro di GenStudio in Planning, non è possibile modificare l&#39;area di lavoro da Workfront Planning.

### Tipi di record nell’area di lavoro di GenStudio

* I tipi di record visibili sia in GenStudio for Performance Marketing che in Planning dispongono di un indicatore GenStudio in Workfront Planning.

  ![Scheda del tipo di record di GenStudio in Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro di GenStudio in Planning, è possibile eseguire le operazioni seguenti da Workfront Planning:
   * Modificare le informazioni sui tipi di record di GenStudio (aspetto e impostazioni avanzate).
   * Condividere tipi di record GenStudio con altri utenti.
   * Creare tipi di record. Questi tipi di record rimangono solo in Workfront Planning. Non vengono visualizzati in GenStudio.
   * Consente ai record dell&#39;area di lavoro di GenStudio di connettersi da altre aree di lavoro.
   * Consente di aggiungere record dall&#39;area di lavoro di GenStudio ad altre aree di lavoro.
* Se si dispone delle autorizzazioni Contribute per l&#39;area di lavoro di GenStudio in Planning, non è possibile modificare i tipi di record di GenStudio da Planning.

### Record nell’area di lavoro di GenStudio

* Quando si modificano i record di GenStudio da GenStudio for Performance Marketing, le modifiche sono visibili nell&#39;area di lavoro di GenStudio in tutte le istanze di Workfront.
* Non è possibile creare o eliminare record di attivazione dall&#39;area di lavoro di GenStudio in Workfront Planning.
* Se si dispone delle autorizzazioni Gestione o Contribuisci all&#39;area di lavoro di GenStudio in Planning, è possibile effettuare le seguenti operazioni da Workfront Planning:
   * Aggiungere o eliminare record che diventano visibili in GenStudio for Performance Marketing o vengono rimossi da esso.

     I record eliminati da Workfront Planning o da GenStudio for Performance Marketing vengono inseriti nel contenitore di Workfront Planning eliminato di recente per 30 giorni. GenStudio for Performance Marketing non dispone di un raccoglitore eliminato di recente.
   * Ripristinare un record dal raccoglitore eliminato di recente. Il ripristino dei record eliminati li riposiziona in Workfront Planning e GenStudio for Performance Marketing.
   * Aggiungere record nei modi seguenti:

      * Manualmente, da zero, da qualsiasi vista utilizzando il pulsante Nuovo record
      * Importandoli utilizzando un file CSV o Excel nella vista a tabella
      * Manualmente, in qualsiasi vista di Workfront Planning
      * Inviando una richiesta a un modulo di richiesta di tipo record in Workfront.

  Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* È possibile modificare le informazioni sui record di tutti i record nell&#39;area di lavoro di GenStudio da Workfront Planning.

  Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Campi del tipo di record nell’area di lavoro di GenStudio

* Per impostazione predefinita, i campi del tipo di record vengono importati da GenStudio for Performance Marketing in Workfront Planning.
* Non è possibile aggiungere campi ai tipi di record di GenStudio for Performance Marketing.
<!--Iskuhi said this is not possible but I can add fields: * You cannot create or delete Activation records' fields from the GenStudio workspace in Workfront Planning. -->
* Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro di GenStudio in Planning, è possibile eseguire le operazioni seguenti da Workfront Planning:

   * Modifica le impostazioni dei campi di GenStudio.
   * Creare campi per i tipi di record GenStudio, se si dispone dell&#39;accesso Gestione nell&#39;area di lavoro Gen Studio.

     Quando si creano campi per i tipi di record di GenStudio in Planning, questi sono visibili dalle seguenti aree:

      * Visualizzazioni di Workfront Planning
      * Pagine dei dettagli dei record di Workfront Planning
      * Pagine dettagli record GenStudio

     >[!TIP]
     >
     >I campi creati in Workfront Planning non sono visibili nella vista a elenco di GenStudio.

   * Nascondere i campi nella vista tabella di un tipo di record GenStudio in Workfront Planning.
&lt;!—* Eliminare i campi creati in Workfront Planning per i tipi di record di GenStudio da Workfront Planning. — questo non è possibile, secondo Iskuhi; il collegamento è lì, ma genererà un errore—>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Quando si dispone delle autorizzazioni Contribute per l&#39;area di lavoro di GenStudio in Planning:

   * Non è possibile modificare le impostazioni dei campi, eliminare o aggiungere campi dall&#39;area di lavoro di GenStudio in Workfront Planning.
   * È possibile nascondere i campi dalla vista tabella in Workfront Planning.

#### I campi Creato da e Approvato da

* È possibile aggiungere i campi Creato da e Approvato da per i tipi di record GenStudio in Workfront Planning da Workfront Planning.
* I record visualizzati nei tipi di record Canale e Regione visualizzeranno &quot;Sistema&quot; come Creato dall’utente. Questi record vengono creati automaticamente quando l&#39;area di lavoro di GenStudio viene creata in Workfront Planning.
* Nei record creati in GenStudio dopo la disponibilità dell&#39;area di lavoro in Workfront Planning verrà visualizzato il nome dell&#39;utente IMS che ha creato il record nel campo Creato da, anche se l&#39;utente ha creato i record in GenStudio e non è un utente di Workfront.
* Nel campo Approvato da viene visualizzato il nome dell&#39;approvatore quando viene sottomesso un modulo di richiesta per creare un record nel tipo di record GenStudio in Workfront Planning.
* I campi Creato da e Approvato da vengono visualizzati nei dettagli dei record in GenStudio for Performance Marketing. Non vengono visualizzati nella vista a elenco.

### Visualizzazioni record nell’area di lavoro di GenStudio

>[!NOTE]
>
>I tipi di record di GenStudio vengono visualizzati nella vista tabella predefinita importata dalla vista a elenco di GenStudio for Performance Marketing.
>
>Non è possibile eliminare la vista tabella originale importata per impostazione predefinita da GenStudio for Performance Marketing.

* Non è possibile creare più viste in GenStudio for Performance Marketing.

* Se si dispone delle autorizzazioni Gestione per l&#39;area di lavoro di GenStudio in Planning, è possibile eseguire le operazioni seguenti da Workfront Planning:

   * Creare visualizzazioni per i tipi di record di GenStudio.

     Per informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

   * Rinominare, condividere, esportare, duplicare o eliminare visualizzazioni personalizzate dai tipi di record di GenStudio.

* Quando si dispone delle autorizzazioni Contribute per l&#39;area di lavoro di GenStudio in Planning, è possibile effettuare le seguenti operazioni da Workfront Planning:

   * Creare visualizzazioni per i tipi di record di GenStudio.

     Per informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

   * Rinominare, esportare, duplicare o eliminare visualizzazioni personalizzate dai tipi di record di GenStudio.

     Impossibile condividere le viste dall&#39;area di lavoro di GenStudio in Workfront Planning

### Registrare le connessioni nell’area di lavoro di GenStudio

È possibile creare connessioni tra tipi di record nelle aree di lavoro di GenStudio in cui si dispone delle autorizzazioni di gestione.

In Workfront Planning è possibile effettuare le seguenti connessioni tra i tipi di record di GenStudio e altri tipi di record o oggetti:

* Due tipi di record GenStudio
* Un tipo di record GenStudio e un tipo di record Planning dello stesso workspace
* Un tipo di record GenStudio e un tipo di record Planning da un&#39;altra area di lavoro, se i tipi di record sono configurati per la connessione da un&#39;altra area di lavoro.
* Un tipo di record GenStudio e un tipo di oggetto Workfront (progetti, portafogli, programmi, società, gruppi)
* Un tipo di record GenStudio e un tipo di oggetto AEM Assets.

### Moduli di richiesta e automazioni nel tipo di record GenStudio

* È possibile aggiungere moduli di richiesta a un tipo di record GenStudio in Workfront Planning.

  Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* In Workfront Planning è possibile configurare le automazioni per un tipo di record GenStudio.

  Per informazioni, vedere [Configurare le automazioni di Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

## Ambiente di anteprima

* Anche l’area di lavoro GenStudio accessibile dall’ambiente di produzione viene visualizzata nell’ambiente di anteprima della stessa istanza di Workfront.
* È possibile eseguire tutte le attività descritte in questo articolo nell&#39;area di lavoro di GenStudio in Workfront Planning nell&#39;ambiente di anteprima, ma tali modifiche non saranno visibili da GenStudio.

  Solo le modifiche apportate agli elementi nell&#39;ambiente di produzione vengono sincronizzate tra Workfront Planning e GenStudio.

  GenStudio non dispone di un ambiente di anteprima.

