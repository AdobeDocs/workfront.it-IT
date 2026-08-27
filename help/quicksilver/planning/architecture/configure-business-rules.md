---
title: Configura regole business di tipo record
description: È possibile configurare regole business di tipo record che definiscono il modo in cui i record di quel tipo vengono gestiti in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 31db7a4ef190793558bcb2fa10beb2585e1068e4
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 1%

---


# Configurare le regole business di tipo record

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

È possibile configurare regole business di tipo record che definiscono il modo in cui i record di quel tipo vengono gestiti in Adobe Workfront Planning.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per eseguire i passaggi descritti in questo articolo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p></li>
Oppure
<li><p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard flusso di lavoro</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard di pianificazione</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro e per un tipo di record</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la configurazione delle regole aziendali

* È possibile configurare le regole per la modifica o l&#39;eliminazione dei record, a seconda delle condizioni definite.

  Ad esempio, puoi creare le condizioni per richiedere che alcuni campi abbiano un valore. Se il valore non è presente in tali campi, gli utenti non possono modificare o eliminare tale record.
* Non è possibile aggiungere regole business ai tipi di record globali nelle aree di lavoro principali o secondarie.
* Non è possibile configurare regole per la creazione dei record. Tutti coloro che dispongono delle autorizzazioni Gestione per il tipo di record possono creare record.
* È possibile creare una condizione per la regola business che faccia riferimento a tutti i tipi di campo ad eccezione dei seguenti:
  * Campi formula
  * Campi di ricerca
  * Campi di riferimento

## Configurare le regole business

1. Passare a un tipo di record.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su Regole aziendali.


*********** DA CLAUDE - SOTTO - DEVE MODIFICARE *******************

## Impostazione delle regole business in Workfront Planning: Guida dettagliata

Hai mai registrato il passaggio a &quot;Pronto per l’esecuzione&quot; solo per scoprire in seguito che metà dei campi richiesti — Marchio, Indicazione, Date di lancio — non sono mai stati compilati? Quando qualcuno se ne accorge, c&#39;è già un progetto a valle con dati mancanti, e qualcuno deve rintracciare i dettagli e compilarli a mano.

Le regole business correggono questo problema. Consentono di impostare un punto di controllo semplice: **prima che un record possa passare a uno stato specifico, è necessario compilare alcuni campi.** In caso contrario, la persona che apporta la modifica vedrà esattamente ciò che manca e non potrà procedere finché non sarà stato risolto.

Questa guida illustra le funzioni delle regole aziendali, come configurarne una e cosa sperimenterà il team una volta live.

### Quali sono le operazioni effettive delle regole aziendali?

Le regole business associano una condizione a una **modifica stato**. Invece di imporre dati completi nel momento in cui qualcuno crea un record (che rallenterebbe tutti), la regola viene attivata solo in un momento specifico e deliberato: quando uno stato sta per cambiare in uno stato configurato.

Una regola si presenta così in un linguaggio semplice:

> &quot;Prima che un record possa essere spostato in **Pronto per l&#39;esecuzione**, il campo **Marchio** deve avere un valore.&quot;

Se il campo è vuoto, la modifica dello stato viene bloccata e la persona riceve un messaggio chiaro che indica cosa correggere. Una volta compilato e riprovato, la modifica viene completata.

Alcuni aspetti importanti sono *non*:

* **Non blocca la creazione del record.** Le persone possono ancora creare un nuovo record all&#39;istante e compilarlo nel tempo, esattamente come oggi.
* **Non compila automaticamente nulla né cambia automaticamente lo stato.** Una persona deve sempre effettuare il cambiamento di stato autonomamente.
* **Non contrassegna retroattivamente i record precedenti.** I record già presenti nello stato di destinazione non vengono interessati. Il controllo viene eseguito solo alla successiva esecuzione di un tentativo di spostamento di un record *in* tale stato.



### Prima di iniziare

