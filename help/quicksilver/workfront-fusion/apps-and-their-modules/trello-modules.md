---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Trello
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Trello e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL Trello] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Trello], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Trello] moduli, è necessario disporre di un [!UICONTROL Trello] conto.

## Connetti [!UICONTROL Trello] a [!DNL Workfront Fusion]

Per istruzioni su come collegare le [!UICONTROL Trello] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello] moduli e relativi campi

Quando si configura [!UICONTROL Trello] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!UICONTROL Trello] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Bacheche](#boards)
* [Elenchi](#lists)
* [Schede](#cards)
* [Membri](#members)
* [Elenchi di controllo](#checklists)
* [Etichette](#labels)
* [Commenti](#comments)

### Bacheche

+++ **[!UICONTROL Schede di controllo]**

Questo modulo di attivazione inizia uno scenario in cui viene aggiunta una nuova bacheca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Numero massimo di bacheche [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare una bacheca]**

Questo modulo di azione crea una nuova bacheca con le impostazioni selezionate.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere o mappare un nome per la nuova bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td> <p>Se necessario, inserite o mappate la descrizione della bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Immetti o mappa l'ID dell'organizzazione. L’ID organizzazione può essere recuperato utilizzando un altro modulo, ad esempio il modulo Attività di controllo .</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Livello di autorizzazione]</p> </td> 
   <td> <p>Le commissioni hanno regole di voto e di commento diverse per ogni livello di autorizzazione. Ad esempio: se la tua bacheca è [!UICONTROL Private] e imposti le regole di voto e commento come [!UICONTROL All], ricevi un errore. </p> <p>Il voto e il commento sono limitati ai seguenti gruppi per ogni livello di autorizzazione:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: —&gt;Membri, membri e osservatori</li> 
     <li><strong>[!UICONTROL Per organizzazione]</strong>: —&gt;Membri, membri e osservatori, membri dell'organizzazione</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;Membri, membri e osservatori, membri dell'organizzazione, tutti</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voto]</p> </td> 
   <td> <p>Selezionare un'opzione per specificare chi può votare su questa bacheca. Vedere il campo [!UICONTROL Permission level] (Livello di autorizzazione) per le limitazioni di voto sui livelli di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Commenti]</p> </td> 
   <td> <p>Selezionate un'opzione per specificare gli utenti che possono commentare le schede per questa bacheca. Vedere il campo [!UICONTROL Permission level] (Livello di autorizzazione) per commentare le limitazioni dei livelli di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>Seleziona chi può invitare altre persone in questa bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>Seleziona se i membri del team possono iscriversi alla bacheca personalmente o se devono essere invitati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Etichette predefinite]</p> </td> 
   <td> <p>Selezionate se utilizzare il set di etichette predefinito per la nuova bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Elenchi predefiniti]</p> </td> 
   <td> <p>Seleziona se aggiungere il set predefinito di elenchi alla bacheca ([!UICONTROL To Do], [!UICONTROL Doing], [!UICONTROL Done]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>Selezionate o mappate l'ID della bacheca che desiderate copiare nella nuova bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Copertine per schede]</p> </td> 
   <td> <p>Seleziona <strong>[!UICONTROL Sì]</strong> per attivare le coperture delle schede per la bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Background]</p> </td> 
   <td> <p>Selezionare il colore dello sfondo o dello sfondo personalizzato.</p> <p>Nota: Gli sfondi personalizzati sono disponibili solo per gli abbonati a [!UICONTROL Trello Gold e Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invecchiamento scheda]</p> </td> 
   <td> <p>Selezionare tra due modalità di invecchiamento della scheda. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Le carte diventano progressivamente più trasparenti con l'età. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Le carte si strapperanno, gialle e si rompono come una vecchia mappa dei pirati quando invecchiano.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modificare una bacheca]**

Questo modulo di azione modifica le impostazioni di una bacheca esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Immettere o mappare l'ID [!UICONTROL Trello] univoco della bacheca che si desidera creare nel modulo. È possibile recuperare l'ID della bacheca utilizzando un altro modulo, ad esempio il modulo Bacheche di controllo</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo nome]</td> 
   <td> <p> Immettere o mappare un nuovo nome per la bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuova descrizione]</td> 
   <td> <p> Se necessario, inserite o mappate una nuova descrizione della bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Inserite o mappate l'ID [!UICONTROL Trello] univoco della bacheca che desiderate modificare dal modulo. È possibile recuperare l'ID bacheca utilizzando un altro modulo, ad esempio [!DNL Watch Activities] modulo .</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Selezionate un'opzione per specificare se l'utente che agisce è iscritto alla bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Livello di autorizzazione]</p> </td> 
   <td> <p>Le commissioni hanno regole di voto e di commento diverse per ogni livello di autorizzazione. Ad esempio: se la tua bacheca è [!UICONTROL Private] e imposti le regole di voto e commento come [!UICONTROL All], ricevi un errore. </p> <p>Il voto e il commento sono limitati ai seguenti gruppi per ogni livello di autorizzazione:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: —&gt;Membri, membri e osservatori</li> 
     <li><strong>[!UICONTROL Per organizzazione]</strong>: —&gt;Membri, membri e osservatori, membri dell'organizzazione</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;Membri, membri e osservatori, membri dell'organizzazione, tutti</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voto]</p> </td> 
   <td> <p>Selezionare un'opzione per specificare chi può votare su questa bacheca. Vedere il campo [!UICONTROL Permission level] (Livello di autorizzazione) per le limitazioni di voto sui livelli di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Commenti]</p> </td> 
   <td> <p>Selezionate un'opzione per specificare gli utenti che possono commentare le schede per questa bacheca. Vedere il campo [!UICONTROL Permission level] (Livello di autorizzazione) per commentare le limitazioni dei livelli di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>Seleziona chi può invitare le persone in questa bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> Seleziona se i membri del team possono iscriversi alla bacheca personalmente o se devono essere invitati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Coperture per schede]</td> 
   <td> <p> Seleziona se le coperture delle schede devono essere visualizzate su questa bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background] </td> 
   <td> <p>Selezionare il colore dello sfondo o dello sfondo personalizzato.</p> <p>Nota: Gli sfondi personalizzati sono disponibili solo per gli abbonati a [!UICONTROL Trello Gold e Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> Se hai selezionato di utilizzare uno sfondo personalizzato nel campo [!UICONTROL Background] , immetti o mappa l’ID dello sfondo da utilizzare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invecchiamento scheda]</p> </td> 
   <td> <p>Selezionare tra due modalità di invecchiamento della scheda. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Le carte diventano progressivamente più trasparenti con l'età. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Le carte si strapperanno, gialle e si rompono come una vecchia mappa dei pirati quando invecchiano.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feed calendario abilitato]</td> 
   <td> <p> Seleziona se il feed del calendario è abilitato o meno.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; nome dell'etichetta]</td> 
   <td> <p> Assegna un nome all’etichetta di colore desiderata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Selezionate un'opzione per indicare se desiderate archiviare (chiudere) la bacheca. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ottenere una bacheca]**

