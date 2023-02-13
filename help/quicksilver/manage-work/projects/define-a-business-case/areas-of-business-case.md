---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Panoramica delle aree del Business Case
description: Questo articolo descrive le aree del Business Case di un progetto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# Panoramica delle aree del Business Case

Questo articolo descrive le aree del Business Case di un progetto.

Per informazioni sulla creazione di un Business Case per un progetto, consulta [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L’amministratore di Adobe Workfront o l’amministratore di gruppo deve abilitare tutte le sezioni del Business Case prima che siano visibili sul progetto, fatta eccezione per la sezione Informazioni progetto . La sezione Informazioni progetto è attivata per impostazione predefinita.

Per ulteriori informazioni sull&#39;abilitazione delle aree del Business Case, vedere la sezione &quot;Business Case&quot; in  [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Di seguito sono elencate le aree nel Business Case di un progetto:

* Info Prog
* Obiettivi
* Spese
* Budget di risorse
* Rischi
* Scorecard
* Moduli personalizzati
* Riassunto del Business Case

## Info Prog

La **Informazioni progetto** l&#39;area del Business Case non è configurabile dall&#39;amministratore Workfront. Tutti i progetti dispongono di un’area Informazioni progetto nel Business Case. 

La sezione Informazioni progetto del Business case include le informazioni di base di un progetto, prima che il progetto sia effettivamente iniziato.

È consigliabile modificare i campi seguenti:

* **Descrizione**: Specifica una descrizione del progetto.
* **Proprietario progetto**

   Per impostazione predefinita, l’utente che crea il progetto è anche il proprietario del progetto. È possibile modificare questo campo e indicare un altro utente attivo come proprietario del progetto.

* **Sponsor Progetto**

   Considera l’aggiunta di un altro utente oltre al proprietario del progetto come sponsor del progetto. Lo sponsor riceve l&#39;approvazione del Business Case. 

* **Portfolio**: Specifica un Portfolio per il progetto. È necessario creare il Portfolio e inserirlo nello stato di **Attivo** prima che sia disponibile per la selezione in questo menu a discesa.

   Per ulteriori informazioni sui portfolio, consulta [Panoramica del Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Per ulteriori informazioni sulla creazione di Portfoli, consulta [Creare un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Vantaggio pianificato**: Stimare quale sarà il beneficio monetario previsto per la tua organizzazione al termine del progetto. Può essere un qualsiasi ammontare di valuta e deve essere un valore positivo. Ad esempio $10.000.
* **Stato**: Per impostazione predefinita, lo stato di una richiesta di progetto è impostato su **Idea**.

   Se si modifica lo stato in un valore diverso da Idea o Pianificazione, la proprietà **Invia** Il pulsante scompare dall&#39;area Sintetico casi aziendali e non è più possibile inviare il Business Case per l&#39;approvazione. 

* **Data di inizio fissa**: Specifica la data di inizio del progetto.
* **Data di fine fissa**: Specifica la data in cui vuoi che il progetto termini.

   >[!NOTE]
   >
   >Le date di inizio e fine fisse nel caso aziendale non influiscono sulle date di inizio e di completamento pianificate del progetto. Questi rappresentano le date richieste dal creatore del progetto per il momento in cui il progetto si svilupperebbe idealmente. Le date di inizio e di completamento pianificati del progetto mostrano invece la tempistica pianificata per il progetto, in base alle attività del progetto.

## Obiettivi

Gli obiettivi definiscono gli obiettivi del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla. In questo campo vengono visualizzati gli obiettivi in ordine di priorità.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
Puoi creare obiettivi strategici per la tua organizzazione che non sono collegati al singolo Business Case di un progetto. Devi avere accesso agli obiettivi di Adobe Workfront per poter creare obiettivi strategici. Puoi quindi collegarli a progetti esterni ai rispettivi casi aziendali. Per informazioni sulla creazione di obiettivi utilizzando gli obiettivi di Workfront, vedi [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

La definizione degli obiettivi è facoltativa per il progetto per ricevere un punteggio in Portfoli Optimizer. Questa sezione è l’unica sezione facoltativa nel Business Case. Tutte le altre sezioni del Business Case devono essere completate prima che il progetto venga valutato in Portfoli Optimizer. È possibile indicare un livello di priorità per un obiettivo durante la creazione dell&#39;obiettivo.

Per ulteriori informazioni sugli obiettivi, vedi  [Creare gli obiettivi del caso aziendale](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Spese

Le spese rappresentano i costi non lavorativi che potrebbero essere sostenuti durante la durata di un progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla. 

Tutte le spese inserite nel Business Case vengono inoltre inserite nella scheda Spese del progetto, come Spese pianificate.

Le spese influiscono sui seguenti campi del progetto:

* Bdg prv
* Valore Netto

Per ulteriori informazioni sui costi preventivati e sui valori netti, vedere [Panoramica dei campi finanziari del Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Per ulteriori informazioni sulle spese, vedi  [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

L&#39;amministratore Workfront può impostare tipi di spesa personalizzati.

Per ulteriori informazioni sulla creazione di tipi di spesa personalizzati, consulta [Crea tipi di spesa personalizzati](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Budget di risorse

È possibile eseguire le azioni seguenti nell&#39;area Resource Budgeting del caso Business:

* Associa pool di risorse al progetto.
* Budget delle risorse a livello di progetto.

Le ore previste in budget per le risorse nel progetto vengono visualizzate nell&#39;area Budget risorse del Business Case, generando il costo del lavoro a budget del progetto. Questa area del Business Case è attivata per impostazione predefinita.

Per ulteriori informazioni sulle risorse di budget per il progetto nel Business Case, vedi [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Quando si visualizza la sezione Resource Budgeting del Business Case, tenere presente quanto segue:

* Puoi eseguire il budget delle informazioni sulle risorse qui utilizzando i seguenti strumenti:

   * Planner risorse

      Per informazioni, consulta [Risorse di budget nel Business Case utilizzando il Resource Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Scenario Planner : se la tua azienda ha acquistato una licenza aggiuntiva per Adobe Scenario Planner

      Per ulteriori informazioni, consulta [Risorse di budget nel caso aziendale utilizzando il Planner scenario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

* Le informazioni visualizzate qui vengono visualizzate anche nel Planner risorse o nel Planner scenario a livello di sistema. 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Dopo aver impostato il budget per le risorse, nell&#39;area Budget risorse viene visualizzato il costo manodopera a budget del progetto se i ruoli sono associati ai tassi Costo per ora. Il costo del lavoro a budget viene visualizzato nella valuta del progetto.

   >[!IMPORTANT]
   Il costo del lavoro a budget è il costo associato ai ruoli del progetto e non agli utenti. La somma di tutti i costi del lavoro a budget per gli utenti può essere uguale o meno al costo del lavoro a budget del ruolo del lavoro associato agli utenti. 

   Per ulteriori informazioni sul costo del lavoro a budget, vedere [Panoramica dei campi finanziari del Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   Per ulteriori informazioni sulla creazione di ruoli di lavoro e sull&#39;associazione dei tassi di costo per ora con essi, vedere [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Rischi

I rischi sono fattori che potrebbero impedire il completamento di un progetto in tempo o in budget. La definizione di questi fattori è importante per il responsabile del Portfolio o il promotore del progetto per prendere una decisione istruita sull&#39;approvazione del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla.

È possibile associare un costo potenziale ai rischi che si definiscono nel caso in cui si verifichino. Il costo dei rischi di un progetto influisce sul valore netto del progetto. 

Per ulteriori informazioni sul valore netto del progetto, consulta [Panoramica dei campi finanziari del Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Per ulteriori informazioni sulla creazione dei rischi, consulta  [Creare e modificare i rischi relativi ai progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Il tuo amministratore Workfront può impostare tipi di rischio personalizzati.

Per ulteriori informazioni sulla creazione e la modifica di tipi di rischio personalizzati, consulta [Modificare e creare tipi di rischio](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Le scorecard misurano l’allineamento del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla.

Per ulteriori informazioni sull’applicazione di una scorecard a un progetto e sulla generazione di un punteggio di allineamento, consulta [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Per applicare una scorecard, è necessario crearne una all’amministratore Workfront. La **Scorecard** l&#39;area del Business Case viene visualizzata solo se viene creata una scorecard.

Per ulteriori informazioni sulla creazione di una scorecard, vedi  [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Moduli personalizzati

Puoi allegare Forms personalizzato a un progetto durante la definizione di un caso aziendale. Questa area non è abilitata per impostazione predefinita nel Business Case. L’amministratore di Workfront deve abilitarlo per visualizzarlo nel Business Case.

Per ulteriori informazioni sull&#39;abilitazione delle aree del Business Case, vedere [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per applicare un modulo personalizzato, è innanzitutto necessario che l’amministratore di Workfront crei un modulo personalizzato.

Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

È possibile utilizzare moduli personalizzati per raccogliere informazioni aggiuntive non visualizzate negli altri campi del Business Case.

Per ulteriori informazioni sull’applicazione di un modulo personalizzato, vedere [Allegare un modulo personalizzato a un business case](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Riassunto del Business Case

* [Panoramica del sintetico del caso aziendale](#overview-of-the-business-case-summary)
* [Esportare il Business Case](#export-the-business-case)

### Panoramica del sintetico del caso aziendale {#overview-of-the-business-case-summary}

Puoi visualizzare un riepilogo delle finanze del progetto principale e se un progetto è allineato o meno con una scorecard nel pannello Riepilogo del caso commerciale, nell’angolo in alto a destra del Business Case .

Non è possibile modificare il sintetico del caso aziendale. Questa è solo una rapida visualizzazione dello stato del progetto in quanto si riferisce ai campi finanziari e alla scorecard. \
 

I campi seguenti vengono visualizzati nel riepilogo del Business Case:

* Valore netto del progetto
* Costo preventivato del progetto
* Costo potenziale del rischio
* Il beneficio previsto
* Punteggio di allineamento

Per ulteriori informazioni su questi campi, consulta [Panoramica dei campi finanziari del Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Esportare il Business Case {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

È possibile esportare il Business Case in un file PDF, nel caso sia necessario stamparlo o allegarlo a un&#39;e-mail in un formato più compatto. 

Per informazioni, consulta [Esportare il Business Case di un progetto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
