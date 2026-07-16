---
title: Panoramica di Adobe Workfront Planning Access
description: Non tutti gli utenti dell’organizzazione dispongono dello stesso accesso e delle stesse autorizzazioni per utilizzare Adobe Workfront Planning. Questo articolo descrive l'accesso e le autorizzazioni che gli utenti potrebbero avere per utilizzare le funzionalità di Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QuLxjUMlRgN0FvlDwR0JVQ-m-wV-z3C6sh30lJYRKfU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ab0d036ea3bbcdad2daaed6b09864272fd1beb11
workflow-type: tm+mt
source-wordcount: 1010
ht-degree: 3%

---

# Panoramica sull’accesso a Pianificazione di Adobe Workfront

<!--do not use the snippet for IMPORTANT , as it links to this article-->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning. Workfront Planning è un prodotto standalone o una funzionalità acquistata in più da Adobe Workfront.
>
>
>Questo articolo contiene informazioni generali su Workfront Planning quando i clienti acquistano anche un pacchetto Workfront o Workflow.
>
>Per l&#39;elenco completo degli articoli che contengono la documentazione per Workfront Planning, vedere [Informazioni generali e indice degli articoli per Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Per informazioni su Workfront Planning come prodotto autonomo, vedere [Introduzione ad Adobe Workfront Planning come prodotto autonomo](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Questo articolo descrive l&#39;accesso e le impostazioni necessarie per utilizzare le funzionalità di Workfront Planning.

## Requisiti di accesso

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Per utilizzare Workfront Planning, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
   <tr>
   <tr>
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi pacchetto Workfront o Workflow Planning
   e qualsiasi pacchetto di Workfront Planning</p>
   <p><b>NOTA</b></p>
   <p>Per accedere ai tipi di record collegabili:</p>
   <ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning</p></li>
   <li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime e Ultimate</p></li></ul>

<p>Per accedere ai tipi di record globali:</p>
   <ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
   <li><p>Qualsiasi pacchetto Workflow e un pacchetto Planning Prime e Ultimate</p></li></ul> </td></tr>
   <!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
   </tr>
   -->
   <tr>
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td>
   <td>
   <ul><li><p>Qualsiasi flusso di lavoro e qualsiasi licenza Planning, per visualizzare le informazioni di Workfront Planning</p></li>
   <li><p>Uno standard di workflow e uno standard di pianificazione, per creare aree di lavoro e visualizzazioni</p></li></ul>
    </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Qualsiasi flusso di lavoro e qualsiasi tipo di licenza Planning nel livello di accesso</p>  
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td>
   <td>
   <ul>
   <li><p>Visualizzare o modificare le autorizzazioni per le aree di lavoro, i tipi di record e le visualizzazioni che non sono stati creati per accedervi e i relativi oggetti.</p></li>
   <li><p>Autorizzazioni di Contribute o superiori per aree di lavoro e tipi di record non creati per modificarli e creare, modificare o eliminare tipi di record.</p></li>
   <li><p><span class="preview">Consente di gestire le autorizzazioni per i record per modificarli, condividerli o eliminarli.</p>
   <li><p>Autorizzazioni Contribute (Contribute) o superiori per le visualizzazioni non create, per modificarle, eliminarle e condividerle</p>
   </li>
    <li><p>Gli amministratori di Planning possono gestire le aree di lavoro che non hanno creato. </p></li>
    <li><p>Gli amministratori di Planning non possono accedere alle viste che non hanno creato. </p></li></ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> 
   <p>Per impostazione predefinita, gli utenti e gli amministratori di Planning Standard dispongono delle aree Planning abilitate.</p>
   <p> Agli utenti con una licenza Workflow Light o Planning Contributor deve essere assegnato un modello di layout che includa l'opzione Planning nelle seguenti aree:</p>
   <ul><li>Menu principale</li>
   <li>Pannello a sinistra di progetti, portfolio e programmi</li>
   </ul>   
   </td>
  </tr>
 </tbody>
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Livelli di accesso e licenze di Workfront Planning

È possibile assegnare a un utente una licenza di amministratore di Planning quando lo si aggiunge a Adobe Admin Console come amministratore.

