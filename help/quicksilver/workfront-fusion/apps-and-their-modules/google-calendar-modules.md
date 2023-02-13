---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Google Calendar
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Google Calendar, nonché collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Calendario Google], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Google Calendar] moduli, è necessario disporre di un [!DNL Google] conto.

## [!DNL Google Calendar] moduli e relativi campi

Quando si configura [!DNL Google Calendar] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Calendar] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Eventi](#events)
* [Calendari](#calendars)
* [Regole di controllo accessi](#access-control-rules)
* [Iteratori (obsoleti)](#iterators-deprecated)
* [Altro](#other)

### Eventi

* [[!UICONTROL Eventi di controllo]](#watch-events)
* [[!UICONTROL Eventi di ricerca]](#search-events)
* [[!UICONTROL Ottieni un evento]](#get-an-event)
* [[!UICONTROL Creare un evento]](#create-an-event)
* [[!UICONTROL Aggiornare un evento]](#update-an-event)
* [[!UICONTROL Eliminare un evento]](#delete-an-event)


#### [!UICONTROL Eventi di controllo]

Questo modulo trigger esegue uno scenario quando un nuovo evento viene aggiunto, aggiornato, eliminato, avviato o terminato nel calendario specificato. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Calendario [!UICONTROL] </td> 
   <td> <p>Selezionare il calendario con cui si desidera utilizzare il modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>Scegliere se visualizzare gli eventi per Data creazione, Data aggiornamento, Data inizio o Data fine.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostra eventi eliminati]</td> 
   <td> <p>Abilita questa opzione per includere gli eventi eliminati.</p> </td> 
  </tr> 
  <tr> 
   <td>Query [!UICONTROL] </td> 
   <td> <p>Immettere il testo da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Imposta il numero massimo di eventi che [!DNL Workfront Fusion] funziona con durante un ciclo (il numero di ripetizioni per esecuzione di scenari). Se il valore è impostato su un valore troppo alto, la connessione potrebbe essere interrotta sul lato del servizio di terze parti specificato (timeout). [!DNL Workfront Fusion] non ha alcuna influenza su questo. È consigliabile impostare un valore più basso e definire un valore più alto per il numero massimo di cicli oppure eseguire lo scenario con maggiore frequenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventi di ricerca]

Questo modulo di azione cerca un evento nel calendario selezionato.

È possibile specificare il calendario e i parametri della ricerca.

Il modulo restituisce l’ID dell’evento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come collegare le [!DNL Google Calendar] account a Workfront Fusion, vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe Workfront Fusion - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di inizio]</td> 
   <td> <p> Immettere o mappare la data di inizio dell'evento. Questo modulo recupera anche gli eventi che iniziano prima di questa data, che si verificano ancora nella data di inizio immessa. </p> <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di fine]</td> 
   <td> <p> Immetti o mappa la data alla fine dell’evento. </p> <p> Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eventi singoli]</td> 
   <td> <p> Abilita questa opzione per trattare gli eventi ricorrenti come istanze singole. Ad esempio, se disponi di una riunione settimanale e questa opzione è abilitata, il modulo restituisce la riunione di ogni settimana come evento separato.</p> </td> 
  </tr> 
  <tr> 
   <td>Query [!UICONTROL]</td> 
   <td> <p>Immetti o mappa il termine di ricerca per cui desideri eseguire la ricerca. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona l’ordine degli eventi restituiti nel risultato.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Time]</strong>: Ordina per data e ora di inizio (crescente). Questa opzione è disponibile solo quando si esegue una query su singoli eventi.</li> 
     <li><strong>[!UICONTROL Aggiornato]</strong>: Ordina per ultima modifica (crescente).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Imposta il numero massimo di eventi [!DNL Workfront Fusion] restituisce durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un evento]

Questo modulo di azione restituisce i metadati per un singolo evento nel calendario specificato.

Specificare il calendario e l&#39;evento.

Il modulo restituisce l’ID dell’evento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Immetti o mappa l’ID del calendario contenente l’evento che desideri ottenere.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID evento] </td> 
   <td> <p>Immetti l’ID evento del [!DNL Google Calendar] evento che si desidera ottenere.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un evento]

Questo modulo di azione crea un evento.

Puoi specificare il calendario e i parametri dell’evento.

Il modulo restituisce l’ID dell’evento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come collegare le [!DNL Google Calendar] account a Workfront Fusion, vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe Workfront Fusion - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Creare un evento]</td> 
   <td> <p>Seleziona la modalità di creazione dell’evento.</p> 
    <ul> 
     <li><b>[!UICONTROL In Dettaglio]</b><p>Questa opzione ti consente di fornire maggiori dettagli sull’evento.<br></p></li> 
     <li><b>[!UICONTROL Rapido]</b><p>È sufficiente selezionare il calendario e inserire un nome per l’evento. È possibile includere nel nome i dettagli relativi all’ora e al luogo, e [!DNL Google Calendar] pianificherà l'evento per quel luogo e quell'ora.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario in cui si desidera visualizzare l’evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Seleziona il colore che l'evento mostra sul calendario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome evento]</td> 
   <td> <p> Inserisci o mappa un nome per l’evento. </p> <p>Nota: Se hai selezionato [!UICONTROL Quick add] nel campo [!UICONTROL Crea un evento], puoi includere la data e l’ora dell’evento e [!DNL Workfront Fusion] crea l’evento per la data e l’ora specificate. Esempio: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Se hai selezionato [!UICONTROL Quick add] ma non includi una data e un’ora nel nome dell’evento, l’evento viene creato a partire dall’ora corrente e dura un’ora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>Abilita questa opzione se l’evento è un evento di tutto il giorno (non richiede l’ora di inizio e di fine).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di inizio]</td> 
   <td> <p>Se si tratta di un evento di tutto il giorno, immetti la data di inizio dell’evento. </p> <p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di fine]</td> 
   <td> <p> Se si tratta di un evento di tutto il giorno, immetti la data di fine dell’evento. </p> <p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descrizione]</td> 
   <td>Immetti o mappa una descrizione dell’evento. Questo campo supporta HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>Immettere una posizione per l'evento nel modulo di testo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizza le impostazioni predefinite per i promemoria per questo evento]</td> 
   <td>Abilita questa opzione per utilizzare le impostazioni predefinite per i promemoria. Se imposti un promemoria personalizzato nel campo Promemoria [!UICONTROL] , questo valore viene impostato su No.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Promemoria] </td> 
   <td> <p>Aggiungi un promemoria per l’evento. Per ogni promemoria, seleziona il metodo con cui vuoi ricevere un promemoria e definisci per quanto tempo (in minuti) prima dell’evento a cui desideri inviare il promemoria.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Partecipanti]</td> 
   <td>Aggiungi i partecipanti all’evento. Per ogni partecipante, immetti o mappa il proprio nome e indirizzo e-mail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostra come]</td> 
   <td>Selezionare se si desidera che gli utenti che visualizzano il calendario visualizzino l'utente come Occupato o Disponibile durante questo evento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>Selezionare la visibilità dell'evento. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Predefinito]</b></p> <p>L’evento ha la visibilità impostata nelle impostazioni del calendario.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Questo evento è visibile a tutti gli utenti con cui è condiviso il calendario.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Solo i partecipanti possono vedere questo evento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Invia notifica sulla creazione dell’evento]</td> 
   <td> <p>Seleziona se inviare notifiche sulla creazione di un nuovo evento a tutti gli ospiti, a non-[!DNL Google Calendar] o a nessuno.</p> <p>Suggerimento: È consigliabile utilizzare l’opzione [!UICONTROL None] solo per i casi di utilizzo della migrazione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gli ospiti possono modificare l’evento]</td> 
   <td> <p>Abilita questa opzione se desideri che gli ospiti siano in grado di modificare questo evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ricorrenza]</td> 
   <td>Aggiungi eventuali regole di ricorrenza da applicare a questo evento. Ogni regola richiede un elenco di righe [!UICONTROL Rrule], [!UICONTROL EXPORT], [!UICONTROL RDATE] e [!UICONTROL EXDATE] per un evento ricorrente. Tieni presente che le righe [!UICONTROL DTSTART] e [!UICONTROL DTEND] non sono consentite in questo campo; l’ora di inizio e di fine dell’evento è specificata nei campi start e end. Questo campo viene omesso per eventi singoli o per istanze di eventi ricorrenti. Per ulteriori informazioni, consulta <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un evento]

