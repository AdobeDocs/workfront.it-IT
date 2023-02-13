---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connettore
navigation-topic: apps-and-their-modules
title: Calendario di Microsoft Office 365
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano il calendario Microsoft Office 365 e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Office 365 Calendar], nonché collegarlo a più applicazioni e servizi di terze parti.

Per utilizzare [!DNL Office 365 Calendar] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Office 365 Excel] conto. Puoi crearne una in [www.office.com](http://www.office.com/).

Per istruzioni su come collegare l&#39;account Office 365 a [!DNL Workfront Fusion], vedi [Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Dopo aver concesso il consenso, vieni reindirizzato nuovamente al [!UICONTROL Workfront Fusion] pagina di amministrazione in cui puoi continuare a creare lo scenario.

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

Per utilizzare [!DNL Microsoft Office 365 Calendar] moduli, è necessario disporre di un [!DNL Microsoft Office 365 Calendar] conto.

## [!DNL Microsoft Office 365 Calendar] moduli e relativi campi

Quando si configura [!DNL Microsoft Office 365 Calendar] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft Office 365 Calendar] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendario](#calendar)
* [Altro](#other)

### Evento

* [[!UICONTROL Eventi di controllo]](#watch-events)
* [[!UICONTROL Eventi di ricerca]](#search-events)
* [[!UICONTROL Ottieni un evento]](#get-an-event)
* [[!UICONTROL Creare un evento]](#create-an-event)
* [[!UICONTROL Aggiornare un evento]](#update-an-event)
* [[!UICONTROL Eliminare un evento]](#delete-an-event)

#### [!UICONTROL Eventi di controllo]

Questo modulo trigger recupera i dettagli di un evento quando l’evento viene creato, aggiornato, eliminato, avviato o terminato nel calendario selezionato.

>[!NOTE]
>
>Per cercare le occorrenze eliminate di una serie di eventi, selezionare [!UICONTROL Per ora di aggiornamento] in [!UICONTROL Eventi di controllo] campo . Questo modulo non controlla gli eventi singoli eliminati o le serie di eventi eliminate.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eventi Watch]</td> 
   <td> <p>Selezionare la modalità di visualizzazione degli eventi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Per Ora Di Creazione]</strong> </p> <p>Guarda i nuovi eventi.</p> </li> 
     <li> <p><strong>[!UICONTROL Per Ora Di Aggiornamento]</strong> </p> <p>Controlla gli eventi aggiornati.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Seleziona il gruppo di calendario [!UICONTROL] che contiene il calendario in cui desideri visualizzare gli eventi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario specifico che si desidera visualizzare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Imposta le condizioni del filtro per filtrare i risultati per oggetto, ID evento o corpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere il numero massimo di messaggi [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventi di ricerca]

Questo modulo di ricerca conserva i dettagli di un evento quando l’evento viene creato, aggiornato, eliminato, avviato o terminato nel calendario selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Seleziona il gruppo di calendario [!UICONTROL] che contiene il calendario in cui desideri visualizzare gli eventi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendario [!UICONTROL]</td> 
   <td> <p>Selezionare il calendario specifico che si desidera visualizzare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Imposta le condizioni del filtro per filtrare i risultati. Puoi filtrare in base alle seguenti proprietà:</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL ID evento]</li> 
     <li>[!UICONTROL Data e ora di creazione]</li> 
     <li>[!UICONTROL Data e ora dell'ultima modifica]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare la modalità di ordine dei risultati.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, crescente o decrescente</li> 
     <li><strong>[!UICONTROL Data e ora di creazione]</strong>, crescente o decrescente</li> 
     <li><strong>[!UICONTROL Data e ora dell'ultima modifica]</strong>, crescente o decrescente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere il numero massimo di eventi [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un evento]

Questo modulo di azione recupera i dettagli dell&#39;evento specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Immetti o mappa l’ID dell’evento di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un evento]

Questo modulo di azione crea un nuovo evento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa un titolo per l’evento creato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio]</td> 
   <td> Immettere un singolo punto di tempo in cui l'evento inizia in una rappresentazione combinata di data e ora. Usa il formato <code>({date}T{time}</code>; ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di fine]</td> 
   <td> Immettere un singolo punto di tempo in cui l'evento termina con una rappresentazione combinata di data e ora. Usa il formato <code>{date}T{time}</code>; ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Promemoria su</td> 
   <td>Seleziona se attivare un promemoria per questo evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Promemoria]</td> 
   <td>Immettere o mappare il numero di minuti prima dell'inizio dell'evento quando deve essere attivato il promemoria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l'importanza di questo evento.</p> 
    <ul> 
     <li>[!UICONTROL Bassa]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sensibilità </td> 
   <td> <p>Selezionare la sensibilità dell'evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normale]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come Personale]".</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come privato]". Questo evento non viene inoltrato o reindirizzato dalle regole della casella in entrata del destinatario.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidenziale]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come riservato]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto del corpo]</td> 
   <td>Seleziona se il contenuto del corpo è testo normale o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del corpo]</td> 
   <td>Inserisci o mappa il corpo del messaggio associato all’evento. Può essere in formato HTML o testo (come specificato nel campo [!UICONTROL Body Content Type] sopra).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Immetti i dettagli della posizione dell’evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Risposta richiesta]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> per richiedere all’invitato di inviare una risposta all’invito all’evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra come]</td> 
   <td> <p>Seleziona la modalità di visualizzazione dell’evento agli utenti che visualizzano il calendario.</p> 
    <ul> 
     <li>[!UICONTROL Gratis]</li> 
     <li>[!UICONTROL Provvisorio]</li> 
     <li>[!UICONTROL Occupato]</li> 
     <li>[!UICONTROL Fuori sede]</li> 
     <li>[!UICONTROL Lavoro altrove]</li> 
     <li>[!UICONTROL Sconosciuto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partecipanti]</p> </td> 
   <td> <p>Aggiungi i partecipanti all’evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Inserisci il nome del partecipante.</p> </li> 
     <li> <p><strong>E-MAIL [!UICONTROL]</strong> </p> <p>Inserisci l’indirizzo e-mail del partecipante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Immetti o mappa le categorie a cui desideri che l’evento venga visualizzato nel calendario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un evento]

Questo modulo di azione aggiorna un evento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td>Immetti, mappa o seleziona l’ID dell’evento da aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa un titolo per l’evento creato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio]</td> 
   <td> Immettere un singolo punto di tempo in cui l'evento inizia in una rappresentazione combinata di data e ora. Usa il formato <code>{date}T{time}</code>; ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di fine]</td> 
   <td> Immettere un singolo punto di tempo in cui l'evento termina con una rappresentazione combinata di data e ora. Usa il formato <code>({date}T{time}</code>; ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Promemoria su</td> 
   <td>Seleziona se attivare un promemoria per questo evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Promemoria]</td> 
   <td>Immettere o mappare il numero di minuti prima dell'inizio dell'evento quando deve essere attivato il promemoria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l'importanza di questo evento.</p> 
    <ul> 
     <li>[!UICONTROL Bassa]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sensibilità </td> 
   <td> <p>Selezionare la sensibilità dell'evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normale]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come Personale]".</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come privato]". Questo evento non viene inoltrato o reindirizzato dalle regole della casella in entrata del destinatario.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidenziale]</strong> </p> <p>Il destinatario vede un messaggio "[!UICONTROL Tratta questo come riservato]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto del corpo]</td> 
   <td>Seleziona se il contenuto del corpo del messaggio associato all’evento è di testo normale o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del corpo]</td> 
   <td>Inserisci o mappa il corpo del messaggio associato all’evento. Può essere in formato HTML o testo (come specificato nel campo [!UICONTROL Body Content Type] sopra).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Immetti i dettagli della posizione dell’evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Risposta richiesta]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> per richiedere all’invitato di inviare una risposta all’invito all’evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra come]</td> 
   <td> <p>Seleziona la modalità di visualizzazione dell’evento agli utenti che visualizzano il calendario.</p> 
    <ul> 
     <li>[!UICONTROL Gratis]</li> 
     <li>[!UICONTROL Provvisorio]</li> 
     <li>[!UICONTROL Occupato]</li> 
     <li>[!UICONTROL Fuori sede]</li> 
     <li>[!UICONTROL Lavoro altrove]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partecipanti]</p> </td> 
   <td> <p>Aggiungi i partecipanti all’evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Inserisci il nome del partecipante.</p> </li> 
     <li> <p><strong>E-MAIL [!UICONTROL]</strong> </p> <p>Inserisci l’indirizzo e-mail del partecipante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Immetti o mappa le categorie a cui desideri che l’evento venga visualizzato nel calendario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un evento]

