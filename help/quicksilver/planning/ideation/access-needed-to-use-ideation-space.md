---
title: Accesso necessario per utilizzare lo spazio ideazioni
description: Adobe Workfront Planning ora offre una funzionalità aggiuntiva da ideare prima di avviare le campagne. Sfrutta la potenza dell’intelligenza artificiale per trasformare dati e input diretti in piani tangibili e fornire ai team un punto di partenza informato invece di una pagina vuota con spazio di ideazione Adobe.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: cf783443d618874e1241d91895bcc78d78db23df
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%
---

# Accesso necessario per utilizzare lo spazio ideazione

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning ora offre una funzionalità aggiuntiva da ideare prima di avviare le campagne. Sfrutta la potenza dell’intelligenza artificiale per trasformare dati e input diretti in piani tangibili e fornire ai team un punto di partenza informato invece di una pagina vuota con spazio di ideazione Adobe.

In questo articolo vengono descritti l&#39;accesso e le autorizzazioni necessarie per accedere allo spazio di ideazione da Workfront Planning.

Per informazioni generali sullo spazio ideazione, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Requisiti del prodotto


Lo spazio Ideazione non è un prodotto standalone, ma una funzionalità aggiuntiva di Adobe Workfront Planning.

Puoi accedere allo spazio Ideazione se l’organizzazione e i pacchetti a cui hai accesso sono i seguenti, a seconda di quando accedi allo spazio Ideazione:

* Durante il rilascio di Open Beta, è necessario disporre dei seguenti elementi:

  * Un pacchetto Adobe Workfront Workflow con un pacchetto Workfront Planning

* Dopo il rilascio della disponibilità generale, è possibile che si verifichi una delle seguenti condizioni:

  * Un pacchetto Adobe Workfront Workflow con un pacchetto Workfront Planning
  * Adobe Workfront Planning come prodotto standalone

Per informazioni sulle fasi di rilascio dello spazio ideazione, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

>[!NOTE]
>
>Lo spazio ideazione è accessibile solo dal menu principale di Adobe Workfront o da Workfront Planning. Non è necessario un accesso separato per accedere allo spazio ideazione. È immediatamente disponibile se è possibile accedere a Workfront.

<!--
No longer the case: 

Your organization must purchase a package for the following products to access the Ideation space: 

* An Adobe Workfront Workflow package in addition to a Planning package

    Or
    
    An Adobe Workfront Planning purchased as a standalone product. 
* An Adobe GenStudio for Performance Marketing license

    >[!TIP]
    >
    >GenStudio for Performance Marketing is needed to have access to the correct font entitlements. 

-->

<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Requisiti del livello di accesso di Workfront Planning

L’accesso allo spazio delle idee è configurato in Workfront.

Per accedere a Ideation Space, il livello di accesso a Workfront deve includere quanto segue:

* Una licenza Flusso di lavoro standard, quando la società ha acquistato un pacchetto Flusso di lavoro in aggiunta a un pacchetto Pianificazione.
* Una licenza di Planning standard, quando la società ha acquistato con un flusso di lavoro e un pacchetto di Planning, oppure un prodotto di Workfront Planning come prodotto standalone.
* L’impostazione Disable Ideation space (Disabilita spazio ideazione) nella sezione Set additional restrictions (Imposta restrizioni aggiuntive) del livello di accesso deve essere deselezionata. <!--***********check the UI for this***********-->

## Requisiti delle autorizzazioni di Workfront Planning

Ogni record Planning è collegato a un breve nello spazio Ideazione.

Le autorizzazioni di descrizione dello spazio ideazione vengono ereditate dalle autorizzazioni dei record di Workfront Planning. <!--not sure if this is right, because now you can share the ideation with others??-->

Per creare record è necessario disporre delle autorizzazioni di gestione per un tipo di record in Planning per poter creare o modificare un record nello spazio di ideazione.

Gli utenti di Planning con autorizzazioni di visualizzazione sui record possono visualizzare lo spazio di ideazione di un record.

Nella tabella seguente viene illustrata la connessione tra le autorizzazioni dei record di Workfront Planning e le autorizzazioni della descrizione breve dello spazio di ideazione:

| Autorizzazione a livello di record di pianificazione | Autorizzazioni di breve livello per lo spazio ideazione |
|---|---|
| Gestire le autorizzazioni per un record | Può creare un breve nello spazio ideazione del record |
| Visualizzare le autorizzazioni di un record | È in grado di leggere il resoconto di tale record nello spazio ideazione, ma non di modificarlo |

## Autorizzazioni per lo spazio ideazioni

<!--this is also duplicated in the intro of the Share an ideation space article-->

Le autorizzazioni di pianificazione vengono trasferite nello spazio di ideazione di un record.

Inoltre, puoi assegnare ad altri utenti le autorizzazioni per utilizzare lo spazio delle idee e aggiungervi idee.

Considera i seguenti aspetti:

* I creatori di idee hanno sempre i permessi editor per le proprie idee.

* È necessario disporre delle autorizzazioni di editor per uno spazio di ideazione per creare resoconti brevi ed esportarli in altre applicazioni.

Di seguito sono riportate le autorizzazioni per lo spazio di ideazione e le funzionalità offerte:

| Autorizzazione per spazio ideazione | Funzionalità |
|---|---|
| Editor | Può modificare, scaricare e condividere lo spazio delle idee |
| Commentatore | Può visualizzare e commentare lo spazio delle ideazioni |
| Visualizzatore | Può visualizzare lo spazio delle ideazioni |

Per ulteriori informazioni sulla condivisione di uno spazio delle idee, vedere [Condividere uno spazio delle idee](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--
there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users
-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