Questo modulo di azione modifica un evento esistente.

Specifica il calendario e l’ID evento.

Il modulo restituisce l’ID dell’evento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Calendario [!UICONTROL] </td> 
   <td> <p>Selezionare il calendario con cui si desidera lavorare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID evento] </td> 
   <td> <p>Immetti l’ID evento dal creato in precedenza [!DNL Google Calendar] evento che si desidera aggiornare.</p> </td> 
  </tr> 
 </tbody> 
</table>

È possibile aggiornare le informazioni sull’evento immettendo nuovi valori nel campo desiderato. Per informazioni dettagliate sui singoli campi, consulta [[!UICONTROL Creare un evento]](#create-an-event).

#### [!UICONTROL Eliminare un evento]

Questo modulo di azione elimina un evento.

Specifica il calendario e l’ID evento.

Il modulo restituisce l’ID dell’evento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario contenente l’evento da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID evento]</td> 
   <td> <p> Immetti l’ID evento da un creato in precedenza [!DNL Google Calendar] evento da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Invia notifica relativa all’eliminazione dell’evento]</td> 
   <td>Seleziona se desideri inviare notifiche sull’eliminazione dell’evento a tutti gli ospiti, ospiti che non utilizzano [!DNL Google Calendar]o nessuno.</td> 
  </tr> 
 </tbody> 
