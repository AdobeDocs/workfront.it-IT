---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitazioni di visualizzazione di Programmazione delle risorse
description: Per migliorare le prestazioni, Adobe Workfront limita la quantità di informazioni che è possibile visualizzare e la quantità di informazioni che è possibile esportare dalla Programmazione delle risorse.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Limitazioni della visualizzazione di Programmazione delle risorse

Per migliorare le prestazioni, Adobe Workfront limita la quantità di informazioni che è possibile visualizzare e la quantità di informazioni che è possibile esportare dalla Programmazione delle risorse.

Quando si avvicina questo limite, Workfront visualizza un messaggio di avviso per comunicare che si è raggiunto tale limite.

Se le informazioni che si prevede di visualizzare nella Programmazione delle risorse non vengono visualizzate, è possibile che si stia tentando di visualizzare troppe informazioni e che alcuni dati non siano stati visualizzati a causa di questa limitazione.

Per prestazioni ottimali nella visualizzazione e nell&#39;esportazione della Programmazione delle risorse, si consiglia quanto segue:

* Utilizzare i filtri per ridurre la quantità di informazioni visualizzate nella Programmazione delle risorse e visualizzare solo le informazioni pertinenti.
* Utilizzare tutte le opzioni di esportazione per ridurre la quantità di informazioni esportate contemporaneamente e per assicurarsi di esportare solo le informazioni pertinenti.\
  Per ulteriori informazioni sull&#39;utilizzo dei filtri e sulle opzioni di esportazione nella Programmazione risorse, vedere [Informazioni sui filtri nella Programmazione risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Per informazioni sull&#39;esportazione di informazioni dalla Programmazione delle risorse, vedere [Esportare informazioni dalla Programmazione delle risorse](../../resource-mgmt/resource-planning/export-resource-planner.md).

La quantità di informazioni che è possibile visualizzare o esportare dipende dalla vista applicata e dall&#39;ambiente utilizzato per accedere alla Programmazione delle risorse.

## Limitazioni nella vista Progetto

Quando si applica la vista Progetto alla Programmazione risorse, tenere presente quanto segue:

* Puoi visualizzare solo i progetti che hai accesso per gestire.
* È possibile espandere ogni progetto per visualizzare i ruoli associati e ogni ruolo per visualizzare gli utenti associati.

  Puoi visualizzare fino a 300 progetti scorrendo l’elenco fino alla fine, a meno che non siano presenti più di 30.000 righe di progetti, ruoli e utenti. Viene quindi visualizzato un messaggio di avvertenza per indicare che è stato raggiunto il limite di 30.000 righe.

* Puoi visualizzare tre o quattro periodi di tempo alla volta, a seconda delle dimensioni dello schermo.

Dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati, considera quanto segue durante l’esportazione delle informazioni dalla vista Progetto della Programmazione delle risorse:

* Quando si sceglie di esportare tutto (progetti, ruoli e utenti) nella Programmazione delle risorse, tutti gli oggetti che corrispondono ai criteri vengono visualizzati nel file esportato, indipendentemente dal fatto che sia stato eseguito lo scorrimento verso la parte inferiore dell&#39;elenco per visualizzarli o meno.
* Le righe senza informazioni di allocazione vengono incluse nel file esportato.

* Puoi esportare fino a 30.000 righe.

## Limitazioni nella vista Ruolo

Quando applichi la vista Ruolo alla Programmazione delle risorse, dopo aver applicato tutti i filtri appropriati, considera quanto segue:

* Puoi visualizzare solo i ruoli associati ai progetti che puoi gestire.

* Puoi visualizzare fino a 300 ruoli quando scorri verso la parte inferiore dell’elenco, a meno che non siano presenti più di 30.000 righe di ruoli, progetti e utenti. Viene quindi visualizzato un messaggio di avvertenza per indicare che è stato raggiunto il limite di 30.000 righe per ciò che è possibile visualizzare sullo schermo.
* Puoi espandere ogni ruolo per visualizzare un elenco di progetti e ogni progetto per visualizzare un elenco di utenti che possono svolgere tali ruoli nei progetti.

  Per impostazione predefinita vengono visualizzati 20 progetti e puoi utilizzare l’opzione Carica altro per visualizzare altri progetti oppure scorri sotto ogni progetto per caricare altri utenti.

* Puoi visualizzare tre o quattro periodi di tempo, a seconda delle dimensioni dello schermo.

Dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati, considera quanto segue durante l’esportazione delle informazioni dalla vista Ruolo della Programmazione delle risorse:

* Quando si sceglie di esportare tutto (ruoli, progetti e utenti) nella Programmazione delle risorse, tutti gli oggetti che corrispondono ai criteri vengono visualizzati nel file esportato, indipendentemente dal fatto che sia stato eseguito lo scorrimento verso la parte inferiore dell&#39;elenco per visualizzarli o meno.
* Le righe senza informazioni di allocazione vengono incluse nel file esportato.
* Puoi esportare fino a 30.000 righe.

## Limitazioni nella vista utente

Quando si applica la vista Utente alla Programmazione delle risorse, tenere presente quanto segue:

* Puoi visualizzare tutti gli utenti che soddisfano i seguenti criteri:

   * Accesso alla visualizzazione
   * Sono attivi
   * Hai effettuato l’accesso almeno una volta.

* Puoi espandere ogni utente per visualizzare i progetti associati e ogni progetto per visualizzare i ruoli associati.\
  I primi 50 progetti e ruoli vengono visualizzati per impostazione predefinita ed è possibile utilizzare l’opzione Carica altro per visualizzare ulteriori progetti o ruoli.

  >[!NOTE]
  >
  >Se l&#39;elenco degli utenti è stato filtrato in base ai progetti, è possibile espandere solo gli utenti associati ai progetti filtrati e visualizzare anche le informazioni sulle ore

* Puoi vedere fino a 2.000 utenti nell’interfaccia web. Quando raggiungi questo limite, Workfront visualizza un messaggio di avviso.
* Puoi visualizzare tre o quattro periodi di tempo, a seconda delle dimensioni dello schermo.

Dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati, considera quanto segue durante l’esportazione delle informazioni dalla vista Utente della Programmazione delle risorse:

* Quando si sceglie di esportare tutto (utenti, ruoli e progetti) nella Programmazione delle risorse, tutti i ruoli, i progetti e gli utenti vengono inclusi nel file esportato, espansi o meno nell&#39;interfaccia Web.

* Puoi esportare fino a 30.000 righe contenenti utenti, oltre ai progetti e ai ruoli elencati di seguito, indipendentemente dal fatto che sia stato eseguito lo scorrimento verso la parte inferiore dell’elenco per visualizzarli o meno. Tutti gli utenti, i progetti e i ruoli vengono inclusi nel file esportato, a prescindere che siano espansi o meno nell&#39;interfaccia Web.
* Le righe senza informazioni di allocazione vengono incluse nel file esportato.