Questo modulo di azione elimina un evento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Immetti o mappa l’ID dell’evento da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendario

* [[!UICONTROL Calendari elenco]](#list-calendars)
* [[!UICONTROL Ottieni un calendario]](#get-a-calendar)
* [[!UICONTROL Creare un calendario]](#create-a-calendar)
* [[!UICONTROL Aggiornare un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminare un calendario]](#delete-a-calendar)

#### [!UICONTROL Calendari elenco]

Questo modulo di ricerca recupera un elenco di tutti i calendari dell&#39;utente autenticato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selezionare il gruppo di calendari che contiene i calendari da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere il numero massimo di calendari [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un calendario]

Questo modulo di azione recupera i dettagli su un singolo calendario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td> <p>Immettere o mappare l'ID del calendario di cui si desidera recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un calendario]

Questo modulo di azione crea un nuovo calendario nel tuo account Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome calendario]</td> 
   <td> <p>Immettere un nome per il nuovo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un calendario]

Questo modulo di azione modifica un calendario esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td>Immetti l’ [!UICONTROL Calendar ID] per il calendario che desideri aggiornare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo nome calendario]</td> 
   <td> <p>Immettere un nome per il nuovo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un calendario]

Questo modulo di azione elimina un calendario esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID calendario [!UICONTROL]</td> 
   <td>Immetti l'ID calendario [!UICONTROL] per il calendario che desideri eliminare.</td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/events</code></p> </td> 
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
