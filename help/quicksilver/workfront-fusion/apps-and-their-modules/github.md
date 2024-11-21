---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli GitHub
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che utilizzano GitHub e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1839'
ht-degree: 0%

---

# [!DNL GitHub] moduli

In uno scenario [!DNL Adobe Workfront Fusion], puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL GitHub], nonché collegarlo a più applicazioni e servizi di terze parti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!DNL GitHub], è necessario disporre di un account [!DNL GitHub].

## Connetti [!DNL GitHub] a [!DNL Workfront Fusion]

Per istruzioni sulla connessione dell&#39;account [!DNL GitHub] a [!UICONTROL Workfront Fusion], vedere [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] moduli e relativi campi.

Quando configuri [!DNL GitHub] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL GitHub], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

* [[!UICONTROL Problemi di controllo]](#watch-issues)
* [[!UICONTROL Esaminare gli archivi]](#watch-repositories)
* [[!UICONTROL Forchette di controllo]](#watch-forks)
* [[!UICONTROL Osserva commenti]](#watch-comments)
* [[!UICONTROL Osserva richieste pull]](#watch-pull-requests)

#### [!UICONTROL Problemi di controllo]

Questo modulo si attiva quando viene aggiunto un nuovo problema o quando viene modificato un problema esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Voglio guardare]</td> 
   <td>Seleziona se desideri controllare tutti gli archivi o un solo archivio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Se hai scelto di monitorare i problemi in un solo archivio, seleziona l’archivio che desideri monitorare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri controllare solo i nuovi problemi, i nuovi problemi e tutte le modifiche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Puoi filtrare i problemi che desideri controllare in base alla modalità di associazione.</p> 
    <ul> 
     <li>[!UICONTROL Tutti i problemi]</li> 
     <li>[!UICONTROL Solo i problemi assegnati a me]</li> 
     <li>[!UICONTROL Solo problemi creati dall'utente]</li> 
     <li>[!UICONTROL Solo problemi che mi menzionano]</li> 
     <li>[!UICONTROL Solo i problemi per i quali sono abbonato agli aggiornamenti]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleziona se desideri guardare solo i problemi aperti o solo i problemi chiusi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etichette]</td> 
   <td>Aggiungi un tag. Il modulo verifica la presenza di problemi con questo tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Esaminare gli archivi]

Questo modulo viene attivato quando viene creato o modificato un archivio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di archivi restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri controllare i nuovi archivi e tutte le modifiche o solo i nuovi archivi.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Forchette di controllo]

Questo modulo si attiva quando viene creato un nuovo fork.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio da controllare per i fork.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di fork restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva commenti]

Questo modulo viene attivato quando viene aggiunto un nuovo commento o quando viene modificato un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio che desideri monitorare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero problema]</td> 
   <td>Se desideri limitare la ricerca cercando solo i nuovi commenti su un problema specifico, inserisci il numero del problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Specificare se si desidera controllare solo i nuovi commenti o i commenti e tutte le modifiche.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva richieste pull]