</table>

### Calendari

* [[!UICONTROL Elencare calendari]](#list-calendars)
* [[!UICONTROL Ottieni un calendario]](#get-a-calendar)
* [[!UICONTROL Crea un calendario]](#create-a-calendar)
* [[!UICONTROL Aggiornare un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminare un calendario]](#delete-a-calendar)
* [[!UICONTROL Cancella un calendario]](#clear-a-calendar)

#### [!UICONTROL Elencare calendari]

Questo modulo di azione restituisce i calendari nell&#39;elenco del calendario di un utente.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruolo di accesso minimo]</td> 
   <td> <p>Selezionare il ruolo di accesso minimo per l'utente. Il modulo restituisce i calendari in base a questo ruolo di accesso minimo.</p> 
    <ul> 
     <li><strong>[!UICONTROL Reader disponibilità libero]</strong>: L'utente può leggere informazioni sulla disponibilità. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: L’utente può leggere e modificare gli eventi e accedere agli elenchi di controllo. </li> 
     <li><strong>Reader [!UICONTROL]</strong>: L’utente può leggere eventi non privati. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utente può leggere e modificare gli eventi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra calendari nascosti]</td> 
   <td>Abilita questa opzione per includere i calendari nascosti nell’elenco restituito dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Imposta il numero massimo di calendari [!DNL Workfront Fusion] restituisce durante un ciclo di esecuzione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un calendario]

Questo modulo di azione recupera un calendario.

Specifica l&#39;ID del calendario da recuperare.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario da recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea un calendario]

Questo modulo di azione crea un nuovo calendario.

Specificare un nome per il calendario.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome calendario]</td> 
   <td> <p> Immettere un nome per il nuovo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un calendario]

Questo modulo di azione aggiorna un calendario.

Specifica l&#39;ID del calendario da aggiornare.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome calendario]</td> 
   <td> <p> Immettere un nuovo nome per il calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un calendario]

Questo modulo di azione elimina un calendario.

Specifica l&#39;ID del calendario da eliminare.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td> <p>Immettere o mappare l'ID del calendario che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cancella un calendario]

Questo modulo di azione rimuove tutti gli eventi dal calendario principale di un account.

Specificare la connessione che si connette all&#39;account contenente il calendario che si desidera cancellare.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Regole di controllo accessi

