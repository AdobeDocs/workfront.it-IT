---
content-type: api
navigation-topic: general-api
title: Controllo delle versioni delle sottoscrizioni agli eventi
description: API di abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 82694183c32938905f1f8542c430d3c453274cb6
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# Controllo delle versioni delle sottoscrizioni agli eventi

In Workfront sono disponibili due versioni delle sottoscrizioni di eventi. Questo articolo descrive le differenze tra di essi.

La nuova versione non è una modifica all’API Workfront, ma piuttosto una modifica alla funzionalità di abbonamento agli eventi.

La possibilità di aggiornare o effettuare il downgrade degli abbonamenti agli eventi assicura che, quando vengono apportate modifiche alla struttura degli eventi, gli abbonamenti esistenti non si interrompano, consentendo di testare e aggiornare alla nuova versione senza interruzioni nell’abbonamento agli eventi.


Quando aggiorni o esegui il downgrade dell’abbonamento a un’altra versione, ricevi eventi duplicati per ogni consegna di eventi per una finestra di cinque minuti dopo la modifica della versione. I duplicati includono uno per ogni abbonamento all’evento versione 1 e versione 2. In questo modo non si perde nessun evento a causa della modifica della versione dell’abbonamento all’evento.

Per informazioni sugli endpoint utilizzati per l&#39;aggiornamento o il downgrade delle sottoscrizioni di eventi, vedere [Controllo delle versioni delle sottoscrizioni di eventi](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) nell&#39;articolo API delle sottoscrizioni di eventi.

>[!IMPORTANT]
>
>Le seguenti versioni influiranno sul controllo delle versioni delle sottoscrizioni agli eventi:
>
>* **Versione 25.2** (10 aprile 2025): tutte le nuove sottoscrizioni create dopo la versione 25.2 vengono create come versione 2.
>* **Versione 25.3** (17 luglio 2025): non è più possibile effettuare il downgrade delle sottoscrizioni alla versione 1 dopo la versione 25.3.
>* **1 settembre 2025**: tutte le sottoscrizioni della versione 1 rimanenti sono state migrate alla versione 2.

## Modifiche tra versione 1 e versione 2

Sono state apportate le seguenti modifiche per le sottoscrizioni di eventi versione 2:


