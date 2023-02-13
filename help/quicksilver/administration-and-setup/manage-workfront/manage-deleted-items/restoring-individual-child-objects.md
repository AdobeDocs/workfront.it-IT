---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Ripristino di singoli oggetti secondari
description: Questo documento descrive come ottenere assistenza per recuperare singoli oggetti secondari che sono stati eliminati dagli ambienti di produzione o anteprima di Adobe Workfront meno di 30 giorni prima.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Ripristino di singoli oggetti secondari

Questo documento descrive come ottenere assistenza per recuperare singoli oggetti secondari che sono stati eliminati dagli ambienti di produzione o anteprima di Adobe Workfront meno di 30 giorni prima.

Un amministratore Workfront può ripristinare progetti, attività, problemi e documenti in ogni istanza di Workfront, come descritto in [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Tuttavia, solo il team del database di Workfront può ripristinare oggetti quali attività, problemi, documenti, moduli personalizzati, ore e note indipendentemente dall&#39;oggetto principale.

I dati dell’ambiente live sono disponibili nella Sandbox di anteprima per un massimo di 7 giorni. Ciò significa che puoi esportare i dati autonomi dall’ambiente Sandbox di anteprima utilizzando i seguenti metodi:

* Kick-Start
* Creazione di un report ed esportazione dei risultati

Per ulteriori informazioni sull&#39;esportazione di dati da Workfront, vedi [Esportare i dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Puoi importare i dati esportati nei seguenti modi:

* Manualmente, se utilizzi rapporti esportati
* In blocco, se utilizzi Kick-Starts

   Per ulteriori informazioni sull’importazione di dati in Workfront tramite Kick-Starts, consulta [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

L’ambiente Sandbox di anteprima viene aggiornato durante le finestre di manutenzione nel corso del fine settimana.

Per ulteriori informazioni sulle finestre di manutenzione per l’ambiente Sandbox di anteprima, consulta [trust.workfront.com](https://trust.workfront.com/).

>[!IMPORTANT]
>
>I documenti costituiscono un&#39;eccezione a questi metodi di restauro. Puoi scaricarli manualmente dall’ambiente di anteprima e ricaricarli nell’ambiente di produzione. Se desideri scaricare e caricare documenti in blocco, dovrai richiedere un ripristino dei dati da Workfront.

## Informazioni necessarie per il ripristino dei dati

Una volta determinato che un oggetto eliminato deve essere ripristinato dal nostro Team di database, raccogliere tutte le informazioni disponibili al riguardo. Per consentire agli amministratori di database di trovare l’oggetto e avviare un ripristino, sono necessarie le seguenti informazioni:

* Nome oggetto
* Tipo di oggetto (attività, problema, progetto, ecc.)
* Data e ora stimate dell’eliminazione
* GUID oggetto (se possibile)

   Fare riferimento alle seguenti informazioni quando si individua il GUID di un oggetto:

   * Il GUID si trova facendo riferimento alle notifiche e-mail attivate interagendo con l’oggetto (assegnazioni a, commenti su, ecc.)
   * Esempio di GUID trovato alla fine di un URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Una volta raccolte queste informazioni o se hai bisogno di assistenza, chiama il nostro team di assistenza clienti al numero 844-306-HELP(4357) o invia un ticket online.

## Processo di ripristino dei dati

1. Dopo che il nostro team di assistenza clienti riceverà le tue informazioni, le inoltrerà al nostro team di assistenza clienti.
1. Il nostro team di assistenza clienti contatterà il nostro team di database.
1. Una volta che il team del database ha avuto la possibilità di rivedere i dati che vengono ripristinati, è possibile fornire una stima più accurata dell&#39;ETA. Un ripristino richiede generalmente tre giorni, ma può richiedere più tempo a seconda del tipo e del volume di dati ripristinati.
1. Il team del database ripristinerà le informazioni nell&#39;ambiente Sandbox di anteprima in cui sarà possibile esaminare i dati ripristinati. Il nostro team di assistenza clienti ti informerà quando i dati possono essere trovati nella Sandbox di anteprima.
1. Una volta effettuato il ripristino nella sandbox, informa il nostro team di assistenza clienti e contatterà il nostro team di database per informarli che può ripristinare i dati nel tuo ambiente di produzione.
1. Potrai rivedere i dati ripristinati prima della chiusura della richiesta.
