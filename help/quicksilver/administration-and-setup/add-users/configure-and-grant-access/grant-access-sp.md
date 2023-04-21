---
title: Concedere l'accesso a Scenario Planner
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a Planner scenario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Concedere l&#39;accesso a Scenario Planner

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a Planner scenario, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Oltre ad accedere a Scenario Planner, un utente con un livello di accesso non amministratore di sistema deve avere accesso ai dati finanziari per visualizzare tutte le informazioni finanziarie contenute in un piano, ad esempio budget, costi e tassi di ruolo del lavoro. Per ulteriori informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Aziende o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Rivedi o superiore. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Panoramica sulle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per Adobe Workfront Scenario Planner per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere Workfront Scenario Planner, consulta <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Accesso necessario per utilizzare il planner dello scenario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Visualizza l'accesso o una versione successiva al Planner scenario</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Richiedere l'accesso a un piano nel Planner scenario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare l&#39;accesso dell&#39;utente a Scenario Planner utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’opzione a destra di **Pianificazione scenario** da utilizzare per questo livello di accesso.

   >[!NOTE]
   >
   >Il tipo di licenza Esterno o Richiedi non consente l&#39;accesso Visualizza o Modifica a Planner scenario.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

## Accesso a Scenario Planner per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con il Planner scenario, consulta la sezione [Area planner dello scenario](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso a Planner scenario per impostazione del livello di accesso

Le seguenti informazioni possono essere utili per comprendere come utilizzare le impostazioni del livello di accesso per controllare l&#39;accesso degli utenti alle informazioni in Workfront Scenario Planner.

* [Nessun accesso](#no-access)
* [Visualizza accesso](#view-access)
* [Modifica accesso](#edit-access)

### Nessun accesso {#no-access}

Un utente senza accesso a Planner scenario non può visualizzare l&#39;icona Scenari nel Menu principale quando viene aggiunto al proprio modello di layout, né visualizzare i piani e le iniziative condivisi con tale utente. Se il collegamento a un piano è condiviso con un utente che non ha accesso a Planner scenario, l&#39;utente non può visualizzare o modificare il piano.

### Visualizza accesso {#view-access}

Gli utenti con accesso Visualizza a Planner scenario possono effettuare le seguenti operazioni:

* Vedere l&#39;icona Scenari nel menu principale ![](assets/esp-icon-in-main-menu.png), anche se l’area Piani è vuota a meno che l’utente non faccia clic su un collegamento di piano condiviso da un altro utente.
* Visualizza un piano quando un altro utente condivide il collegamento ad esso.

   Ciò include tutte le informazioni sul ruolo del lavoro nel piano.

   Include inoltre informazioni sui tassi di ruolo e sui costi del piano se l&#39;utente destinatario ha accesso anche ai dati finanziari. Per ulteriori informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Modifica accesso {#edit-access}

Gli utenti con accesso Modifica a Planner scenario possono effettuare le seguenti operazioni:

* Vedere l&#39;icona Scenari nel menu principale ![](assets/esp-icon-in-main-menu.png) e utilizzarlo per accedere ai dati del piano.
* Crea piani.
* Visualizza, modifica ed elimina i piani creati.
* Visualizza, modifica ed elimina i piani a cui gli altri utenti hanno accesso utilizzando un collegamento condiviso.

   Ciò include tutte le informazioni sul ruolo del lavoro in un piano.

   Include inoltre le informazioni sui tassi di ruolo e sui costi del piano se l’utente destinatario ha accesso ai dati finanziari. Per ulteriori informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
