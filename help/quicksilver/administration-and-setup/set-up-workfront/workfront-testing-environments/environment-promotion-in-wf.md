---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Spostamento di oggetti da un ambiente a un altro in Workfront
description: La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Non supporta la possibilità di spostare oggetti transazionali (con eccezioni limitate).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Panoramica sullo spostamento di oggetti tra ambienti Workfront (promozione dell&#39;ambiente)

La funzionalità di promozione dell&#39;ambiente consente di spostare gli oggetti da un ambiente Workfront a un altro. Ad esempio, puoi creare un modello e configurarlo nel tuo ambiente sandbox, sapendo che eventuali test eseguiti non influiranno sui dati effettivi della tua organizzazione. Dopo aver configurato e testato il modello, puoi spostarlo nell’ambiente di produzione pronto per l’uso.

Questo processo viene definito &quot;promozione dell&#39;ambiente&quot;.

È possibile eseguire questo processo in Workfront creando un pacchetto di oggetti da spostare e quindi installandolo nel nuovo ambiente.

* Per istruzioni specifiche sull’esecuzione di questo processo in Workfront, consulta:

   * [Creare o modificare un pacchetto di promozione dell’ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installare un pacchetto di promozione dell’ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Per istruzioni sull’esecuzione di questo processo tramite l’API di Workfront, consulta [Sposta oggetti tra [!DNL Workfront] ambienti che utilizzano [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Oggetti supportati per la promozione dell’ambiente

La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Non supporta la possibilità di spostare oggetti transazionali (con eccezioni limitate).

* [Oggetti di lavoro](#work-objects)
* [Oggetti di reporting](#reporting-objects)
* [Oggetti dati personalizzati](#custom-data-objects)
* [Oggetti organizzazione](#organization-objects)
* [Altri oggetti di configurazione](#other-configuration-objects)


### Oggetti di lavoro

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Progetto (PROJ) | Progetto<br>Attività<br>Assegnazione<br>Predecessore<br>Azienda<br>Percentuale sostituzione<br>Gruppo<br>Ruolo<br>Team<br>Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Pianificazione<br>Giorno non feriale<br>Definizione coda<br>Gruppo di argomenti coda<br>Argomento Coda<br>Regola di Instradamento<br>Percorso milestone<br>Milestone<br>Tipo di Ora<br>Pool di Risorse<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Modello (TMPL) | Modello<br>Attività modello<br>Assegnazione attività modello<br>Predecessore attività modello<br>Azienda<br>Percentuale sostituzione<br>Gruppo<br>Ruolo<br>Team<br>Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Pianificazione<br>Giorno non feriale<br>Definizione coda<br>Gruppo di argomenti coda<br>Argomento Coda<br>Regola di Instradamento<br>Percorso milestone<br>Milestone<br>Tipo di Ora<br>Pool di Risorse<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |

### Oggetti di reporting

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Modello di layout (UITMPL) | Modello di layout<br>Dashboard<br>Calendario<br>Sezione calendario<br>Pagina esterna<br>Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Dashboard (PTLTAB) | Dashboard<br>Calendario<br>Sezione calendario<br>Pagina esterna<br>Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Calendario (calendario) | Calendario<br>Sezione calendario |
| Pagina esterna (EXTSEC) | Pagina Esterna |
| Rapporto (PTLSEC) | Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Filtro (UIFT) | Filtro<br>Parametro |
| Raggruppamento (UIGB) | Raggruppamento<br>Parametro |
| Visualizza (UIVW) | Visualizza<br>Parametro |

### Oggetti dati personalizzati

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Categoria (CTGY) | Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria<br>Gruppo |
| Parametro (PARAM) | Parametro<br>Opzione Parametro |
| Raggruppa Parametri (PGRP) | Gruppo di parametri |

### Oggetti organizzazione

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Gruppo (GROUP) | Gruppo <br>Sottogruppi (fino a 5 livelli) *<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Ruolo (ROLE) | Ruolo |
| Team (TEAM) | Team<br>Gruppo |
| Società (CMPY) | Azienda<br>Percentuale sostituzione<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Parametro <br>Logica di visualizzazione della categoria<br>Gruppo |
| Portfolio (PORTA) | Portfolio<br>Programma<br>Gruppo<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Programma (PRGM) | Programma<br>Portfolio<br>Gruppo<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |

### Altri oggetti di configurazione

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Processo di approvazione (ARVPRC) | Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Ruolo<br>Team<br>Gruppo |
| Pianificazione (SCHED) | Pianificazione<br>Giorno non feriale<br>Gruppo |
| Percorso milestone (MPATH) | Percorso milestone<br>Milestone |
| Timesheet Ricorrente (TSPRO) | Timesheet Ricorrente<br>Tipo di Ora |
| Tipo di Ora (HOURT) | Tipo di ora |
| Tipo di spesa (EXPTYP) | Tipo di Spesa |
| Tipo di rischio (RSKTYP) | Tipo Rischio |
| Pool di Risorse (RSPL) | Gruppo di risorse |

\* Attualmente non disponibile


## Stati di promozione dell’ambiente

I pacchetti di promozione dell’ambiente procedono attraverso diversi stati man mano che vengono creati e preparati per essere spostati tra gli ambienti. Puoi visualizzare questi stati nell’elenco dei pacchetti all’interno di Workfront oppure nelle risposte API, se utilizzi l’API Workfront.

Questi stati includono:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLAGGIO</td> 
   <td><p>Questo stato viene assegnato automaticamente durante il montaggio degli oggetti. </p><p>L'assemblaggio si riferisce al processo automatizzato di identificazione degli oggetti e dei sottooggetti da includere in un package e di aggiunta di tali oggetti e dei relativi dati al package.</p><p>Questo stato non può essere impostato direttamente da un cliente.</p></td> 
  </tr> 
  <tr> 
   <td>BOZZA</td> 
   <td><p>Questo stato viene assegnato al termine di un processo di assemblaggio o durante la creazione di un pacchetto di promozione vuoto.</p><p>Il cliente può ripristinare lo stato attuale del pacchetto promozionale.</p><p>In questo stato, il pacchetto di promozione non può essere installato in alcun ambiente.</p></td> 
  </tr> 
  <tr> 
   <td>TEST</td> 
   <td><p>Questo stato consente di installare un pacchetto di promozione in qualsiasi sandbox di anteprima o di aggiornamento personalizzato. In questo stato, il pacchetto non può essere installato in Produzione.</p></td> 
  </tr> 
  <tr> 
   <td>ATTIVO</td> 
   <td><p>Questo stato consente di installare un pacchetto promozionale in qualsiasi ambiente, inclusa la produzione.</p><p>Quando lo stato di un pacchetto è impostato su ACTIVE, <code>publishedAt</code> La data viene impostata automaticamente sulla marca temporale corrente della richiesta.</p></td> 
  </tr> 
  <tr> 
   <td>DISABILITATO</td> 
   <td><p>Questo stato verrà utilizzato per nascondere i pacchetti promozionali utilizzati in precedenza che non verranno installati in alcun ambiente in futuro.</p><p>Quando un pacchetto si trova in questo stato, non può essere installato in alcun ambiente.</p><p>Quando lo stato di un pacchetto è impostato su DISABLED, il <code>retiredAt</code> La data viene impostata automaticamente sulla marca temporale corrente della richiesta.</p><p>Si consiglia di utilizzare questo stato anziché il<code>DELETE /package</code> endpoint perché è recuperabile e la cronologia di installazione viene mantenuta per tutte le distribuzioni effettuate con questo pacchetto.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLAGGIO NON RIUSCITO</td> 
   <td><p>Se la fase ASSEMBLING non riesce, il pacchetto promozionale viene automaticamente posto in questo stato.</p><p>Per riportare il pacchetto alla fase ASSEMBLING, è necessario attivare nuovamente il processo di estrazione.</p></td> 
  </tr> 
  </tbody> 
</table>