Un paio di cose devono essere vere prima di poter configurare le regole:

1. **La funzionalità deve essere attivata per la tua organizzazione.** Questa operazione viene eseguita dal lato di Adobe (tramite un flag di funzione), non da te stesso abilitato. Se non vedi la sezione delle regole business descritta di seguito, verifica con il tuo contatto Adobe che sia stato abilitato per il tenant.
2. **Sono necessarie autorizzazioni di amministratore o configuratore area di lavoro.** I pianificatori regolari non possono creare o modificare regole, ma solo le persone che gestiscono la configurazione dell&#39;area di lavoro.

### Passaggio 1: aprire l&#39;area di configurazione delle regole business

Le regole business vivono insieme alle altre impostazioni dell&#39;amministratore, non sarà necessario ricercare un pannello &quot;Pianificazione&quot; separato. Dall’area di configurazione del flusso di lavoro:

1. Vai all&#39;area principale **configurazione flusso di lavoro / configurazione amministratore** per il tuo workspace.
2. Cercare nella sezione **regole business** il tipo di record che si desidera configurare, ad esempio &quot;Materiali&quot; o &quot;Campagne&quot;.


### Passaggio 2: scegliere il tipo di record

Le regole sono configurate per tipo di record, quindi scegliere quello a cui si desidera aggiungere una regola. Ad esempio, se si desidera assicurarsi che in ogni record Materiali siano presenti campi chiave compilati prima dell&#39;esecuzione, selezionare **Materiali**.



### Passaggio 3: creare una nuova regola

Per ogni regola, puoi specificare tre elementi:

| Impostazioni | Esempio |
|---|---|
| **Tipo di record** | Materiali |
| **Stato destinazione** | Pronto per l’esecuzione |
| **Campo obbligatorio** | Brand |

In altre parole: &quot;Quando lo stato di un record Materiali viene modificato in **Pronto per l&#39;esecuzione**, il campo **Marchio** deve avere un valore.&quot;

È possibile aggiungere più regole per lo stesso stato. Ad esempio, potrebbe essere necessario compilare tutti i campi Marchio, Area terapeutica, Indicazione e Data di lancio stimata prima che un record possa essere spostato in &quot;Pronto per l’esecuzione&quot;, ognuno secondo la propria regola, e tutti devono essere controllati insieme.

**Quali campi è possibile richiedere?**
- Campi record collegati (ad esempio, un record Marchio o Indicazione collegato): la regola viene superata non appena viene collegato almeno un record.
- Campi di testo standard (riga singola o paragrafo): la regola viene passata una volta che è presente un valore.
- Campi data: la regola viene superata una volta impostata una data.

**Cosa non è ancora possibile utilizzare:** i campi formula e i campi di ricerca non sono supportati come destinazioni delle regole in questa versione, in quanto vengono calcolati in background anziché essere compilati direttamente da una persona.

### Passaggio 4: scrivi il messaggio che verrà visualizzato dagli utenti

Quando crei una regola, fornisci anche il messaggio che compare se qualcuno tenta di apportare la modifica senza compilare il campo. Mantieni il messaggio specifico e actionable, ad esempio:

> &quot;Il marchio è obbligatorio&quot;.

Non devi preoccuparti di formattare un intero banner di errore: il sistema gestisce la combinazione di messaggi se vengono violate più regole contemporaneamente (vedi sotto).

### Passaggio 5: salvare la regola

Una volta salvata, la regola entra in vigore **immediatamente** per tutti gli utenti dell&#39;area di lavoro, senza dover disconnettersi, aggiornare o attendere una distribuzione. La volta successiva in cui si tenta di spostare un record in tale stato, la regola viene controllata.

### Esperienza effettiva del team

Ecco cosa cambia per le persone che usano Planning giorno per giorno, una volta che una regola è attiva.

#### Se un campo obbligatorio è vuoto