### Modifiche generali


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Campi interessati</b></p> </th> 
   <th> <p><b>Versione 1 (comportamento precedente)</b></p> </th> 
   <th> <p><b>Versione 2 (modifica)</b></p> </th> 
   <th> <p><b>Azione di risoluzione</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Valori dei parametri</p> </td> 
   <td> <p>Per qualsiasi oggetto creato da un modello che include un modulo personalizzato, è stato inviato un evento <code>CREATE</code>, quindi è stato inviato un <code>UPDATE</code> con i valori dei parametri (inclusi i campi calcolati e i relativi valori).    </p> </td> 
   <td> <p>Quando un oggetto viene creato da un modello che include un modulo personalizzato con valori dei parametri calcolati, verrà inviato solo un evento <code>CREATE</code> che conterrà i valori dei parametri, inclusi i campi calcolati.</p> </td> 
   <td> <p>Se disponi di un abbonamento per <tr><ul><ul><code>UPDATE<code> events and are expecting to receive an <code>UPDATE</code> event after an object is created with calculated parameter values, you will no longer receive that <code>UPDATE</code> event. If you wish to see calculated parameter values on object creation, you must create an additional <code>CREATE</code> subscription.</p> </td> 
  </tr> 
   
   <td> <p>Multi-Select type fields</p> </td> 
   <td> <p>For any type of event that contains a change on a multi-select type field, if the field only contained one value it would be converted to and sent as a string. Otherwise it would be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is converted and sent as <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Regardless of how many values are in the array, it will be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is sent as <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>If you have a subscription with a filter on a multi-select field, and the value as a string, you must create a new subscription with the same filter that has the value as an array. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Modifiche specifiche dell&#39;oggetto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Codice oggetto</b> </th> 
   <th> <b>Campi interessati</b> </th> 
   <th> <b>Versione 1 (comportamento precedente)</b></th> 
   <th> <b>Versione 2 (Modifica)</b> </th> 
   <th> <b>Azione di risoluzione</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSEGNA</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Quando l'oggetto è stato aggiornato, l'evento <code>UPDATE</code> a volte mostrava in modo errato che i campi interessati cambiavano da <code>null</code> a <code>ID value</code>.</td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per i campi interessati.</td> 
   <td>Nessuno. Se disponi di un filtro per i campi interessati, riceverai un evento <code>UPDATE</code> solo se questi campi sono stati effettivamente modificati, non se è stato modificato un altro valore.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Quando un valore di parametro è stato aggiornato in questo oggetto, l'evento <code>UPDATE</code> ha mostrato erroneamente che il campo interessato è cambiato da <code>null</code> a <code>object id</code>. </td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per i campi interessati.</td> 
   <td>Nessuno. Se disponi di un filtro per i campi interessati, riceverai un evento <code>UPDATE</code> solo se questi campi sono stati effettivamente modificati, non se è stato modificato un altro valore.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Quando un documento è stato eliminato, l'evento <code>DELETE</code> mostrava erroneamente il campo interessato come una matrice vuota nello stato prima.    </td> 
   <td>L'evento <code>DELETE</code> mostra correttamente il campo interessato nello stato prima.</td> 
   <td>Nessuno. L'evento <code>DELETE</code> verrà comunque inviato, ma ora mostra i dati corretti per il campo interessato. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Quando questo oggetto viene aggiornato, vengono inviati due eventi <code>UPDATE</code>. Il primo non includeva i campi interessati, mentre il secondo evento sì.</td> 
   <td>Tutti gli aggiornamenti dei campi, inclusi i campi interessati, sono presenti in un solo evento <code>UPDATE</code> e non viene inviato un secondo evento non necessario.     </td> 
   <td>Nessuno. Se disponi di un filtro per i campi interessati, gli eventi vengono consegnati nel primo evento. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Quando un valore di parametro è stato aggiornato in una Spesa, l'evento <code>UPDATE</code> mostrava erroneamente la modifica di topReferenceObjCode da <code>EXPNS</code> a <code>PROJ</code> e la modifica di <code>referenceObjectName</code> da <code>null</code> a <code>string value of project name</code>.      </td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per i campi interessati.</td> 
   <td>Nessuno. Se disponi di un filtro per i campi interessati, riceverai un evento <code>UPDATE</code> solo se questi campi sono stati effettivamente modificati, non se è stato modificato un altro valore.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Quando un oggetto Expense è stato eliminato, è stato inviato un evento <code>UPDATE</code> modificando i campi interessati in null prima dell'invio dell'evento <code>DELETE</code>.    </td> 
   <td>L'evento <code>UPDATE</code> aggiuntivo non viene inviato. L'evento <code>DELETE</code> contiene valori corretti per i campi interessati nello stato prima. </td> 
   <td>Se si dispone di un filtro per i campi interessati sugli eventi <code>UPDATE</code> e si prevede di riceverlo quando l'oggetto viene eliminato, l'evento <code>UPDATE</code> non verrà più ricevuto. Se si desidera visualizzare questi campi quando l'oggetto viene eliminato, è necessario creare una sottoscrizione <code>DELETE</code> aggiuntiva.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Quando l'oggetto è stato eliminato, l'evento <code>DELETE</code> mostrava erroneamente i campi interessati come <code>null</code> nello stato prima. </td> 
   <td>L'evento <code>DELETE</code> mostra correttamente i campi interessati nello stato prima.</td> 
   <td>Nessuno. L'evento <code>DELETE</code> è ancora inviato, ma ora mostra i dati corretti per i campi interessati. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Quando un valore di parametro è stato aggiornato in questo oggetto, l'evento <code>UPDATE</code> ha mostrato erroneamente che il campo interessato è cambiato da <code>null</code> a <code>ID value</code>. </td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per il campo interessato.</td> 
   <td>Nessuno. Se disponi di un filtro per il campo interessato, riceverai un evento <code>UPDATE</code> solo se tale campo è stato effettivamente modificato, non se è stato modificato un altro valore di parametro.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Quando l'oggetto è stato aggiornato, l'evento <code>UPDATE</code> a volte mostrava in modo errato che i campi interessati cambiavano da <code>null</code> a <code>ID value</code>.</td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostreranno il valore corretto per i campi interessati.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Quando un valore di parametro è stato aggiornato in questo oggetto, l'evento <code>UPDATE</code> ha mostrato erroneamente che il campo interessato è cambiato da <code>null</code> a <code>ID value</code>. </td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per il campo interessato.</td> 
   <td>Nessuno. Se disponi di un filtro per il campo interessato, riceverai un evento <code>UPDATE</code> solo se tale campo è stato effettivamente modificato, non se è stato modificato un altro valore di parametro.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Quando l'oggetto è stato aggiornato, l'evento <code>UPDATE</code> a volte mostrava in modo errato che i campi interessati cambiavano da <code>null</code> a <code>ID value</code>.</td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per il campo interessato.</td> 
   <td>Nessuno. Se disponi di un filtro per il campo interessato, riceverai un evento <code>UPDATE</code> solo se tale campo è stato effettivamente modificato, non se è stato modificato un altro valore di parametro.
  </tr> 
  <tr> 
   <th rowspan="2">ATTIVITÀ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Quando un valore di parametro è stato aggiornato in questo oggetto, l'evento <code>UPDATE</code> ha mostrato erroneamente che il campo interessato è cambiato da <code>null</code> a <code>ID value</code>. </td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per il campo interessato.</td> 
   <td>Nessuno. Se disponi di un filtro per il campo interessato, riceverai un evento <code>UPDATE</code> solo se tale campo è stato effettivamente modificato, non se è stato modificato un altro valore di parametro.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Quando l'oggetto è stato aggiornato, l'evento <code>UPDATE</code> a volte mostrava in modo errato che i campi interessati cambiavano da <code>null</code> a <code>ID value</code>.</td> 
   <td>Tutti gli eventi <code>UPDATE</code> mostrano il valore corretto per il campo interessato.</td> 
   <td>Nessuno. Se disponi di un filtro per il campo interessato, riceverai un evento <code>UPDATE</code> solo se tale campo è stato effettivamente modificato, non se è stato modificato un altro valore di parametro.
 </tbody> 
</table>


## Aggiornare la versione della sottoscrizione dell’evento in uno scenario Workfront Fusion

Workfront Fusion utilizza gli abbonamenti agli eventi per controllare le modifiche in Workfront per attivare gli scenari. Puoi aggiornare la versione della sottoscrizione dell’evento utilizzata direttamente da Fusion in uno scenario, utilizzando il modulo Workfront > Aggiorna versione payload eventi.

Per istruzioni sull&#39;utilizzo di questo modulo, vedere [Moduli Workfront](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) nella documentazione di Workfront Fusion.
