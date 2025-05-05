---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 20
description: Adobe Workfront ha rilasciato la versione API 20 il 6 aprile 2022. La versione 20 dell’API presenta le seguenti modifiche rispetto alla versione 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# Novità dell’API versione 20

Adobe Workfront ha rilasciato la versione API 20 il 4 maggio 2025. La versione 20 dell’API presenta le seguenti modifiche rispetto alla versione 19.

## Risorse aggiunte

Non sono state aggiunte risorse per API versione 20.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Risorse rimosse

Nessuna risorsa rimossa per API versione 20

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
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>azioni proibite</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>azioni secondarie</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>fatturato</li>
              <li>budget</li>
              <li>BudgetedCost</li>
              <li>BudgetedHours</li>
              <li>BudgetedLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Sono stati aggiunti i flag <code>DYNAMIC</code>, <code>LAZY_READ</code> e <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>È stato aggiunto il flag <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>È stato aggiunto il possibile valore <code>URH</code> (Ore Utente e Ruolo) </li>
          <li><p><b>revenueType</b></p> <p>Sono stati aggiunti i possibili valori <code>URH</code> (Ore utente e ruolo), <code>URC</code> (Ore utente e ruolo w/Cap) e <code>URF</code> (Ore utente e ruolo Plus Fisso)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
          <p>Sono stati aggiunti i seguenti campi:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assegnazione (ASSEGNA)

Un oggetto Assignment rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato a lavorarci.

L&#39;oggetto Assignment ha aggiunto i flag `ATTRIBUTE_ATTACHABLE` e `DOMAIN_EXTENDABLE`.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Un oggetto Avatar è una foto utente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Aggiunta completata</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi core</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Aggiunta completata</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operazioni</td>
      <td>
        <ul>
          <li>
            <p><b>COPIA</b>
            </p>
             <p>Aggiunta completata</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>budget</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>È stato aggiunto il flag <code>CURRENCY</code></li>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>È stato aggiunto il flag <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Record fatturazione (BILL)

Un oggetto BillingRecord registra i ricavi, le ore o le spese che possono essere fatturati. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>quantità</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Aggiunta completata</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>configurazioni</b>
            </p>
             <p>Aggiunta completata</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Società (CMPY)

Un oggetto Company rappresenta un&#39;organizzazione costituita da un insieme di persone.

L&#39;oggetto Company ha aggiunto il flag `SHARABLE`.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
             <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuemove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>tariffa</li>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b>valuta</b>
            </p>
             <p>Aggiunta completata</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Aggiunta completata</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Un oggetto OpTask è comunemente noto come Issue. Un problema è un elemento di lavoro che in genere indica la presenza di un problema che impedisce il completamento di un&#39;attività o di un progetto. Un problema può anche essere una richiesta dell’helpdesk. Anche gli ordini di modifica, le richieste e i bug sono problemi.

L&#39;oggetto OpTask ha aggiunto il flag DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
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
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (ricerca interna)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Ricerca interna a selezione multipla)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORTA)

Un oggetto Portfolio è una raccolta di progetti che competono per le stesse risorse, in genere denaro o persone per completarli.

L&#39;oggetto Portfolio ha aggiunto il flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>allineato</li>
              <li>budget</li>
              <li>valuta</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programma (PRGM)

Un oggetto Program è un sottoinsieme di progetti all&#39;interno di un portfolio, in cui è possibile raggruppare progetti simili.

L&#39;oggetto Program ha aggiunto il flag `DOMAIN_EXTENDABLE`.

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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>fatturato</li>
              <li>budget</li>
              <li>BudgetedCost</li>
              <li>BudgetedHours</li>
              <li>BudgetedLaborCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>È stato aggiunto il flag <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Rimuovi dai dati personalizzati)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Aggiungi sottoprogetti)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Tariffa (RATE)

Un oggetto Rate rappresenta una tariffa di fatturazione in Workfront.

L&#39;oggetto Rate ha aggiunto il flag `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Sono stati aggiunti i seguenti campi:
          <ul>
          <li>valuta</li>
          <li>bloccato</li>
          <li>tipo</li>
          <li>valore</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Ruolo (ROLE)

Un oggetto Ruolo (ruolo) rappresenta una capacità funzionale o un insieme di competenze che un utente potrebbe acquisire, ad esempio Designer o Product Manager.

L&#39;oggetto Role ha aggiunto il flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
          <p>Sono stati aggiunti i seguenti campi:
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>formato</b>
            </p>
             <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un oggetto ScoreCardQuestion rappresenta una domanda aggiunta a una scorecard. Queste domande sono solitamente determinate dal manager Portfolio e le loro risposte consentono al manager di comprendere quanto un progetto sia in linea con gli obiettivi del portfolio.

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
             <p>Sono stati aggiunti i seguenti valori possibili:</p>
             <ul>
              <li><p><code>INTRNL</code> (ricerca interna)</p></li>
              <li><p><code>MULTINTRNL</code> (Ricerca interna a selezione multipla)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Attività (TASK)

Un oggetto Task rappresenta un elemento di lavoro che deve essere eseguito come passo verso il raggiungimento di un obiettivo finale (completamento di un progetto).

L&#39;oggetto Task ha aggiunto il flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Sono stati aggiunti i seguenti valori possibili:<ul><li><code>URH</code> (Ore Utente e Ruolo)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Sono stati aggiunti i seguenti valori possibili:<ul><li><code>URH</code> (Ore Utente e Ruolo)</li><li><code>URC</code> (Ore Utente e Ruolo w/Cap)</li><li><code>URF</code> (Ore Utente e Ruolo più Fisso)</li></ul></li>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>budget</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
          <p>Sono stati aggiunti i seguenti campi:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

Un oggetto TemplateTask rappresenta un oggetto Task che fa parte di un oggetto Template. Le Attività Modello diventano Attività nel Progetto in cui viene utilizzato il Modello.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingImporto</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Sono stati aggiunti i seguenti valori possibili:<ul><li><code>URH</code> (Ore Utente e Ruolo)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Sono stati aggiunti i seguenti valori possibili:<ul><li><code>URH</code> (Ore Utente e Ruolo)</li><li><code>URC</code> (Ore Utente e Ruolo w/Cap)</li><li><code>URF</code> (Ore Utente e Ruolo più Fisso)</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Rimosso</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Utente (USER)

Un oggetto User rappresenta una persona con un account in Workfront che può accedere e interagire con il sistema.

L&#39;oggetto utente ha aggiunto i campi `ATTRIBUTE_ATTACHABLE` e `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
          <p>Sono stati aggiunti i seguenti campi:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
            <p>I campi seguenti hanno aggiunto il flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>I seguenti campi hanno cambiato il loro tipo da <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Sono stati aggiunti i flag <code>DYNAMIC</code>, <code>LAZY_READ</code> e <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>È stato aggiunto il flag <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>È stato aggiunto il possibile valore <code>URH</code> (Ore Utente e Ruolo) </li>
          <li><p><b>revenueType</b></p> <p>Sono stati aggiunti i possibili valori <code>URH</code> (Ore utente e ruolo), <code>URC</code> (Ore utente e ruolo w/Cap) e <code>URF</code> (Ore utente e ruolo Plus Fisso)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



