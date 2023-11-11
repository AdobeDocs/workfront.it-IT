---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connettore
navigation-topic: apps-and-their-modules
title: Calendario di Microsoft Office 365
description: In un [!DNL Adobe Workfront Fusion] scenario, è possibile automatizzare i flussi di lavoro che utilizzano Microsoft Office 365 Calendar, nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Office 365 Calendar], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per utilizzare [!DNL Office 365 Calendar] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Office 365 Excel] account. Puoi crearne una in [www.office.com](https://www.office.com/).

Per istruzioni sulla connessione dell&#39;account Office 365 a [!DNL Workfront Fusion], vedi [Creare una connessione a Adobe [!DNL Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Dopo aver concesso il consenso, vieni reindirizzato al [!UICONTROL Workfront Fusion] pagina di amministrazione in cui puoi continuare a creare lo scenario.

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Da utilizzare [!DNL Microsoft Office 365 Calendar] moduli, è necessario disporre di un [!DNL Microsoft Office 365 Calendar] account.

## [!DNL Microsoft Office 365 Calendar] moduli e relativi campi

Quando si configura [!DNL Microsoft Office 365 Calendar] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft Office 365 Calendar] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendario](#calendar)
* [Altro](#other)

### Evento

* [[!UICONTROL Guarda gli eventi]](#watch-events)
* [[!UICONTROL Cerca Eventi]](#search-events)
* [[!UICONTROL Ottieni un evento]](#get-an-event)
* [[!UICONTROL Creare un evento]](#create-an-event)
* [[!UICONTROL Aggiornare un evento]](#update-an-event)
* [[!UICONTROL Eliminare un evento]](#delete-an-event)

#### [!UICONTROL Guarda gli eventi]

Questo modulo trigger recupera i dettagli di un evento quando viene creato, aggiornato, eliminato, avviato o terminato nel calendario selezionato.

>[!NOTE]
>
>Per controllare le occorrenze eliminate di una serie di eventi, seleziona [!UICONTROL Per ora di aggiornamento] nel [!UICONTROL Guarda gli eventi] campo. Questo modulo non verifica la presenza di singoli eventi o serie di eventi eliminati.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Osserva eventi]</td> 
   <td> <p>Seleziona la modalità di visualizzazione degli eventi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Per Ora Di Creazione]</strong> </p> <p>Guarda i nuovi eventi.</p> </li> 
     <li> <p><strong>[!UICONTROL Per Ora Di Aggiornamento]</strong> </p> <p>Controlla gli eventi aggiornati.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selezionare il gruppo di calendari [!UICONTROL] che contiene il calendario in cui si desidera visualizzare gli eventi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Selezionare il calendario specifico che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Imposta le condizioni del filtro per filtrare i risultati per oggetto, ID evento o corpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti il numero massimo di messaggi [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca Eventi]

Questo modulo di ricerca recupera i dettagli di un evento quando viene creato, aggiornato, eliminato, avviato o terminato nel calendario selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selezionare il gruppo di calendari [!UICONTROL] che contiene il calendario in cui si desidera visualizzare gli eventi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Selezionare il calendario specifico che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Imposta le condizioni del filtro per filtrare i risultati. Puoi filtrare in base alle seguenti proprietà:</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL ID evento]</li> 
     <li>Data e ora di creazione di [!UICONTROL]</li> 
     <li>[!UICONTROL Data e ora ultima modifica]</li> 
     <li>[!UICONTROL Anteprima corpo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la modalità desiderata per ordinare i risultati.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, crescente o decrescente</li> 
     <li><strong>Data e ora di creazione di [!UICONTROL]</strong>, crescente o decrescente</li> 
     <li><strong>[!UICONTROL Data e ora ultima modifica]</strong>, crescente o decrescente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immetti il numero massimo di eventi [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un evento]

Questo modulo di azione recupera i dettagli dell’evento specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa un titolo per l’evento creato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio]</td> 
   <td> Immettere un singolo punto di inizio dell'evento in una rappresentazione combinata data e ora. Utilizza il formato <code>({date}T{time}</code>ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di fine]</td> 
   <td> Immettere un singolo punto di ora in cui l'evento termina con una rappresentazione combinata data e ora. Utilizza il formato <code>{date}T{time}</code>ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Promemoria attivato]</td> 
   <td>Seleziona se desideri attivare un promemoria per questo evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Immetti o mappa il numero di minuti prima dell’inizio dell’evento in cui deve attivarsi il promemoria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza di questo evento.</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Medio]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Seleziona la riservatezza dell’evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normale]</strong> </li> 
     <li> <p><strong>[!UICONTROL - Personale]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL Please treat this as Personal]" (Considera questo come personale).</p> </li> 
     <li> <p><strong>[!UICONTROL Privato]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL Please treat this as Private]" (Considera privato questo elemento). Questo evento non viene inoltrato o reindirizzato dalle regole della casella in entrata del destinatario.</p> </li> 
     <li> <p><strong>[!UICONTROL Riservato]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL È da considerarsi riservato]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto corpo]</td> 
   <td>Seleziona se il corpo del testo è testo normale o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td>Inserisci o mappa il corpo del messaggio associato all’evento. Può essere in formato HTML o testo (come specificato nel campo [!UICONTROL Body Content Type] qui sopra).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Immettere i dettagli della posizione dell'evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Risposta [!UICONTROL richiesta]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> per richiedere all'invitato di inviare una risposta all'invito all'evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra come]</td> 
   <td> <p>Selezionare la modalità di visualizzazione dell'evento per gli utenti che visualizzano il calendario.</p> 
    <ul> 
     <li>[!UICONTROL libero]</li> 
     <li>[!UICONTROL Provvisorio]</li> 
     <li>[!UICONTROL Occupato]</li> 
     <li>[!UICONTROL Fuori sede]</li> 
     <li>[!UICONTROL Lavora altrove]</li> 
     <li>[!UICONTROL Sconosciuto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partecipanti]</p> </td> 
   <td> <p>Aggiungi i partecipanti all'evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del partecipante.</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail]</strong> </p> <p>Immettere l'indirizzo di posta elettronica del partecipante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Immetti o mappa le categorie che desideri che l’evento venga visualizzato nel calendario.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td>Inserisci, mappa o seleziona l’ID dell’evento da aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa un titolo per l’evento creato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio]</td> 
   <td> Immettere un singolo punto di inizio dell'evento in una rappresentazione combinata data e ora. Utilizza il formato <code>{date}T{time}</code>ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di fine]</td> 
   <td> Immettere un singolo punto di ora in cui l'evento termina con una rappresentazione combinata data e ora. Utilizza il formato <code>({date}T{time}</code>ad esempio, <code>2017-08-29T04:00:00.0000000</code>. Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Promemoria attivato]</td> 
   <td>Seleziona se desideri attivare un promemoria per questo evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Immetti o mappa il numero di minuti prima dell’inizio dell’evento in cui deve attivarsi il promemoria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza di questo evento.</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Medio]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Seleziona la riservatezza dell’evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normale]</strong> </li> 
     <li> <p><strong>[!UICONTROL - Personale]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL Please treat this as Personal]" (Considera questo come personale).</p> </li> 
     <li> <p><strong>[!UICONTROL Privato]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL Please treat this as Private]" (Considera privato questo elemento). Questo evento non viene inoltrato o reindirizzato dalle regole della casella in entrata del destinatario.</p> </li> 
     <li> <p><strong>[!UICONTROL Riservato]</strong> </p> <p>Il destinatario visualizza un messaggio "[!UICONTROL È da considerarsi riservato]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto corpo]</td> 
   <td>Seleziona se il contenuto del corpo del messaggio associato all’evento è testo normale o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td>Inserisci o mappa il corpo del messaggio associato all’evento. Può essere in formato HTML o testo (come specificato nel campo [!UICONTROL Body Content Type] qui sopra).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Immettere i dettagli della posizione dell'evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Risposta [!UICONTROL richiesta]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> per richiedere all'invitato di inviare una risposta all'invito all'evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra come]</td> 
   <td> <p>Selezionare la modalità di visualizzazione dell'evento per gli utenti che visualizzano il calendario.</p> 
    <ul> 
     <li>[!UICONTROL libero]</li> 
     <li>[!UICONTROL Provvisorio]</li> 
     <li>[!UICONTROL Occupato]</li> 
     <li>[!UICONTROL Fuori sede]</li> 
     <li>[!UICONTROL Lavora altrove]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partecipanti]</p> </td> 
   <td> <p>Aggiungi i partecipanti all'evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del partecipante.</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail]</strong> </p> <p>Immettere l'indirizzo di posta elettronica del partecipante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Immetti o mappa le categorie che desideri che l’evento venga visualizzato nel calendario.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID evento]</td> 
   <td> <p>Inserisci o mappa l’ID dell’evento da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendario

* [[!UICONTROL Elenca calendari]](#list-calendars)
* [[!UICONTROL Ottieni un calendario]](#get-a-calendar)
* [[!UICONTROL Creare un calendario]](#create-a-calendar)
* [[!UICONTROL Aggiornare un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminare un calendario]](#delete-a-calendar)

#### [!UICONTROL Elenca calendari]

Questo modulo di ricerca recupera un elenco di tutti i calendari dell’utente autenticato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selezionare il gruppo di calendari [!UICONTROL] contenente i calendari da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere il numero massimo di calendari [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un calendario]

Questo modulo di azione recupera i dettagli di un singolo calendario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID calendario]</td> 
   <td> <p>Immetti o mappa l’ID del calendario di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un calendario]

Questo modulo di azione crea un nuovo calendario nell’account Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID calendario]</td> 
   <td>Immettere l'ID del calendario [!UICONTROL] per il calendario che si desidera aggiornare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome nuovo calendario]</td> 
   <td> <p>Immettere un nome per il nuovo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un calendario]

Questo modulo elimina un calendario esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID calendario]</td> 
   <td>Immettere l'ID [!UICONTROL Calendar] per il calendario che si desidera eliminare.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Inserisci un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
