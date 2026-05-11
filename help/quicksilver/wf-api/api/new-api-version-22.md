---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 22 dell’API
description: Adobe Workfront ha rilasciato la versione API 22 l’11 maggio 2026. La versione 22 dell’API presenta le seguenti modifiche rispetto alla versione 21.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 3%

---

# Novità della versione 22 dell’API

Adobe Workfront ha rilasciato la versione API 22 l’8 maggio 2026. La versione 22 dell’API presenta le seguenti modifiche rispetto alla versione 21.

## Risorse aggiunte

Le seguenti risorse sono state aggiunte per API versione 22.

### ReportShareableFolder (RPSHFD)

Puoi utilizzare cartelle di rapporti condivisibili per organizzare i rapporti e condividerle con altri utenti. Questa funzione è progettata per i team che gestiscono grandi volumi di rapporti e richiedono un controllo degli accessi scalabile e coerente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campi predefiniti</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>AGGIUNGI</li>
          <li>CONTEGGIO</li>
          <li>DELETE</li>
          <li>MODIFICA</li>
          <li>GET</li>
          <li>RAPPORTO</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Risorse rimosse

Le seguenti risorse sono state rimosse dall’API versione 22.

### UserLocation (USRLOC)

Questo oggetto è stato rimosso.

## Risorse modificate

Le seguenti risorse sono state modificate per l’API versione 22.

### Livello di accesso (ACSLVL)

Un oggetto AccessLevel è associato agli utenti e descrive il set di autorizzazioni AccessLevelPermissions che determinano gli elementi a cui l&#39;utente può accedere.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato con modifiche ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Autorizzazioni livello di accesso (ALVPER)

Un oggetto AccessLevelPermissions rappresenta un&#39;autorizzazione specifica per accedere, creare o modificare un oggetto Workfront. Queste autorizzazioni possono quindi essere associate a un Livello di accesso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I seguenti campi sono stati modificati con modifiche ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Richiesta di accesso (ACSREQ)

Se un utente non ha accesso a un oggetto in Workfront di cui ha bisogno, può richiedere l’accesso a tale oggetto. L&#39;oggetto AccessRequest rappresenta questa richiesta.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato con modifiche ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>action</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Regola di accesso (ACSRUL)

Un oggetto AccessRule rappresenta un set di regole nei livelli di accesso personalizzati che determina il modo in cui gli utenti possono condividere i progetti creati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I seguenti campi sono stati modificati con modifiche ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approvazione (APPROVAZIONE)

Per un determinato elemento di lavoro, ad esempio un’attività, un documento o una scheda orario, può essere necessario che un supervisore o un altro utente approvi l’elemento di lavoro. Un oggetto Approval rappresenta l&#39;azione di approvazione di un elemento di lavoro.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Categoria (CTGY)

Un oggetto Category è un modulo personalizzato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>È stato aggiunto il seguente campo.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Società (CMPY)

Un oggetto Company rappresenta un&#39;organizzazione costituita da un insieme di persone.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

L&#39;oggetto CustomEnum consente di convertire i codici di stato in testo leggibile.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>Aggiunto
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Query</td>
      <td>Aggiunto
        <ul>
          <li><p><b>assignmentStatus</b></p></li>
          <li><p><b>bookingStatus</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Cliente (CUST)

Un oggetto Customer rappresenta un&#39;organizzazione che utilizza un&#39;istanza di Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Stati di prenotazione)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Stati assegnazione)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Preferenze cliente (CUSTPR)

Un oggetto CustomerPreferences rappresenta l&#39;insieme di preferenze impostate da un cliente per l&#39;istanza di Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili per supportare Enterprise Storage Management:</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Documento (DOC)

Un oggetto Document rappresenta un file, ad esempio materiale scritto, immagini o altre forme di informazioni.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>La seguente azione è stata modificata.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