Questo modulo di azione recupera i dettagli di una bacheca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Immettere o mappare l'ID della bacheca di cui si desidera recuperare le informazioni.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Questo modulo di ricerca recupera informazioni su una bacheca specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query [!UICONTROL] </td> 
   <td> <p>Immettere o mappare il nome (o una parte del nome) della bacheca di cui si desidera ottenere le informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di schede restituite]</td> 
   <td> <p> Immettere il numero massimo di bacheche [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione. Questo valore deve essere minore o uguale a 1000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parziale] </p> </td> 
   <td> <p>Per impostazione predefinita, questo modulo cerca nel contenuto membro le corrispondenze esatte di ogni parola nella query. Quando [!UICONTROL Partial] è abilitato, il modulo cerca il contenuto che inizia con qualsiasi parola nella query.</p> <p> Ad esempio, se utilizzi la parola "sviluppo" per cercare una bacheca intitolata "Report sullo stato di sviluppo", per impostazione predefinita dovrai cercare l'intera parola. Se hai [!UICONTROL Partial] abilitato, puoi cercare "dev" ma non "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>Inserite "mine" o mappate un elenco separato da virgole degli ID bacheca.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiviare o annullare l&#39;archiviazione di una bacheca]**

Questo modulo d&#39;azione chiude o riapre una bacheca specificata dall&#39;utente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Inserite o mappate l'ID della bacheca che desiderate chiudere o riaprire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivia o annulla l'archiviazione]</td> 
   <td> <p> Selezionate se desiderate chiudere (archiviare) o riaprire (annullare l'archiviazione) la bacheca.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Assegnare un membro a una bacheca]**

Questo modulo di azione assegna un membro a una bacheca specificata dall&#39;utente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Selezionate la bacheca in cui desiderate aggiungere un membro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail]</td> 
   <td> <p> Inserite o mappate l'indirizzo e-mail del membro che desiderate aggiungere alla bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Member type]</p> </td> 
   <td> <p>Selezionate il tipo di membro che desiderate aggiungere alla bacheca.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: Un amministratore della bacheca può eseguire qualsiasi azione sulla bacheca.</li> 
     <li><strong>[!UICONTROL Normale]</strong>: Un membro normale è semplicemente un membro del consiglio di amministrazione.</li> 
     <li><strong>[!UICONTROL Observer]</strong>: Un osservatore è un membro con accesso in sola lettura al consiglio di amministrazione. <br>Gli osservatori sono disponibili solo per i team con [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome completo]</td> 
   <td> <p> Inserite il nome completo dell'utente che desiderate aggiungere alla bacheca.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Annullare l&#39;assegnazione di un membro da una bacheca]**

Questo modulo di azione rimuove un membro da una bacheca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Immettete (mappate o selezionate) l'ID della bacheca da cui desiderate rimuovere l'utente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>Selezionate il membro da rimuovere dalla bacheca.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Elenchi

+++ **[!UICONTROL Schede di controllo spostate in un elenco]**

Questo modulo di attivazione si attiva quando una scheda viene spostata in un elenco specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Selezionate la bacheca che contiene l'elenco di schede da controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Selezionare l'elenco che si desidera controllare per le schede.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Numero massimo di schede [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare un elenco]**

Questo modulo di azione crea un elenco su una bacheca specificata .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Inserite o mappate l'ID della bacheca in cui desiderate creare un elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere o mappare un nome per il nuovo elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleziona se desideri aggiungere l’elenco in alto o aggiungerlo in fondo alla scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia elenco]</td> 
   <td> <p> Seleziona la modalità di immissione dell’ID dell’elenco da copiare.</p> 
    <ul> 
     <li> <p><strong>Immettere manualmente</strong> </p> <p>In <strong>[!UICONTROL List ID]</strong> immetti o mappa l’ID dell’elenco da copiare.<br></p> </li> 
     <li> <p><strong>Seleziona</strong> </p> <p>Selezionate la bacheca che contiene l'elenco da copiare, quindi selezionate l'elenco.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modificare un elenco]**

