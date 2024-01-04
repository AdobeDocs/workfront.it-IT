---
product-area: reporting
navigation-topic: text-mode-reporting
title: Creare filtri in modalità testo complessi utilizzando istruzioni EXISTS
description: Creare filtri in modalità testo complessi utilizzando istruzioni EXISTS
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2766'
ht-degree: 0%

---

# Creare filtri in modalità testo complessi utilizzando istruzioni EXISTS

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Questo articolo richiede una conoscenza approfondita dell’API di Adobe Workfront e dell’interfaccia di reporting in modalità testo. Per informazioni sull’API di Workfront, consulta [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).\
>Per informazioni sull&#39;utilizzo della modalità testo, vedere [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Panoramica delle relazioni tra oggetti in Workfront

Tutti gli oggetti sono collegati ad altri oggetti nel database di Workfront.

Comprendere la gerarchia e l’interdipendenza degli oggetti consente di individuare gli oggetti a cui è possibile fare riferimento nei rapporti.

Per informazioni sugli oggetti presenti in Workfront e sulla relativa gerarchia e interdipendenza, vedere [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Durante la creazione di filtri, è possibile fare riferimento ad altri oggetti connessi all&#39;oggetto del filtro entro un massimo di 2 livelli di relazione utilizzando l&#39;interfaccia standard di reporting.

Ad esempio, puoi fare riferimento all’ID Portfolio in un filtro di problemi per visualizzare solo i problemi sui progetti associati a un determinato portfolio utilizzando l’interfaccia standard. In questo caso, il portfolio è 2 livelli lontano dalle emissioni.

Tuttavia, non è possibile fare riferimento al proprietario del Portfolio in un filtro di problemi utilizzando l’interfaccia standard per visualizzare solo i problemi dei progetti associati a portfolio in cui il proprietario è un utente specifico. È necessario utilizzare la modalità testo per accedere al campo Nome proprietario Portfolio, che è a tre livelli da problemi.

![issue_to_portfolio_owner_screen_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Per un elenco completo degli oggetti in Workfront, vedi [API Explorer](../../../wf-api/general/api-explorer.md).

Per informazioni su come navigare in API Explorer e trovare oggetti, vedi [Utilizzo di API Explorer](../../../wf-api/general/using-api-explorer.md).

Quando si creano i filtri, è necessario creare istruzioni complesse nell&#39;interfaccia in modalità testo per fare riferimento a questi tipi di oggetti.

Per informazioni sulla creazione di filtri complessi, vedi [Panoramica dei filtri in modalità testo complessi che utilizzano istruzioni EXISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) sezione.

## Panoramica dei filtri in modalità testo complessa che utilizzano istruzioni EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Quando si creano filtri che si estendono su più livelli nella gerarchia degli oggetti o si filtrano gli oggetti mancanti, tenere presente quanto segue:

* È necessario creare filtri complessi quando si desidera fare riferimento a oggetti non direttamente connessi all&#39;oggetto filtro.
* È necessario utilizzare un&#39;istruzione EXISTS per eseguire le operazioni seguenti:

   * Creare filtri che si estendono su più livelli.
   * Creare filtri che cercano oggetti mancanti.\
     Ad esempio, quando crei un rapporto utente, puoi filtrare gli utenti che non hanno registrato il tempo per un determinato periodo di tempo.

Quando si utilizzano istruzioni EXISTS in un filtro, considera le seguenti regole:

* È possibile fare riferimento a tre oggetti in un filtro EXISTS:

   * Oggetto del filtro (oggetto originale).
   * Oggetto di cui si desidera fare riferimento al campo (oggetto Target).
   * Oggetto che connette gli oggetti Original e Target, nel caso in cui non siano connessi direttamente tra loro (oggetto di collegamento).

* I filtri che utilizzano EXISTS contengono due istruzioni separate collegate da un segno di uguale:

   * L&#39;istruzione che precede il segno di uguale fa riferimento all&#39;oggetto a cui si fa riferimento, ovvero l&#39;oggetto Linking o l&#39;oggetto Target.
   * L&#39;istruzione dopo il segno di uguale fa riferimento all&#39;oggetto da cui si fa riferimento (l&#39;oggetto originale).

* Per connettere le istruzioni, è necessario utilizzare il codice oggetto dell&#39;oggetto di collegamento.\
  Puoi trovare il codice oggetto di tutti gli oggetti in API Explorer.\
  Per informazioni su API Explorer, vedi [API Explorer](../../../wf-api/general/api-explorer.md).

* Quando manca un oggetto di collegamento perché gli oggetti originale e di destinazione sono collegati direttamente tra loro, è possibile utilizzare il codice oggetto dell&#39;oggetto di destinazione anziché l&#39;oggetto di collegamento.
* È possibile fare riferimento a più campi (campi di destinazione) sullo stesso oggetto (oggetto di destinazione), nel qual caso è necessario connettere le righe che fanno riferimento ai campi mediante AND.\
  Per un esempio di filtro per più campi appartenenti all&#39;oggetto Target, vedere [Esempio 4: filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard allineamento Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) in questo articolo.

* L&#39;unico modificatore supportato per un&#39;istruzione EXISTS è NOTEXISTS.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare i filtri in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare i filtri in un report</p> <p>Gestire le autorizzazioni per un filtro per modificarlo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare filtri in modalità testo complessi che si estendono su più livelli nella gerarchia degli oggetti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

È possibile creare un filtro che faccia riferimento a oggetti su più livelli della gerarchia degli oggetti in cui è presente l&#39;oggetto filtro. Ad esempio, puoi creare un filtro di problemi per i problemi relativi a progetti non associati a un determinato proprietario del Portfolio.

Per creare questo filtro è sempre necessario utilizzare un&#39;istruzione EXISTS e l&#39;interfaccia della modalità testo.

Per esempi di filtri, vedi [Esempio 1: filtrare i problemi per nome del proprietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in questo articolo.

Per creare un filtro che si estenda su più livelli nella gerarchia degli oggetti:

1. Identifica l’oggetto del filtro. Questo oggetto viene definito oggetto originale.\
   Ad esempio, Problema.
1. Identifica il campo in base al quale desideri filtrare. Questo oggetto viene definito campo di destinazione e appartiene a un oggetto di destinazione.\
   Ad esempio, il campo ownerID (Campo di destinazione) che appartiene al Portfolio (Oggetto di destinazione).
1. (Condizionale) Se l’oggetto originale (problema) e il campo di destinazione (ownerID) non sono collegati direttamente tra loro, è necessario trovare un terzo oggetto, un oggetto di collegamento (progetto), che li colleghi. L&#39;oggetto di collegamento deve disporre di almeno un campo a cui si fa riferimento dalle schede Campi o Riferimenti dell&#39;oggetto originale (Campo di collegamento visualizzato nell&#39;oggetto originale) e di un campo di collegamento all&#39;oggetto di destinazione visualizzato nelle schede Campi o Riferimenti dell&#39;oggetto di collegamento. Il campo di collegamento all&#39;oggetto di destinazione visualizzato nell&#39;oggetto di collegamento o il campo di collegamento visualizzato nell&#39;oggetto di collegamento deve corrispondere al campo di destinazione.\
   Ad esempio, l’ID (Progetto) (Campo di collegamento visualizzato nell’oggetto originale) è referenziato da Problemi (oggetto originale). (Portfoli) ownerID (Collegamento del campo all&#39;oggetto di destinazione) viene visualizzato nella scheda Fields del progetto (oggetto di collegamento). OwnerID Portfolio è anche un campo sull&#39;oggetto di destinazione (Portfolio). Il campo di collegamento nell&#39;oggetto di collegamento corrisponde al campo di destinazione.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Utilizzando API Explorer, identifica **Codice oggetto** dell&#39;oggetto di collegamento (Project).\
   Ad esempio, il codice oggetto per Project è PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Creare un filtro per l&#39;oggetto originale.\
   Ad esempio, crea un filtro Problema.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. Incolla il seguente esempio di formula nell’interfaccia della modalità testo del nuovo filtro e sostituisci il testo suggerito con gli oggetti e i campi corretti:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Per un esempio che utilizza i campi identificati in precedenza, vedi [Esempio 1: filtrare i problemi per nome del proprietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in questo articolo.

1. Clic **Salva filtro**.

## Creare filtri in modalità testo complesso per gli oggetti mancanti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Puoi creare un filtro che faccia riferimento a oggetti mancanti. Ad esempio, puoi creare un filtro utenti che mostra quali utenti non hanno effettuato l’accesso a Workfront.

È sempre necessario utilizzare un’ *ESISTE* e l’interfaccia della modalità testo per generare questo filtro.

Per esempi di filtri per gli oggetti mancanti, vedi le sezioni seguenti in questo articolo:

* [Esempio 2: filtro per gli oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Esempio 3: filtro per gli oggetti mancanti: utenti che non registrano il tempo per un determinato periodo di tempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Per creare un filtro che faccia riferimento a oggetti mancanti:

1. Identifica l’oggetto del filtro. Questo oggetto viene definito oggetto originale.\
   Ad esempio, Parametro o Campo personalizzato.
1. Identifica il campo in base al quale desideri filtrare. Questo oggetto viene definito campo di destinazione e appartiene a un oggetto di destinazione.\
   Ad esempio, il campo categoryID (campo di destinazione) che appartiene a Categoria (oggetto di destinazione).
1. Poiché l&#39;oggetto originale (Parameter) e il campo di destinazione (categoryID) non sono collegati direttamente tra loro, è necessario trovare un terzo oggetto, un oggetto di collegamento (Parametro categoria), che li connette. L&#39;oggetto di collegamento deve disporre di almeno un campo a cui si fa riferimento dalle schede Campi o Riferimenti dell&#39;oggetto originale (Campo di collegamento visualizzato nell&#39;oggetto originale) e di un campo di collegamento all&#39;oggetto di destinazione visualizzato nelle schede Campi o Riferimenti dell&#39;oggetto di collegamento. Il campo di collegamento all&#39;oggetto di destinazione visualizzato nell&#39;oggetto di collegamento o il campo di collegamento visualizzato nell&#39;oggetto di collegamento deve corrispondere al campo di destinazione.\
   Ad esempio, l&#39;ID del parametro Categoria (campo di collegamento visualizzato nell&#39;oggetto originale) è indicato da Parametro (oggetto originale). parameterID (Collegamento di un campo all’oggetto Target) viene visualizzato nella scheda Fields del parametro Category (Collegamento di un oggetto). Il campo di collegamento all&#39;oggetto di destinazione visualizzato nell&#39;oggetto di collegamento corrisponde al campo di destinazione.
1. Utilizzando API Explorer, identifica **Codice oggetto** dell&#39;oggetto di collegamento (parametro di categoria).\
   Ad esempio, il codice oggetto per il parametro di categoria è CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Creare un filtro per l&#39;oggetto originale.\
   Ad esempio, crea un filtro Parametro.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. (Facoltativo) Se si applica un filtro per gli oggetti mancanti, incollare il seguente esempio di formula nell&#39;interfaccia della modalità testo del nuovo filtro e sostituire il testo suggerito con gli oggetti e i campi corretti:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Per un esempio di reporting sui campi personalizzati non associati a Custom Forms, vedi [Esempio 2: filtro per gli oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) in questo articolo.

1. Clic **Salva filtro**.

## Esempi di filtri in modalità testo che si estendono su più livelli nella gerarchia degli oggetti

* [Esempio 1: filtrare i problemi per nome del proprietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Esempio 2: filtro per gli oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Esempio 3: filtro per gli oggetti mancanti: utenti che non registrano il tempo per un determinato periodo di tempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Esempio 4: filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard allineamento Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Esempio 1: filtrare i problemi per nome del proprietario del Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Utilizzando l’interfaccia in modalità testo, puoi creare un filtro per un elenco di problemi in modo da visualizzare solo i problemi che si trovano su progetti associati a un portfolio il cui proprietario è un utente specifico.

Per filtrare i problemi in base al nome del proprietario del Portfolio:

1. Creare un filtro Problema.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. Fai riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Incolla il seguente codice in **Impostare le regole di filtro per il report** area in cui sostituire il codice generico precedente:
   <pre>ESISTE:A:$$OBJCODE=PROJ<br>ESISTE:A:ID=FIELD:projectID<br>ESISTE:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* L’oggetto originale è l’oggetto del rapporto: Issue
   >* L&#39;oggetto di destinazione è Portfolio.
   >* L&#39;oggetto di collegamento è Progetto.
   >* Il campo di destinazione e il campo di collegamento all&#39;oggetto di destinazione a cui si fa riferimento dall&#39;oggetto di collegamento sono ownerID.
   >* Il codice oggetto dell&#39;oggetto di collegamento è PROJ.
   >* Il campo di collegamento visualizzato nell&#39;oggetto originale è projectID e il campo di collegamento è ID.

1. Sostituisci il valore del campo di destinazione (ownerID) nell’ultima istruzione con un ID utente del tuo ambiente.
1. Clic **Salva filtro**.

### Esempio 2: filtro per gli oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Tramite l’interfaccia in modalità testo, puoi creare un filtro per visualizzare i campi personalizzati (parametri) non associati a Forms personalizzato (categorie). Questo filtro collega i parametri alle categorie, che sono connesse tramite un altro oggetto, Parametro categoria. Poiché i due campi non sono collegati direttamente tra loro e si filtrano le informazioni mancanti, è necessario utilizzare un&#39;istruzione EXISTS.

>[!IMPORTANT]
>
>Un parametro è un campo esistente nella libreria dei campi a cui si fa riferimento in un modulo personalizzato. Un parametro di categoria è la versione di un campo visualizzato in un modulo specifico. Se ad esempio lo stesso campo viene visualizzato in 5 moduli, nel database di Workfront saranno presenti 1 Parametro e 5 Parametri Categoria.

Per filtrare i campi personalizzati non associati a un modulo personalizzato:

1. Crea un filtro Parametro o Campo personalizzato.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. Fai riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Incolla il seguente codice in **Impostare le regole di filtro per il report** area in cui sostituire il codice generico precedente:
   <pre>ESISTE:A:$$OBJCODE=CTGYPA<br>ESISTE:A:parameterID=FIELD:ID<br>ESISTE:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* L&#39;oggetto originale è l&#39;oggetto del report: Parameter.
   >* L&#39;oggetto di destinazione è Categoria.
   >* L&#39;oggetto di collegamento è il parametro di categoria.
   >* Il codice Object dell&#39;oggetto di collegamento è CTGYPA.
   >* Il campo di collegamento all&#39;oggetto di destinazione è parameterID perché esiste sia nella tabella oggetto di collegamento che nella tabella oggetto di destinazione.
   >* Il campo di collegamento visualizzato nell&#39;oggetto originale è ID (del parametro Categoria).

1. Clic **Salva filtro**.

### Esempio 3: filtro per gli oggetti mancanti: utenti che non registrano il tempo per un determinato periodo di tempo {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Tramite l’interfaccia in modalità testo, puoi creare un filtro per visualizzare gli utenti che non hanno registrato il tempo per un determinato periodo di tempo. Questo filtro collega gli utenti alle ore, che sono collegate direttamente tra loro. Tuttavia, è necessario utilizzare un&#39;istruzione EXISTS e l&#39;interfaccia della modalità testo per poter filtrare le informazioni mancanti.

Per filtrare gli utenti che non hanno registrato l&#39;ora durante la settimana scorsa:

1. Creare un filtro Utente.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. Fai riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Incolla il seguente codice in **Impostare le regole di filtro per il report** area in cui sostituire il codice generico precedente:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* L’oggetto originale è l’oggetto del rapporto: Utente.
   >* L&#39;oggetto di destinazione è Ora.
   >* In questo esempio non è necessario un oggetto di collegamento perché Utenti e Ore sono connessi direttamente nel database di Workfront.
   >* Poiché non è presente alcun oggetto di collegamento, è necessario utilizzare il codice oggetto dell&#39;oggetto di destinazione: HOUR.
   >* Il campo di collegamento all&#39;oggetto di destinazione è ownerID (visualizzato sull&#39;oggetto originale, mentre l&#39;oggetto di collegamento risulta mancante).
   >* Il campo di collegamento visualizzato sull&#39;oggetto originale è ID (dell&#39;ora) (viene visualizzato sull&#39;oggetto di destinazione, mentre l&#39;oggetto di collegamento risulta mancante).
   >* ESISTE:A:L&#39;istruzione entryDate fa riferimento ai campi che definiscono l&#39;oggetto di destinazione (Hour) e utilizza la stessa sintassi utilizzata in un&#39;istruzione di filtro regolare. In questo modo, verranno visualizzati solo gli utenti che non hanno registrato il tempo per un periodo di tempo specifico, in questo caso la settimana precedente.
   >* Il modificatore NOTEXISTS indica che si stanno cercando elementi (ore) che non esistono per l’oggetto del rapporto (Utenti).

1. Clic **Salva filtro**.

### Esempio 4: filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard allineamento Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Utilizzando l’interfaccia in modalità testo, puoi creare un filtro che fa riferimento a più di un campo sull’oggetto di destinazione. In questo caso, le istruzioni di filtro che fanno riferimento ai campi di destinazione devono essere collegate da AND.

È ad esempio possibile filtrare un elenco di attività in modo da visualizzare solo le attività che soddisfano i criteri seguenti:

* Si trovano in un progetto associato a un portfolio il cui proprietario è un utente specifico.
* Si trovano in un progetto associato a un portfolio i cui progetti non sono associati a una scorecard di allineamento specifica.

Per filtrare le attività in base al nome del proprietario del Portfolio e all’ID della scorecard di allineamento del Portfolio:

1. Crea un filtro Attività.\
   Per informazioni sulla creazione di filtri, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clic **Passa alla modalità testo**.
1. Incolla il seguente codice in **Impostare le regole di filtro per il report** area:
   <pre>ESISTE:A:$$OBJCODE=PROJ<br>ESISTE:A:ID=FIELD:projectID<br>ESISTE:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>E:A:ESISTE:A:$$EXISTSMOD=NOTEXISTS<br>E:A:ESISTE:A:$$OBJCODE=PROJ<br>E:A:ESISTE:A:ID=FIELD:projectID<br>E:A:ESISTE:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* L&#39;oggetto originale è l&#39;oggetto del filtro: Task.
   >* L&#39;oggetto di destinazione è Portfolio.
   >* Il primo campo di destinazione è ownerID.
   >* Il secondo campo di destinazione è l’ID della scorecard di allineamento.
   >* L&#39;oggetto di collegamento è Progetto.
   >* Il codice oggetto dell&#39;oggetto di collegamento è PROJ.
   >* Il campo di collegamento all’oggetto di destinazione è l’ID (del Portfolio).
   >* Il campo di collegamento visualizzato nell&#39;oggetto originale è projectID.
   >* Sostituisci ownerID con un ID utente del tuo ambiente.

1. Clic **Salva filtro**.
