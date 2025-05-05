---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: 2021-4-release-activity
title: Panoramica sulla versione 21.4
description: Questa pagina fornisce informazioni sulle funzionalità sia per Adobe Workfront Classic che per la nuova esperienza Adobe Workfront inclusa nella versione 21.4. per aumentare la produttività e la collaborazione.[Una riga di marketing per la versione]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '4718'
ht-degree: 0%

---

# Panoramica sulla versione 21.4

Questa pagina fornisce informazioni sulle funzionalità sia per Adobe Workfront Classic che per la nuova esperienza Adobe Workfront inclusa nella versione 21.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione nella settimana del 4 ottobre 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti Agile](#agile-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
* [Miglioramenti al reporting](#reporting-enhancements)
* [Richieste migliorate](#requests-enhancements)
* [Miglioramenti agli strumenti di correzione](#proofing-enhancements)
* [Miglioramenti all&#39;integrazione](#integration-enhancements)
* [Miglioramenti per dispositivi mobili](#mobile-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">Per gli amministratori: vedi quali gruppi sono associati a un processo di approvazione</a> </p> <p>Per aiutarti a individuare i gruppi associati ai processi di approvazione nel tuo sistema, abbiamo aggiunto una colonna Nome gruppo alla vista Standard nella pagina Approvazioni in Configurazione. Ora è possibile visualizzare queste informazioni senza dover creare una visualizzazione personalizzata.</p> </td> 
   <td> <p><b>Disponibile in queste date:</b> </p> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Novità per gli amministratori: i gruppi possono configurare le proprie preferenze per le ore e le schede orario</a> </p> <p>In un’organizzazione di grandi dimensioni, alcuni gruppi potrebbero dover configurare le preferenze delle ore e delle schede orario in modo indipendente per adattarsi ai propri flussi di lavoro univoci, anziché ereditare le preferenze configurate da un amministratore a livello di sistema. Ora gli amministratori di Workfront possono sbloccare una scheda orario e una preferenza per le ore per tutti i gruppi del sistema in modo da poterla configurare autonomamente.</p> <p>Questa funzionalità è stata aggiunta di recente anche per le preferenze del progetto e per le preferenze di attività e problemi.</p> </td> 
   <td> <p><b>Disponibile in queste date:</b> </p> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4 <span style="color: #ff0000;"> (inizialmente disponibile in produzione solo per i clienti nel cluster 4)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuovo per gli amministratori di Workfront: configura modelli di layout per gli utenti con provisioning automatico nella nuova esperienza Workfront</a> </p> <p>Ora puoi configurare i modelli di layout nella nuova esperienza Workfront per gli utenti con provisioning automatico. Nel menu a discesa Attributi utente di Workfront in cui mappate gli attributi utente (Configurazione &gt; Sistema &gt; Single Sign-On), è ora disponibile una nuova voce di menu "Nuovo modello di layout" per effettuare questa configurazione. In precedenza, era possibile configurare modelli di layout per gli utenti con provisioning automatico solo in Workfront Classic.</p> </td> 
   <td> <p><b>Disponibile in queste date:</b> </p> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nel nuovo campo vengono visualizzati i gruppi a cui appartengono gli utenti</a> </p> <p>Ora è facile scoprire a quali gruppi appartengono i tuoi utenti. In un report o in una visualizzazione in cui sono elencati gli utenti, è possibile creare una colonna utilizzando il nuovo campo Altri gruppi. Questo campo elenca i gruppi di cui è membro ogni utente.</p> </td> 
   <td> <p><b>Disponibile in queste date:</b> </p> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Nella pagina dei dettagli blueprint viene ora visualizzata un'immagine</a> </p> <p>Nella pagina dei dettagli di ogni blueprint ora viene visualizzata un’immagine del modello di progetto installato con la blueprint. L’immagine fornisce un’anteprima del contenuto della blueprint in modo da sapere cosa stai per installare. Facoltativamente, puoi visualizzare l’anteprima dell’immagine completa nel browser o scaricarla.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Preferenze blueprint per nuovi problemi</a> </p> <p>Sono ora disponibili nuove preferenze per alcuni blueprint. Vengono installati per impostazione predefinita, ma è possibile rinunciare all’installazione delle preferenze quando si configurano i dettagli di installazione.</p> <p>Le preferenze includono gruppi di argomenti della coda, argomenti della coda e regole di routing per raccogliere le informazioni corrette quando viene inviato un problema o una richiesta e inviare il problema o la richiesta alla mansione o al team corretti. L’utilizzo delle preferenze consente di creare coerenza nel modo in cui i nuovi problemi o richieste vengono acquisiti sui progetti.</p> <p>L’utilizzo di queste preferenze non fa sì che i progetti creati dal modello vengano inseriti nelle code di richiesta.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nuovo per gli amministratori di gruppi: visualizza e gestisci gli elementi eliminati e ripristinati di recente da un gruppo</a> </p> <p>Stiamo continuando a semplificare la gestione dei gruppi e degli oggetti associati in un’unica posizione. Ora puoi visualizzare e lavorare con gli elementi eliminati e ripristinati di recente da un gruppo dall’area Gruppi. In questo modo è possibile evitare di dover passare all'area Recently Deleted o Recently Restored in Configurazione per gestire tali elementi. Inoltre, l'elenco degli elementi del gruppo con cui si sta lavorando è separato dagli altri elementi eliminati e ripristinati nel sistema.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 26 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Novità per gli amministratori di gruppi: le preferenze del gruppo ora interessano i modelli di gruppo</a> </p> <p>È ora più semplice assicurarsi che i modelli di progetto del gruppo soddisfino le esigenze del gruppo. Quando si assegna un nuovo modello di progetto a un gruppo al momento della creazione, il modello eredita varie impostazioni dalle preferenze di progetto e attività del gruppo.</p> <p>Quando si crea una nuova attività modello all'interno di un modello di progetto associato a un gruppo, l'attività modello eredita varie impostazioni dalle preferenze attività del gruppo.</p> <p>In precedenza, i modelli di progetto e le attività dei modelli di progetto ereditavano queste impostazioni dalle preferenze di progetto e attività impostate a livello di sistema.</p> <p>Se si crea un modello o un'attività modello senza un gruppo, ad esempio dalla pagina principale Modelli, le impostazioni di cui sopra vengono ereditate dalle preferenze di progetto e attività a livello di sistema. Tuttavia, se in seguito si assegna un gruppo all'attività modello o modello, le preferenze del gruppo non hanno effetto su di esso.</p> </td> 
   <td> <p>Versione di anteprima: 26 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Novità per gli amministratori: scopri i moduli personalizzati che utilizzano un campo personalizzato</a> </p> <p>Ora è più semplice modificare un campo personalizzato in un modulo personalizzato. Con un solo clic nel modulo personalizzato, puoi scoprire tutti gli altri moduli personalizzati che utilizzano il campo. È importante valutare se tali moduli avranno bisogno di modifiche per continuare a funzionare correttamente dopo la modifica.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 19 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nuovo per gli amministratori di gruppi: Blocca e sblocca le preferenze di progetto, attività e problema per un gruppo</a> </p> <p>Ora puoi verificare che tutti gli utenti del gruppo e dei suoi sottogruppi utilizzino la stessa impostazione per le preferenze di un progetto, un’attività o un problema. Dopo che un amministratore di Workfront ha sbloccato una preferenza a livello di sistema, è possibile configurarla e quindi bloccarla per il proprio gruppo. Anche se è ancora possibile riconfigurare una preferenza di gruppo bloccato, gli amministratori dei sottogruppi inferiori non possono farlo separatamente per i loro gruppi.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 12 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nuovo per gli amministratori di gruppi: crea e modifica modelli dall'area Gruppi</a> </p> <p>Stiamo continuando a semplificare la gestione dei gruppi e degli oggetti associati in un'unica posizione. Ora è possibile visualizzare e lavorare con i modelli di un gruppo dall’area Gruppi in Configurazione. In questo modo non è più necessario passare all'area Modelli per gestire i modelli di un gruppo. Inoltre, l'elenco dei modelli di gruppo su cui si sta lavorando è separato dagli altri in tutto il sistema.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 12 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">Immettere e salvare le informazioni in un modulo personalizzato allegato alla volta</a> </p> <p>È ora più semplice fornire informazioni nella sezione Dettagli per un oggetto: digita e salva le informazioni in un singolo campo personalizzato o in un'area espandibile (ad esempio Panoramica e Dati finanziari), anche se i campi obbligatori in altri moduli personalizzati sull'oggetto non sono ancora stati compilati.</p> <p>In precedenza, quando si immettevano informazioni in un modulo personalizzato o in un'area espandibile per un oggetto, tutti i moduli personalizzati allegati all'oggetto entravano in modalità di modifica e tutti i campi obbligatori dovevano essere completati prima di poter salvare le modifiche. Si è verificato un problema se non è stato possibile completare un campo obbligatorio perché destinato a un altro utente.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 22 luglio 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">Nuovo per gli amministratori di gruppi: creare e gestire gli stati per un gruppo a qualsiasi livello</a> </p> <p>Per semplificare la gestione e il controllo indipendente dei flussi di lavoro da parte di tutti i livelli dell’organizzazione, è stata introdotta la possibilità di creare e gestire gli stati dei sottogruppi. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 3 giugno 2021 (durante il ciclo di rilascio 21.3)<br></p> <p>Versione di produzione: 22 luglio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Novità per gli amministratori di Workfront: esegui autonomamente la migrazione dei modelli di layout da Workfront Classic alla nuova esperienza Workfront</a> </p> <p>Per aiutarti a gestire i modelli di layout quando gli utenti passano all’utilizzo della nuova esperienza Workfront, abbiamo creato un pulsante che puoi utilizzare per migrare i modelli di layout da Workfront Classic alla nuova esperienza senza affidarti all’Assistenza clienti di Workfront.</p> <p>In precedenza, solo l’Assistenza clienti Workfront poteva migrare i modelli di layout da Workfront Classic alla nuova esperienza Workfront.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 1 luglio 2021<br></p> <p>Versione di produzione: 15 luglio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">Quando si associa un modello a un gruppo, selezionare un processo di approvazione del gruppo in Dettagli coda e Argomenti coda</a> </p> <p>È stata aggiunta una nuova opzione al processo di associazione di un modello a un gruppo. Ora è possibile selezionare i processi di approvazione specifici del gruppo per i problemi nei Dettagli coda del modello o in uno dei relativi Argomenti coda.</p> <p>Nella versione 21.3, quando è stata aggiunta la possibilità di associare un modello di gruppo a un gruppo, è possibile selezionare un processo di approvazione specifico per il gruppo nel modello, ma non è possibile farlo nei Dettagli coda o Argomenti coda del modello.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 1 luglio 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti al progetto {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">Includi immagini negli aggiornamenti</a> </p> <p>Nella scheda Aggiornamenti di un oggetto è ora possibile aggiungere immagini facendo clic sull'icona Immagine sulla barra degli strumenti. È inoltre possibile trascinare un'immagine nell'area di aggiornamento. Per poter visualizzare l’icona Immagine, l’amministratore di Workfront deve abilitare l’aggiunta delle immagini.</p> <p>È possibile aggiungere immagini sia negli aggiornamenti che nelle risposte. Una miniatura immagine nell’aggiornamento indica che i destinatari possono visualizzare in anteprima l’immagine nel browser o scaricarla, e le notifiche e-mail e in-app mostrano che le immagini sono associate all’aggiornamento.</p> <p>In precedenza, l’unico modo per condividere un’immagine in Workfront era allegarla a un oggetto come documento. Le immagini aggiunte nella scheda Aggiornamenti sono disponibili solo in tale scheda e non nella scheda Documenti.</p> <p>Prima che gli utenti di Workfront possano includere immagini negli aggiornamenti, questa funzione deve essere abilitata dall’amministratore Adobe Workfront.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Algoritmo aggiornato per le assegnazioni intelligenti</a> </p> <p>È stato migliorato l’algoritmo utilizzato per le assegnazioni intelligenti. Con questo nuovo miglioramento, Workfront esamina le 30 assegnazioni più recenti effettuate dall’utente connesso per fornire suggerimenti quando assegna attività e problemi. L’elenco dei suggerimenti può contenere fino a 50 utenti. </p> <p>Prima di questo miglioramento, Workfront stava considerando le assegnazioni sulle attività padre e altri attributi utente correlati a tali assegnazioni quando suggeriva gli utenti.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuova esperienza durante la creazione di un progetto da un modello</a> </p> <p>Per rendere il tuo utilizzo di Workfront coerente con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per la creazione di un progetto da un modello. La funzionalità per la creazione di un progetto utilizzando un modello non è stata modificata. Tuttavia, alcuni dei miglioramenti apportati a questa nuova interfaccia includono:</p> 
    <ul> 
     <li> <p>Anteprima delle informazioni sul modello prima di allegarlo</p> </li> 
     <li> <p>Aggiungere modelli a un elenco di preferiti durante il processo di creazione del progetto</p> </li> 
    </ul> <p>È stata aggiornata l’interfaccia per la creazione del progetto sia quando lo si crea dall’area Progetti che dall’area Modelli.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuova esperienza durante l'associazione di modelli ai progetti</a> </p> <p>Per rendere il tuo utilizzo di Workfront coerente con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per allegare un modello a un progetto. La funzionalità per allegare un modello non è stata modificata. Tuttavia, l'interfaccia riprogettata presenta alcuni miglioramenti, tra cui i seguenti:</p> 
    <ul> 
     <li> <p>Anteprima delle informazioni sul modello prima di allegarlo</p> </li> 
     <li> <p>Aggiungere modelli a un elenco di preferiti durante il processo di creazione degli allegati</p> </li> 
     <li> <p>Visualizza tutte le opzioni per la gestione delle impostazioni di modello e progetto in un'unica pagina continua</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 26 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}">Valori unitari di durata e unità di durata per le attività</a> </p> <p>Per un’esperienza utente più pulita e semplificata, il valore del campo Durata è stato unito all’unità di durata. Prima di questo miglioramento, l’unità di tempo visualizzata in un campo a discesa separato dopo il campo Durata.</p> <p>Oltre ai campi Durata nelle caselle Dettagli attività, Modifica attività e Nuova attività, stiamo aggiornando i campi seguenti per far corrispondere questa esperienza:</p> 
    <ul> 
     <li> <p>Campo durata durante l'esecuzione di assegnazioni avanzate</p> </li> 
     <li> <p>Campo Ritardo livellamento durante la creazione o la modifica di un'attività</p> </li> 
     <li> <p>Campo di frequenza durante la creazione di un'attività ricorrente (disponibile a breve)</p> </li> 
     <li> <p>Campo Lag durante l’aggiunta di un predecessore (disponibile a breve)</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 19 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">Disabilita l'aggiunta di problemi in linea nei progetti</a> </p> <p>Per garantire che gli utenti forniscano informazioni accurate quando aggiungono problemi ai progetti completando un modulo per i problemi, è stata introdotta una nuova impostazione che consente di gestire l’aggiunta in linea di problemi a un progetto o alle relative attività. Questa impostazione è attivata per impostazione predefinita nella nuova area Impostazioni problemi della casella Modifica progetto. La disattivazione di questa opzione disattiva l’opzione Aggiungi altri problemi nella sezione Problemi di un progetto, impedendo agli utenti di aggiungere altri problemi all’elenco. Gli utenti possono comunque aggiungere problemi ai progetti utilizzando l’opzione Nuovo problema nella sezione Problemi o utilizzando una coda di richieste, se ne è stata configurata una per il progetto.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 5 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">Miglioramento della visualizzazione dei campi personalizzati per caselle di controllo e pulsanti di scelta</a> </p> <p>La visualizzazione e la selezione delle opzioni relative alle caselle di controllo e ai pulsanti di scelta nei moduli personalizzati sono diventate più semplici. Un campo personalizzato con molte opzioni relative alle caselle di controllo o ai pulsanti di scelta viene ora visualizzato in più colonne della pagina. Precedentemente, venivano visualizzate in una singola colonna, che richiedeva uno scorrimento aggiuntivo per gli utenti che compilavano il modulo.</p> <p>Ciò dipende dal modo in cui vengono posizionati i campi nel modulo personalizzato. Se si inserisce un altro campo nella stessa riga con il campo casella di controllo o pulsante di opzione, le opzioni potrebbero disporre di spazio orizzontale sufficiente per la visualizzazione in una singola colonna.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 29 luglio 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti alla gestione delle risorse {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">Assegnazioni rapide nel Bilanciatore dei carichi di lavoro</a> </p> <p>È ora possibile bilanciare in modo efficiente le risorse nel Bilanciatore dei carichi di lavoro con il minimo clic trascinando un elemento dall’area Non assegnato e rilasciandolo sulla riga di un utente nell’area Assegnato. Tramite il trascinamento della selezione è inoltre possibile annullare l'assegnazione degli elementi agli utenti e riportarli nell'area Non assegnato, nonché spostarli in altri utenti. </p> <p>Prima di questo miglioramento, era possibile assegnare gli elementi solo facendo clic sul menu Altro di un’attività o di un problema e utilizzando l’opzione Assegna. Ora le ore pianificate assegnate all’utente vengono aggiornate in tempo reale durante il trascinamento delle attività.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuova opzione predefinita per il Bilanciatore dei carichi di lavoro</a> </p> <p>Come parte del nostro sforzo per rendere obsoleta la programmazione e lo strumento di assegnazione delle risorse principale del Bilanciatore dei carichi di lavoro Workfront Workfront, abbiamo reso il Bilanciatore dei carichi di lavoro l’opzione predefinita per tutti i nuovi utenti. Attualmente, l'opzione predefinita è Pianificazione. Questa modifica si applica a tutte le aree da cui è possibile accedere alla pianificazione, inclusa l’area Risorse (nella nuova esperienza Adobe Workfront) o l’area Persone (in Adobe Workfront Classic), nonché a livello di progetto e team.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuova esperienza filtro nel Bilanciatore dei carichi di lavoro</a> </p> <p>Abbiamo riprogettato l’esperienza filtro nel Bilanciatore dei carichi di lavoro per includere le seguenti funzionalità aggiuntive:</p> 
    <ul> 
     <li> <p>Interfaccia utente più semplice e intuitiva, in linea con la nuova esperienza Workfront</p> </li> 
     <li> <p>Campi aggiuntivi in base ai quali è possibile filtrare</p> </li> 
     <li> <p>Possibilità di duplicare un filtro</p> </li> 
     <li> <p>Condivisione di filtri con altri utenti</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 16 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti Agile {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Assegnazioni utente su bacheche Kanban e Scrum</a> </p> <p>Abbiamo aggiornato le schede delle storie sulle bacheche Kanban e Scrum per facilitare l’assegnazione di un utente alla storia. Ora puoi fare clic su un avatar del team o dell’utente per aggiungere un’assegnazione quando la scheda delle storie viene espansa. In precedenza, era necessario individuare e fare clic su un'icona separata con il segno più.</p> </td> 
   <td> <p>Versione di anteprima: 9 settembre 2021 <br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurare le modalità di applicazione delle date quando si aggiungono elementi di lavoro a un'iterazione Scrum</a> </p> <p>Per impostazione predefinita, quando si aggiunge un elemento di lavoro a un'iterazione, le date di inizio pianificato e di completamento pianificato dell'elemento di lavoro vengono modificate in modo da corrispondere alle date di inizio e di completamento dell'iterazione. Ora è possibile scegliere di mantenere la data di inizio pianificata e la data di completamento pianificata originali su tutti gli elementi di lavoro di un team.</p> <p>Questa opzione si applica solo ai team Scrum e non ai team Kanban.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">Modifiche alla visualizzazione Agile nei progetti</a> </p> <p>Come parte della versione 21.3, sono stati apportati miglioramenti all'intestazione della scheda agile e agli storyboard (vedi <a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">Aggiornamenti all'intestazione della scheda agile e allo storyboard</a>). Questi aggiornamenti si applicavano alle iterazioni e alla visualizzazione agile dei progetti.</p> <p>Con la versione 21.4, questi miglioramenti vengono ripristinati per la visualizzazione agile dei progetti. Non vengono apportate modifiche alle iterazioni Agile.</p> <p>Di seguito sono riportate le modifiche che vengono ripristinate per quanto riguarda la visualizzazione agile dei progetti:</p> 
    <ul> 
     <li> <p>Le schede delle storie e le colonne della bacheca hanno larghezze regolabili.</p> </li> 
     <li> <p>Le colonne non presentano ombreggiature di sfondo.</p> </li> 
     <li> <p>Le schede non dispongono di etichette di identificazione (brano principale, sottoattività, brano, attività o problema).</p> </li> 
     <li> <p>La colonna Storia principale è stata rinominata in Storie.</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 16 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Aggiungi nuove storie e nuovi problemi dal Kanban Board</a> </p> <p>Ora puoi creare una nuova storia o un nuovo problema direttamente dalla bacheca Kanban. In questo modo è più semplice aggiungere rapidamente una nuova storia senza dover passare a un progetto, report o dashboard per creare un'attività.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 22 luglio 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti al reporting {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuovo aspetto per il campo Assegnazioni negli elenchi e nei report aggiornati</a> </p> <p>Per mantenere l’aspetto moderno delle altre aree della nuova esperienza Workfront, è stato modificato lo stile del campo Assegnazioni negli elenchi e nei rapporti aggiornati. La riprogettazione include una nuova icona Ruolo, una nuova icona Persone per le assegnazioni avanzate, una nuova icona Accesso limitato e altro ancora.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima Beta: 8 aprile 2021 (con versione 21.2)<br></p> <p>Versione di produzione: 15 luglio 2021<span class="uitext" style="color: #dc143c;">(originariamente rilasciato in produzione il con la versione 21.2)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuovo aspetto per i campi typeahead negli elenchi e nei report aggiornati</a> </p> <p>Per conferire un aspetto moderno alle altre aree della nuova esperienza Workfront, è stato modificato lo stile dei campi typeahead negli elenchi e nei report aggiornati. Queste modifiche includono vari miglioramenti.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima Beta: 8 aprile 2021 (con versione 21.2)<br></p> <p>Versione di produzione: 15 luglio 2021 <span class="uitext" style="color: #dc143c;">(originariamente rilasciato in produzione il con la versione 21.2)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Richieste di miglioramenti {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">La ricerca migliorata per le richieste ora include caratteri speciali</a> </p> <p>Per velocizzare e semplificare la ricerca delle code di richieste durante l’invio di richieste, è stato migliorato l’algoritmo di ricerca per trovare le code che potrebbero contenere caratteri speciali.</p> <p>Ad esempio, per trovare una coda di richieste denominata "*Workfront" digita "*Workfront" o "Workfront" nel campo Tipo di richiesta.</p> <p>Sono supportati tutti i caratteri speciali.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 9 settembre 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuovo aspetto per le code di richieste incorporate nella nuova esperienza Workfront</a> </p> <p>Per mantenere lo stesso aspetto nell’invio delle richieste in tutta la nuova esperienza Workfront, è stata riprogettata l’interfaccia per aggiungere richieste a una coda di richieste incorporata. Prima di questo miglioramento, l’interfaccia per l’aggiunta di richieste da un dashboard corrispondeva all’ambiente Workfront Classic.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 26 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti delle bozze {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Funzionalità di verifica migliorate per revisori e richiedenti</a> </p> <p>Per fornire un’esperienza più integrata tra Workfront e Proof, sono stati apportati diversi miglioramenti alle funzionalità di verifica per revisori e richiedenti:</p> 
    <ul> 
     <li> <p>Puoi assegnare i ruoli Moderatore o Autore a qualsiasi utente in Workfront, indipendentemente dal fatto che disponga di una licenza di verifica, assegnando loro diritti aggiuntivi, come l’applicazione di azioni o la risoluzione di commenti.</p> </li> 
     <li> <p>Puoi aggiungere revisori e richiedenti alle bozze che richiedono un accesso o che devono essere firmate elettronicamente.</p> </li> 
     <li> <p>Tutti gli utenti usufruiscono inoltre della connettività migliorata tra Workfront e Proof. Ora, quando si disattiva un utente o si aggiorna l’indirizzo e-mail di un utente, i propri aggiornamenti vengono rispecchiati correttamente nella verifica se modificati in Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 5 agosto 2021 <br></p> <p>Versione di produzione: con la versione 21.4 <span class="uitext" style="color: #dc143c;">(rimossa dall’anteprima e dalla produzione il 20 ottobre 2021. Originariamente rilasciato solo ai clienti EMEA completamente integrati. Questa funzionalità verrà reintrodotta per tutti i clienti in un secondo momento.)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti dell’integrazione {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">Collega documenti da Dropbox Business</a> </p> <p>Abbiamo aggiunto Dropbox Business come integrazione di documenti disponibile. Ora è possibile accedere ai documenti archiviati in Dropbox Business direttamente da Workfront.</p> <p>Dropbox Business consente di collegare documenti condivisi e caricarli in cartelle condivise. Dropbox (non Dropbox Business) consente solo al proprietario dei documenti di visualizzare il documento in Workfront.</p> <p>L’amministratore di Workfront può abilitare questa integrazione per la tua organizzazione.</p> </td> 
   <td> <p><b>Disponibile in queste date:</b> </p> <p>Anteprima versione: N/D<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Aggiornamenti a Workfront per Slack</a> </p> <p>Nell’integrazione Workfront for Slack sono ora visibili i seguenti aggiornamenti:</p> <p>L'integrazione di Workfront per Slack ora ha un nuovo aspetto. Inoltre, ora ricevi le notifiche Workfront for Slack in tempo reale. </p> <p>Ad esempio, se si è assegnati a un'attività, la notifica viene ricevuta non appena si è assegnati. </p> <p>In precedenza, poteva verificarsi un ritardo prima che la notifica apparisse in Slack.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 29 luglio 2021<br></p> <p>Versione di produzione: 29 luglio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">Visualizza più chiaramente i dettagli di accesso all'account quando fornisci il consenso alle integrazioni Adobe Workfront</a> </p> <p>Le schermate di consenso per le integrazioni Adobe Workfront ora sono aggiornate. Ora puoi vedere le azioni e le aree specifiche a cui le integrazioni hanno accesso, in modo da comprendere meglio cosa stai consentendo all’integrazione o all’applicazione di accedere.</p> <p>Questa nuova schermata di consenso si applica a qualsiasi integrazione Adobe Workfront che utilizza OAuth 2.0. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 29 luglio 2021<br></p> <p>Versione di produzione: 29 luglio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}">Autenticazione chiave API non più necessaria per le integrazioni</a> </p> <p>Le integrazioni Workfront hanno recentemente iniziato a utilizzare OAuth2 per maggiore sicurezza e usabilità. Come parte di questo spostamento, Workfront non richiede più le chiavi API per l’autenticazione delle integrazioni.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 5 agosto 2021<br></p> <p>Versione di produzione: 5 agosto 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti per dispositivi mobili {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">Rivedi e approva le bozze nell'app mobile</a> </p> <p>L’app mobile di Adobe Workfront ora mostra tutte le approvazioni della bozza assegnate all’utente nell’elenco delle approvazioni in Il mio lavoro. Puoi rivedere un documento di bozza direttamente nell’app e prendere una decisione al riguardo.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima versione: N/D<br></p> <p>Versione di produzione: settimana dell’11 ottobre 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> 
    <ul> 
     <li> <p>app store di iOS</p> </li> 
     <li> <p>app store di Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Crea una nuova richiesta dalla home area dell'app mobile</a> </p> <p>Ora puoi creare una nuova richiesta dalla home area nell’app mobile di Adobe Workfront. Toccando il pulsante "aggiungi" nella barra di navigazione mobile viene visualizzata un’opzione per Richiedi oltre ad Attività. In precedenza, per creare una richiesta era necessario passare alla pagina Richieste.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima versione: N/D<br></p> <p>Versione di produzione: 4 agosto 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> 
    <ul> 
     <li> <p>app store di iOS</p> </li> 
     <li> <p>app store di Android</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Altri miglioramenti {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuove scelte rapide da tastiera per il rientro e l'annullamento del rientro negli elenchi</a> </p> <p>Per fornire un’esperienza accessibile a tutti gli utenti del sistema e rispettare i principi standard di navigazione da tastiera, i comandi da tastiera rientro/rientro sono stati modificati. </p> <p>Per Mac, premere Opzione + &gt; per applicare un rientro a una voce dell'elenco e Opzione + &lt; per applicare un rientro negativo. </p> <p>Per Windows, premere Alt + &gt; per applicare un rientro a una voce di elenco e Alt + &lt; per applicare un rientro negativo.</p> <p>In precedenza, la scelta rapida da tastiera per il rientro in un elenco era Tab e l’annullamento del rientro era Maiusc + Tab. Tuttavia, quando si utilizzava il tasto TAB per applicare i rientri e i rientri, non era possibile scorrere tutti i campi attivi nell’interfaccia.</p> <p>Questa modifica si applica solo agli elenchi aggiornati e non a quelli legacy. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima: 12 agosto 2021<br></p> <p>Versione di produzione: con la versione 21.4</p> <p><strong>Disponibile in questi ambienti:</strong> </p> 
    <ul> 
     <li> <p>La nuova esperienza Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione della versione 21.4. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

## Miglioramenti di Workfront Scenario Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

Con la versione 21.4 di Workfront Scenario Planner sono in arrivo nuove funzioni. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, consulta [Attività di rilascio di Adobe Workfront Scenario Planner](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
-->

## Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non ci sono aggiornamenti per gli Obiettivi di Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API versione 14

Per API versione 14, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione 14](../../../wf-api/api/new-api-version-14.md) dell&#39;API.

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](../../../wf-api/api/api-version-support-schedule.md).

## Webinar sulla versione 21.4

Il webinar sulla versione di Workfront 21.4 è stato presentato il 23 settembre 2021. È possibile visualizzare la registrazione del webinar dalla pagina [Eventi in Workfront One](https://one.workfront.com/s/event).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la [pagina Aggiornamenti delle versioni di formazione](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home).

## Funzionalità non più supportata

### Internet Explorer 11

Con la rimozione del supporto per Internet Explorer, Workfront ora supporta ufficialmente Microsoft Edge.

Per ulteriori informazioni sui browser supportati, vedere [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