Questo modulo di azione modifica un elenco esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Immetti o mappa l’ID dell’elenco da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere o mappare un nuovo nome per l'elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Mappare o selezionate la bacheca in cui desiderate spostare l'elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleziona se desideri aggiungere l’elenco in alto o aggiungerlo in fondo alla scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sottoscritto]</td> 
   <td> <p>Abilita questa opzione se desideri abbonarti all’elenco il membro attivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ottieni elenco]**

Questo modulo di azione recupera i dettagli su un elenco specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Immetti o mappa l’ID dell’elenco di cui desideri recuperare le informazioni.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Schede

+++ **[!UICONTROL Schede di controllo]**

Questo modulo di attivazione è attivato quando viene aggiunta una nuova scheda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Oggetto guardato]</td> 
   <td> <p>Selezionare la posizione in cui si desidera visualizzare le schede.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tutte le schede]</strong> </li> 
     <li> <p><strong>Carte su schede specifiche</strong> </p> <p>Selezionare la bacheca che si desidera controllare per le schede</p> </li> 
     <li> <p><strong>[!UICONTROL Carte su un elenco specifico]</strong> </p> <p>Selezionate la bacheca che contiene l'elenco da controllare per le schede, quindi selezionate l'elenco.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Numero massimo di schede [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare una scheda]**

