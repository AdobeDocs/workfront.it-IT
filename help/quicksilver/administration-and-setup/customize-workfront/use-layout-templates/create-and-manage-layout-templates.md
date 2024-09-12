---
title: Creare e gestire modelli di layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: In qualità di amministratore di Workfront o di un gruppo, puoi creare e modificare modelli di layout per personalizzare gli elementi di layout in Workfront per i tuoi utenti.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 1%

---

# Creare e gestire modelli di layout

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Adobe Workfront o di un gruppo, puoi creare e modificare modelli di layout per personalizzare i seguenti elementi di layout in Workfront per i tuoi utenti:

* Menu principale
* Pannello di navigazione a sinistra
* Area Home
* Visualizzazioni, filtri e raggruppamenti utilizzati dagli utenti con elenchi e rapporti.
* Terminologia su schermo
* Intestazioni di progetti, attività e problemi

Dopo aver creato o modificato un modello di layout, è possibile assegnarlo a singoli utenti, team, gruppi o mansioni.

Il layout Workfront predefinito di ogni utente dipende dal livello di accesso e dal tipo di licenza. Ad esempio, alcuni utenti potrebbero non visualizzare alcune aree nel menu principale. Per ulteriori informazioni, vedere [Informazioni sul layout predefinito di Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p>
  <p> Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per la creazione e la gestione di modelli di layout

* Gli utenti possono personalizzare alcune aree del proprio layout. Quando si modifica un modello di layout, le modifiche vengono unite alle personalizzazioni apportate senza sovrascriverle o reimpostarle. Ciò si verifica anche se si assegnano gli utenti a un nuovo modello di layout.
* Gli amministratori di gruppi e gli utenti con una licenza Pianificazione che possono modificare altri utenti possono aggiungere modelli di layout a livello di sistema e di gruppo agli utenti che possono gestire durante la modifica del profilo.
* Gli amministratori di gruppi non possono assegnare modelli di layout a mansioni o team.

Per ulteriori informazioni sui modelli layout, vedere [Modelli layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Creare o modificare un modello di layout

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Interfaccia** > **Modelli di layout**.

1. Fare clic su **Nuovo modello di layout**.

   Oppure

   Fare clic sul nome del modello di layout che si desidera modificare.

1. Se si sta creando un nuovo modello di layout, digitare un **Nome modello di layout** e (facoltativo) una **Descrizione**.

1. Personalizza le aree dell’interfaccia utente, come descritto nei seguenti articoli:

   * [Personalizzare il menu principale utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizzare il pannello sinistro utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizzare le pagine bloccate utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizza la home e il riepilogo utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizzare la pagina di destinazione utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizzare la terminologia dell’interfaccia utente utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continua a testare il modello di layout e a renderlo disponibile agli utenti, come descritto negli articoli seguenti:

   * [Verifica un nuovo modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Concedere l&#39;accesso amministrativo per un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Assegnare utenti a un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>È inoltre possibile creare un modello di layout copiandolo e modificandone la copia. Per ulteriori informazioni, vedere [Copiare un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

