---
title: Accesso necessario per utilizzare lo spazio ideazioni
description: Adobe Workfront Planning ora offre una funzionalità aggiuntiva da ideare prima di avviare le campagne. Sfrutta la potenza dell’intelligenza artificiale per trasformare dati e input diretti in piani tangibili e fornire ai team un punto di partenza informato invece di una pagina vuota con spazio di ideazione Adobe.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%
---

# Accesso necessario per utilizzare lo spazio ideazione

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambito del programma **Ideation Space Beta**. </span>

<span class="preview">Per ulteriori informazioni, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning ora offre una funzionalità aggiuntiva da ideare prima di avviare le campagne.

Quando utilizzi Ideation Space, puoi sfruttare le funzionalità di conversazione di Adobe Enterprise CX Coworker per trasformare dati e input diretti in piani tangibili e fornire ai team un punto di partenza informato, anziché una pagina vuota.

In questo articolo vengono descritti l&#39;accesso e le autorizzazioni necessarie per accedere allo spazio di ideazione da Workfront Planning.

Per informazioni generali sullo spazio ideazione, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Requisiti del prodotto

Lo spazio Ideazione non è un prodotto standalone, ma una funzionalità aggiuntiva di Adobe Workfront Planning.

Puoi accedere allo spazio Ideazione se l’organizzazione dispone dei seguenti prodotti:

* Adobe Workfront con Workfront Planning
* CX Coworker aziendale

A seconda che si acceda allo spazio Ideazione, è necessario avere accesso ai seguenti pacchetti:

* Durante il rilascio di Open Beta, è necessario disporre dei seguenti elementi:

  * Un pacchetto Adobe Workfront Workflow con un pacchetto Workfront Planning

* Dopo il rilascio della disponibilità generale, è possibile che si verifichi una delle seguenti condizioni:

  * Un pacchetto Adobe Workfront Workflow con un pacchetto Workfront Planning
  * Adobe Workfront Planning come prodotto standalone

>[!NOTE]
>
>Lo spazio ideazione è accessibile solo dal menu principale di Workfront o da Workfront Planning. Non è necessario un accesso separato per accedere allo spazio ideazione. È immediatamente disponibile se è possibile accedere a Workfront.

Per informazioni sulle fasi di rilascio dello spazio ideazione, vedere [Introduzione allo spazio ideazione per Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).


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

## Requisiti di sistema e livello di accesso

L’accesso allo spazio per le idee è configurato in Workfront attivando una combinazione di impostazioni a livello di sistema e di livello di accesso.

Per accedere allo spazio ideazione in Workfront sono necessarie le seguenti impostazioni:

* Attivare le impostazioni delle preferenze di Collaboratore e MCP nell&#39;area Preferenze di sistema di Configura <!--check the UI because Becky was going to change it-->

  Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

  >[!IMPORTANT]
  >
  >CX Enterprise Coworker non è attualmente disponibile per le organizzazioni del settore sanitario, finanziario o di altri settori con dati sensibili. L’Assistente AI è disponibile per queste organizzazioni. Tuttavia, lo spazio Ideazione non è disponibile per i clienti Workfront che non dispongono di CX Coworker.

* Deseleziona l’impostazione Disattiva spazio ideazione nella sezione Imposta restrizioni aggiuntive del livello di accesso.

  >[!TIP]
  >
  >In qualità di amministratore di Workfront, puoi limitare l’accesso allo spazio Ideazione a determinati utenti deselezionando l’impostazione Disattiva spazio ideazione nel loro livello di accesso.

  Per informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisiti di licenza

Per accedere a Ideation Space, il livello di accesso a Workfront deve includere i seguenti tipi di licenza:

* Una licenza Flusso di lavoro standard, quando la società ha acquistato un pacchetto Flusso di lavoro in aggiunta a un pacchetto Pianificazione.
* Una licenza di Standard Planning, quando la società ha acquistato uno dei seguenti prodotti:

  * Un flusso di lavoro e un pacchetto Planning, durante la versione beta aperta
  * Un flusso di lavoro e un pacchetto Planning oppure un prodotto Workfront Planning come prodotto standalone, dopo la disponibilità generale.

## Requisiti delle autorizzazioni di Workfront

Quando si utilizza lo spazio di ideazione da Workfront Planning, ogni record di Planning viene connesso a un breve in spazio di ideazione.

Le autorizzazioni di descrizione dello spazio ideazione vengono ereditate dalle autorizzazioni dei record di Workfront Planning. <!--not sure if this is right, because now you can share the ideation with others??-->

Per creare o modificare un record nello spazio di ideazione, è necessario disporre delle autorizzazioni Contribute o di livello superiore per un tipo di record in Planning.

Gli utenti di Planning con autorizzazioni di visualizzazione sui record possono visualizzare lo spazio di ideazione di un record.

Nella tabella seguente viene illustrata la connessione tra le autorizzazioni dei record di Workfront Planning e le autorizzazioni della descrizione breve dello spazio di ideazione:

| Autorizzazione a livello di record di pianificazione | Autorizzazioni di breve livello per lo spazio ideazione |
|---|---|
| Autorizzazioni di contribuzione o superiori per un record | Può creare un breve nello spazio ideazione del record |
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