Questo modulo di azione crea una scheda in un elenco selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID elenco]</td> 
   <td> <p> Seleziona come inserire l'ID dell'elenco in cui si desidera aggiungere una scheda.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL List ID]</strong> immetti o mappa l'ID dell'elenco in cui desideri aggiungere una scheda.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene l'elenco da copiare, quindi selezionate l'elenco.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Per ogni etichetta da aggiungere alla scheda, immetti l’ID dell’etichetta. L’ID può essere recuperato, ad esempio, utilizzando il modulo [!UICONTROL Retrieve Labels] (Etichette di recupero).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>Per ogni membro che si desidera aggiungere alla scheda, immettere l'ID del membro. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere un nome per la nuova scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Descrizione]</p> </td> 
   <td> <p>Inserire la descrizione della scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleziona se desideri aggiungere la scheda all'inizio o la scheda [!UICONTROL aggiungi] in fondo all'elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di scadenza]</td> 
   <td> <p> Immettere una data di scadenza per la scheda. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due completati]</td> 
   <td> <p> Abilita questa opzione per contrassegnare il completamento della scheda alla data di scadenza.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td> <p>Immetti o mappa l'URL di un file da aggiungere come allegato alla scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL File di origine]</p> </td> 
   <td> <p>Immettere o mappare le informazioni relative a un file da aggiungere come allegato alla scheda.</p> 
    <ul> 
     <li>[!UICONTROL File name]: Immetti o mappa il nome del file, inclusa l’estensione del file.</li> 
     <li> 
     <p>Selezionare un file da un modulo precedente o mappare il nome e i dati del file</p> 
     <p>Nota: C'è un limite di caricamento dei file di 10 MB per allegato. Tuttavia, i membri [!UICONTROL Business Class] e [!UICONTROL Trello Gold] hanno un limite di caricamento dei file di 250 MB per allegato.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia scheda]</td> 
   <td> <p> Seleziona l'ID della scheda da copiare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda che desideri copiare.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda da copiare, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modificare una scheda]**

Questo modulo di azione modifica una scheda esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Card ID]</td> 
   <td> <p> Seleziona l'ID della scheda da modificare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda che desideri modificare.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda da modificare, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo nome]</td> 
   <td> <p>Immettere o mappare un nuovo nome per la scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nuova descrizione]</p> </td> 
   <td> <p>Immetti o mappa una nuova descrizione per la scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Spostare una scheda]</p> </td> 
   <td> <p>Selezionate la bacheca o la bacheca e l'elenco in cui desiderate spostare la scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Aggiungi gli ID delle etichette da aggiungere alla scheda. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleziona se desideri aggiungere la scheda all'inizio o la scheda [!UICONTROL aggiungi] in fondo all'elenco.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di scadenza]</td> 
   <td> <p> Immettere una data di scadenza per la scheda. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due completati]</td> 
   <td> <p> Se questa opzione è attivata, la scheda viene contrassegnata come completata alla data di scadenza.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>Aggiungi o mappa l'ID dei membri che desideri aggiungere alla scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID copertura allegato]</p> </td> 
   <td> <p>Immettere o mappare l'ID dell'allegato immagine che si desidera utilizzare come copertina della scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Seleziona se il membro deve essere iscritto alla scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Selezionate un'opzione per indicare se desiderate archiviare (chiudere) la scheda. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ottieni una scheda]**

Questo modulo di azione recupera i dettagli di una scheda selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p>Inserite l'ID della bacheca che contiene la scheda di cui desiderate recuperare i dettagli. Questo consente di visualizzare i nomi dei campi personalizzati della bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti l'ID della scheda]</td> 
   <td> <p> Seleziona la modalità di immissione dell'ID della scheda di cui desideri recuperare i dettagli.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda di cui desideri recuperare i dettagli.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda di cui desiderate recuperare i dettagli, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Cerca schede]**

