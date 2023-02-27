---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 15
description: Adobe Workfront ha rilasciato l’API versione 14 il 14 giugno 2022. La versione 15 dell’API presenta le seguenti modifiche rispetto alla versione 14.
author: Becky
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# Novità dell’API versione 15

Adobe Workfront ha rilasciato l’API versione 15 il 14 giugno 2022. La versione 15 dell’API presenta le seguenti modifiche rispetto alla versione 14.

## Risorse aggiunte

* [Iniziativa (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [Approvazione utente (USRAPV)](#UserAppr)

### Iniziativa (INITIV)

L&#39;oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di ruoli di lavoro, i costi fissi e il benefit pianificato.

Per maggiori informazioni sulle iniziative, vedi [Panoramica delle iniziative nel planner dello scenario](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Si tratta di un oggetto interno.</p>
          </li>
          <li>
            <p><b>durata</b>
            </p>
            <p>Quantità di tempo tra endDate e startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Data di completamento prevista per l'iniziativa.</p>
          </li>
          <li>
            <p><b>enterByID</b>
            </p>
            <p>ID associato all’utente che ha inviato la richiesta.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>ID associato all’azione</p>
          </li>
          <li>
            <p><b>InitiativeID</b>
            </p>
            <p>ID associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>La data dell'ultima pubblicazione dell'iniziativa in Workfront Scenario Planner.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Nome dell'iniziativa</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>ID del piano associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Nome del piano associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>ID del progetto associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>ID dello scenario in Workfront Scenario Planner associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>Data di inizio prevista dell'iniziativa.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>enterBy</b>
            </p>
          </li>
          <li>
            <p><b>progetto</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>
            <p><b>CONTEGGIO</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORTO </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

L&#39;oggetto IssueDef rappresenta un insieme di dati relativi al formato dei problemi. Questo oggetto può essere associato a progetti o modelli e influisce sui problemi aggiunti a tale progetto o modello.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L&#39;oggetto ObjectIntegration rappresenta questo collegamento.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Si tratta di un oggetto interno.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>La data e l'ora in cui ObjectIntegration è stato immesso nel sistema Workfront.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>ID Workfront univoco dell'oggetto ObjectIntegration specifico.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>Il software esterno con cui l'oggetto ObjectIntegration crea un collegamento. I valori possibili sono:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>L'oggetto in Workfront a cui è associata ObjectIntegration.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Codice oggetto dell'oggetto in Workfront a cui è associata ObjectIntegration.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

L&#39;oggetto TaskDef rappresenta un insieme di dati relativi al formato delle attività. Questo oggetto può essere associato a progetti o modelli e influisce sulle attività aggiunte a tale progetto o modello.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovazioneProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approvazione utente (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>approvatore</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>richiedente</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi predefiniti</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>approvare</b>
            </p>
          </li>
          <li>
            <p><b>respingere</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>
            <p><b>AGGIUNGI</b>
            </p>
          </li>
          <li>
            <p><b>CONTEGGIO</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORTO</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Risorse rimosse

Non sono state rimosse risorse per l’API versione 15.

## Risorse modificate

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Omologazione (omologazione)](#Approval)

* [Categoria (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Gruppo (GRUPPO)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [Attività/problema (OPTASK)](#OpTask)

* [Parametro (PARAM)](#Paramete)

* [Portfolio (PORTO)](#Portfoli)

* [Programma (PRGM)](#Program)

* [Progetto (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Attività (ATTIVITÀ)](#Task)

* [Modello (TMPL)](#Template)

* [Scheda attività (TSHET)](#Timeshee)

* [Visualizza (UIVIEW)](#View)

* [Aggiorna (AGGIORNAMENTO)](#Update)

* [Utente (UTENTE)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Lavoro (LAVORO)](#Work)

### AccessLevel (ACSLVL)

Un oggetto AccessLevel è associato agli utenti e descrive il set di AccessLevelPermissions che determinano a cosa può accedere l&#39;utente.

Per ulteriori informazioni sui livelli di accesso, vedi [Livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>VTMAWMG (Visualizza team associati ai miei gruppi)</p>
              </li>
              <li>
                <p>VALLTM (visualizza tutti i team)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

Un oggetto AccessLevelPermissions rappresenta un&#39;autorizzazione specifica per accedere, creare o modificare un oggetto Workfront. Tali autorizzazioni possono quindi essere associate a un livello di accesso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondarioActions</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Se un utente non ha accesso a un oggetto in Workfront di cui ha bisogno, può richiedere l&#39;accesso a tale oggetto. L&#39;oggetto AccessRequest rappresenta questa richiesta.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>action</b> (stringa)</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (stringa)</p>
            <p>È stato aggiunto il seguente valore possibile:</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Un oggetto AccessRule rappresenta un set di regole nei livelli di accesso personalizzati che determina il modo in cui gli utenti possono condividere i progetti creati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondarioActions</b> (string[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Omologazione (omologazione)

Un dato elemento di lavoro, ad esempio un&#39;attività, un documento o una scheda attività, può richiedere che un supervisore o un altro utente si disconnetta dall&#39;elemento di lavoro. Un oggetto Approvazione rappresenta l&#39;azione di disconnessione su un elemento di lavoro.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>iniziativa</b>
            </p>
            <p>Aggiunta completata.</p>
            <p>L'oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di ruoli di lavoro, i costi fissi e il benefit pianificato. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Aggiunta completata.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Aggiunta completata.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Aggiunta completata.</p>
            <p>In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> (stringa)</p>
            <p>È stato aggiunto il seguente valore possibile:</p>
            <ul>
              <li>
                <p>GRUPPO (Gruppo)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Aggiunta completata.</p>
            <p style="font-weight: normal;">Questo parametro è una matrice di possibili oggetti a cui è possibile associare il modulo personalizzato. È stato aggiunto per supportare la possibilità di allegare un modulo personalizzato a più tipi di oggetti.</p>
            <p>Valori possibili: </p>
            <p>CMPY, PORTA, PRGM, PROJ, ATTIVITÀ, OPTASK, UTENTE, DOCU, EXPNS, ITRN, BILL, GRUPPO</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Aggiunta completata.</p>
            <p style="font-weight: normal;">Questo parametro è una matrice di possibili oggetti a cui è possibile associare il modulo personalizzato. È stato aggiunto per supportare la possibilità di allegare un modulo personalizzato a più tipi di oggetti.</p>
            <p>Valori possibili: </p>
            <p>CMPY, PORTA, PRGM, PROJ, ATTIVITÀ, OPTASK, UTENTE, DOCU, EXPNS, ITRN, BILL, GRUPPO</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Aggiunta completata.</p>
          </li>
          <li>
            <p><b>journalObjCodes</b>
            </p>
            <p>Aggiunta completata.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Aggiunta completata.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CustomerPreferences (CUSTPR)

Un oggetto CustomerPreferences rappresenta il set di preferenze che un cliente ha impostato per la propria istanza di Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Integrazione SharePoint (Graph API) abilitata)</p>
                <p>Questo valore supporta l’integrazione Sharepoint aggiornata.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Consenti agli utenti di creare progetti senza utilizzare un modello)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

I documenti possono essere organizzati in cartelle. È possibile creare cartelle personali nell&#39;area Documenti personali. L&#39;oggetto DocumentFolder rappresenta una di queste cartelle.

L&#39;oggetto DocumentFolder ha aggiunto il flag `SHARABLE`.

### DocumentVersion (DOCV)

Un oggetto DocumentVersion rappresenta una versione specifica di un file (ad esempio materiale scritto, immagini o altre forme di informazione).

Per ulteriori informazioni sulle versioni dei documenti, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>È stato aggiunto il seguente valore: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Questo valore supporta l’integrazione Sharepoint aggiornata.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppo (GRUPPO)

Un oggetto Group rappresenta un set di utenti e team. I gruppi rappresentano spesso la struttura dipartimentale.

Per ulteriori informazioni sui gruppi, consulta Gruppi e team .

L&#39;oggetto Group ha aggiunto il flag `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <p>Sono stati aggiunti i campi seguenti:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Una categoria è un modulo personalizzato. Questo parametro è stato aggiunto per supportare la possibilità di aggiungere Custom Forms agli oggetti Group. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Si tratta di un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <p>Sono stati aggiunti i campi seguenti:</p>
        <ul>
          <li>
            <p><b>approvatore</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>richiedente</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <p>Sono stati aggiunti i campi seguenti:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi predefiniti</td>
      <td >
        <p>È stato aggiunto il seguente campo:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Si tratta di un parametro booleano con un valore true se un oggetto è attivo e false se non lo è. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di digitazione e possono essere associati ad altri oggetti.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <p>Sono stati aggiunti i campi seguenti:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Questa azione ricalcola le espressioni nei campi modulo personalizzati.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

È possibile impostare l&#39;oggetto JournalEntry per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Journal Entry, ogni volta che tale campo viene modificato viene creata una voce Journal corrispondente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>È stato aggiunto il seguente valore: </p>
        <ul>
          <li>
            <p>DW (download)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Un oggetto LinkedFolder rappresenta una cartella collegata da un provider di documenti esterno, ad esempio Google Drive o Dropbox.

Per ulteriori informazioni sulle cartelle collegate, vedere Collegamento di documenti da applicazioni esterne.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>È stato aggiunto il seguente valore: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Questo valore supporta l’integrazione Sharepoint aggiornata.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Attività/problema (OPTASK)

Un oggetto OpTask è comunemente noto come Problema. Un problema è un elemento di lavoro che in genere indica che c&#39;è un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell&#39;Help Desk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <p>Sono state aggiunte le seguenti azioni:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>L'azione seguente è stata modificata:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Campo aggiunto <code>parentID</code></p>
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
      <td>
        <p>È stato aggiunto il seguente campo:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Sono stati modificati i campi seguenti:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>È stato aggiunto il valore possibile <code>WIDGET </code>(Widget) </p>
            <p>Questo valore supporta l’utilizzo di immagini nei moduli personalizzati.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>È stato aggiunto il valore possibile <code>WIDGET </code>(Widget)</p>
            <p>Questo valore supporta l’utilizzo di immagini nei moduli personalizzati.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORTO)

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarle.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programma (PRGM)

Un oggetto Program è un sottoinsieme di progetti all&#39;interno di un portfolio, dove progetti simili possono essere raggruppati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Progetto (PROJ)

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento di base principale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo specifico comune.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <ul>
          <li>
            <p><b>iniziativa</b>
            </p>
            <p>L'oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di ruoli di lavoro, i costi fissi e il benefit pianificato. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un oggetto QueueDef rappresenta una coda, ovvero un progetto pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare problemi a tale area.

Per ulteriori informazioni sulle code di richiesta, vedi [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica team accesi)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modificare i team nei gruppi gestiti (solo amministratori di gruppo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un oggetto ScoreCardQuestion rappresenta una domanda che è stata aggiunta a una scorecard. Queste domande sono solitamente determinate dal gestore del Portfolio e le loro risposte consentono al manager di comprendere quanto un progetto sia in linea con gli obiettivi del portfolio.

Per ulteriori informazioni sulle domande della scorecard, vedi [Creare una scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>È stato aggiunto il valore possibile <code>WIDGET </code>(Widget)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Attività (ATTIVITÀ)

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Modello (TMPL)

Un oggetto Template rappresenta un pattern per un progetto. I progetti possono essere creati da modelli per risparmiare tempo. Un modello contiene un team e attività, che verranno copiati in qualsiasi progetto creato dal modello.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Scheda attività (TSHET)

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <p>Il campo seguente è stato rimosso:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Visualizza (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Sono stati rimossi i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Layout a quattro colonne)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Aggiornamenti)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Aggiornamenti)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Lavori in corso)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Dati personalizzati)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Aggiorna Dati Customizzati)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Aggiornamento di stato)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Aggiornamento di stato)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Aggiornamento di stato)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Aggiornamento di stato)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Lista dei Dettagli)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Sezione della Lista dei Dettagli)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aggiorna (AGGIORNAMENTO)

È possibile aggiornare gli elementi di lavoro in Workfront per informare gli utenti dello stato corrente. Un oggetto Update rappresenta uno di questi aggiornamenti. Gli aggiornamenti possono essere immessi dagli utenti o creati dal sistema Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>È stato aggiunto il valore possibile <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Utente (UTENTE)

Un oggetto User rappresenta una persona con un account in Workfront in grado di accedere e interagire con il sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li>
            <p><b>userApproved</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote (USRNOT)

Un oggetto UserNote è una notifica.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Richiesto di provare un documento)</p>
              </li>
              <li>
                <p><code>DUV </code>(Consente di visualizzare un documento)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Lavoro (LAVORO)

Un oggetto Work è un&#39;interfaccia comune ereditata da Task e OpTask e condivide il codice comune tra i due.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In alcuni casi, è possibile collegare gli elementi di lavoro di Workfront direttamente agli oggetti in un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
