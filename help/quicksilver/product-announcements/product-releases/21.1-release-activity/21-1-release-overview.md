---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: Panoramica sulla versione 21.1
description: La versione 21.1 è stata resa disponibile nell’ambiente di produzione la settimana del .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3658'
ht-degree: 0%

---

# Panoramica sulla versione 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Questa pagina fornisce informazioni sulle funzionalità sia per Adobe Workfront Classic che per la nuova esperienza Adobe Workfront inclusa nella versione 21.1.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Con questa versione, vengono rilasciate nuove funzionalità e miglioramenti per guidare il ritorno del 2021 con strategie adattabili, processi di lavoro automatizzati e un’infrastruttura digitale connessa per consentire il successo in tutta l’azienda.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Questi miglioramenti sono attualmente disponibili

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

nell’ambiente di produzione.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

Sono stati rilasciati la settimana del 15 febbraio 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
* [Miglioramenti alla gestione dei progetti](#project-management-enhancements)
* [Miglioramenti delle analisi](#enhanced-analytics-improvements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Introduzione di una nuova impostazione del livello di accesso per la copia dei progetti</a> </p> <p>Per consentirti di controllare meglio, in qualità di amministratore di sistema, le operazioni che i responsabili della pianificazione possono eseguire con un progetto, abbiamo reso più granulare l’accesso di modifica ai progetti nel livello di accesso, introducendo una nuova impostazione che consente di abilitare o disabilitare la possibilità di copiare i progetti. Prima di questa modifica, quando abilitavi l’accesso degli utenti a Modifica progetti, questi potevano automaticamente copiarli. Con la nuova funzione, puoi consentire a un utente di modificare i progetti senza necessariamente averne accesso alla copia disabilitando la nuova impostazione Copia.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">In un modulo personalizzato su un oggetto, seleziona tutti gli elementi in un campo a discesa a selezione multipla</a> </p> <p>Nella pagina Dettagli di un oggetto, quando si compila un campo a discesa a selezione multipla in un modulo personalizzato, è possibile fare clic su Seleziona tutto se è necessario selezionare tutte le opzioni disponibili.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Attualmente non disponibile quando si invia una nuova richiesta).</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Ricalcolare tutti i campi modulo personalizzato per un oggetto</a> </p> <p>Ora è più facile assicurarsi che tutti i dati nei campi personalizzati calcolati siano correnti per un oggetto. Una nuova opzione di menu Ricalcola espressioni consente di ricalcolare rapidamente tutti i dati contenuti in questi campi.</p> <p>Questa funzione è particolarmente utile quando qualcuno modifica dati in un altro oggetto a cui fa riferimento un campo personalizzato calcolato nell’oggetto.</p> <p>In precedenza, gli utenti dovevano utilizzare soluzioni alternative per assicurarsi che tutti i dati nei campi personalizzati calcolati fossero correnti. Ad esempio, hanno modificato l’oggetto insieme ad altri oggetti per utilizzare l’opzione di ricalcolo disponibile per la modifica in serie.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 10 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Sblocca le preferenze per attività e problemi per gli amministratori di gruppi</a> </p> <p>Gli amministratori di Workfront ora possono dare agli amministratori di gruppi più autonomia sbloccando le preferenze di singole attività e problemi. Quando una preferenza viene sbloccata, gli amministratori di gruppi possono configurarla per i propri gruppi in modo da soddisfare le esigenze specifiche e i processi interni di ciascun gruppo.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Prima del 24 giugno 2021, questo era disponibile come parte di un rollout graduale solo per i clienti nei cluster 4 e 6 e per alcuni altri clienti. Ora è disponibile in Produzione per tutti i clienti.)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurare separatamente le impostazioni del livello di accesso per portfolio e programmi</a> </p> <p>Ora è più semplice gestire l’accesso degli utenti a portfolio e programmi, in quanto è possibile configurare separatamente le impostazioni del livello di accesso.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Selezionare tutte le caselle di controllo di una serie durante la modifica delle informazioni in un modulo personalizzato</a> </p> <p>Nella pagina Dettagli di un oggetto, quando si compila un campo Modulo personalizzato contenente caselle di controllo, è possibile fare clic su Seleziona tutto se è necessario selezionare tutte le caselle di controllo disponibili.</p> <p>Questa opzione viene visualizzata solo se il campo contiene più di 2 caselle di controllo.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Attualmente non disponibile quando si invia una richiesta).</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Configurare l’Workfront di e-mail di inserire nell'elenco Consentiti</a> </p> <p>Per una migliore protezione dei dati, ora puoi utilizzare un elenco Consentiti di dominio e-mail per eseguire le seguenti operazioni:</p> 
    <ul> 
     <li> <p>Controlla dove possono andare le e-mail di Workfront se contengono rapporti o documenti memorizzati in Workfront</p> </li> 
     <li> <p>I domini e-mail di controllo possono trovarsi nell’indirizzo e-mail che gli utenti possono specificare nel loro profilo utente</p> </li> 
    </ul> <p>Ad esempio, se desideri proteggere i dati sensibili, come un rapporto che elenca i clienti a rischio, puoi includere nel inserisco nell'elenco Consentiti di selezione dell’e-mail solo il dominio o i domini e-mail interni In questo modo, gli utenti non possono inviare tale rapporto (o qualsiasi altro rapporto di Workfront) a un indirizzo e-mail esterno.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: con la versione 21.1 </p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Assegnare un amministratore di gruppo a un sottogruppo</a> </p> <p>Per facilitare il funzionamento indipendente dei livelli dell’organizzazione, è stata aggiunta la possibilità di assegnare un amministratore di gruppo a un sottogruppo. A questo punto è possibile assicurarsi di delegare la gestione dei sottogruppi alle persone giuste.</p> <p>In precedenza, solo un gruppo di primo livello poteva avere Amministratori di gruppo e questi amministratori gestivano tutti i sottogruppi al di sotto del gruppo di primo livello.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Utilizzare progetti di gruppo e processi di approvazione nell'area Gruppi</a> </p> <p>Gli amministratori di gruppi possono visualizzare e utilizzare facilmente i progetti e i processi di approvazione del gruppo ora che sono elencati nell'area Gruppi. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Configurare le notifiche degli eventi per i gruppi</a> <span style="color: #dc143c; font-weight: bold;">Novità in anteprima.</span></p> <p>Gli amministratori di Workfront ora possono dare maggiore autonomia agli amministratori di gruppi consentendo loro di configurare le notifiche degli eventi per i loro gruppi di livello superiore. I sottogruppi ereditano le configurazioni di notifica degli eventi dal gruppo padre principale.</p> <p>In precedenza, le notifiche degli eventi potevano essere configurate solo da un amministratore Workfront a livello di sistema, il che significa che tutti i gruppi dovevano utilizzare lo stesso set di notifiche degli eventi.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 22 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Disponibile inizialmente in produzione solo per i clienti del cluster 4 come parte di un rollout graduale; disponibile poco dopo per altri cluster)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Visualizza il numero di licenze utilizzate e assegnate in un gruppo</a> </p> <p>Per determinare il livello di distribuzione delle licenze, è ora possibile visualizzare il numero di licenze utilizzate in un gruppo ed eventuali sottogruppi al di sotto di esso.</p> <p>Se si gestisce un gruppo di primo livello, è possibile visualizzare sia il numero di licenze utilizzate in un gruppo (e nei relativi sottogruppi) sia il numero massimo di licenze allocate per il gruppo.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Bilanciatore dei carichi di lavoro per i progetti</a> </p> <p>Il Bilanciatore dei carichi di lavoro è ora disponibile all’interno di un progetto. Ora puoi scegliere se utilizzare il Bilanciatore dei carichi di lavoro o lo strumento Pianificazione per gestire le risorse del progetto.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 17 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront Balancer disponibile per un team</a> </p> <p>Il Bilanciatore dei carichi di lavoro è ora disponibile all’interno di un team. Ora puoi scegliere se utilizzare il Bilanciatore dei carichi di lavoro o lo strumento Pianificazione per gestire le risorse del team. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti alla gestione dei progetti {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Esportazione ora disponibile nella sezione Metriche di un progetto</a> </p> <p>Per condividere più facilmente lo stato e l’avanzamento di un progetto, ora puoi esportare l’intero dashboard nella sezione Metriche di un progetto in un file .png.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 15 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Aggiorna la percentuale di completamento del problema quando il progetto o l’attività viene convertito dall’aggiornamento del problema</a> </p> <p>È stato aggiornato il funzionamento della percentuale di completamento dei problemi per i problemi convertiti in progetti o attività. Con la nuova funzionalità, quando un problema viene convertito in un’attività o in un progetto, la percentuale di completamento del problema viene aggiornata in sincronia con la percentuale di completamento dell’attività o del progetto di risoluzione quando l’impostazione "Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell’oggetto risolutivo cambia" è abilitata dalla configurazione.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Campi rimossi dalla pagina Nuova richiesta</a> </p> <p>Durante la riprogettazione della pagina Nuova richiesta, sono stati aggiornati i campi Nuovi problemi configurati nella sezione Configurazione coda di un progetto.</p> <p>I campi Nuovi problemi vengono visualizzati solo quando si crea un problema dalla sezione Problemi del progetto. Non vengono visualizzati quando si invia un problema utilizzando una coda di richieste nell’area Richieste.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Rimosso dalla versione)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuova esperienza nell’invio di richieste nell’area Richieste</a> </p> <p>Per garantire la coerenza con la nuova esperienza Workfront e aumentare l’efficienza nell’invio delle richieste, abbiamo riprogettato la casella Nuova richiesta nell’area Richieste.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Rimosso dal rilascio; rimarrà in Anteprima e rilascerà in Produzione con 21.2)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Condividere un collegamento a una coda di richieste durante l’invio di una richiesta</a> </p> <p>È ora possibile condividere un collegamento a una coda di richieste, a un gruppo di argomenti o a un argomento della coda Durante la creazione di una richiesta.</p> <p>Prima di inviare una nuova richiesta, è possibile copiare un collegamento alla coda delle richieste, al gruppo di argomenti o all'argomento della coda della richiesta e condividerlo con altri utenti o incorporarlo in un dashboard.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 13 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1 <span style="color: #dc143c; font-weight: bold;">(Rimosso dal rilascio; rimarrà in Anteprima e rilascerà in Produzione con 21.2)</span></p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Elenco Nuove richieste inviate</a> </p> <p>Per consentirti di gestire le richieste inviate in modo più semplice e coerente, sono state rimosse le sezioni Richieste inviate e Tutte le richieste nell’area Richieste e sostituite con un nuovo elenco Inviato. L’elenco ha un aspetto familiare che corrisponde a tutti gli altri elenchi nel sistema, consentendoti di filtrare per diverse categorie di richieste inviate e di cercare rapidamente una richiesta che potrebbe essere difficile da trovare.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Cercare un gruppo da assegnare a un progetto e visualizzarne i dettagli</a> </p> <p>È ora più semplice assicurarsi di identificare il gruppo corretto quando si assegna un gruppo a un progetto. Passa il puntatore del mouse sul nome di un gruppo trovato nella casella Gruppo, quindi fai clic sull'icona delle informazioni visualizzata accanto al nome per visualizzare la descrizione dei dettagli del gruppo.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 17 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuovo rapporto Delega utenti</a> </p> <p>In precedenza, le informazioni per le deleghe di approvazione di attività, problemi e progetti potevano essere visualizzate solo dal delegato nella sua area Home. Per consentire ad altri utenti di visualizzare queste informazioni, gli utenti del piano possono ora creare il rapporto Delega utente, che indica:</p> 
    <ul> 
     <li> <p>Chi ha delegato queste approvazioni a un altro utente</p> </li> 
     <li> <p>Quale utente ha delegato queste approvazioni</p> </li> 
     <li> <p>La data di inizio e di fine di tali deleghe</p> </li> 
    </ul> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 17 dicembre 2020</p> <p>Versione di produzione: 21 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Miglioramenti delle analisi {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funzionalità</strong> </p> </td> 
   <td> <p><strong>Date e ambienti di rilascio</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">La pagina Persone è ora disponibile per tutti i cluster</a> </p> <p>La pagina Persone è ora disponibile in Workfront Classic per il cluster 4. Questa pagina include i grafici Attività per team, Capacità risorse e Capacità team.</p> <p>Questa pagina era precedentemente disponibile con la versione 20.3 sia in Workfront Classic che nella nuova esperienza Workfront per tutti gli altri cluster.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 28 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront (precedentemente disponibile)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Le funzioni di analisi avanzate vengono ora visualizzate per impostazione predefinita</a> </p> <p>Nota: questa modifica si applica solo agli utenti che sono stati aggiunti di recente ai modelli di layout. Anche gli utenti assegnati a un modello di layout personalizzato non sono interessati da questa modifica.</p> <p>Nel modello di layout predefinito, l’area Analytics è ora attivata per impostazione predefinita, il che significa che gli utenti assegnati a questo modello di layout ora visualizzano l’area Analytics nella barra di navigazione globale in Workfront Classic e il menu principale nella nuova esperienza Workfront.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 6 novembre 2020</p> <p>Versione di produzione: 3 dicembre 2020</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Analisi avanzate disponibili per tutti i cluster</a> </p> <p>L'analisi avanzata è disponibile per tutti i cluster Workfront, inclusi i clienti del cluster 6.</p> <p>In precedenza, l’analisi avanzata non era disponibile con Google Cloud Platform, impedendo ai clienti nel cluster 6 di accedere all’area Analytics. Ora i clienti aziendali e aziendali del cluster 6 possono accedere all’area di Analytics.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 20 novembre 2020</p> <p>Versione di produzione: 3 dicembre 2020</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Miglioramenti delle notifiche Adobe Workfront nei Microsoft Teams</a> </p> <p>Per semplificare l’utilizzo di Workfront nei Microsoft Teams, sono stati aggiunti diversi miglioramenti alle notifiche dei Microsoft Teams inviate da Workfront.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione anteprima beta: N/D</p> <p>Versione di produzione: 12 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuove breadcrumb di navigazione nell’app Adobe Workfront</a> </p> <p>Abbiamo aggiunto la navigazione breadcrumb all’app mobile Workfront. Ora è possibile utilizzare questa funzione per passare agli elementi di lavoro padre all’interno di un progetto.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione anteprima beta: N/D</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Testo formattatosupportato nei moduli personalizzati nell’app Workfront</a> </p> <p>Ora è possibile utilizzare la formattazione RTF nei campi di testo del modulo personalizzato nell’app mobile di Workfront.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione anteprima beta: N/D</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">Gli utenti SSO possono ora accedere nuovamente all’app Workfront con tecnologia Face ID o Fingerprint</a> </p> <p>Se la tua organizzazione utilizza l'SSO, ora puoi utilizzare il tuo Face ID o l'impronta digitale per accedere all'app mobile di Workfront dopo il timeout della sessione. Devi accedere con le tue credenziali SSO inizialmente però.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione anteprima beta: N/D</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
--&gt;

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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Aggiornamenti ai requisiti di errore della sottoscrizione eventi</a> </p> <p>Stiamo aggiornando i requisiti di soft-disable per gli errori di abbonamento agli eventi. Oltre ai requisiti esistenti, le sottoscrizioni di eventi verranno ora disabilitate se non riescono a raggiungere una consegna corretta entro 2.000 tentativi. In tal modo si intende rafforzare l'attuale regola del fallimento del 70% che, in determinate condizioni, può portare a un numero eccessivo di fallimenti.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione anteprima beta: N/D</p> <p>Versione di produzione: 11 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuovi campi del team disponibili per il riepilogo giornaliero</a> </p> <p>Abbiamo aggiunto i campi Approvazione team e Assegnazioni all’e-mail Riepilogo giornaliero azioni necessarie.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 17 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">Sostituzione dell’opzione POP email nelle code di richiesta</a> </p> <p>Stiamo sostituendo l’opzione e-mail POP per le code di richieste con un nuovo sistema gestito da Workfront. Sarà comunque possibile inviare le richieste tramite e-mail, ma sarà necessario impostare un nuovo indirizzo e-mail gestito da Workfront nell’area Coda richieste. </p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Anteprima beta: 17 dicembre 2020</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Limita la modifica delle ore nelle schede orario</a> </p> <p>Per fornire un maggiore controllo sulle schede orario e sulla modifica delle ore, è stata aggiunta un'impostazione che consente di limitare la modifica delle ore ai proprietari delle schede orario e agli amministratori di sistema.</p> <p>In precedenza, gli utenti con l’opzione Schede orario e ore abilitata nel loro livello di accesso potevano modificare le ore su qualsiasi scheda orario.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 21 gennaio 2021</p> <p>Versione di produzione: con la versione 21.1</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Sono stati migliorati i filtri e le visualizzazioni nell’area Schede orario</a> </p> <p>Sono stati aggiunti i filtri per progetti e problemi, nonché le opzioni Visualizza e Raggruppamento nella pagina Ricerca.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: 21 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Nascondi la casella del lavoro straordinario nelle schede orario</a> </p> <p>Ora puoi nascondere la casella del lavoro straordinario per semplificare la confusione degli utenti se non tieni traccia del lavoro straordinario in Workfront. È possibile nascondere la casella del lavoro straordinario per una scheda attività monouso o nel Timesheet Ricorrente.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 2 dicembre 2020</p> <p>Versione di produzione: 16 dicembre 2020</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Espandere o comprimere gli elementi nella navigazione delle breadcrumb</a> </p> <p>Per semplificare la visualizzazione dell’intero percorso della breadcrumb, sono state aggiunte le funzionalità di espansione e compressione.</p> <p>Ora, tutti gli elementi troncati vengono raggruppati prima del progetto con il testo "altro". Ad esempio, "3 ulteriori" indica che non vengono visualizzati 3 oggetti.</p> <p>In precedenza, era necessario fare clic sui puntini di sospensione per visualizzare gli oggetti troncati in un menu a discesa.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 7 gennaio 2020</p> <p>Versione di produzione: 21 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuovo aspetto per la navigazione nel breadcrumb</a> </p> <p>Per aiutare gli utenti a identificare meglio la loro posizione in Workfront e a navigare più facilmente tra gli oggetti, abbiamo apportato diversi miglioramenti alla navigazione delle breadcrumb.</p> </td> 
   <td><strong>Disponibile in queste date:</strong> <p>Versione di anteprima beta: 10 dicembre 2020</p> <p>Versione di produzione: 21 gennaio 2021</p> <p><strong>Disponibile in questi ambienti:</strong> </p> <p>La nuova esperienza Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

## Miglioramenti agli obiettivi di Workfront

La maggior parte delle nuove funzioni arriva alla versione degli Obiettivi di Workfront con la versione 21.1. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, consulta [Obiettivi di Adobe Workfront con la versione 21.1](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Miglioramenti di Workfront Scenario Planner

Nuove funzioni in arrivo in Workfront Scenario Planner versione con la versione 21.1. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, consulta [Adobe Workfront Scenario Planner con la versione 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione della versione 21.1. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## Miglioramenti API

La versione 12 dell’API è ora disponibile con la versione 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 12 dell’API](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

Per ulteriori informazioni sulle versioni API, consulta [Pianificazione del supporto e del controllo delle versioni API](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione 21.1, consulta [Aggiornamenti di manutenzione per Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Notifiche

* [Nuovi indirizzi IP per l’e-mail di Workfront con la versione 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Inserisce nell&#39;elenco Consentiti di indirizzi IP aggiuntivi per gli abbonamenti agli eventi](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [È richiesta la Inserisce nell&#39;elenco Consentiti di domini aggiuntivi per l’accesso a Workfront da parte di un’istanza di](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Obsolescenza Flash](#flash-deprecation)
* [Webinar sulla versione 21.1](#21-1-release-webinar)
* [Modifica della frequenza di rilascio dell’anteprima](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Nuovi indirizzi IP per l’e-mail di Workfront con la versione 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

Per aumentare il successo della distribuzione delle e-mail, con la versione di produzione 21.1 per i cluster 1, 2, 3, 4 e 5 verranno aggiunti nuovi indirizzi IP.

Per informazioni dettagliate sugli indirizzi IP da aggiungere per il cluster, vedere [Nuovi indirizzi IP per l’e-mail di Adobe Workfront con la versione 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

Per individuare il cluster su cui si sta eseguendo l&#39;istanza, passare a Configurazione > Sistema > Informazioni cliente.

### Inserisce nell&#39;elenco Consentiti di indirizzi IP aggiuntivi per gli abbonamenti agli eventi {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

Nel tentativo di aumentare il successo della consegna degli abbonamenti agli eventi, stiamo aggiungendo 4 nuovi indirizzi IP con la versione di produzione 21.1 nel primo trimestre del 2021. Per garantire che gli utenti continuino a ricevere gli abbonamenti agli eventi, è necessario aggiungere questi indirizzi IP al inserisco nell&#39;elenco Consentiti di prima di febbraio 2021.

Contatta il tuo reparto IT e/o di sicurezza interno per assistenza nell’aggiunta dei nuovi IP presenti nell’articolo, [API di abbonamento agli eventi](../../../wf-api/general/event-subs-api.md).

### È richiesta la Inserisce nell&#39;elenco Consentiti di domini aggiuntivi per l’accesso a Workfront da parte di un’istanza di {#allowlist-of-additional-domains-required-for-accessing-workfront}

Se la tua organizzazione utilizza un firewall, per garantire un accesso ininterrotto a Workfront devi aggiungere i seguenti domini aggiuntivi al inserisco nell&#39;elenco Consentiti di accesso:

* event.split.io
* sdk.split.io

Per ulteriori informazioni, consulta [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Obsolescenza Flash {#flash-deprecation}

Tutti gli strumenti basati su Flash sono stati rimossi da tutti i prodotti il 19 novembre 2020.

Per ulteriori informazioni sulle soluzioni sostitutive per ogni strumento specifico basato su Flash, vedere l&#39;articolo seguente: [Sostituzione degli strumenti basati su Flash in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Webinar sulla versione 21.1 {#21-1-release-webinar}

Il webinar sulla versione di Workfront 21.1 verrà presentato il 3 febbraio alle 11:00 EDT / 16:00 BST. Registrati al webinar [qui](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Modifica della frequenza di rilascio dell’anteprima {#change-in-preview-release-cadence}

A partire dal 20 maggio 2020, Workfront ha iniziato a rendere disponibili funzionalità nell’ambiente di anteprima su base settimanale. Prima di questa modifica, in genere la funzionalità veniva rilasciata nell’ambiente di anteprima ogni due settimane.

Per ulteriori informazioni, consulta [Modifica nelle domande frequenti sulla cadenza di rilascio dell’anteprima di Workfront](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Con Workfront One, potrai scoprire i contenuti, le risorse e le notizie più importanti da Workfront, il tutto in un&#39;unica posizione, con un unico accesso. Abbiamo unificato i siti Esperienza, Community e Formazione per facilitare la ricerca delle tue esigenze.

[Ulteriori informazioni su Workfront One](https://www.workfront.com/campaigns/workfront-one).
