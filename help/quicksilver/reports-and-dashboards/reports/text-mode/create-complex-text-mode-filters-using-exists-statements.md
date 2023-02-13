---
product-area: reporting
navigation-topic: text-mode-reporting
title: Creare filtri complessi in modalità testo utilizzando le istruzioni EXISTS
description: Creare filtri complessi in modalità testo utilizzando le istruzioni EXISTS
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Creare filtri complessi in modalità testo utilizzando le istruzioni EXISTS

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Questo articolo richiede una comprensione approfondita dell’API di Adobe Workfront e dell’interfaccia di reporting in modalità testo. Per informazioni sull’API di Workfront, consulta [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).\
>Per informazioni sull’utilizzo della modalità testo, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Panoramica delle relazioni tra oggetti in Workfront

Tutti gli oggetti sono collegati ad altri oggetti nel database Workfront.

La comprensione della gerarchia e dell’interdipendenza degli oggetti consente di individuare gli oggetti a cui è possibile fare riferimento nei rapporti.

Per informazioni sugli oggetti in Workfront e sulla gerarchia e l’interdipendenza degli oggetti, consulta [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Quando si creano i filtri, è possibile fare riferimento ad altri oggetti collegati all’oggetto del filtro entro 2 livelli di relazione utilizzando l’interfaccia standard di reporting.

Ad esempio, puoi fare riferimento all’ID Portfolio in un filtro per problemi per visualizzare solo i problemi relativi ai progetti associati a un determinato portfolio utilizzando l’interfaccia standard. In questo caso, il portafoglio si trova a 2 livelli di distanza dalle emissioni.

Tuttavia, non puoi fare riferimento al proprietario del Portfolio in un filtro di problemi utilizzando l&#39;interfaccia standard per visualizzare solo i problemi dei progetti associati ai portfolio in cui il proprietario è un utente specifico. È necessario utilizzare la modalità testo per accedere al campo Nome proprietario Portfolio, a tre livelli di distanza dai problemi.

![issue_to_portfolio_owner_right_line_icon.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Per un elenco completo degli oggetti in Workfront, consulta la sezione [Esplora API](../../../wf-api/general/api-explorer.md).

Per informazioni su come navigare in API Explorer e trovare oggetti, consulta [Utilizzo di API Explorer](../../../wf-api/general/using-api-explorer.md).

Quando si creano i filtri, è necessario creare istruzioni complesse nell’interfaccia in modalità testo per fare riferimento a questi tipi di oggetti.

Per informazioni sulla creazione di filtri complessi, consulta la sezione [Panoramica dei filtri in modalità testo complessi che utilizzano istruzioni ESISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) sezione .

## Panoramica dei filtri della modalità testo complessi che utilizzano le istruzioni EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Quando si creano filtri che si estendono su più livelli nella gerarchia degli oggetti o si applicano filtri per gli oggetti mancanti, tenere presente quanto segue:

* È necessario creare filtri complessi quando si desidera fare riferimento a oggetti non direttamente collegati all’oggetto filtro.
* È necessario utilizzare un&#39;istruzione EXISTS per eseguire le operazioni seguenti:

   * Creare filtri che si estendono su più livelli.
   * Creare filtri per cercare oggetti mancanti.\
      Ad esempio, durante la creazione di un rapporto utente, puoi filtrare gli utenti che non hanno eseguito l’accesso per un certo periodo di tempo.

Quando utilizzi istruzioni EXISTS in un filtro, considera le regole seguenti:

* In un filtro EXISTS è possibile fare riferimento a tre oggetti:

   * Oggetto del filtro (Oggetto originale).
   * L&#39;oggetto a cui si desidera fare riferimento nel campo (oggetto Target).
   * L’oggetto che collega gli oggetti originali e di destinazione, nel caso in cui non siano collegati direttamente tra loro (oggetto di collegamento).

* I filtri che utilizzano EXISTS contengono due istruzioni separate collegate da un segno di uguale:

   * L&#39;istruzione prima del segno di uguale fa riferimento all&#39;oggetto a cui si fa riferimento (il collegamento o l&#39;oggetto Target).
   * L&#39;istruzione dopo il segno di uguale si riferisce all&#39;oggetto a cui si fa riferimento (l&#39;oggetto originale).

* Per collegare le istruzioni è necessario utilizzare il codice oggetto dell&#39;oggetto di collegamento.\
   È possibile trovare il codice oggetto di tutti gli oggetti in API Explorer.\
   Per informazioni su API Explorer, consulta la sezione [Esplora API](https://one.workfront.com/s/api-explorer).

* Se manca un oggetto di collegamento perché gli oggetti Originale e Target sono collegati direttamente tra loro, è possibile utilizzare il codice oggetto dell&#39;oggetto di destinazione anziché l&#39;oggetto di collegamento.
* È possibile fare riferimento a più campi (Campi di destinazione) sullo stesso oggetto (Oggetto di destinazione), nel qual caso è necessario collegare le righe che fanno riferimento ai campi tramite AND.\
   Per un esempio di filtro per più campi appartenenti all&#39;oggetto Target, consulta la sezione [Esempio 4: Filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard di allineamento Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) in questo articolo.

* L&#39;unico modificatore supportato per un&#39;istruzione EXISTS è NOTEXISTS.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare i filtri in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare i filtri in un rapporto</p> <p>Gestire le autorizzazioni per un filtro per modificarlo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creazione di filtri in modalità testo complessi che si estendono su più livelli nella gerarchia degli oggetti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

È possibile creare un filtro che faccia riferimento a oggetti su più livelli della gerarchia degli oggetti in cui si trova l’oggetto filtro. Ad esempio, puoi creare un filtro per i problemi relativi a progetti non associati a un determinato proprietario del Portfolio.

Per creare questo filtro è sempre necessario utilizzare un&#39;istruzione EXISTS e l&#39;interfaccia della modalità testo.

Per esempi di filtri, consulta la sezione [Esempio 1: Filtrare i problemi per nome proprietario Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in questo articolo.

Per creare un filtro per più livelli nella gerarchia degli oggetti:

1. Identifica l’oggetto del filtro. Questo oggetto viene definito oggetto originale.\
   Ad esempio, Problema.
1. Identifica il campo per il quale desideri filtrare. Questo oggetto è il campo di destinazione che appartiene a un oggetto Target.\
   Ad esempio, il campo ownerID (Campo Target) che appartiene al Portfolio (Oggetto Target).
1. (Condizionale) Se l&#39;oggetto originale (problema) e il campo di destinazione (ownerID) non sono direttamente collegati tra loro, è necessario trovare un terzo oggetto, un oggetto di collegamento (Project), che li connette. L’oggetto di collegamento deve avere almeno un campo a cui viene fatto riferimento dalle schede Campi o Riferimenti dell’oggetto originale (Campo di collegamento visualizzato sull’oggetto originale) e deve inoltre disporre di un campo di collegamento all’oggetto di destinazione visualizzato nelle schede Campi o Riferimenti dell’oggetto di collegamento. Il campo di collegamento all’oggetto di destinazione visualizzato sull’oggetto di collegamento (o sul campo di collegamento visualizzato sull’oggetto di collegamento) deve corrispondere al campo di destinazione.\
   Ad esempio, l’ID (Progetto) (Campo di collegamento visualizzato sull’oggetto originale) è referenziato da Issues (Oggetto originale). (Portfolio) ownerID (Campo di collegamento all’oggetto Target) viene visualizzato nella scheda Campi del progetto (Oggetto di collegamento). L&#39;ID proprietario del Portfolio è anche un campo dell&#39;oggetto Target (Portfolio). Il campo di collegamento sull’oggetto di collegamento corrisponde al campo di destinazione.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Utilizzando l&#39;API Explorer, identificare il **Codice oggetto** dell&#39;oggetto di collegamento (Project).\
   Ad esempio, il codice oggetto per Project è PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Crea un filtro per l’oggetto originale.\
   Ad esempio, crea un filtro Problema.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. Incolla l’esempio di formula seguente all’interfaccia in modalità testo del nuovo filtro e sostituisci il testo suggerito con gli oggetti e i campi corretti:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Per un esempio utilizzando i campi precedentemente identificati, consulta la sezione [Esempio 1: Filtrare i problemi per nome proprietario Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) in questo articolo.

1. Fai clic su **Salva filtro**.

## Creazione di filtri della modalità testo complessi per gli oggetti mancanti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

È possibile creare un filtro che faccia riferimento a oggetti mancanti. Ad esempio, puoi creare un filtro utente che mostra gli utenti che non hanno effettuato l’accesso alle ore in Workfront.

Devi sempre utilizzare un *ESISTE* e l&#39;interfaccia della modalità testo per creare questo filtro.

Per esempi di filtri per gli oggetti mancanti, consulta le sezioni seguenti in questo articolo:

* [Esempio 2: Filtro per oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Esempio 3: Filtro per oggetti mancanti: utenti che non hanno effettuato il log time per un certo periodo di tempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Per creare un filtro che faccia riferimento a oggetti mancanti:

1. Identifica l’oggetto del filtro. Questo oggetto viene definito oggetto originale.\
   Ad esempio, Parametro o Campo personalizzato.
1. Identifica il campo per il quale desideri filtrare. Questo oggetto è il campo di destinazione che appartiene a un oggetto Target.\
   Ad esempio, il campo categoryID (Campo di destinazione) che appartiene a Category (Oggetto di destinazione).
1. Poiché l’oggetto originale (Parametro) e il campo di destinazione (categoryID) non sono direttamente collegati tra loro, è necessario trovare un terzo oggetto, un oggetto di collegamento (un parametro di categoria), che li connette. L’oggetto di collegamento deve avere almeno un campo a cui viene fatto riferimento dalle schede Campi o Riferimenti dell’oggetto originale (Campo di collegamento visualizzato sull’oggetto originale) e deve inoltre disporre di un campo di collegamento all’oggetto di destinazione visualizzato nelle schede Campi o Riferimenti dell’oggetto di collegamento. Il campo di collegamento all’oggetto di destinazione visualizzato sull’oggetto di collegamento (o sul campo di collegamento visualizzato sull’oggetto di collegamento) deve corrispondere al campo di destinazione.\
   Ad esempio, l’ID del parametro Category (Campo di collegamento visualizzato sull’oggetto originale) viene referenziato da Parameter(Oggetto originale). parameterID (Linking Field to Target Object) viene visualizzato nella scheda Fields del parametro Category (Collegamento Object). Il campo di collegamento all’oggetto di destinazione visualizzato sull’oggetto di collegamento corrisponde al campo di destinazione.
1. Utilizzando l&#39;API Explorer, identificare il **Codice oggetto** dell’oggetto di collegamento (parametro di categoria).\
   Ad esempio, il codice oggetto per il parametro Category è CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Crea un filtro per l’oggetto originale.\
   Ad esempio, crea un filtro Parametro.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. (Condizionale) Se stai filtrando oggetti mancanti, incolla il seguente esempio di formula nell’interfaccia in modalità testo del nuovo filtro e sostituisci il testo suggerito con gli oggetti e i campi corretti:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Per un esempio di reporting sui campi personalizzati non associati a Custom Forms, consulta [Esempio 2: Filtro per oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) in questo articolo.

1. Fai clic su **Salva filtro**.

## Esempi di filtri in modalità testo che si estendono su più livelli nella gerarchia degli oggetti

* [Esempio 1: Filtrare i problemi per nome proprietario Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Esempio 2: Filtro per oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Esempio 3: Filtro per oggetti mancanti: utenti che non hanno effettuato il log time per un certo periodo di tempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Esempio 4: Filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard di allineamento Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Esempio 1: Filtrare i problemi per nome proprietario Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Utilizzando l’interfaccia in modalità testo, puoi creare un filtro per un elenco di problemi per visualizzare solo i problemi relativi a progetti associati a un portfolio il cui proprietario è un utente specifico.

Per filtrare i problemi in base al nome del proprietario del Portfolio:

1. Crea un filtro Problemi.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. Fare riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Incolla il seguente codice nel **Impostare regole di filtro per il rapporto** area in sostituzione del codice generico di cui sopra:

   <pre>ESISTE:A:$$OBJCODE=PROJ<br>ESISTE:A:ID=FIELD:projectID<br>ESISTE:A:portfolio:proprietarioID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* L&#39;oggetto Originale è l&#39;oggetto del rapporto: Problema
   >* L&#39;oggetto Target è Portfolio.
   >* L&#39;oggetto di collegamento è Project.
   >* Il campo di destinazione e il campo di collegamento all’oggetto di destinazione a cui si fa riferimento dall’oggetto di collegamento è ownerID.
   >* Il codice Object dell&#39;oggetto di collegamento qui è PROJ.
   >* Il campo di collegamento visualizzato sull’oggetto originale è projectID e il campo di collegamento è ID.


1. Sostituisci il valore del campo di destinazione (ownerID) nell’ultima istruzione con un ID utente proveniente dall’ambiente.
1. Fai clic su **Salva filtro**.

### Esempio 2: Filtro per oggetti mancanti: campi personalizzati che non vengono visualizzati in alcun modulo personalizzato {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Utilizzando l’interfaccia in modalità testo, è possibile creare un filtro per visualizzare i campi personalizzati (Parametri) non associati a Custom Forms (Categorie). Questo filtro collega i parametri a Categorie, che sono collegati tramite un altro oggetto, Parametro categoria. Poiché i due campi non sono collegati direttamente tra loro e poiché stai filtrando le informazioni mancanti, devi utilizzare un&#39;istruzione EXISTS.

>[!IMPORTANT]
>
>Un parametro è un campo esistente nella libreria campi a cui fa riferimento in un modulo personalizzato. Un parametro di categoria è la versione di un campo visualizzato in un modulo specifico. Ad esempio, se lo stesso campo viene visualizzato in 5 moduli, nel database Workfront saranno presenti 1 parametro e 5 parametri di categoria.

Per filtrare i campi personalizzati non associati a un modulo personalizzato:

1. Crea un filtro Parametro o Campo personalizzato.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. Fare riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Incolla il seguente codice nel **Impostare regole di filtro per il rapporto** area in sostituzione del codice generico di cui sopra:

   <pre>ESISTE:A:$$OBJCODE=CTGYPA<br>ESISTE:A:parameterID=FIELD:ID<br>ESISTE:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* L&#39;oggetto Originale è l&#39;oggetto del rapporto: Parametro.
   >* L&#39;oggetto Target è Category.
   >* L&#39;oggetto di collegamento è un parametro di categoria.
   >* Il codice Object dell&#39;oggetto di collegamento è CTGYPA.
   >* Il campo di collegamento all’oggetto Target è parameterID perché parameterID esiste sia nella tabella degli oggetti di collegamento che nella tabella degli oggetti di destinazione.
   >* Il campo di collegamento visualizzato sull’oggetto originale è ID (del parametro della categoria).


1. Fai clic su **Salva filtro**.

### Esempio 3: Filtro per oggetti mancanti: utenti che non hanno effettuato il log time per un certo periodo di tempo {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Utilizzando l’interfaccia in modalità testo, puoi creare un filtro per visualizzare gli utenti che non hanno registrato il tempo per un determinato periodo di tempo. Questo filtro collega gli utenti alle ore, che sono collegate direttamente tra loro. Tuttavia, è necessario utilizzare un&#39;istruzione EXISTS e l&#39;interfaccia della modalità testo per filtrare le informazioni mancanti.

Per filtrare gli utenti che non hanno effettuato il log time durante la settimana scorsa:

1. Crea un filtro utente.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. Fare riferimento al seguente codice generico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Incolla il seguente codice nel **Impostare regole di filtro per il rapporto** area in sostituzione del codice generico di cui sopra:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* L&#39;oggetto Originale è l&#39;oggetto del rapporto: Utente.
   >* L&#39;oggetto Target è ora.
   >* In questo esempio non è necessario un oggetto di collegamento perché Utenti e ore sono direttamente connessi nel database Workfront.
   >* Poiché non è presente alcun oggetto di collegamento, è necessario utilizzare il codice oggetto dell’oggetto di destinazione: ORA.
   >* Il campo di collegamento all’oggetto Target è ownerID (visualizzato sull’oggetto originale); l&#39;oggetto di collegamento è mancante).
   >* Il campo di collegamento visualizzato sull’oggetto originale è ID (dell’ora) (che viene visualizzato sull’oggetto di destinazione; manca l&#39;oggetto di collegamento).
   >* ESISTE:A:L&#39;istruzione entryDate si riferisce ai campi che definiscono l&#39;oggetto Target (ora) e utilizza la stessa sintassi di un&#39;istruzione filtro regolare. In questo modo puoi visualizzare solo gli utenti che non hanno effettuato il log time per un periodo di tempo specifico, in questo caso la settimana precedente.
   >* Il modificatore NOTEXISTS indica che stiamo cercando elementi (ore) che non esistono per l’oggetto del rapporto (Utenti).


1. Fai clic su **Salva filtro**.

### Esempio 4: Filtrare per più campi: attività per nome proprietario Portfolio e ID scorecard di allineamento Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Utilizzando l’interfaccia in modalità testo, puoi creare un filtro che fa riferimento a più campi sull’oggetto Target. In questo caso, le istruzioni di filtro che fanno riferimento ai campi di destinazione devono essere collegate da AND.

Ad esempio, è possibile filtrare un elenco di attività per visualizzare solo le attività che soddisfano i criteri seguenti:

* Si trovano in un progetto associato a un portfolio il cui proprietario è un utente specifico.
* Si trovano in un progetto associato a un portfolio i cui progetti non sono associati a una specifica scorecard di allineamento.

Per filtrare le attività in base al nome del proprietario del Portfolio e all’ID della scorecard di allineamento del Portfolio:

1. Crea un filtro Attività.\
   Per informazioni sulla creazione dei filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic su **Passa alla modalità testo**.
1. Incolla il seguente codice nel **Impostare regole di filtro per il rapporto** area:
   <pre>ESISTE:A:$$OBJCODE=PROJ<br>ESISTE:A:ID=FIELD:projectID<br>ESISTE:A:portfolio:proprietarioID=4d80ce520000528787d57807732a33f<br>E:A:ESISTE:A:$$EXISTSMOD=NOTEXISTS<br>E:A:ESISTE:A:$$OBJCODE=PROJ<br>E:A:ESISTE:A:ID=FIELD:projectID<br>E:A:ESISTE:A:portfolio:alignScoreCardID=4da387b0001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* L&#39;oggetto Originale è l&#39;oggetto del filtro: Attività.
   >* L&#39;oggetto Target è Portfolio.
   >* Il primo campo di destinazione è ownerID.
   >* Il secondo campo di destinazione è l’ID della scorecard di allineamento.
   >* L&#39;oggetto di collegamento è Project.
   >* Il codice oggetto dell&#39;oggetto di collegamento è PROJ.
   >* Il campo di collegamento all’oggetto Target è l’ID (del Portfolio).
   >* Il campo di collegamento visualizzato sull&#39;oggetto originale è projectID.
   >* Sostituisci il ownerID con un ID utente proveniente dall’ambiente.


1. Fai clic su **Salva filtro**.
