---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli GitHub
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano GitHub e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL GitHub], nonché collegarlo a più applicazioni e servizi di terze parti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL GitHub] moduli, è necessario disporre di un [!DNL GitHub] conto.

## Connetti [!DNL GitHub] a [!DNL Workfront Fusion]

Per istruzioni su come collegare le [!DNL GitHub] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] moduli e relativi campi.

Quando si configura [!DNL GitHub] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL GitHub] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

* [[!UICONTROL Problemi di controllo]](#watch-issues)
* [[!UICONTROL Guarda gli archivi]](#watch-repositories)
* [[!UICONTROL Orologi forni]](#watch-forks)
* [[!UICONTROL Osserva commenti]](#watch-comments)
* [[!UICONTROL Richieste di pull di controllo]](#watch-pull-requests)

#### [!UICONTROL Problemi di controllo]

Questo modulo viene attivato quando viene aggiunto un nuovo problema o viene modificato un problema esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Voglio guardare]</td> 
   <td>Seleziona se desideri guardare tutti gli archivi o un solo archivio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Se hai scelto di guardare i problemi in un solo archivio, seleziona l’archivio da guardare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri tenere traccia solo dei nuovi problemi o dei nuovi problemi e di tutte le modifiche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Puoi filtrare i problemi di cui desideri tenere conto in base al modo in cui sono associati.</p> 
    <ul> 
     <li>[!UICONTROL Tutti i problemi]</li> 
     <li>[!UICONTROL Solo problemi assegnati all'utente]</li> 
     <li>[!UICONTROL Solo problemi creati da me]</li> 
     <li>[!UICONTROL Solo problemi che mi menzionano]</li> 
     <li>[!UICONTROL Solo problemi per i quali sono iscritto agli aggiornamenti per]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleziona se visualizzare solo i problemi aperti o solo quelli chiusi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Aggiungi un tag . Il modulo controlla i problemi relativi a questo tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda gli archivi]

Questo modulo viene attivato quando un archivio viene creato o modificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di archivi restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri controllare i nuovi archivi e tutte le modifiche, o solo i nuovi archivi.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Orologi forni]

Questo modulo viene attivato quando viene creato un nuovo fork.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selezionare l'archivio che si desidera controllare per i fork.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di fork restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva commenti]

Questo modulo viene attivato quando viene aggiunto un nuovo commento o viene modificato un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selezionare l'archivio da controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero del problema]</td> 
   <td>Se si desidera limitare la ricerca cercando solo i nuovi commenti effettuati su un problema specifico, immettere il numero del problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera controllare solo i nuovi commenti o commenti e tutte le modifiche.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Richieste di pull di controllo]

Questo modulo viene attivato quando viene aggiunta una nuova richiesta di pull o viene modificata una richiesta di pull esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selezionare l'archivio da controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di richieste di pull restituite]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleziona se desideri guardare solo le richieste di pull aperte, solo quelle chiuse o tutte le richieste di pull. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleziona se cercare solo le nuove richieste di pull o le nuove richieste di pull e tutte le modifiche.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Cercare un problema]](#search-for-an-issue)
* [[!UICONTROL Crea un problema]](#create-an-issue)
* [[!UICONTROL Aggiornare un problema]](#update-an-issue)
* [[!UICONTROL Ottieni un problema]](#get-an-issue)
* [[!UICONTROL Aggiungi assegnatari]](#add-assignees)
* [[!UICONTROL Rimuovi assegnatari]](#remove-assignees)
* [[!UICONTROL Aggiungere etichette a un problema]](#add-labels-to-an-issue)
* [[!UICONTROL Rimuovere un&#39;etichetta da un problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Creare un commento]](#create-a-comment)
* [[!UICONTROL Elencare commenti]](#list-comments)

#### [!UICONTROL Cercare un problema]

Questo modulo cerca i problemi che corrispondono ai criteri di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di problemi restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo (il numero di ripetizioni per esecuzione di scenari). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare la modalità di ordinamento dei risultati della ricerca.</p> 
    <ul> 
     <li> <p>[!UICONTROL Best match] </p> </li> 
     <li>[!UICONTROL Data di creazione]</li> 
     <li>[!UICONTROL Data aggiornata]</li> 
     <li>[!UICONTROL Numero di commenti]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina direzione]</td> 
   <td> <p>Selezionare crescente o decrescente. </p> <p>Per le date, seleziona <strong>[!UICONTROL decrescente]</strong> restituirà prima la data più recente. </p> <p>Per il numero di commenti, selezionare <strong>[!UICONTROL decrescente]</strong> restituirà prima il problema con il numero più alto di commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query [!UICONTROL]</td> 
   <td>Inserisci o mappa la query di ricerca. Per una descrizione dettagliata delle opzioni di ricerca, vedi <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Problemi di ricerca e richieste di pull</a> sulla [!DNL GitHub] sito della guida.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l'archivio in cui desideri creare un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono delle autorizzazioni di scrittura per l'archivio e i membri dell'organizzazione che dispongono delle autorizzazioni di lettura per l'archivio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleziona la fase cardine da associare al nuovo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
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

#### [!UICONTROL Aggiornare un problema]

Questo modulo aggiorna un [!DNL GitHub] problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l'archivio in cui desideri aggiornare un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono delle autorizzazioni di scrittura per l'archivio e i membri dell'organizzazione con autorizzazioni di lettura per l'archivio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Selezionare l'attività cardine che si desidera associare al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
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
   <td>Immetti o mappa un titolo per il problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Inserisci o mappa il corpo del problema, ad esempio una descrizione o informazioni aggiuntive</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un problema]

Questo modulo recupera i dettagli sul problema specificato

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio contenente il problema di cui desideri recuperare i dettagli.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema di cui desideri recuperare i dettagli. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi assegnatari]

Questo modulo aggiunge assegnazioni al problema specificato

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio che contiene il problema a cui desideri aggiungere gli assegnatari.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnatario]</td> 
   <td>Seleziona le persone da assegnare al problema. Gli assegnatari disponibili includono tutti coloro che dispongono delle autorizzazioni di scrittura per l'archivio e i membri dell'organizzazione con autorizzazioni di lettura per l'archivio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema a cui desideri aggiungere gli assegnatari. </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio che contiene il problema da cui vuoi rimuovere gli assegnatari.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnatario]</td> 
   <td>Seleziona le persone da rimuovere dal problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema da cui vuoi rimuovere gli assegnatari. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere etichette a un problema]

Questo modulo aggiunge etichette a un problema. Le etichette sono definite a livello di archivio e possono essere create solo da un utente con accesso in scrittura all&#39;archivio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio che contiene il problema a cui desideri aggiungere le etichette.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleziona le etichette da aggiungere al problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema a cui desideri aggiungere le etichette.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio che contiene il problema da cui vuoi rimuovere un’etichetta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleziona l’etichetta da rimuovere dal problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema dal quale vuoi rimuovere un’etichetta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un commento]

Questo modulo crea un commento sul problema specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleziona l’archivio che contiene il problema in cui desideri creare un commento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema sul quale desideri creare un commento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Inserisci o mappa il contenuto del commento.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elencare commenti]

Questo modulo elenca tutti i commenti sul problema specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL GitHub] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selezionare l'archivio contenente il problema da cui si desidera elencare i commenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Immetti o mappa il numero del problema dal quale desideri elencare i commenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da]</td> 
   <td>Il modulo restituirà i commenti creati dopo tale data. Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di commenti restituiti]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo. </td> 
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