* [[!UICONTROL Elenca regole di controllo accessi]](#list-access-control-rules)
* [[!UICONTROL Ottieni una regola di controllo di accesso]](#get-an-access-control-rule)
* [[!UICONTROL Creare una regola di controllo di accesso]](#create-an-access-control-rule)
* [[!UICONTROL Aggiornare una regola di controllo degli accessi]](#update-an-access-control-rule)
* [[!UICONTROL Eliminare una regola di controllo di accesso]](#delete-an-access-control-rule)

#### [!UICONTROL Elenca regole di controllo accessi]

Questo modulo di azione restituisce le regole nell&#39;elenco dei controlli di accesso in un calendario.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario contenente le regole di controllo di accesso che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Imposta il numero massimo di risultati [!DNL Workfront Fusion] restituisce durante un ciclo di esecuzione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una regola di controllo di accesso]

Questo modulo di azione restituisce i metadati di una regola di controllo di accesso.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario contenente la regola di controllo di accesso che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID regola di controllo di accesso]</td> 
   <td>Selezionare la regola di controllo di accesso che si desidera recuperare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una regola di controllo di accesso]

Questo modulo di azione crea una nuova regola di controllo di accesso.

Specificare un nome per il calendario.

Il modulo restituisce l’ID della regola di controllo accessi e di tutti i campi associati, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario in cui si desidera creare una regola di controllo accessi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Selezionare il ruolo da assegnare alla regola di accesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Reader disponibilità libero]</strong>: L'utente può leggere informazioni sulla disponibilità. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: L’utente può leggere e modificare gli eventi e accedere agli elenchi di controllo. </li> 
     <li><strong>Reader [!UICONTROL]</strong>: L’utente può leggere eventi non privati. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utente può leggere e modificare gli eventi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Selezionare il tipo di ambito. </p> 
    <ul> 
     <li><strong>[!UICONTROL Predefinito]</strong>: Ambito pubblico. Questo è il valore predefinito. </li> 
     <li><strong>[!UICONTROL Utente]</strong>: Limita l’ambito a un singolo utente. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Limita l'ambito a un gruppo. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Limita l’ambito a un dominio. </li> 
    </ul> <p>Nota: Le autorizzazioni concesse all'ambito [!UICONTROL Default], o pubblico, si applicano a qualsiasi utente autenticato o meno.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>Immettere l'indirizzo e-mail di un utente o di un gruppo o il nome di un dominio, a seconda del tipo di ambito.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Invio di notifiche]</td> 
   <td> <p>Abilita questa opzione per inviare notifiche sulla modifica dell’accesso. </p> <p>Nota: Nessuna notifica sulla rimozione degli accessi. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare una regola di controllo degli accessi]

Questo modulo di azione aggiorna una regola di controllo di accesso.

Specificare un nome per il calendario.

Il modulo restituisce l’ID della regola di controllo accessi e di tutti i campi associati, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario contenente la regola di controllo di accesso che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID regola di controllo di accesso]</td> 
   <td>Selezionare la regola di controllo di accesso che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Selezionare il ruolo da assegnare alla regola di accesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Nessuno]</strong>: Questo ruolo non fornisce accesso.</li> 
     <li><strong>[!UICONTROL Reader disponibilità libero]</strong>: L'utente può leggere informazioni sulla disponibilità. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: L’utente può leggere e modificare gli eventi e accedere agli elenchi di controllo. </li> 
     <li><strong>Reader [!UICONTROL]</strong>: L’utente può leggere eventi non privati. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utente può leggere e modificare gli eventi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Invio di notifiche]</td> 
   <td> <p>Abilita questa opzione per inviare notifiche sulla modifica dell’accesso. </p> <p>Nota: Nessuna notifica sulla rimozione degli accessi. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una regola di controllo di accesso]

Questo modulo di azione elimina una regola di controllo di accesso.

Specificare un nome per il calendario.

Il modulo restituisce l’ID della regola di controllo accessi e di tutti i campi associati, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID calendario [!UICONTROL]</td> 
   <td> <p>Seleziona o mappa l’ID del calendario contenente la regola di controllo accessi che desideri eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID regola di controllo di accesso]</td> 
   <td>Seleziona o mappa l’ID della regola di controllo accessi che desideri eliminare.</td> 
  </tr> 
 </tbody> 
</table>

### Iteratori (obsoleti)

La [!UICONTROL iterare allegati] e [!UICONTROL iterare i partecipanti] moduli obsoleti. Per eseguire l&#39;iterazione di allegati o partecipanti, utilizzare il [!UICONTROL Controllo del flusso] > [!UICONTROL Iteratore] modulo . Per ulteriori informazioni, consulta [Modulo iteratore in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Altro

* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Ottieni informazioni gratuite]](#get-freebusy-information)

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Calendar] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Immettere un percorso relativo a <code>https://www.googleapis.com/calendar</code>. Esempio: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni informazioni gratuite]

Questo modulo di azione restituisce informazioni gratuite e occupate per un set di calendari.

Il modulo restituisce l’ID del calendario e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come collegare le [!DNL Google Calendar] account a Workfront Fusion, vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe Workfront Fusion - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo minimo]</td> 
   <td> <p> Immettere l'inizio dell'intervallo per il quale si desidera recuperare le informazioni.</p> <p> Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo massimo]</td> 
   <td> <p> Immettere la fine dell'intervallo per il quale si desidera recuperare le informazioni. </p> <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Calendari [!UICONTROL]</td> 
   <td> <p>Per ogni calendario da cui si desidera recuperare le informazioni, fare clic su <strong>Aggiungi</strong> e immetti o mappa l'ID calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Attiva uno scenario prima di un evento

È possibile attivare uno scenario un&#39;ora specificata prima di un evento con l&#39;aiuto di standard [!DNL Google Calendar] promemoria e-mail e [!UICONTROL Webhook] >[!UICONTROL Cassetta postale personalizzata] modulo .

1. Utilizza la [!UICONTROL Calendario Google] >[!UICONTROL Aggiornare un evento] modulo per aggiungere un promemoria e-mail all’evento:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Crea un nuovo scenario a partire da [!UICONTROL Webhook] >[!UICONTROL Cassetta postale personalizzata] modulo .

   1. Copia l&#39;indirizzo e-mail del mailhook.
   1. Salvare lo scenario ed eseguirlo.

1. In [!DNL Gmail], reindirizzare [!DNL Google Calendar] invia un promemoria via email all&#39;indirizzo email del mailhook:

   1. Apri il tuo **[!UICONTROL [!DNL Gmail]impostazioni]**.
   1. Apri **[!UICONTROL Inoltro e POP/IMAP]** scheda .
   1. Fai clic su **[!UICONTROL Aggiungi un indirizzo di inoltro].**
   1. Incolla l&#39;indirizzo e-mail della cassetta postale copiata, fai clic su &#x200B;**[!UICONTROL Successivo]**, confermare premendo **[!UICONTROL Procedi]** nella finestra popup, quindi fare clic su **[!UICONTROL OK]**.

   1. In [!DNL Workfront Fusion], passa al nuovo scenario che deve terminare l’esecuzione ricevendo l’e-mail di conferma.
   1. Fai clic sulla bolla sopra il modulo per controllare l&#39;output del modulo.
   1. Espandi la `Text` e copia il codice di conferma:

      ![](assets/confirmation-code-350x252.png)

   1. In Gmail, incolla il codice di conferma nella casella di modifica e fai clic su &#x200B;**[!UICONTROL Verifica]**:

      ![](assets/paste-code-350x46.png)

   1. Apri **[!UICONTROL Filtri e indirizzi bloccati]** scheda .
   1. Fai clic su **[!UICONTROL Crea un nuovo filtro]**.
   1. Imposta un filtro per tutte le e-mail provenienti da `     calendar-notification@google.com` e fai clic su &#x200B;**[!UICONTROL Creare un filtro]**:
   1. Seleziona **[!UICONTROL Inoltra a]** e scegliere l&#39;indirizzo e-mail del mailing hook dall&#39;elenco.
   1. Fai clic su **[!UICONTROL Crea filtro]** per creare il filtro.

1. (Facoltativo) In [!DNL Workfront Fusion], aggiungi [!UICONTROL Analizzatore di testo] > [!UICONTROL Pattern di corrispondenza] modulo dopo [!UICONTROL Webhook] >[!UICONTROL Cassetta postale personalizzata] per analizzare il codice HTML dell’e-mail e ottenere tutte le informazioni necessarie.

   Ad esempio, puoi configurare il modulo come segue per ottenere l’ID dell’evento:

   *Pattern*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Testo*: La `HTML content` prodotto dal [!UICONTROL Webhook] >[!UICONTROL Cassetta postale personalizzata] modulo .