Questo modulo di azione restituisce schede corrispondenti alla query di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Selezionate le bacheche da cercare. Se non è selezionata alcuna bacheca, la ricerca viene eseguita su tutte le bacheche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Query [!UICONTROL]</p> </td> 
   <td> <p>Inserisci la query di ricerca. Puoi perfezionare la ricerca utilizzando i seguenti operatori di ricerca:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>È possibile aggiungere "-" a qualsiasi operatore per eseguire una ricerca negativa, ad esempio <code>[!UICONTROL -has:members]</code> per cercare le schede senza alcun membro assegnato.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Restituisce le schede assegnate a un membro. È inoltre possibile utilizzare <code>member:</code>. Utilizzo <code>@me</code> per includere solo le carte.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Restituisce schede etichettate. È inoltre possibile utilizzare <code>label:</code>. Ad esempio: <code>label:"FIX IT"</code> restituirà schede con l’etichetta denominata "FIX IT".</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Restituisce schede all'interno di una bacheca specifica. Ad esempio: <code>board:Trello</code> restituirà schede sulle bacheche con [!UICONTROL Trello] nel nome della bacheca.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Restituisce schede all'interno dell'elenco denominato "name".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Restituisce schede con allegati. La <code>has</code>: può essere utilizzato anche con altri attributi, come <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>oppure <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Restituisce le schede dovute entro 24 ore. La <code>due:</code> può essere utilizzato anche con altri intervalli di tempo, come <code>due:week</code>, <code>due:month</code>oppure <code>due:overdue</code>. Puoi anche cercare un intervallo di giorni specifico. Ad esempio, l’aggiunta <code>due:14</code> per cercare include le schede dovute nei successivi 14 giorni.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Restituisce le schede create nelle ultime 24 ore. La<code> created:</code> può essere utilizzato anche con altri intervalli di tempo, come <code>created:week</code> o <code>created:month</code>. Puoi anche cercare un intervallo di giorni specifico. Ad esempio, l’aggiunta <code>created:14</code> nella ricerca sono incluse le schede create negli ultimi 14 giorni.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Restituisce le schede modificate nelle ultime 24 ore. La <code>edited:</code> può essere utilizzato anche con altri intervalli di tempo, come <code>edited:week</code> o <code>edited:month</code>. Puoi anche cercare un intervallo di giorni specifico. Ad esempio, l’aggiunta <code>edited:21</code> nella ricerca sono incluse le schede modificate negli ultimi 21 giorni.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Restituisce schede che corrispondono al testo delle descrizioni delle schede, delle liste di controllo, dei commenti o dei nomi delle schede. Ad esempio, commento: "FIX IT" restituirà schede con "FIX IT" in un commento.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Restituisce schede aperte o archiviate. Se non viene specificato nessuno dei due tipi, [!UICONTROL Trello] restituisce entrambi i tipi.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Include solo le schede sulle bacheche stellate.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di schede restituite]</td> 
   <td> <p> Numero massimo di schede [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione. Questo valore deve essere minore o uguale a 1000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parziale] </td> 
   <td> <p>Per impostazione predefinita, questo modulo cerca nel contenuto membro le corrispondenze esatte di ogni parola nella query. Quando [!UICONTROL Partial] è abilitato, il modulo cerca il contenuto che inizia con qualsiasi parola nella query.</p> <p> Ad esempio, se utilizzi la parola "sviluppo" per cercare una bacheca intitolata "Report sullo stato di sviluppo", per impostazione predefinita dovrai cercare l'intera parola. Se hai [!UICONTROL Partial] abilitato, puoi cercare "dev" ma non "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card] </td> 
   <td> <p>Aggiungi le schede che desideri cercare in modo specifico.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiviare o annullare l&#39;archiviazione di una scheda]**