1. Un planner apre un record e modifica lo stato in &quot;Gated&quot; (ad esempio, &quot;Pronto per l’esecuzione&quot;).
2. Il sistema controlla tutte le regole associate a tale stato.
3. Se un campo obbligatorio è vuoto, la modifica è **rifiutata**. Lo stato torna allo stato originale.
4. Viene visualizzato un messaggio con i nomi dei campi mancanti:
   > *&quot;Modifica dello stato bloccata: è necessario popolare &#39;Brand&#39; e &#39;Estimated Launch Date&#39; prima di passare a &#39;Ready for Execution&#39;.&quot;*
5. Il planner compila i campi mancanti e prova a cambiare di nuovo lo stato.
6. Questa volta, la regola viene superata e lo stato viene aggiornato normalmente.

#### Se è già stato compilato tutto

Non cambia nulla. Lo stato viene aggiornato immediatamente, senza passaggi o pop-up aggiuntivi. Le regole di business sono invisibili finché non sono effettivamente necessarie.

#### Se mancano più campi contemporaneamente

Tutte le regole violate vengono verificate insieme e il messaggio elenca tutti i campi mancanti in una sola volta: i responsabili della pianificazione non devono correggere un campo, riprovare, ricevere informazioni sul successivo e ripetere.

### Passaggio 6: modificare o rimuovere una regola in un secondo momento

Le regole non sono fissate sulla pietra. Per apportare modifiche:

1. Tornare all&#39;area di configurazione delle regole business per il tipo di record.
2. Individuare la regola che si desidera modificare.
3. Modificare il campo, lo stato di destinazione o il messaggio richiesto oppure eliminare completamente la regola.
4. Salva. La modifica viene applicata immediatamente alle modifiche di stato future.

Nota: la modifica o l&#39;eliminazione di una regola **influisce solo sulle transizioni future.** I record che hanno già raggiunto lo stato target prima della modifica non vengono rivalutati.
3## Alcune informazioni utili

* **I record vengono bloccati separatamente dopo un cambiamento di stato.** Le regole business (come descritto qui) controllano solo la completezza del campo *prima* che venga eseguita una modifica dello stato. Un&#39;altra caratteristica correlata determina se un record viene completamente bloccato dalle modifiche o dall&#39;eliminazione una volta raggiunto un determinato stato. Questa caratteristica non è inclusa in questa sezione.
* **Le modifiche di stato in blocco** (modifica dello stato di molti record contemporaneamente) non sono ancora completamente definite per il modo in cui interagiscono con le regole aziendali. Se il team si basa in larga misura su azioni in blocco, verifica il comportamento corrente con il contatto Adobe.
* **Se una regola non può essere valutata** a causa di un errore di sistema, la transizione viene bloccata anziché essere consentita in modo invisibile all&#39;utente. Un record incompleto non verrà mai superato a causa di un problema di back-end.
* **La disattivazione della funzionalità** non comporta l&#39;eliminazione delle regole configurate, ma solo la loro sospensione. Riattivandole, le ripristina esattamente come erano, senza bisogno di riconfigurazione.

### Riferimento rapido: impostazione della prima regola

1. Conferma che la funzione sia abilitata per il tenant.
2. Passare alla configurazione del flusso di lavoro → regole business per il tipo di record.
3. Scegliere il tipo di record, ad esempio Materiali.
4. Crea una regola: stato target + campo obbligatorio.
5. Scrivi un messaggio di errore chiaro e specifico.
6. Salva — è subito in diretta.
7. Ripetere l&#39;operazione per ogni campo desiderato.
8. Verifica da solo: prova a modificare lo stato di un record con il campo vuoto, conferma che venga visualizzato il messaggio previsto, compila il campo e conferma che la modifica dello stato sia stata completata.

Tutto qui. Da qui in poi, chiunque converta un documento in avanti riceverà un chiaro segnale se qualcosa manca, invece di un progetto a valle che appare incompleto.