Per informazioni, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Non è possibile modificare il livello di accesso Amministratore di Planning in Workfront Planning.

Quando si configurano i livelli di accesso in Workfront, è possibile assegnare i seguenti tipi di licenza:

* Tipi di licenze del flusso di lavoro
* Tipi di licenze Planning

Per accedere a Workfront Planning, agli utenti devono essere assegnati entrambi i tipi di licenza al proprio livello di accesso.

È possibile assegnare le seguenti licenze Planning a un livello di accesso:

* **Planning Standard**: concedere agli utenti questo accesso se devono creare e gestire tutti gli oggetti Planning senza essere amministratori.
* **Collaboratore Planning**: concedere agli utenti questo accesso se devono contribuire ai record ma non devono creare oggetti Planning.

  >[!TIP]
  >
  >Il tipo di licenza Collaboratore Planning non è disponibile se l&#39;organizzazione ha acquistato un numero di licenze Workflow e Planning diverso.


* **Nessuno**: quando si assegna questo tipo di licenza Planning, si rimuove in modo specifico l&#39;accesso Planning agli utenti assegnati a questo livello di accesso.

  >[!IMPORTANT]
  >
  >Le licenze Planning e le licenze Workflow collaborano per consentire agli utenti di accedere a Workfront.
  >
  >È possibile assegnare a un utente diversi livelli di accesso tra Workflow e Planning, ma la licenza Workflow non può essere inferiore alla licenza Planning.
  >
  >Ad esempio, è possibile assegnare a un utente una licenza Workflow Standard e una licenza Planning Contributor, ma non una licenza Workflow Contributor e una licenza Planning Standard.
  >
  >Il tipo di licenza Flusso di lavoro non può essere vuoto se l&#39;utente deve accedere a Workflow o Planning.

Per ulteriori informazioni, vedere [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Configurare il livello di accesso

Per informazioni sulla configurazione dell&#39;accesso in Workfront, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Assegna licenze agli utenti

È possibile assegnare le licenze agli utenti quando si assegna loro un livello di accesso durante la modifica o la creazione.

Per informazioni, vedere [Modifica profilo utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Concedere le autorizzazioni

In Workfront Planning è possibile concedere autorizzazioni alle seguenti entità:

* Aree di lavoro
* Tipi di record
* Viste
* Record

Per ulteriori informazioni, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Il tipo di licenza Adobe Workfront funziona con il tipo di licenza Workfront Planning e le autorizzazioni Planning per consentire l&#39;accesso alla visualizzazione, al contributo o alla gestione degli oggetti Workfront Planning.

Per informazioni su come i tipi di licenza influiscono sui livelli di autorizzazione per gli oggetti di Workfront Planning, vedere [Panoramica sui tipi di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Condividere l&#39;area Planning utilizzando un modello di layout

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema nelle seguenti aree:

* Menu principale
* Pannello a sinistra di progetti, portfolio o programmi

Se si dispone di un&#39;altra licenza Workfront e si desidera contribuire al lavoro di Workfront Planning, è necessario che l&#39;amministratore di sistema aggiunga le aree Pianificazione.

L&#39;amministratore può aggiungere l&#39;opzione Pianificazione alle seguenti aree modificando e assegnando l&#39;utente a un modello di layout:

* Menu principale
* Pagina di destinazione
* Pannello a sinistra per progetti, portfolio e programmi
* Pin

Per aggiungere o rimuovere aree di Workfront Planning dagli utenti dell&#39;istanza di Workfront:

1. Accedi a **Workfront** come amministratore Workfront.

1. Vai a **Menu principale** > **Configurazione** > **Interfaccia** > **Modelli di layout** e apri o crea un modello di layout.

   Per informazioni sulla personalizzazione di un modello di layout, vedere [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Assegnare il modello di layout agli utenti che si desidera abbiano accesso a Workfront Planning.

   Per informazioni, vedere [Assegnare gli utenti a un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Tutti gli utenti assegnati al modello ora possono accedere a Workfront Planning nel loro menu principale.

   Gli utenti possono iniziare a creare workspace, tipi di record, record e campi.