Questo modulo di azione archivia o invia nuovamente una scheda alla bacheca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> Immetti o mappa l'ID della scheda che desideri archiviare o inviare nuovamente alla bacheca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivia o annulla l'archiviazione]</td> 
   <td> <p> Seleziona se chiudere la scheda (archivio) o inviarla nuovamente alla bacheca (annullamento dell'archiviazione).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Aggiungi un allegato]**

Questo modulo di azione aggiunge un allegato alla scheda selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti l'ID della scheda]</td> 
   <td> <p> Seleziona la modalità di immissione dell'ID della scheda di cui desideri recuperare i dettagli.</p> 
    <ul> 
     <li> <p><strong>Immettere manualmente</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda di cui desideri recuperare i dettagli.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda di cui desiderate recuperare i dettagli, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di allegato]</p> </td> 
   <td> <p>Seleziona se desideri caricare il file direttamente o fornire un URL al file.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Immettere l'URL del file e specificare un nome per l'allegato.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Membri

+++ **[!UICONTROL Assegnare un membro a una bacheca]**

Vedere &quot;[!UICONTROL Assegnare un membro a una bacheca]&quot; [Schede](#boards).

+++

+++ **[!UICONTROL Annullare l&#39;assegnazione di un membro da una bacheca]**

Vedere &quot;[!UICONTROL Annullare l&#39;assegnazione di un membro da una bacheca]&quot; [Schede](#boards).

+++

+++ **[!UICONTROL Aggiungi un membro a una scheda]**

Questo modulo di azione aggiunge il membro specificato alla scheda specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserisci ID scheda e ID membro]</p> </td> 
   <td> <p>Scegli come inserire l'ID della scheda e l'ID membro.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Card ID]</strong> e <strong>[!UICONTROL Member ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca contenente la scheda a cui desiderate aggiungere un membro, quindi selezionate l'elenco che contiene la scheda, la scheda stessa e il membro che desiderate aggiungere alla scheda.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Cerca membri]**

Questo modulo di azione recupera informazioni su [!UICONTROL Trello] membri.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query [!UICONTROL] </td> 
   <td> <p>Immettere il nome utente o il nome utente completo dell'utente che si desidera trovare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parziale] </td> 
   <td> <p>Per impostazione predefinita, questo modulo cerca nel contenuto membro le corrispondenze esatte di ogni parola nella query. Quando [!UICONTROL Partial] è abilitato, il modulo cerca il contenuto che inizia con qualsiasi parola nella query.</p> <p> Ad esempio, se utilizzi la parola "sviluppo" per cercare una bacheca intitolata "Report sullo stato di sviluppo", per impostazione predefinita dovrai cercare l'intera parola. Se hai [!UICONTROL Partial] abilitato, puoi cercare "dev" ma non "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di membri restituiti]</td> 
   <td> <p> Numero massimo di membri [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Elenchi di controllo

+++ **[!UICONTROL Creare una checklist]**

Questo modulo di azione crea una checklist sulla scheda selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID scheda]</td> 
   <td> <p> Seleziona l’ID della scheda in cui desideri aggiungere una lista di controllo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere una checklist.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere una lista di controllo, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere o mappare un nome per la checklist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleziona se desideri aggiungere la checklist all’inizio o aggiungere la checklist alla parte inferiore della scheda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserisci ID checklist]</p> </td> 
   <td> <p>Immettere o mappare l'ID di una checklist sorgente che si desidera copiare in quella nuova.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crea un elemento della lista di controllo]**

Questo modulo di azione aggiunge un elemento a una checklist specifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci ID checklist]</td> 
   <td> <p> Selezionare la modalità di immissione dell'ID della lista di controllo in cui si desidera aggiungere un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>ID checklist [!UICONTROL]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere una checklist.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere una lista di controllo, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda, quindi selezionate la lista di controllo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nome elemento]</p> </td> 
   <td> <p>Immettere o mappare un nome per il nuovo elemento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Seleziona se desideri aggiungere l’elemento in alto o in basso nella lista di controllo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Controllato]</p> </td> 
   <td> <p>Abilita questa opzione se desideri aggiungere l’elemento come già selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modificare un elemento della lista di controllo]**

