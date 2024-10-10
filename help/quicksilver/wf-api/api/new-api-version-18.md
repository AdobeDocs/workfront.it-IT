---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 18 dell’API
description: Adobe Workfront ha rilasciato la versione API 18 il 6 aprile 2022. La versione 18 dell’API presenta le seguenti modifiche rispetto alla versione 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Novità della versione 18 dell’API

Adobe Workfront ha rilasciato la versione API 18 l’8 aprile 2024. La versione 18 dell’API presenta le seguenti modifiche rispetto alla versione 17.

## Risorse aggiunte

Non sono state aggiunte risorse per API versione 18.

## Risorse rimosse

Nessuna risorsa rimossa per API versione 18

## Risorse modificate

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
            <p><b>coreAction</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
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
            <p><b>azione</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
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
            <p><b>coreAction</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
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
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### In attesa di approvazione (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>
            <p>Sono state aggiunte le seguenti operazioni:
            </p>
            <ul>
              <li>
                <p><b>AGGIUNGI</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Linea di base (BLIN)

Le linee di base sono istantanee delle prestazioni di un progetto in un determinato momento. Memorizzano informazioni chiave sul progetto, come date chiave, avanzamento, costi e ricavi.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AttivitàPrevista (BSTSK)

Le linee di base sono istantanee delle prestazioni di un progetto in un determinato momento. Memorizzano informazioni chiave sul progetto, come date chiave, avanzamento, costi e ricavi. Quando si crea una previsione, le informazioni sulle attività vengono acquisite anche sulle attività previste della previsione.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
            <p><b>catObjCode</b>:
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoria di risorse non manodopera)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Ora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Scheda tariffe)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoria di risorse non manodopera)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Ora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Scheda tariffe)
                </p>
              </li>
             </ul>
             </p>
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
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>È stato aggiunto il seguente parametro:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>spostaInCartella</b>:
            </p>
            <p>Aggiunto. Questa nuova azione accetta i seguenti parametri:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Dati finanziari (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi predefiniti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.open)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decision.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
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
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Sono stati aggiunti i seguenti campi:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Sono stati aggiunti i seguenti campi:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
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
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Aggiunto.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### RuoloUtenteProgetto (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>È stato aggiunto il seguente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p>È stato aggiunto il seguente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DefCoda (QUED)

Un oggetto QueueDef rappresenta una coda, ovvero un progetto che è stato pubblicato nell&#39;area Help Desk per consentire agli utenti di inviare problemi.

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
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Visualizza tassi di costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Visualizza tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Visualizza contabilità generale)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifica tassi di costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifica tariffe di fatturazione)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifica contabilità generale)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tariffa (RATE)

Un oggetto Rate rappresenta una tariffa di fatturazione in Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Sono stati aggiunti i seguenti flag:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DINAMICO
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Aggiunto.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>nomeVisualizzato</b>
            </p><p>Aggiunto.</p>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>
            </p>
             <p>È stato aggiunto il seguente campo:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Un oggetto TemplateTask rappresenta un oggetto Task che fa parte di un oggetto Template. Le Attività Modello diventano Attività nel Progetto in cui viene utilizzato il Modello.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>È stato aggiunto il seguente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p>È stato aggiunto il seguente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>È stato rimosso il seguente campo:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
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
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>aggiornamentiRecentiObjIDs</b>
            </p>
            <p>Aggiunto.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Un oggetto UserPrefValue rappresenta una preferenza utente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>valore</b>
            </p>
            <p>È stata aggiunta la convalida <code>MAX_LENGTH</code></p>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>Sono stati aggiunti i seguenti campi:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