Questo modulo si attiva quando viene aggiunta una nuova richiesta di pull o viene modificata una richiesta di pull esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio che desideri monitorare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di richieste pull restituite]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleziona se desideri controllare le richieste [!UICONTROL only open pull], [!UICONTROL only closed ones] o tutte le richieste pull. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri controllare solo le nuove richieste pull, le nuove richieste pull e tutte le modifiche.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Ricerca di un problema]](#search-for-an-issue)
* [[!UICONTROL Crea un problema]](#create-an-issue)
* [[!UICONTROL Aggiorna un problema]](#update-an-issue)
* [[!UICONTROL Segnala un problema]](#get-an-issue)
* [[!UICONTROL Aggiungi assegnatari]](#add-assignees)
* [[!UICONTROL Rimuovi assegnatari]](#remove-assignees)
* [[!UICONTROL Aggiungere etichette a un problema]](#add-labels-to-an-issue)
* [[!UICONTROL Rimuovere un&#39;etichetta da un problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Crea un commento]](#create-a-comment)
* [[!UICONTROL Elenca commenti]](#list-comments)

#### [!UICONTROL Ricerca di un problema]

Questo modulo cerca i problemi che corrispondono ai criteri di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo (il numero di ripetizioni per esecuzione dello scenario). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare la modalità di ordinamento dei risultati della ricerca.</p> 
    <ul> 
     <li> <p>[!UICONTROL Corrispondenza migliore] </p> </li> 
     <li>[!UICONTROL Date created]</li> 
     <li>[!UICONTROL Date updated]</li> 
     <li>[!UICONTROL Numero di commenti]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina direzione]</td> 
   <td> <p>Seleziona crescente o decrescente. </p> <p>Per le date, selezionando <strong>[!UICONTROL discendente]</strong> verrà restituita prima la data più recente. </p> <p>Per [!UICONTROL numero di commenti], selezionando <strong>[!UICONTROL discendente]</strong> verrà restituito il problema con il numero più alto di commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Immettere o mappare la query di ricerca. Per una descrizione dettagliata delle opzioni di ricerca, vedere <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Ricerca di problemi e richieste pull</a> nel sito della Guida di [!DNL GitHub].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea un problema]

Questo modulo crea un nuovo problema nell’archivio selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio in cui desideri creare un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono di autorizzazioni di scrittura per l'archivio e i membri dell'organizzazione con autorizzazioni di lettura per l'archivio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleziona la milestone da associare al nuovo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etichette]</td> 
   <td>Seleziona le etichette da applicare al nuovo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Inserisci o mappa un titolo per il nuovo problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Inserisci o mappa il corpo del problema, ad esempio una descrizione o informazioni aggiuntive</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna un problema]

Questo modulo aggiorna un problema [!DNL GitHub] esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio in cui desideri aggiornare un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono di autorizzazioni di scrittura per il repository e i membri dell'organizzazione con autorizzazioni di lettura per il repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleziona l’attività cardine da associare al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etichette]</td> 
   <td>Seleziona le etichette da applicare al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema da aggiornare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleziona lo stato in cui desideri aggiornare il problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Inserisci o mappa un titolo per il problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Inserisci o mappa il corpo del problema, ad esempio una descrizione o informazioni aggiuntive</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Segnala un problema]

Questo modulo recupera i dettagli del problema specificato

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio contenente il problema di cui desideri recuperare i dettagli.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Inserisci o mappa il numero del problema di cui desideri recuperare i dettagli. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi assegnatari]

Questo modulo aggiunge gli assegnatari al problema specificato

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio contenente il problema a cui desideri aggiungere gli assegnatari.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono di autorizzazioni di scrittura per il repository e i membri dell'organizzazione con autorizzazioni di lettura per il repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Inserisci o mappa il numero del problema a cui desideri aggiungere gli assegnatari. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovi assegnatari]

Questo modulo rimuove gli assegnatari dal problema specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Selezionare l'archivio contenente il problema da cui si desidera rimuovere gli assegnatari.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL assegnatario]</td> 
   <td>Seleziona le persone da rimuovere dal problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immettere o mappare il numero del problema da cui si desidera rimuovere gli assegnatari. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere etichette a un problema]

Questo modulo aggiunge etichette a un problema. Le etichette sono definite a livello di repository e possono essere create solo da utenti con accesso in scrittura al repository.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio contenente il problema a cui desideri aggiungere le etichette.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etichette]</td> 
   <td>Seleziona le etichette da aggiungere al problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Inserisci o mappa il numero del problema a cui desideri aggiungere le etichette.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere un&#39;etichetta da un problema]

Questo modulo rimuove una singola etichetta da un problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Selezionare l'archivio contenente il problema da cui si desidera rimuovere un'etichetta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etichette]</td> 
   <td>Seleziona l’etichetta da rimuovere dal problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immettere o mappare il numero del problema da cui si desidera rimuovere un'etichetta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea un commento]

Questo modulo crea un commento sul problema specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Selezionare l'archivio contenente il problema per il quale si desidera creare un commento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Inserisci o mappa il numero del problema sul quale desideri creare un commento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Inserisci o mappa il contenuto del commento.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca commenti]

In questo modulo sono elencati tutti i commenti relativi al problema specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL GitHub] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archivio [!UICONTROL]</td> 
   <td>Seleziona l’archivio contenente il problema da cui desideri elencare i commenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Inserisci o mappa il numero del problema dal quale desideri elencare i commenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da]</td> 
   <td>Il modulo restituirà i commenti creati dopo tale data. Per un elenco dei formati di data supportati, vedere <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di commenti restituiti]</td> 
   <td>Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
