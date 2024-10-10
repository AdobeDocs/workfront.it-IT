---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 19 dell’API
description: Adobe Workfront ha rilasciato la versione API 19 il 6 aprile 2022. La versione 19 dell’API presenta le seguenti modifiche rispetto alla versione 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: e3f50efa03a43c44e9defd0a724b0516504b0e83
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Novità della versione 19 dell’API

Adobe Workfront ha rilasciato la versione API 19 l’8 aprile 2024. La versione 19 dell’API presenta le seguenti modifiche rispetto alla versione 18.

## Risorse aggiunte

Non sono state aggiunte risorse per API versione 19.

## Risorse rimosse

Nessuna risorsa rimossa per API versione 19

## Risorse modificate

### Livello di accesso (ACSLVL)

Un oggetto AccessLevel è associato agli utenti e descrive il set di autorizzazioni AccessLevelPermissions che determinano gli elementi a cui l&#39;utente può accedere.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Sono stati aggiunti i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>Disattiva Assistente di Workfront AI (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assegnazione (ASSEGNA)

Un oggetto Assignment rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato a lavorarci.

L&#39;oggetto Assignment ha aggiunto il flag **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Sono stati aggiunti i seguenti campi diretti:
        <ul>
          <li>
            <p><b>categoryID</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
            </p>
          </li>
          <li>
            <p><b>priorità</b><p>Questo campo consente i seguenti valori:
            <ul>
              <li>0 (nessuna)</li>
              <li>1 (bassa)</li>
              <li>2 (Normale)</li>
              <li>3 (alta)</li>
              <li>4 (Urgente)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>Sono stati aggiunti i seguenti campi di riferimento:
        <ul>
          <li>
            <p><b>categoria</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>Sono stati aggiunti i seguenti campi della raccolta:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Categoria (CTGY)

Un oggetto Category è un modulo personalizzato.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Per supportare la possibilità di aggiungere un modulo personalizzato a un'assegnazione sono stati aggiunti i seguenti campi.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Sono stati aggiunti i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>Assegnazione (ASSEGNA)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Sono stati aggiunti i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>Assegnazione (ASSEGNA)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classificatore (CLSF)

Un classificatore è una posizione.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>Sono state aggiunte le seguenti azioni:
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Cliente

Un oggetto Customer rappresenta un&#39;organizzazione che utilizza un&#39;istanza di Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Sono stati aggiunti i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>Priorità assegnazione (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>L'oggetto CustomEnum consente di convertire i codici di stato in testo leggibile.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Preferenze cliente (CUSTPR)

Un oggetto CustomerPreferences rappresenta l&#39;insieme di preferenze impostate da un cliente per l&#39;istanza di Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Sono stati rimossi i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>Abilitare l'integrazione di Zoom nel flusso di aggiornamenti (password:zoomIntegrationEnabled)
                </p>
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
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>È stato aggiunto il campo <code>folderID</code>.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Aggiunto.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### Tasso di cambio (EXRATE)

Un oggetto ExchangeRate rappresenta un tasso di cambio impostato in Workfront. Gli oggetti ExchangeRate non sono dinamici.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
      <ul>
      <li>I campi seguenti hanno aggiunto la convalida <code>REQUIRED</code>:
        <ul>
          <li><p><b>valuta</b></li>
          <li><p><b>tariffa</b></li></ul>
      <li>Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
      <ul>
        <li>Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppo (GROUP)

Un oggetto Group rappresenta un insieme di utenti e team. I gruppi spesso rappresentano la struttura di reparto.

L&#39;oggetto Group ha aggiunto il flag **SHARABLE**.

### Ora (HOUR)

Un oggetto Hour rappresenta un&#39;ora registrata da un utente su una scheda orario.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
      Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>Le seguenti modifiche sono state apportate al campo <b>ore</b>.</p>
          <ul> 
          <li> Convalida <b>GREATER_THAN</b> rimossa</li>
          <li> Aggiunta convalida <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
      Sono state aggiunte le seguenti azioni:
        <ul>
          <li><p><b>approva</b></li>
          <li><p><b>annulla approvazione</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### VoceDiario (JRNLE)

L&#39;oggetto JournalEntry può essere impostato per registrare informazioni su campi oggetto specifici ogni volta che tali campi vengono modificati. Quando un campo è impostato per essere registrato come parte dell&#39;oggetto Voce diario, viene creata una voce corrispondente ogni volta che tale campo viene modificato.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>flag</b><p>Sono stati aggiunti i seguenti valori possibili:
            </p>
            <ul>
              <li>
                <p>È tasso di costo (CR)
                </p>
              </li>
              <li>
                <p>È la tariffa di fatturazione (BR)
                </p>
              </li>
              <li>
                <p>È finanza generale (GF)
                </p>
              </li>
              <li>
                <p>È il finanziamento combinato (FC)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parametro (PARAM)

Un oggetto Parameter è un campo personalizzato.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>È stato aggiunto il seguente valore possibile:
            <ul>
            <li>Durata (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Sono stati aggiunti i seguenti valori possibili:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Immagine (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Ricerca esterna (EXTRNL)</li>
            <li>Ricerca esterna a selezione multipla (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo Planning (WFPLANNING)</li>
            <li>KPI rapportato alla scala cronologica</li>
            <li>Rollup (ROLLUP)</li>
            <li>Documenti (DOCUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>Configurazioni</b><p>Aggiunto.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Ruolo (ROLE)

Un oggetto Ruolo (ruolo) rappresenta una capacità funzionale o un insieme di competenze che un utente potrebbe acquisire, ad esempio Designer o Product Manager.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
    Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        Sono stati aggiunti i seguenti campi:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Un oggetto ScoreCardQuestion rappresenta una domanda aggiunta a una scorecard. Queste domande sono solitamente determinate dal manager del Portfolio e le loro risposte consentono al manager di capire quanto un progetto sia in linea con gli obiettivi del portfolio.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
            <p><b>displayType</b></p><p>Sono stati aggiunti i seguenti valori possibili:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Immagine (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Ricerca esterna (EXTRNL)</li>
            <li>Ricerca esterna a selezione multipla (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo Planning (WFPLANNING)</li>
            <li>KPI rapportato alla scala cronologica</li>
            <li>Rollup (ROLLUP)</li>
            <li>Documenti (DOCUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### AssegnazioneModello (TASSGN)

Un oggetto TemplateAssignment rappresenta la connessione tra un&#39;attività modello e l&#39;utente, il team o il gruppo assegnato a lavorarci. Quando si utilizza il modello per un progetto, l&#39;utente, il team o il gruppo viene assegnato all&#39;attività.

L&#39;oggetto TemplateAssignment ha aggiunto il flag **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>Sono stati aggiunti i seguenti campi diretti:
        <ul>
          <li>
            <p><b>categoryID</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>Sono stati aggiunti i seguenti campi di riferimento:
        <ul>
          <li>
            <p><b>categoria</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>Sono stati aggiunti i seguenti campi della raccolta:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Una categoria è un modulo personalizzato. Questo campo consente di aggiungere un modulo personalizzato a un'assegnazione.
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
  <tbody>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Rimosso.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


