---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 21 dell’API
description: Adobe Workfront ha rilasciato la versione API 21 il 23 ottobre 2025. La versione 21 dell’API presenta le seguenti modifiche rispetto alla versione 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: d72c5b4337ea04dbfef4622908824a0bd138b551
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 4%

---

# Novità dell’API versione 20

Adobe Workfront ha rilasciato la versione API 21 il 23 ottobre 2025. La versione 21 dell’API presenta le seguenti modifiche rispetto alla versione 20.

## Risorse aggiunte

### StaffingPlanTemplate (SPTMPL)

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
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>AGGIUNGI</li>
          <li>COUNT</li>
          <li>ELIMINA</li>
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

### AssignmentBillingRole (ASBLRL)

L&#39;oggetto AssignmentBillingRole e tutti i relativi campi sono stati rimossi.

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
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
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
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
         </li>
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
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>assegnazioni team</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Assegnazione (ASSEGNA)

Un oggetto Assignment rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato a lavorarci.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Rimosso</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Cliente (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Disabilita l'utilizzo di un'applet Java per i calcoli della sequenza temporale)
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Documento (DOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

L&#39;oggetto DocumentFolder ha aggiunto il contrassegno `RESTORABLE`.

### Ora (HOUR)

Un oggetto Hour rappresenta un&#39;ora registrata da un utente su una scheda orario.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>getTerejectionCommentmporaryCloudURL</b>
            </p>
            <p>È stata aggiunta la convalida <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
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
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (RTF lessicale)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (rollup riga singola)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Aggiunto</p>
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
            <p><b>isActive</b>
            </p>
            <p>Aggiunto</p>
           </li>
           </ul>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>valuta</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
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
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifica informazioni di contatto)</p>
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
            <p><b>helpDeskProjects</b>
            </p>
            <p>Aggiunto</p>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>Rimosso</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Rimosso</p>
              </li>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>formato</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un oggetto ScoreCardQuestion rappresenta una domanda aggiunta a una scorecard. Queste domande sono solitamente determinate dal manager Portfolio e le loro risposte consentono al manager di comprendere quanto un progetto sia in linea con gli obiettivi del portfolio.<table>
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
            <p>È stato aggiunto il seguente valore possibile:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (rollup riga singola)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Piano di assegnazione del personale

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Aggiunto</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Aggiunto</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Aggiunto</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Aggiunto</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Aggiunto</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>assegnazioni team</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Team

L&#39;oggetto Team ha aggiunto i flag `DATA_EXTENDIBLE` e `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi di riferimento</td>
      <td>
        <ul>
          <li>
            <p><b>categoria</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### AssegnazioneModello

L&#39;oggetto TemplateAssignment ha aggiunto il flag `ATTRIBUTE_ATTACHABLE`.

### Scheda orario (TSHET)

Un oggetto Timesheet rappresenta un foglio ore virtuale che consente agli utenti di immettere le ore effettivamente lavorate per le attività, i progetti e i tipi di ore di lavoro comune.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi core</td>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>assegnazioni team</b>
            </p>
            <p>Aggiunto</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


