---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 17 dell’API
description: Adobe Workfront ha rilasciato la versione API 17 il 6 aprile 2022. La versione 17 dell’API presenta le seguenti modifiche rispetto alla versione 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 1%

---

# Novità della versione 17 dell’API

Adobe Workfront ha rilasciato la versione API 17 il 12 ottobre 2023. La versione 17 dell’API presenta le seguenti modifiche rispetto alla versione 16.

## Risorse aggiunte

<!--

### Booking (BOOKNG)

-->

### DocumentoEsterno (EXTDOC)

Un oggetto ExternalDocument è un documento o un&#39;altra risorsa digitale che si trova in un provider di archiviazione documenti esterno a Workfront. Queste risorse possono essere collegate da e verso Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>descrizione</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>int.</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>percorso</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>dimensione</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>descrizione</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>int.</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>percorso</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>dimensione</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>valore</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi predefiniti</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Query</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li><p><b>cliente</b></p></li>
          <li><p><b>utente</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Risorse rimosse

Nessuna risorsa rimossa per API versione 17

## Risorse modificate

Le seguenti risorse sono state modificate per l’API versione 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Linea di base (BLIN)

Le linee di base sono istantanee delle prestazioni di un progetto in un determinato momento. Memorizzano informazioni chiave sul progetto, come date chiave, avanzamento, costi e ricavi.

L&#39;oggetto Baseline ha rimosso il flag **INLINE_EDITABLE**.

### Record fatturazione (BILL)

Un oggetto BillingRecord registra i ricavi, le ore o le spese che possono essere fatturati. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.

L&#39;oggetto BillingRecord ha rimosso il flag **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Società (CMPY)

Un oggetto Company rappresenta un&#39;organizzazione costituita da un insieme di persone.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Rimosso</p>
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
            <p><b>nome</b>
            </p>
            <p>È stato aggiunto il possibile valore "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p?<p>Questo consente a un’organizzazione di impostare la nuova esperienza Home come predefinita per i propri utenti.</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>È stato aggiunto il possibile valore "Frame.io" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>tipoFile</b>
            </p>
            <p>È stato aggiunto il possibile valore "enum.filetype.site" (sito)</p>
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
      <td>Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Aggiunto.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Spesa (EXPNS)

Le spese rappresentano i costi non di manodopera che potrebbero essere sostenuti durante la durata di un progetto.

L&#39;oggetto Expense ha rimosso il flag **INLINE_EDITABLE**.

### Gruppo (GROUP)

Un oggetto Group rappresenta un insieme di utenti e team. I gruppi spesso rappresentano la struttura di reparto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Rimosso</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Ora (HOUR)

Un oggetto Hour rappresenta un&#39;ora registrata da un utente su una scheda orario.

L&#39;oggetto Hour ha rimosso il flag **INLINE_EDITABLE**.

### Iterazione (ITRN)

Un oggetto Iteration rappresenta una singola iterazione Agile. Le iterazioni sono periodi di tempo distinti utilizzati per pianificare e completare le storie di Agile.

L&#39;oggetto Iteration ha rimosso il flag **INLINE_EDITABLE**.


### VoceDiario (JRNLE)

