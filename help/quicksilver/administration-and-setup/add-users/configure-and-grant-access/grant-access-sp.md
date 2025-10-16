---
title: Concedi l'accesso a Pianificazione scenario
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a Scenario Planner.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Concedere l’accesso a Scenario Planner

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente a Scenario Planner, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Oltre all&#39;accesso a Scenario Planner, un utente con un livello di accesso diverso da Amministratore di sistema deve avere accesso anche ai dati finanziari per visualizzare tutte le informazioni finanziarie contenute in un piano, ad esempio budget, costi e tassi di ruolo. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacchetto Adobe Workfront</p> </td> 
   <td>Business o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per Adobe Workfront Scenario Planner.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore alla Pianificazione scenario</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per un piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