Questo modulo di azione modifica una checklist esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID scheda e un ID elemento checklist]</td> 
   <td> <p> Seleziona l'ID della scheda e la lista di controllo in cui desideri modificare un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>ID checklist [!UICONTROL]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere una checklist.</p> <p>In <strong>[!UICONTROL ID elemento lista di controllo]</strong> immetti o mappa l’ID della checklist.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere una lista di controllo, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda, quindi selezionate la lista di controllo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID checklist [!UICONTROL]</td> 
   <td>Selezionare o mappare la lista di controllo a cui si desidera spostare la voce di elenco.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nome elemento]</p> </td> 
   <td> <p>Immettere o mappare un nome per il nuovo elemento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Seleziona se desideri aggiungere l’elemento in alto o in basso nella lista di controllo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Seleziona se la voce della lista di controllo è completa o incompleta.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Etichette

+++ **[!UICONTROL Aggiungere un’etichetta a una scheda]**

Questo modulo di azione aggiunge un’etichetta a una scheda selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti l'ID della scheda]</td> 
   <td> <p> Seleziona l’ID della scheda in cui desideri aggiungere una lista di controllo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere una checklist. In<strong>[!UICONTROL Label ID]</strong> immetti o mappa l’ID dell’etichetta da aggiungere.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere una lista di controllo, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda. </p> <p>Seleziona l’etichetta da aggiungere alla scheda.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Commenti

+++ **[!UICONTROL Osserva commenti]**

Recupera i dettagli del commento quando c&#39;è un nuovo commento in una posizione specifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Oggetto guardato]</td> 
   <td> <p>Selezionare la posizione in cui si desidera visualizzare i commenti.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tutte le schede] ovunque</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Selezionate la bacheca da guardare per i commenti</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Selezionate la bacheca che contiene l'elenco da cercare per i commenti, quindi selezionate l'elenco.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Selezionate la bacheca che contiene la scheda che desiderate controllare per i commenti, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Numero massimo di osservazioni [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Creare un commento in una scheda]**

Questo modulo di azione aggiunge un commento a una scheda selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID scheda]</td> 
   <td> <p> Seleziona l’ID della scheda in cui desideri aggiungere un commento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere un commento.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere un commento, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commento] </td> 
   <td> <p>Inserite il commento da aggiungere alla scheda selezionata.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Elencare commenti in una scheda]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Trello] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID scheda]</td> 
   <td> <p> Seleziona l’ID della scheda in cui desideri aggiungere un commento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>In <strong>[!UICONTROL Card ID]</strong> immetti o mappa l’ID della scheda in cui desideri aggiungere un commento.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Selezionate la bacheca che contiene la scheda in cui desiderate aggiungere un commento, quindi selezionate l'elenco che contiene la scheda, quindi selezionate la scheda.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di commenti restituiti]</td> 
   <td> <p> Immettere il numero massimo di commenti [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da] </td> 
   <td> <p>Imposta la data di inizio del periodo in cui è stato creato il commento. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prima] </td> 
   <td> <p>Imposta la data di fine del periodo in cui è stato creato il commento. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] ID oggetto

* [Come trovare l’ID o il collegamento rapido di una scheda in [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Come trovare gli ID di altri oggetti in [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Come trovare l’ID o il collegamento rapido di una scheda in [!DNL Trello]

Per modificare una scheda o creare un nuovo commento, è necessario conoscere l&#39;ID della scheda o il relativo collegamento diretto. Puoi ottenere queste informazioni dall’output del [!UICONTROL Nuova scheda] attivatore. Il collegamento rapido per una scheda può essere ottenuto anche aprendo la scheda e cliccando sul [!UICONTROL Condividi] pulsante . Il collegamento rapido è disponibile nella sezione [!UICONTROL Collegamento a questa scheda] alla fine dell’URL dopo `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Come trovare gli ID di altri oggetti in [!DNL Trello]

Gli ID di bacheca, elenco e commenti possono essere ottenuti solo utilizzando i trigger. La [!DNL trello.com] Il sito web non mostra questi ID.
