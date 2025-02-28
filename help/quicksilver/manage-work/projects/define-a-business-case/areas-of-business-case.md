---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Panoramica delle aree del Business Case
description: Questo articolo descrive le aree del Business Case di un progetto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 2%

---

# Panoramica delle aree del Business Case

Questo articolo descrive le aree del Business Case di un progetto.

Per informazioni sulla creazione di un Business Case per un progetto, vedere [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L’amministratore di Adobe Workfront o l’amministratore di gruppo deve abilitare tutte le sezioni nel Business Case prima che siano visibili nel progetto, ad eccezione della sezione Informazioni progetto. La sezione Informazioni progetto è attivata per impostazione predefinita.

Per ulteriori informazioni sull&#39;abilitazione delle aree del Business Case, vedere la sezione &quot;Business Case&quot; in  [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Di seguito sono riportate le aree nel Business Case di un progetto:

* Info Prog
* Obiettivi
* Spese
* Budget di risorse
* Rischi
* Scorecard
* Moduli personalizzati
* Riassunto del Business Case

## Info Prog

L&#39;area **Informazioni progetto** del caso di business non è configurabile dall&#39;amministratore di Workfront. Tutti i progetti hanno un&#39;area Informazioni progetto nel Business Case. 

La sezione Informazioni progetto del caso di business include le informazioni di base di un progetto, prima che il progetto sia effettivamente iniziato.

Prendi in considerazione la modifica dei seguenti campi:

* **Descrizione**: specifica una descrizione per il progetto.
* **Proprietario progetto**

  Per impostazione predefinita, l’utente che crea il progetto è anche proprietario del progetto. Puoi modificare questo campo e indicare un altro utente attivo come proprietario del progetto.

* **Sponsor Progetto**

  Valuta l’aggiunta di un utente diverso dal proprietario del progetto come sponsor del progetto. Lo sponsor riceve l&#39;approvazione del Business Case. 

* **Portfolio**: specificare un Portfolio per il progetto. È necessario creare il Portfolio e impostarlo sullo stato **Attivo** prima che sia disponibile per la selezione in questo menu a discesa.

  Per ulteriori informazioni sui portfolio, vedere [Panoramica di Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Per ulteriori informazioni sulla creazione di portafogli, vedere [Creare un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Vantaggio pianificato**: stimare il beneficio monetario previsto per l&#39;organizzazione al completamento del progetto. Può essere qualsiasi quantità di valuta e deve essere un valore positivo. Ad esempio, $10.000.
* **Stato**: per impostazione predefinita, lo Stato di una richiesta di progetto è impostato su **Idea**.

  Se si modifica lo stato in un elemento diverso da Idea o Planning, il pulsante **Invia** scompare dall&#39;area Riepilogo caso di business e non è più possibile inviare il caso di business per l&#39;approvazione. 

* **Data di inizio fissata**: specifica la data di inizio desiderata per il progetto.
* **Data di fine fissata**: specifica la data di fine del progetto.

  >[!NOTE]
  >
  >Le date di inizio e di fine fisse nel caso di business non influiscono sulle date di inizio e di completamento pianificate del progetto. Queste rappresentano le date richieste dal creatore del progetto per lo sviluppo ottimale dello stesso. Le date di inizio pianificata e di completamento pianificata del progetto mostrano invece la sequenza temporale pianificata per il progetto, basata sulle attività del progetto stesso.

## Obiettivi

Gli obiettivi definiscono gli obiettivi del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla. Questo campo visualizza gli obiettivi in ordine di priorità.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Puoi creare obiettivi strategici per la tua organizzazione che non sono collegati al singolo caso di business di un progetto. Per poter creare obiettivi strategici, devi poter accedere agli obiettivi di Adobe Workfront. Puoi quindi collegarli a progetti al di fuori dei loro casi aziendali. Per informazioni sulla creazione di obiettivi utilizzando gli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

La definizione degli obiettivi è facoltativa per il progetto che deve ricevere un Punteggio in Portfolio Optimizer. Questa è l&#39;unica sezione facoltativa del Business Case. Prima di assegnare un punteggio al progetto in Portfolio Optimizer, è necessario completare tutte le altre sezioni del Business Case. È possibile indicare un livello di priorità per un obiettivo durante la creazione.

Per ulteriori informazioni sugli obiettivi, consulta  [Crea obiettivi caso di business](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Spese

Le spese rappresentano i costi non di manodopera che potrebbero essere sostenuti durante la durata di un progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla. 

Tutte le spese inserite nel Business Case vengono inoltre immesse nella scheda Spese del progetto, come Spese pianificate.

Le spese interessano i seguenti campi del progetto:

* Bdg prv
* Valore Netto

Per ulteriori informazioni sui costi preventivati e i valori netti, vedere [Panoramica sui campi finanziari del caso aziendale](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Per ulteriori informazioni sulle spese, consulta  [Gestione spese progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

L’amministratore di Workfront può impostare tipi di spesa personalizzati.

Per ulteriori informazioni sulla creazione di tipi di spesa personalizzati, vedere [Creare tipi di spesa personalizzati](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Budget di risorse

Nell&#39;area Budget risorse del caso aziendale è possibile eseguire le azioni riportate di seguito.

* Associa i gruppi di risorse al progetto.
* Preventivare le risorse a livello di progetto.

Le ore preventivate per le risorse del progetto vengono visualizzate nell&#39;area Budget risorse del caso aziendale, generando il costo manodopera preventivato del progetto. Questa area del Business Case è attivata per impostazione predefinita.

Per ulteriori informazioni sulle risorse di budget per il progetto nel Business Case, vedere [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![Impostazione budget risorse caso di business](assets/business-case-sp-selected-with-choose-button-350x121.png)

Quando si visualizza la sezione Budget risorse del caso aziendale, tenere presente quanto segue:

* È possibile preventivare le informazioni sulle risorse utilizzando i seguenti strumenti:

   * Pianificazione risorse

     Per informazioni, vedere [Risorse preventivate nel Business Case utilizzando la pianificazione risorse](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Scenario Planner , se la società ha acquistato una licenza aggiuntiva per Adobe Scenario Planner

     Per ulteriori informazioni, vedere [Risorse budget nel caso di business utilizzando la Pianificazione scenario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

* Le informazioni visualizzate qui vengono visualizzate anche nella Programmazione delle risorse o nella Pianificazione degli scenari a livello di sistema. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Dopo aver impostato le risorse nel budget, il Costo manodopera preventivato del progetto viene visualizzato nell&#39;area Budget risorse se i ruoli sono associati alle tariffe Costo per ora. Il Costo manodopera preventivato viene visualizzato nella valuta del progetto.

  >[!IMPORTANT]
  >
  >Il Costo manodopera preventivato è il costo associato ai ruoli nel progetto e non agli utenti. La somma di tutti i costi manodopera preventivati per gli utenti può essere uguale o meno al costo manodopera preventivato della mansione associata agli utenti. 

  Per ulteriori informazioni sul costo manodopera preventivato, vedere [Panoramica dei campi finanziari del caso aziendale](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Per ulteriori informazioni sulla creazione di mansioni e sull&#39;associazione delle tariffe del costo orario, vedere [Creare e gestire mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Rischi

I rischi sono fattori che possono impedire a un progetto di terminare in tempo o nel rispetto del budget. La definizione di questi fattori è importante perché Portfolio Manager o lo sponsor del progetto possano prendere una decisione consapevole sull&#39;approvazione del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla.

È possibile associare un costo potenziale ai rischi che si stanno definendo nel caso in cui si verifichino. Il costo dei rischi di un progetto influisce sul valore netto del progetto. 

Per ulteriori informazioni sul valore netto del progetto, vedere [Panoramica dei campi finanziari del caso aziendale](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Per ulteriori informazioni sulla creazione di rischi, consulta  [Crea e modifica rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

L’amministratore di Workfront può impostare tipi di rischio personalizzati.

Per ulteriori informazioni sulla creazione e la modifica di tipi di rischio personalizzati, vedere [Modificare e creare tipi di rischio](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Le scorecard misurano l’allineamento del progetto. Questa area è abilitata per impostazione predefinita nel Business Case, ma l’amministratore di Workfront potrebbe scegliere di non visualizzarla.

Per ulteriori informazioni sull&#39;applicazione di una scorecard a un progetto e sulla generazione di un punteggio di allineamento, vedere [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Per applicare una scorecard, l’amministratore di Workfront deve crearne una. L&#39;area **Scorecard** del Business Case non viene visualizzata a meno che non venga creata una scorecard.

Per ulteriori informazioni sulla creazione di una scorecard, consulta  [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Moduli personalizzati

Quando definisci un caso di business, puoi allegare un Forms personalizzato a un progetto. Per impostazione predefinita, quest&#39;area non è abilitata nel Business Case. L&#39;amministratore di Workfront deve abilitarlo per la visualizzazione nel Business Case.

Per ulteriori informazioni sull&#39;abilitazione delle aree del caso di business, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per applicare un modulo personalizzato, l’amministratore di Workfront deve innanzitutto crearne uno personalizzato.

Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

È possibile utilizzare i moduli personalizzati per raccogliere informazioni aggiuntive non visualizzate negli altri campi del Business Case.

Per ulteriori informazioni sull&#39;applicazione di un modulo personalizzato, vedere [Allegare un modulo personalizzato a un caso aziendale](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Riassunto del Business Case

* [Panoramica del riepilogo del caso di business](#overview-of-the-business-case-summary)
* [Esportare il Business Case](#export-the-business-case)

### Panoramica del Business Case Summary {#overview-of-the-business-case-summary}

Nel pannello Riepilogo caso di business, nell&#39;angolo superiore destro del caso di business, è possibile visualizzare un riepilogo dei principali dati finanziari del progetto e se un progetto è allineato o meno con una scorecard.

Non è possibile modificare il Riepilogo caso di business. Questa è solo una rapida visualizzazione dello stato del progetto in quanto si riferisce ai campi finanziari e alla scorecard. \
 

Nel Riepilogo caso di business vengono visualizzati i campi riportati di seguito.

* Valore netto progetto
* Costo preventivato progetto
* Il Costo Potenziale Del Rischio
* Il beneficio pianificato
* Punteggio di allineamento

Per ulteriori informazioni su questi campi, vedere [Panoramica dei campi finanziari del caso aziendale](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Esportare il Business Case {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

È possibile esportare il Business Case in un file PDF, nel caso sia necessario stamparlo o allegarlo a un&#39;e-mail in un formato più compatto. 

Per informazioni, vedere [Esportare il Business Case di un progetto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

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
