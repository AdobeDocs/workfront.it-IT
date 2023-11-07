---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 15 dell’API
description: Adobe Workfront ha rilasciato la versione API 14 il 14 giugno 2022. La versione 15 dell’API presenta le seguenti modifiche rispetto alla versione 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# Novità della versione 15 dell’API

Adobe Workfront ha rilasciato la versione API 15 il 14 giugno 2022. La versione 15 dell’API presenta le seguenti modifiche rispetto alla versione 14.

## Risorse aggiunte

* [Iniziativa (INITIV)](#Initiati)

* [DefProblema (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJECT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [DefAttività (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Iniziativa (INITIV)

L&#39;oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di mansioni, i costi fissi e il beneficio pianificato.

Per ulteriori informazioni sulle iniziative, consulta [Panoramica delle iniziative nella Pianificazione scenario](../../scenario-planner/initiatives-overview.md).

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
            <p>Questo è un oggetto interno.</p>
          </li>
          <li>
            <p><b>durata</b>
            </p>
            <p>Quantità di tempo tra endDate e startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>La data di completamento pianificata per l’iniziativa.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>ID associato all’utente che ha inviato la richiesta.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>ID associato all’azione</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>ID associato all'iniziativa.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Data dell'ultima pubblicazione dell'iniziativa in Workfront Scenario Planner.</p>
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
            <p>ID del progetto associato all’iniziativa.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>ID dello scenario in Workfront Scenario Planner associato all’iniziativa.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>La data di inizio pianificata dell’iniziativa.</p>
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
            <p><b>enteredBy</b>
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
            <p><b>COUNT</b>
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
            <p><b>RICERCA</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DefProblema (ISSDEF)

L’oggetto IssueDef rappresenta un insieme di dati relativi al formato dei problemi. Questo oggetto può essere allegato a progetti o modelli e influisce sui problemi aggiunti a tale progetto o modello.

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

### ObjectIntegration (OBJECT)

In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L&#39;oggetto ObjectIntegration rappresenta questo collegamento.

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
            <p>Questo è un oggetto interno.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>La data e l'ora in cui è stata immessa ObjectIntegration nel sistema Workfront.</p>
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
            <p>Oggetto in Workfront a cui è associata ObjectIntegration.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Il codice oggetto dell'oggetto in Workfront a cui è associata l'ObjectIntegration.</p>
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

### DefAttività (TSKDEF)

L&#39;oggetto TaskDef rappresenta un insieme di dati relativi al formato delle attività. Questo oggetto può essere allegato a progetti o modelli e influisce sulle attività aggiunte a tale progetto o modello.

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
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
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

### UserApproval (USRAPV)

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
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>stato</b>
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
            <p><b>utente</b>
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
            <p><b>stato</b>
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
            <p><b>approva</b>
            </p>
          </li>
          <li>
            <p><b>rifiuta</b>
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
            <p><b>COUNT</b>
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
            <p><b>RICERCA</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Risorse rimosse

Nessuna risorsa rimossa per API versione 15.

## Risorse modificate

* [Livello di accesso (ACSLVL)](#AccessLe)

* [Autorizzazioni livello di accesso (ALVPER)](#AccessLe2)

* [Richiesta di accesso (ACSREQ)](#AccessRe)

* [Regola di accesso (ACSRUL)](#AccessRu)

* [Approvazione (APPROVAZIONE)](#Approval)

* [Categoria (CTGY)](#Category)

* [ParametroCategoria (CTGYPA)](#Category2)

* [Preferenze cliente (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Gruppo (GROUP)](#Group)

* [VoceDiario (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [Attività/Problema Op (OPTASK)](#OpTask)

* [Parametro (PARAM)](#Paramete)

* [Portfolio (PORTA)](#Portfoli)

* [Programma (PRGM)](#Program)

* [Progetto (PROJ)](#Project)

* [DefCoda (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Attività (TASK)](#Task)

* [Modello (TMPL)](#Template)

* [Scheda orario (TSHET)](#Timeshee)

* [Visualizza (UIVIEW)](#View)

* [Aggiorna (AGGIORNA)](#Update)

* [Utente (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Lavoro (WORK)](#Work)

### Livello di accesso (ACSLVL)

Un oggetto AccessLevel è associato agli utenti e descrive il set di autorizzazioni AccessLevelPermissions che determinano gli elementi a cui l&#39;utente può accedere.

Per ulteriori informazioni sui livelli di accesso, consulta [Livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>VTMAWMG (Visualizza i team associati ai miei gruppi)</p>
              </li>
              <li>
                <p>VALLTM (Visualizza tutti i team)</p>
              </li>
            </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>azione</b> (stringa)</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
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

### Regola di accesso (ACSRUL)

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
            <p><b>coreAction</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (stringa[])</p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approvazione (APPROVAZIONE)

Per un determinato elemento di lavoro, ad esempio un&#39;attività, un documento o una scheda orario, può essere necessario che un supervisore o un altro utente approvi l&#39;elemento di lavoro. Un oggetto Approval rappresenta l&#39;azione di approvazione di un elemento di lavoro.

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
            <p>L'oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di mansioni, i costi fissi e il beneficio pianificato. </p>
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
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegations
</b>
            </p>
            <p style="font-weight: normal;">Aggiunta completata.</p>
            <p>In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
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
                <p>GRUPPO (Group)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (stringa[])</p>
            <p>Aggiunta completata.</p>
            <p style="font-weight: normal;">Questo parametro è un array di possibili oggetti a cui è possibile associare il modulo personalizzato. È stato aggiunto per supportare la possibilità di allegare un modulo personalizzato a più tipi di oggetti.</p>
            <p>Valori possibili: </p>
            <p>AZIENDA, PORTA, PRGM, PROJ, ATTIVITÀ, OPTASK, UTENTE, DOCU, EXPNS, ITRN, BILL, GRUPPO</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (stringa[])</p>
            <p>Aggiunta completata.</p>
            <p style="font-weight: normal;">Questo parametro è un array di possibili oggetti a cui è possibile associare il modulo personalizzato. È stato aggiunto per supportare la possibilità di allegare un modulo personalizzato a più tipi di oggetti.</p>
            <p>Valori possibili: </p>
            <p>AZIENDA, PORTA, PRGM, PROJ, ATTIVITÀ, OPTASK, UTENTE, DOCU, EXPNS, ITRN, BILL, GRUPPO</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ParametroCategoria (CTGYPA)

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
            <p><b>journaledObjCodes</b>
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

### Preferenze cliente (CUSTPR)

Un oggetto CustomerPreferences rappresenta l&#39;insieme di preferenze impostate da un cliente per l&#39;istanza di Workfront.

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
                <p>Questo valore supporta l’integrazione aggiornata di Sharepoint.</p>
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

I documenti possono essere organizzati in cartelle. È possibile creare cartelle personali nell&#39;area Documenti personale. L&#39;oggetto DocumentFolder rappresenta una di queste cartelle.

L&#39;oggetto DocumentFolder ha aggiunto il flag `SHARABLE`.

### DocumentVersion (DOCV)

Un oggetto DocumentVersion rappresenta una versione specifica di un file, ad esempio materiale scritto, immagini o altre forme di informazioni.

Per ulteriori informazioni sulle versioni dei documenti, vedere [Carica una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

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
                <p>Questo valore supporta l’integrazione aggiornata di Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppo (GROUP)

Un oggetto Group rappresenta un insieme di utenti e team. I gruppi spesso rappresentano la struttura di reparto.

Per ulteriori informazioni sui gruppi, consulta Gruppi e team.

L&#39;oggetto Group ha aggiunto il flag `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <p>Sono stati aggiunti i seguenti campi:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Una categoria è un modulo personalizzato. Questo parametro è stato aggiunto per supportare la possibilità di aggiungere Forms personalizzati agli oggetti del gruppo. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Si tratta di un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td >
        <p>Sono stati aggiunti i seguenti campi:</p>
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
            <p><b>utente</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <p>Sono stati aggiunti i seguenti campi:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
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
            <p>Si tratta di un parametro booleano con valore true se un oggetto è attivo e false in caso contrario. Gli oggetti impostati su Attivo vengono visualizzati nei menu a discesa e nei campi di completamento automatico e possono essere allegati ad altri oggetti.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <p>Sono stati aggiunti i seguenti campi:</p>
        <ul>
          <li>
            <p><b>CALCULATIONDataExtension</b>
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

### VoceDiario (JRNLE)

L&#39;oggetto JournalEntry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Voce diario, viene creata una voce corrispondente ogni volta che tale campo viene modificato.

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

Per ulteriori informazioni sulle cartelle collegate, vedere Collegare documenti da applicazioni esterne.

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
                <p>Questo valore supporta l’integrazione aggiornata di Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Attività/Problema Op (OPTASK)

Un oggetto OpTask è comunemente noto come Issue. Un problema è un elemento di lavoro che in genere indica la presenza di un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell’helpdesk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

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
        <p>La seguente azione è stata modificata:</p>
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
        <p>Sono stati modificati i seguenti campi:</p>
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

### Portfolio (PORTA)

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarli.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
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

Un oggetto Program è un sottoinsieme di progetti all&#39;interno di un portfolio, in cui è possibile raggruppare progetti simili.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
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

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento fondamentale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo comune specifico.

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
            <p>L'oggetto Initiative crea stime in Workfront Scenario Planner per il tipo e il numero di mansioni, i costi fissi e il beneficio pianificato. </p>
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
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DefCoda (QUED)

Un oggetto QueueDef rappresenta una coda, ovvero un progetto che è stato pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare problemi.

Per ulteriori informazioni sulle code di richieste, consulta [Creare una coda di richieste](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifica i team a cui collaboro)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifica i team nei gruppi che gestisco (solo per amministratori di gruppi))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un oggetto ScoreCardQuestion rappresenta una domanda aggiunta a una scorecard. Queste domande sono solitamente determinate dal manager del Portfolio e le loro risposte consentono al manager di capire quanto un progetto sia in linea con gli obiettivi del portfolio.

Per ulteriori informazioni sulle domande delle scorecard, consulta [Creare una scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

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

### Attività (TASK)

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
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

### Scheda orario (TSHET)

Un oggetto Timesheet rappresenta un foglio ore virtuale che consente agli utenti di immettere le ore effettivamente lavorate per le attività, i progetti e i tipi di ore di lavoro comune.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <p>Il seguente campo è stato rimosso:</p>
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

### Aggiorna (AGGIORNA)

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

### Utente (USER)

Un oggetto User rappresenta una persona con un account in Workfront che può accedere e interagire con il sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
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
                <p><code>DUP </code>(richiesta di verifica di un documento)</p>
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

### Lavoro (WORK)

Un oggetto Work è un&#39;interfaccia comune ereditata sia da Task che da OpTask e condivide il codice comune tra i due.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>In alcuni casi, è possibile collegare elementi di lavoro Workfront direttamente agli oggetti di un prodotto software esterno. L'oggetto ObjectIntegration rappresenta questo collegamento.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
