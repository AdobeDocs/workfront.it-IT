---
title: Concedi l'accesso a Pianificazione scenario
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a Scenario Planner.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Concedere l’accesso a Scenario Planner

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente a Scenario Planner, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Oltre all&#39;accesso a Scenario Planner, un utente con un livello di accesso diverso da Amministratore di sistema deve avere accesso anche ai dati finanziari per visualizzare tutte le informazioni finanziarie contenute in un piano, ad esempio budget, costi e tassi di ruolo. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Business o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Rivedi o superiore. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Panoramica licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per Adobe Workfront Scenario Planner per accedere alle funzionalità descritte in questo articolo.</p> <p>Per informazioni su come ottenere Workfront Scenario Planner, vedere <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Accesso necessario per utilizzare Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o superiore alla Pianificazione scenario</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Richiedere l'accesso a un piano in Pianificazione scenario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Configurare l&#39;accesso degli utenti a Scenario Planner mediante un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fare clic sull&#39;opzione a destra di **Pianificazione scenario** che si desidera utilizzare per questo livello di accesso.

   >[!NOTE]
   >
   >Il tipo di licenza Request (Richiesta) o External (Esterno) non consente l’accesso View (Visualizzazione) o Edit (Modifica) a Scenario Planner (Pianificazione scenario).

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

## Accesso a Scenario Planner per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con Scenario Planner, vedere la sezione [Area di Scenario Planner](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) nell&#39;articolo [Funzionalità disponibili per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso a Scenario Planner per impostazione del livello di accesso

Di seguito sono riportate alcune informazioni utili per comprendere come utilizzare le impostazioni del livello di accesso per controllare l&#39;accesso degli utenti alle informazioni in Workfront Scenario Planner.

* [Nessun accesso](#no-access)
* [Accesso visualizzazione](#view-access)
* [Modifica accesso](#edit-access)

### Nessun accesso {#no-access}

Un utente che non ha accesso a Scenario Planner non può visualizzare l’icona Scenari nel menu principale quando viene aggiunta al proprio modello di layout, né visualizzare i piani e le iniziative condivisi con lui. Se il collegamento a un piano è condiviso con un utente che non ha accesso alla Pianificazione scenario, l&#39;utente non può visualizzare o modificare il piano.

### Visualizza accesso {#view-access}

Gli utenti con accesso in visualizzazione a Scenario Planner possono effettuare le seguenti operazioni:

* Vedere l&#39;icona Scenari nel menu principale ![](assets/esp-icon-in-main-menu.png), anche se l&#39;area Piani è vuota a meno che l&#39;utente non faccia clic su un collegamento di piano condiviso da un altro utente.
* Visualizzare un piano quando un altro utente condivide il collegamento ad esso.

  Ciò include tutte le informazioni sui ruoli nel piano.

  Sono inoltre incluse le tariffe per le mansioni e le informazioni sui costi del piano se l&#39;utente destinatario ha accesso anche ai dati finanziari. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Modifica accesso {#edit-access}

Gli utenti con l’accesso in Modifica a Scenario Planner possono effettuare le seguenti operazioni:

* Vedere l&#39;icona Scenari nel menu principale ![](assets/esp-icon-in-main-menu.png) e utilizzarla per accedere ai dati del piano.
* Creare piani.
* Visualizzare, modificare ed eliminare i piani creati.
* Visualizzare, modificare ed eliminare i piani di altri utenti a cui accedono utilizzando un collegamento condiviso.

  Ciò include tutte le informazioni sui ruoli in un piano.

  Se l&#39;utente destinatario ha accesso ai dati finanziari, vengono inoltre incluse le tariffe per le mansioni e le informazioni sui costi del piano. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
