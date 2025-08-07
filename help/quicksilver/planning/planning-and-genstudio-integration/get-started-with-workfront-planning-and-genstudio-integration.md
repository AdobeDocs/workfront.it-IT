---
title: Guida introduttiva all'integrazione di Workfront Planning e GenStudio for Performance Marketing
description: L’area di lavoro GenStudio for Performance Marketing è disponibile in Adobe Workfront Planning quando la tua azienda ha acquistato entrambi i prodotti. Scopri alcune delle nozioni di base su come semplificare i flussi di lavoro utilizzando questa integrazione.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---

# Guida introduttiva all&#39;integrazione di Workfront Planning e GenStudio for Performance Marketing

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

Le organizzazioni che utilizzano sia Adobe Workfront Planning che Adobe GenStudio for Performance Marketing spesso definiscono concetti di marketing come Campagne, Prodotti e Personas in modo più dettagliato rispetto a quanto supportato da GenStudio per impostazione predefinita.

Esiste un&#39;integrazione nativa tra GenStudio for Performance Marketing e Workfront Planning. Questa integrazione consente agli utenti di Workfront Planning di gestire Campagne, Prodotti, Utenti tipo, Attivazioni, Canali e Aree geografiche utilizzati in GenStudio. Consente inoltre di configurare GenStudio per fare riferimento ai tipi di record esistenti di Workfront Planning, creando un flusso di lavoro di marketing più connesso e coerente.

Questa integrazione consente di evitare l’immissione di dati duplicati, mantenere l’allineamento tra le attività di pianificazione e attivazione e supporta il sistema di record di marketing.

L’area di lavoro GenStudio for Performance Marketing è disponibile in Adobe Workfront Planning quando la tua azienda ha acquistato entrambi i prodotti.

Con l&#39;integrazione tra Workfront Planning e GenStudio for Performance Marketing, è possibile:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Visualizzare l&#39;area di lavoro di GenStudio in Workfront Planning.
* Modificare le campagne in GenStudio e aggiornare le stesse informazioni in tempo reale in Workfront Planning.
* Modifica le campagne in Workfront Planning e aggiorna le stesse informazioni in tempo reale in GenStudio.

## Requisiti di integrazione

* Workfront e GenStudio for Performance Marketing devono essere abilitati nella stessa organizzazione.

  Per ulteriori informazioni su GenStudio, consulta [Guida utente di Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).

* GenStudio non sarà disponibile in Workfront Planning quando la società dispone di più istanze di Workfront. <!--this will change-->

* L’istanza di Workfront fa parte di Adobe Unified Experience, incluso l’utilizzo di Identity Management System (IMS).

  Per informazioni, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Gli utenti che utilizzano sia Planning che GenStudio possono appartenere a una sola istanza di Workfront all’interno dell’organizzazione IMS.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Requisiti di accesso

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p> Amministratore di sistema</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro e a un tipo di record  </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Panoramica dell&#39;integrazione di Workfront Planning e GenStudio

Le sezioni seguenti descrivono quanto segue:

* Funzionalità per l&#39;aggiornamento delle informazioni di Workfront Planning da GenStudio
* Funzionalità per l&#39;aggiornamento delle informazioni di GenStudio da Workfront Planning
* Limitazioni di ciò che è possibile e non è possibile gestire in un&#39;area di lavoro di GenStudio da Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Area di lavoro GenStudio in Workfront Planning

* Se la tua organizzazione dispone di più istanze di Workfront, l’area di lavoro di GenStudio non è visibile da alcuna istanza di Workfront. <!-- this might change-->
* Nell’area di lavoro di GenStudio viene visualizzato un indicatore visivo che indica chiaramente che è stata importata da GenStudio. Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Tutti gli utenti che hanno accesso sia a GenStudio che a Workfront Planning possono inoltre visualizzare l&#39;area di lavoro di GenStudio in Workfront Planning.
* Gli utenti di Workfront Planning devono essere gestiti tramite Adobe Identity Management System (IMS) per poter visualizzare e utilizzare l&#39;area di lavoro di GenStudio da Workfront.

  Gli utenti che utilizzano solo Workfront non possono visualizzare l’area di lavoro di GenStudio, anche quando è disponibile in Workfront.

  Per informazioni, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Tipi di record

* È possibile modificare le informazioni sui tipi di record, ad esempio l&#39;aspetto, da GenStudio in Workfront Planning.
* È possibile condividere i tipi di record di GenStudio con altri utenti in Planning.  <!--checking with Ani H.-->
* È possibile creare tipi di record da Planning nell&#39;area di lavoro di GenStudio. <!-- checking with Ani where these show up in GenS-->
* I tipi di record sincronizzati con GenStudio visualizzano un indicatore visivo che indica chiaramente che i tipi di record vengono importati da GenStudio.

### Record

* È possibile aggiungere o eliminare record in GenStudio in modo che diventino visibili o vengano rimossi da Workfront Planning.
È possibile aggiungere o eliminare record in Workfront Planning in modo che diventino visibili o vengano rimossi da GenStudio.
* È possibile aggiungere record da Workfront Planning nei modi seguenti:

   * Manualmente, da zero, da qualsiasi vista utilizzando il pulsante Nuovo record
   * Importandoli utilizzando un file CSV o Excel
   * Manualmente, in linea, nella vista a tabella
   * Manualmente, direttamente nella vista timeline

  Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* Non è possibile creare o eliminare record di attivazione da Workfront Planning.
* È possibile modificare le informazioni sui record di tutti i record nell&#39;area di lavoro di GenStudio in Planning in qualsiasi campo visibile di Workfront Planning.

  Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Campi

* I campi record vengono importati da GenStudio. È possibile modificare le impostazioni dei campi in Workfront Planning.
* In Workfront Planning è possibile creare più campi per i tipi di record GenStudio se si dispone dell&#39;accesso Gestisci in Gen Studio.
* Quando si creano campi per i tipi di record di GenStudio in Planning, questi sono visibili dalle seguenti aree:
   * Visualizzazioni di pianificazione
   * Pagine dei dettagli dei record di pianificazione
   * Pagine dettagli record GenStudio

  >[!TIP]
  >
  >I campi creati in Workfront Planning non sono visibili nella vista a elenco di GenStudio.

* È possibile nascondere i campi nella vista tabella di un tipo di record di GenStudio in Planning, ma non è possibile eliminare i campi da Workfront Planning.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Viste

* È possibile creare visualizzazioni per i tipi di record di GenStudio.

  Per informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

* È possibile condividere la vista di un tipo di record di GenStudio come si condivide una vista per un tipo di record di Planning.

### Connessioni

* In Workfront Planning è possibile effettuare le seguenti connessioni tra i tipi di record di GenStudio e altri tipi di record o oggetti:

   * Due tipi di record GenStudio e
   * Un tipo di record GenStudio e un tipo di record Planning dello stesso workspace
   * Un tipo di record GenStudio e un tipo di record Planning da un&#39;altra area di lavoro, se i tipi di record sono configurati per la connessione da un&#39;altra area di lavoro.
   * Un tipo di record GenStudio e un tipo di oggetto Workfront (progetti, portafogli, programmi, società, gruppi)