---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 16 dell’API
description: Adobe Workfront ha rilasciato la versione API 16 il 6 aprile 2022. La versione 16 dell’API presenta le seguenti modifiche rispetto alla versione 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Novità della versione 16 dell’API

Adobe Workfront ha rilasciato la versione API 16 il 6 aprile 2023. La versione 16 dell’API presenta le seguenti modifiche rispetto alla versione 15.

## Risorse aggiunte

Non sono state aggiunte risorse per API versione 16.

## Risorse rimosse

Nessuna risorsa rimossa per API versione 16

## Risorse modificate

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Approvazione (APPROVAZIONE)](#approval-approval)
* [Preferenze cliente (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Ora (HOUR)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Nota (NOTA)](#note-note)
* [Attività/Problema Op (OPTASK)](#note-note)
* [Progetto (PROJ)](#project-proj)
* [Tariffa (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Ruolo/Ruolo (ROLE)](#role--job-role-role)
* [Attività (TASK)](#task-task)
* [Scheda orario (TSHET)](#timesheet-tshet)
* [UIFilter / Filtro (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Raggruppamento (UIGB)](#uigroupby--grouping-uigb)
* [Visualizzazione UIView/View (UIVW)](#uiview--view-uivw)
* [Utente (USER)](#user-user)
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
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno necessari. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code> e prende in considerazione il fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Assegnazione (ASSEGNA)

Un oggetto assegnazione rappresenta la connessione tra un elemento di lavoro e l&#39;utente, il team o il gruppo assegnato a lavorarci.

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
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno necessari. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code> e prende in considerazione il fuso orario.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>Questo campo è stato aggiunto ed è un valore booleano che indica se l’assegnazione è contornata. Se i minuti al giorno dell’assegnazione sono stati modificati nel Bilanciatore dei carichi di lavoro, l’assegnazione è stata configurata.</p>
          </li>
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
            <p>Questa azione restituisce un valore booleano che descrive se il cliente ha disabilitato l’opzione di aggiornamento automatico dei titolari di licenze per collaboratori.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Un oggetto ExternalSection è una pagina Web esterna incorporata in un report Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>calcolaURLIframe</b>
            </p>
            <p>Questa opzione è stata aggiunta e calcola l’URL di un iFrame incorporato in un rapporto.</p>
         </li>
          <li>
            <p><b>calcolaURLIframe</b>
            </p>
            <p>Questa funzione è stata aggiunta e calcola gli URL di iFrame incorporati in un rapporto.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>identificatoreOraScheda orario</b>
            </p>
            <p>Aggiunto. Questo parametro viene utilizzato per identificare le ore create con <code>batchSave</code>. </p>
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
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
          <li>
            <p><b>documenti allegati</b>
            </p>
            <p>Questo campo è stato aggiunto e rappresenta un elenco di documenti allegati al commento.</p>
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
      <td role="rowheader">Campi diretti</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno necessari. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code> e prende in considerazione il fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>assegnaMultiplo</b>
            </p>
            <p>Questa azione ha aggiunto il campo <code>teamIDs</code> per supportare la funzionalità di assegnazione di più team a un'attività o a un problema.</p>
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
            <p>Questo campo è stato aggiunto e rappresenta la somma di tutte le ore preventivate nel progetto.</p>
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
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Questi parametri sono stati spostati nell'oggetto Rate dall'oggetto Role, in modo che gli oggetti Role e User possano avere più valori (per intervalli di date separati).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Questi parametri rappresentano l’ID e il codice oggetto dell’oggetto a cui è associato il tasso.
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
           <p>Questa azione è stata aggiunta e allega oggetti Rate all'oggetto specificato. Questo endpoint funziona per tutti gli oggetti Rate Attachable.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Un oggetto RichTextNote è un commento o un aggiornamento di un oggetto Workfront che include testo RTF, ad esempio testo in grassetto o corsivo.

L&#39;oggetto RichTextNote ha rimosso il flag `REPORTABLE`.

### Ruolo/Ruolo (ROLE)

Un oggetto Ruolo (ruolo) rappresenta una capacità funzionale o un insieme di competenze che un utente potrebbe acquisire, ad esempio Designer o Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
           <li>
            <p><b>tariffe</b>
            </p>
            <p>L'oggetto è stato aggiunto e rappresenta gli oggetti Rate associati a questo ruolo.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno necessari. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code> e prende in considerazione il fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">azioni</td>
      <td>
        <ul>
           <li>
            <p><b>assegnaMultiplo</b>
            </p>
            <p>Questa azione ha aggiunto il campo <code>teamIDs</code> per supportare la funzionalità di assegnazione di più team a un'attività o a un problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p>Questo parametro è stato aggiunto e memorizza la durata delle schede orario in giorni indipendentemente dalle modifiche apportate a "Ore equivalenti per Full Workday".  Ad esempio, se l'argomento Ore equivalenti è impostato su 6 e viene registrato un giorno, l'argomento Ore equivalenti viene modificato in 8 ore, <code>totalDays</code> ha ancora il valore 1.</p>
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
            <p>Questa azione è stata aggiunta e accetta una mappa di query di filtro e aggiunge l'unione <code>allowingnull</code> per i campi nullable.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Queste azioni supportano la possibilità di condividere filtri, visualizzazioni e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Raggruppamento (UIGB)


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
            <p>Queste azioni supportano la possibilità di condividere filtri, visualizzazioni e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Visualizzazione UIView/View (UIVW)

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
            <p>Queste azioni supportano la possibilità di condividere filtri, visualizzazioni e raggruppamenti a livello di sistema.</p><p>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Utente (USER)

Un oggetto User rappresenta una persona con un account in Workfront che può accedere e interagire con il sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campi raccolta</td>
      <td>
        <ul>
           <li>
            <p><b>tariffe</b>
            </p>
            <p>L'oggetto è stato aggiunto e rappresenta gli oggetti Rate associati a questo utente.</p>
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
            <p><b>allObjectTypesUnreadNotifications</b>
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
            <p><b>workPerDate</b>
            </p>
            <p>Questo campo è stato aggiunto e mostra il numero di minuti di lavoro al giorno necessari. Ha il formato <code>YYYY-MM-DD: (number of minutes)</code> e prende in considerazione il fuso orario.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
