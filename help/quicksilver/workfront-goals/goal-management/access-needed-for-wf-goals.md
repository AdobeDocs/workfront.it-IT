---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisiti per l’utilizzo degli obiettivi di Workfront
description: Prima di poter accedere agli obiettivi di Adobe Workfront Adobe Workfront, l’amministratore deve verificare che alcune condizioni siano soddisfatte. In questo articolo, scopri i requisiti di accesso, autorizzazioni e layout per accedere agli Obiettivi di Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Requisiti per l’utilizzo degli obiettivi di Workfront

<!--Audited P&P only: 04/2025-->

Prima di poter accedere agli obiettivi di Adobe Workfront Adobe Workfront, l’amministratore deve verificare che siano soddisfatte tutte le seguenti condizioni:

* La tua organizzazione ha acquistato in passato un pacchetto Adobe Workfront Goals. Adobe Workfront Goals non è più disponibile per l’acquisto.

  Per ulteriori informazioni, vedere la sezione [Ottenere l&#39;accesso all&#39;organizzazione per gli obiettivi di Workfront](#obtain-workfront-goals-organization-access) in questo articolo.

* Assegnare il tipo corretto di licenza Workfront. Per informazioni sull&#39;assegnazione dei tipi di licenza e dei livelli di accesso, vedere la sezione [Aggiornare i tipi di licenza e le impostazioni dei livelli di accesso](#update-license-types-and-access-level-settings) in questo articolo.

  >[!NOTE]
  >
  >Gli utenti con un tipo di licenza External non possono accedere agli obiettivi di Workfront.

* Ti consente di accedere agli Obiettivi nel tuo livello di accesso. Per informazioni, consulta [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

  >[!NOTE]
  >
  >Per impostazione predefinita, gli utenti non hanno accesso agli obiettivi nel loro livello di accesso.


* Assegnate un modello di layout che includa l&#39;area Obiettivi nel menu principale.

  >[!NOTE]
  >
  >A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l&#39;area Obiettivi nel menu principale.

  Per informazioni, vedere la sezione [Aggiungere obiettivi Workfront a un modello di layout](#add-workfront-goals-to-a-layout-template) in questo articolo.

* Se devi modificare obiettivi che non hai creato personalmente, il creatore dell’obiettivo deve condividerli con te e concederti le autorizzazioni di gestione.

  Per informazioni, vedere la sezione [Condividere singoli obiettivi con altri utenti](#share-individual-goals-with-other-users) in questo articolo.

## Ottenere l’accesso all’organizzazione Workfront Goals {#obtain-workfront-goals-organization-access}

L’ultimo pacchetto Adobe Workfront che includeva gli Obiettivi di Workfront era Adobe Workfront Ultimate.
Workfront Goals non è più disponibile per l’acquisto di pacchetti più recenti.
Rivolgiti al rappresentante del tuo account per informazioni sugli obiettivi di Workfront.

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Aggiornare i tipi di licenza e le impostazioni del livello di accesso  {#update-license-types-and-access-level-settings}

Se la società ha accesso agli obiettivi di Workfront da un acquisto precedente, l’amministratore Workfront deve concederti quanto segue per accedere agli obiettivi di Workfront:

1. Una delle seguenti licenze:

   * Collaboratore o versione successiva
   * Richiedi o superiore

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. Il seguente livello di accesso:

   * Visualizzare o accedere più facilmente agli Obiettivi nel proprio livello di accesso.

   Per informazioni sull&#39;accesso agli obiettivi, vedere [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

In qualità di amministratore di Workfront, puoi rivedere il numero di licenze Workfront Goals nel tuo sistema e capire quante sono attualmente abilitate. Per ulteriori informazioni, consulta [Gestire le licenze disponibili nel sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront consente di assegnare più licenze Workfront Goals acquistate. Tuttavia, quando si assegnano più licenze di quelle consentite dal contratto Workfront Goals, un account manager Workfront contatterà l&#39;utente per informarlo del superamento del numero di contratto.

## Aggiungere obiettivi Workfront a un modello di layout {#add-workfront-goals-to-a-layout-template}

L’amministratore del Workfront o del gruppo deve assegnarti un modello di layout che includa l’area Obiettivi nel menu principale, in modo da poter accedere agli Obiettivi di Workfront.

![Modello di layout](assets/layout-template-align-highlighted-350x220.png)

L’amministratore di Workfront o l’amministratore di gruppo può anche aggiungere quanto segue al modello di layout per accedere facilmente a Obiettivi di Workfront:

* Una linguetta bloccata
* Imposta l’area Obiettivi come pagina di destinazione

Per informazioni sull’aggiornamento del modello di layout, consulta i seguenti articoli:

* [Creare e gestire modelli di layout](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personalizzare il menu principale utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personalizzare le pagine bloccate utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personalizzare la pagina di destinazione utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Assegnare utenti a un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Condividere singoli obiettivi con altri utenti {#share-individual-goals-with-other-users}

Per impostazione predefinita, tutti gli utenti che hanno almeno accesso in visualizzazione agli obiettivi nel proprio livello di accesso possono visualizzare tutti gli obiettivi in Workfront.

Qualsiasi utente con l’accesso di modifica agli obiettivi può creare gli obiettivi e ottenere automaticamente l’accesso di gestione agli obiettivi creati. Se devono modificare gli obiettivi di altri utenti, qualcuno con le autorizzazioni di gestione per tali obiettivi deve condividere con loro gli obiettivi che non ha creato.

Per informazioni sulla condivisione degli obiettivi con gli utenti e sull&#39;assegnazione delle relative autorizzazioni di gestione, vedere [Condividere un obiettivo in Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
