---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisiti per l’utilizzo degli obiettivi di Workfront
description: Prima di poter accedere agli obiettivi di Adobe Workfront Adobe Workfront, l’amministratore deve verificare che alcune condizioni siano soddisfatte.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Requisiti per l’utilizzo degli obiettivi di Workfront

Prima di poter accedere agli obiettivi di Adobe Workfront Adobe Workfront, l’amministratore deve verificare che siano soddisfatte tutte le seguenti condizioni:

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* La tua organizzazione deve acquistare la licenza corretta per gli obiettivi Workfront. Per informazioni, consulta la sezione [Ottenere l’accesso all’organizzazione Workfront Goals](#obtain-workfront-goals-organization-access)in questo articolo.

* Assegnare il tipo corretto di licenza Workfront. Per informazioni sull’assegnazione dei tipi di licenza e dei livelli di accesso, consulta la sezione [Aggiornare i tipi di licenza e le impostazioni del livello di accesso](#update-license-types-and-access-level-settings) in questo articolo.

>[!NOTE]
>
>Gli utenti con un tipo di licenza External non possono accedere agli obiettivi di Workfront.

* Ti consente di accedere agli Obiettivi nel tuo livello di accesso. Per informazioni, consulta [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Assegnate un modello di layout che includa l&#39;area Obiettivi nel menu principale.

  >[!NOTE]
  >
  >A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale.

  Per informazioni consulta la sezione [Aggiungere obiettivi Workfront a un modello di layout](#add-workfront-goals-to-a-layout-template) in questo articolo.

* Se devi modificare obiettivi che non hai creato personalmente, il creatore dell’obiettivo deve condividerli con te e concederti le autorizzazioni di gestione.

  Per informazioni, consulta la sezione [Condividere singoli obiettivi con altri utenti](#share-individual-goals-with-other-users) in questo articolo.

## Ottenere l’accesso all’organizzazione Workfront Goals {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

La tua organizzazione deve acquistare una licenza aggiuntiva, oltre alla licenza Workfront, per consentire agli utenti di accedere agli obiettivi di Workfront. Dopo che la tua organizzazione ha acquistato la licenza aggiuntiva, Workfront abilita Workfront Goals per il tuo account. Per informazioni sull&#39;acquisto di una licenza per Workfront Goals, contattare l&#39;account manager Workfront.

## Aggiornare i tipi di licenza e le impostazioni del livello di accesso  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

L&#39;amministratore di Workfront deve concedere uno dei seguenti tipi di licenza Workfront per accedere agli obiettivi di Workfront:

* Piano
* Lavoro
* Revisiona
* Richiesta

Dopo che l’amministratore di Workfront ti ha concesso uno di questi tipi di licenza, devi anche darti accesso agli Obiettivi nel tuo livello di accesso. Per informazioni sull’accesso agli obiettivi, consulta [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

In qualità di amministratore di Workfront, puoi rivedere il numero di licenze Workfront Goals nel tuo sistema e capire quante sono attualmente abilitate. Per ulteriori informazioni, consulta [Gestire le licenze disponibili nel sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront consente di assegnare più licenze Workfront Goals acquistate. Tuttavia, quando si assegnano più licenze di quelle consentite dal contratto Workfront Goals, un account manager Workfront contatterà l&#39;utente per informarlo del superamento del numero di contratto.

## Aggiungere obiettivi Workfront a un modello di layout {#add-workfront-goals-to-a-layout-template}

L’amministratore del Workfront o del gruppo deve assegnarti un modello di layout che includa l’area Obiettivi nel menu principale, in modo da poter accedere agli Obiettivi di Workfront.

![](assets/layout-template-align-highlighted-350x220.png)

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

Per informazioni sulla condivisione degli obiettivi con gli utenti e sull’assegnazione delle relative autorizzazioni di gestione, consulta [Condividere un obiettivo in Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