L&#39;oggetto JournalEntry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Voce diario, viene creata una voce corrispondente ogni volta che tale campo viene modificato.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>Approvatore aggiunto (AAA)</li>
              <li>Revisore aggiunto (AAR)</li>
              <li>Revisore rimosso (ARR)</li>
              <li>Approvatore rimosso (ARA)</li>
              <li>Decisione approvata (ADA)</li>
              <li>Decisione approvata con modifiche (ADC)</li>
              <li>Necessità di lavoro per le decisioni (ADN)</li>
              <li>Decisione revocata (ADR)</li>
              <li>Approvatore cambiato (AAC)</li>
              <li>Revisore modificato (ARC)</li>
              <li>Revisione completata (RDC)</li>
              <li>Revisione revocata (RDR)</li>
              <li>Publish (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

Una bacheca Kanban viene utilizzata per monitorare le attività in un ambiente Agile.

L&#39;oggetto Kanban Board ha rimosso il flag **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Un oggetto LinkedFolder rappresenta una cartella collegata da un provider di documenti esterno, ad esempio Google Drive o Dropbox.

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
            <p>È stato aggiunto il valore possibile "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Attività/Problema Op (OPTASK)

Un oggetto OpTask è comunemente noto come Issue. Un problema è un elemento di lavoro che in genere indica la presenza di un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell’helpdesk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

L&#39;oggetto Issue ha rimosso il flag **INLINE_EDITABLE**.

### Progetto (PROJ)

I progetti sono elementi di lavoro all’interno di Workfront e costituiscono un elemento fondamentale nel modo in cui Workfront aiuta le persone a lavorare. Un oggetto Project rappresenta un gruppo di attività con un obiettivo comune specifico.

L&#39;oggetto Project ha rimosso il flag **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Un oggetto ProjectUser rappresenta un utente associato a un progetto specifico.

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
            <p>Aggiunto.</p>
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
            <p>Aggiunto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Tariffa (RATE)

Un oggetto Rate rappresenta una tariffa di fatturazione in Workfront.

L&#39;oggetto Rate ha rimosso il flag **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>Sono state aggiunte le seguenti azioni per supportare la funzionalità Rate Card:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>L'azione <b>setRatesForRole</b> è stata modificata per aggiungere i campi seguenti:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Rischio (RISCHIO)

Un oggetto Rischio rappresenta un possibile evento che può impedire il completamento di un progetto in tempo o entro i limiti del budget. I progetti in fase di pianificazione presentano rischi aggiuntivi per individuare potenziali ostacoli prima dell’approvazione di qualsiasi lavoro.

L&#39;oggetto Risk ha rimosso il flag **INLINE_EDITABLE**.

### Ruolo/Ruolo (ROLE)

Un oggetto Ruolo (ruolo) rappresenta una capacità funzionale o un insieme di competenze che un utente potrebbe acquisire, ad esempio Designer o Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Rimosso</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Attività (TASK)

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

L&#39;oggetto Task ha rimosso il flag **INLINE_EDITABLE**.

### Team (TEAMOB)

Un oggetto Team è un insieme di Utenti che possono essere assegnati a un elemento di lavoro.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Rimosso</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Membro team (TEAMMB)

Un oggetto TeamMember è un utente associato a un team specifico.

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
            <p>Aggiunto.</p>
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
            <p>Aggiunto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

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
            <p>Aggiunto.</p>
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
            <p>Aggiunto.</p>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>Rimosso</p>
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
            <p><b>changeType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori:</p>
            <ul>
              <li>Approvatore aggiunto (assetapprovalAddApprover)</li>
              <li>Revisore aggiunto (assetapprovalAddReviewer)</li>
              <li>Autorizzatore rimosso (assetapprovalRemoveApprover)</li>
              <li>Revisore rimosso (assetapprovalRemoveReviewer)</li>
              <li>Decisione approvata (assetapprovalDecisionApproved)</li>
              <li>Lavoro necessario per le decisioni (assetapprovalDecisionNeedsWork)</li>
              <li>Decisione approvata con modifiche (assetapprovalDecisionApprovedChanges)</li>
              <li>Decisione revocata (assetapprovalDecisionRevoked)</li>
              <li>Approvatore modificato (assetapprovalApproverChanged)</li>
              <li>Revisore modificato (assetapprovalReviewerChanged)</li>
              <li>Revisione completata (assetapprovalReviewerDecisionComplete)</li>
              <li>Revisione revocata (assetapprovalReviewerDecisionRevoked)</li>
              <li>Errore di invio documento esterno (externalDocumentSendError)</li>
              <li>Versione documento pubblicata (documentVersionPublish)</li>
              <li>Flusso di lavoro cartelle collegate (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Utente (USER)

Un oggetto User rappresenta una persona con un account in Workfront che può accedere e interagire con il sistema.

L&#39;oggetto User ha rimosso il flag **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Questo campo è stato aggiunto ed è un numero compreso tra 0 e 1 che rappresenta ogni giorno la percentuale di tempo che un utente può dedicare al lavoro del progetto (lavoro non comune). Il valore 1 indica che l’utente può dedicare il 100% del proprio tempo al lavoro di progetto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>posizioniUtente</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserGroups (USRGPS)

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
            <p>Aggiunto.</p>
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
            <p>Aggiunto.</p>
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
            <p><b>changeType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori:</p>
            <ul>
              <li>Il documento richiede la tua approvazione (AAA)</li>
              <li>Il documento richiede la tua revisione (AAR)</li>
              <li>Il documento non ha più bisogno della tua approvazione (ARA)</li>
              <li>Il documento non necessita più della tua revisione (ARR)</li>
              <li>Il documento richiede l'approvazione (ATA) dell'utente</li>
              <li>Revisione documento necessario (utente) (ATR)</li>
              <li>Il documento non ha più bisogno dell’approvazione (RTA) di (utente)</li>
              <li>Il documento non necessita più della revisione (RTR) di (utente)</li>
              <li>Documento approvato (ADA)</li>
              <li>Documento approvato con modifiche (ADC)</li>
              <li>Il documento richiede lavoro (ADN)</li>
              <li>(Utente) ha contrassegnato (documento) come approvato. La tua approvazione non è più necessaria. AAN)</li>
              <li>(Utente) ha contrassegnato (documento) come approvato con modifiche. La tua approvazione non è più necessaria. (ACN)</li>
              <li>(Utente) ha contrassegnato (documento) come necessario. La tua approvazione non è più necessaria. (AWN)</li>
              <li>Il documento richiede la tua revisione ora anziché l'approvazione (AAC)</li>
              <li>Il documento richiede la tua approvazione ora anziché una revisione (ADN)</li>
              <li>Documento revisionato (RDC)</li>
              <li>Documento revisionato (TRC)</li>
              <li>(Utente) ha rivisto (documento) come completato. La tua recensione non è più necessaria. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

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
            <p>Aggiunto.</p>
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
            <p>Aggiunto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
