---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 16
description: Adobe Workfront ha rilasciato l’API versione 16 il 6 aprile 2022. La versione 16 dell’API presenta le seguenti modifiche rispetto alla versione 15.
author: Becky
feature: Workfront API
source-git-commit: 19978aaa2886008afc3c0faa9cfd18bd7c4b2555
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Novità dell’API versione 16

Adobe Workfront ha rilasciato l’API versione 16 il 6 aprile 2022. La versione 16 dell’API presenta le seguenti modifiche rispetto alla versione 15.

## Risorse aggiunte

Non sono state aggiunte risorse per l’API versione 16.

## Risorse rimosse

Non sono state rimosse risorse per l’API versione 16

## Risorse modificate

* <!--[AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Omologazione (omologazione)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Ora (ORA)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Nota (NOTA)](#note-note)
* [Attività/problema (OPTASK)](#note-note)
* [Progetto (PROJ)](#project-proj)
* [Tasso (TASSO)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Ruolo/Ruolo lavoro (RUOLO)](#role--job-role-role)
* [Attività (ATTIVITÀ)](#task-task)
* [Scheda attività (TSHET)](#timesheet-tshet)
* [UIFilter / Filtro (UIFT)](#uifilter--filter-uift)
* [UIGroupBy/Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView / View (UIVW)](#uiview--view-uivw)
* [Utente (UTENTE)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno che è necessario eseguire. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code>e tiene conto del fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Assegnazione (ASSGN)

Un oggetto di assegnazione rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato per lavorare su di esso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno che è necessario eseguire. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code>e tiene conto del fuso orario.</p>
          </li>
          <li>
            <p><b>isContered</b>
            </p>
            <p>Questo campo è stato aggiunto ed è un valore booleano che indica se l’assegnazione è conteggiata. Se i minuti dell'assegnazione al giorno sono stati modificati nel servizio di bilanciamento del carico di lavoro, l'assegnazione è stata conteggiata.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

L&#39;oggetto CustomEnum consente la conversione dei codici di stato in testo leggibile dall&#39;utente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>Sono stati aggiunti i seguenti valori possibili:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Questa azione restituisce un valore booleano che descrive se il cliente ha disabilitato l’opzione per l’aggiornamento automatico dei titolari di licenza di Contributer.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Un oggetto ExternalSection è una pagina Web esterna incorporata in un rapporto Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>È stato aggiunto e calcola l’URL di un iFrame incorporato in un rapporto.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>È stato aggiunto e calcola gli URL di iFrame incorporati in un rapporto.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Ora (ORA)

Un oggetto Hour rappresenta un&#39;ora registrata da un utente in una scheda attività.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Aggiunta completata. Questo parametro viene utilizzato per identificare le ore create con <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Nota (NOTA)

Un oggetto Note è un commento o un aggiornamento effettuato su un oggetto Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentDocuments</b>
            </p>
            <p>Questo campo è stato aggiunto e rappresenta un elenco di documenti allegati al commento.</p>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno che è necessario eseguire. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code>e tiene conto del fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Questo campo è stato aggiunto <code>teamIDs</code> per supportare la funzionalità di assegnazione di più team a un'attività o a un problema.</p>
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
            <p>Questo campo è stato aggiunto e rappresenta la somma di tutte le ore previste nel budget per il progetto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tasso (TASSO)

Un oggetto Rate rappresenta un tasso di fatturazione in Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Questi parametri sono stati spostati nell’oggetto Rate dall’oggetto Role , in modo che gli oggetti Role (Ruolo) e User possano avere più valori (per intervalli di date separati).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Questi parametri rappresentano l'ID e il codice oggetto dell'oggetto a cui è associato il Rate.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Azioni</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Questa azione è stata aggiunta e associa gli oggetti Rate all'oggetto specificato. Questo endpoint funziona per tutti gli oggetti Rate Attachable.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Un oggetto RichTextNote è un commento o un aggiornamento effettuato su un oggetto Workfront, che include testo RTF, ad esempio testo in grassetto o in corsivo.

L&#39;oggetto RichTextNote ha rimosso il flag `REPORTABLE`.

### Ruolo/Ruolo lavoro (RUOLO)

Un oggetto Role (job role) rappresenta una capacità funzionale o un set di competenze che un utente potrebbe riempire, ad esempio Designer o Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
           <li>
            <p><b>tassi</b>
            </p>
            <p>Questo è stato aggiunto e rappresenta gli oggetti Rate associati a questo ruolo.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Attività (ATTIVITÀ)

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
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno che è necessario eseguire. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code>e tiene conto del fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Questo campo è stato aggiunto <code>teamIDs</code> per supportare la funzionalità di assegnazione di più team a un'attività o a un problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Scheda attività (TSHET)

Un oggetto Scheda attività rappresenta una scheda attività virtuale che consente agli utenti di immettere le ore effettive lavorate per attività, progetti e tipi di orario comune.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>Questo parametro ha rimosso il flag <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Questo parametro ha rimosso il flag <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Questo parametro è stato aggiunto e memorizza la durata dei fogli ore in giorni, indipendentemente dalle modifiche apportate a "Ore equivalenti per Workday completo".  Ad esempio, se l’opzione Ore equivalenti è impostata su 6 e un giorno viene registrato, l’opzione Ore equivalenti viene modificata in 8 ore, <code>totalDays</code> ha ancora un valore pari a 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filtro (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Questa azione è stata aggiunta ed esegue una mappa della query del filtro e aggiunge la <code>allowingnull</code> unire per i campi nullable.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Queste azioni supportano la possibilità di condividere filtri, viste e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy/Grouping (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Queste azioni supportano la possibilità di condividere filtri, viste e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Queste azioni supportano la possibilità di condividere filtri, viste e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Utente (UTENTE)

Un oggetto User rappresenta una persona con un account in Workfront in grado di accedere e interagire con il sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi di raccolta</td>
      <td>
        <ul>
           <li>
            <p><b>tassi</b>
            </p>
            <p>Questo è stato aggiunto e rappresenta gli oggetti Rate associati a questo utente.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Un oggetto UserNote è una notifica.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Query</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>È stato aggiunto il seguente valore possibile:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Lavoro (LAVORO)

Un oggetto Work è un&#39;interfaccia comune ereditata da Task e OpTask e condivide il codice comune tra i due.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno che è necessario eseguire. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code>e tiene conto del fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