I documenti possono essere organizzati in cartelle. È possibile creare cartelle personali nell&#39;area Documenti personale. L&#39;oggetto DocumentFolder rappresenta una di queste cartelle.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Un oggetto DocumentVersion rappresenta una versione specifica di un file, ad esempio materiale scritto, immagini o altre forme di informazioni.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato aggiunto per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      Il seguente campo è stato modificato.
        <ul>
          <li><b>version</b><p>Rimossa la convalida "REQUIRED".</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>È stata aggiunta la seguente azione.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>È stata aggiunta la seguente operazione.
        <ul>
          <li><p><b>MODIFICA</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### Tasso di cambio (EXRATE)

Un oggetto ExchangeRate rappresenta un tasso di cambio impostato in Workfront. Gli oggetti ExchangeRate non sono dinamici.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Sono stati aggiunti i seguenti campi.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### VoceDiario (JRNLE)

L&#39;oggetto JournalEntry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Voce diario, viene creata una voce corrispondente ogni volta che tale campo viene modificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I seguenti campi sono stati modificati.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Sposta cartella)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>contrassegni</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Campo diario (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I seguenti campi sono stati modificati.
        <ul>
          <li>
            <p><b>azione</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Sposta cartella)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask (OPTASK)

Un oggetto OpTask è comunemente noto come Issue. Un problema è un elemento di lavoro che in genere indica la presenza di un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell’helpdesk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li><b>actualWorkRequired</b><p>Sono stati aggiunti i seguenti flag:
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Cerca campi</td>
      <td>
        <ul>
          <li><b>actualWork</b><p>Tipo cambiato da <code>null</code> a <code>double</code>.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>Sono state aggiunte le seguenti operazioni.
        <ul>
          <li><p><b>CONTEGGIO</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>RAPPORTO</b></p>
          <li><p><b>SEARCH</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### Parametro (PARAM)

Un oggetto Parameter è un campo personalizzato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Sono stati aggiunti i seguenti campi.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### RaggruppaParametri (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Sono stati aggiunti i seguenti campi.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

Un oggetto PortalSection è un oggetto Report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>È stato aggiunto il seguente campo.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>È stato aggiunto il seguente campo.
        <ul>
          <li><b>reportShareableFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Portfolio (PORTA)

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarli.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Programma (PRGM)

Un oggetto Program è un sottoinsieme di progetti all&#39;interno di un portfolio, in cui è possibile raggruppare progetti simili.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      Il seguente campo è stato modificato.
        <ul>
          <li><b>portfolioID</b><p>È stata aggiunta la convalida "REQUIRED".</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Progetto (PROJ)

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento fondamentale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo comune specifico.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DefCoda (QUED)

Un oggetto QueueDef rappresenta una definizione di coda di richieste in Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I seguenti campi sono stati modificati con modifiche ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

Un oggetto ScheduledReport rappresenta un report configurato per la consegna.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato con modifiche approfondite ai possibili valori. Per informazioni dettagliate, consulta la documentazione per gli sviluppatori.
        <ul>
          <li><b>formato</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Attività (TASK)

Un oggetto Task rappresenta un elemento di lavoro che deve essere completato per raggiungere un obiettivo finale (completamento di un progetto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Aggiunto</p></li>
          <li><p><b>actualWorkRequired</b></p><p>Flag aggiunti <code>AUTO_LOAD</code> e <code>DYNAMIC</code>.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li>
            <p><b>attivitàOperazioneConvertita</b>
            </p>
            <p>Aggiunto</p>
          </li>
        </ul> 
      </td>
    </tr>
  </tbody>
</table>

### Modello (TMPL)

Un oggetto Template rappresenta un pattern per un progetto. I progetti possono essere creati da modelli per risparmiare tempo. Un modello contiene un team e attività che verranno copiati in qualsiasi progetto creato dal modello.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>I campi seguenti sono stati aggiunti per supportare Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aggiorna (AGGIORNA)

È possibile aggiornare gli elementi di lavoro in Workfront per informare gli utenti dello stato corrente. Un oggetto Update rappresenta uno di questi aggiornamenti. Gli aggiornamenti possono essere immessi dagli utenti o creati dal sistema Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Il seguente campo è stato modificato.
        <ul>
          <li>
            <p><b>azione</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Utente (USER)

Un oggetto User rappresenta una persona con un account in Workfront che può accedere e interagire con il sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>È stato aggiunto il seguente campo.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>Il seguente campo è stato rimosso.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





