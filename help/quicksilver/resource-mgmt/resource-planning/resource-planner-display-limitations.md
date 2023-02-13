---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitazioni della visualizzazione di Resource Planner
description: Per migliorare le prestazioni, Adobe Workfront limita la quantità di informazioni che è possibile visualizzare e la quantità di informazioni che è possibile esportare dal Planner risorse.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Limitazioni della visualizzazione di Resource Planner

Per migliorare le prestazioni, Adobe Workfront limita la quantità di informazioni che è possibile visualizzare e la quantità di informazioni che è possibile esportare dal Planner risorse.

Quando si avvicina questo limite, Workfront visualizza un messaggio di avviso per comunicarti che hai raggiunto quel limite.

Se le informazioni che si prevede di visualizzare nel Planner risorse non vengono visualizzate, è possibile che si stia tentando di visualizzare troppe informazioni e che alcuni dati non siano stati visualizzati a causa di questa limitazione.

Si consiglia quanto segue per ottenere prestazioni ottimali nella visualizzazione ed esportazione del Planner risorse:

* Utilizzare i filtri per ridurre la quantità di informazioni visualizzate nel Planner risorse e visualizzare solo le informazioni pertinenti.
* Utilizza tutte le opzioni di esportazione per ridurre la quantità di informazioni esportate contemporaneamente e per assicurarti di esportare solo informazioni pertinenti.\
   Per ulteriori informazioni sull&#39;uso dei filtri e delle opzioni di esportazione nel Planner risorse, vedere [Filtrare le informazioni nel planner risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).

   Per informazioni sull&#39;esportazione di informazioni dal Planner risorse, vedere [Esporta informazioni dal planner risorse](../../resource-mgmt/resource-planning/export-resource-planner.md).

La quantità di informazioni che è possibile visualizzare o esportare dipende dalla visualizzazione applicata e dall&#39;ambiente utilizzato per accedere al Planner risorse.

## Limitazioni nella vista Progetto

Quando si applica la visualizzazione Progetto al planner risorse, tenere presente quanto segue:

* Puoi visualizzare solo i progetti a cui hai accesso per la gestione.
* Puoi espandere ogni progetto per visualizzare i ruoli associati e ogni ruolo per visualizzare gli utenti associati.

   È possibile visualizzare fino a 300 progetti quando si scorre fino alla parte inferiore dell’elenco, a meno che non siano presenti più di 30.000 righe di progetti, ruoli e utenti. Quindi, ricevi un messaggio di avviso che segnala di aver raggiunto il limite di 30.000 righe.

* È possibile visualizzare tre o quattro periodi alla volta, a seconda delle dimensioni dello schermo.

Quando si esportano informazioni dalla vista Progetto del Planner risorse, tenere presente quanto segue dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati:

* Quando si seleziona di esportare tutti gli elementi (progetti, ruoli e utenti) nel Planner risorse, tutti gli oggetti che corrispondono ai criteri vengono visualizzati nel file esportato, indipendentemente dal fatto che sia stato eseguito lo scorrimento in fondo all’elenco per visualizzarli o meno.
* Le righe senza informazioni di allocazione sono incluse nel file esportato.

* Puoi esportare fino a 30.000 righe.

## Limitazioni nella vista Ruolo

Quando applichi la vista Ruolo al Planner risorse, considera quanto segue dopo aver applicato tutti i filtri appropriati:

* Puoi visualizzare solo i ruoli associati ai progetti che puoi gestire.

* Puoi visualizzare fino a 300 ruoli quando scorri fino alla parte inferiore dell’elenco, a meno che non siano presenti più di 30.000 righe di ruoli, progetti e utenti. Quindi, viene visualizzato un messaggio di avviso che indica che è stato raggiunto il limite di 30.000 righe per ciò che è possibile visualizzare sullo schermo.
* È possibile espandere ogni ruolo per visualizzare un elenco di progetti e ogni progetto per visualizzare un elenco di utenti in grado di eseguire tali ruoli nei progetti.

   Per impostazione predefinita vengono visualizzati 20 progetti e puoi utilizzare l’opzione Carica altro per visualizzare ulteriori progetti oppure scorrere sotto ogni progetto per caricare altri utenti.

* Puoi visualizzare tre o quattro periodi di tempo, a seconda delle dimensioni dello schermo.

Quando si esportano informazioni dalla vista Ruolo del Planner risorse, tenere presente quanto segue dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati:

* Quando si seleziona di esportare tutti gli elementi (ruoli, progetti e utenti) nel Planner risorse, tutti gli oggetti che corrispondono ai criteri vengono visualizzati nel file esportato, indipendentemente dal fatto che sia stato eseguito lo scorrimento in fondo all’elenco per visualizzarli o meno.
* Le righe senza informazioni di allocazione sono incluse nel file esportato.
* Puoi esportare fino a 30.000 righe.

## Limitazioni nella visualizzazione utente

Quando si applica la visualizzazione Utente al Planner risorse, tenere presente quanto segue:

* Puoi visualizzare tutti gli utenti che soddisfano i seguenti criteri:

   * Accesso alla visualizzazione
   * Sono attivi
   * Accesso eseguito almeno una volta.

* È possibile espandere ogni utente per visualizzare i progetti associati e ogni progetto per visualizzare i ruoli associati.\
   I primi 50 progetti e ruoli vengono visualizzati per impostazione predefinita e puoi utilizzare l’opzione Carica altro per visualizzare altri progetti o ruoli.

   >[!NOTE]
   >
   >Se l’elenco degli utenti è stato filtrato in base ai progetti, è possibile espandere solo gli utenti associati ai progetti filtrati e visualizzare anche le informazioni relative all’ora

* Puoi visualizzare fino a 2.000 utenti nell’interfaccia web. Quando raggiungi questo limite, in Workfront viene visualizzato un messaggio di avviso.
* Puoi visualizzare tre o quattro periodi di tempo, a seconda delle dimensioni dello schermo.

Quando si esportano informazioni dalla visualizzazione Utente del Planner risorse, tenere presente quanto segue dopo aver applicato tutti i filtri e le opzioni di esportazione appropriati:

* Quando si seleziona di esportare tutto (utenti, ruoli e progetti) nel Planner risorse, tutti i ruoli, i progetti e gli utenti vengono inclusi nel file esportato, siano essi espansi o meno nell’interfaccia Web.

* Puoi esportare fino a 30.000 righe che contengono utenti, nonché i progetti e i ruoli elencati sotto, indipendentemente dal fatto che sia stato eseguito lo scorrimento nella parte inferiore dell’elenco per visualizzarli o meno. Tutti gli utenti, i progetti e i ruoli sono inclusi nel file esportato, siano essi espansi o meno nell’interfaccia web.
* Le righe senza informazioni di allocazione sono incluse nel file esportato.
