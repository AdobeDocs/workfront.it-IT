---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Ripristina singoli oggetti figlio
description: Questo articolo descrive come ottenere aiuto per il recupero di singoli oggetti secondari eliminati dagli ambienti di produzione o anteprima di Adobe Workfront meno di 30 giorni prima.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Ripristino di singoli oggetti figlio

Questo articolo descrive come ottenere aiuto per il recupero di singoli oggetti secondari eliminati dagli ambienti di produzione o anteprima di Adobe Workfront meno di 30 giorni prima.

Un amministratore di Workfront può ripristinare progetti, attività, problemi e documenti in ogni istanza di Workfront, come descritto in [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Tuttavia, solo il team del database di Workfront può ripristinare oggetti quali attività, problemi, documenti, moduli personalizzati, ore e note indipendentemente dall&#39;oggetto padre.

I dati dell’ambiente live sono disponibili nella Sandbox di anteprima per un massimo di 7 giorni. Ciò significa che puoi esportare i dati autonomi dall’ambiente Sandbox di anteprima utilizzando i seguenti metodi:

* Kick-Start
* Creazione di un rapporto ed esportazione dei risultati

Per ulteriori informazioni sull&#39;esportazione di dati da Workfront, vedere [Esporta dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

È possibile importare i dati esportati nei modi seguenti:

* Manualmente, se si utilizzano i report esportati
* In blocco, se utilizzi Kick-Start

  Per ulteriori informazioni sull&#39;importazione di dati in Workfront tramite Kick-Start, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

L’ambiente Sandbox di anteprima viene aggiornato durante le finestre di manutenzione nel fine settimana.

Per ulteriori informazioni sulle finestre di manutenzione per l&#39;ambiente Sandbox di anteprima, consulta [il sito sullo stato di Adobe](https://status.adobe.com/it).

>[!IMPORTANT]
>
>I documenti sono un&#39;eccezione a questi metodi di ripristino. Puoi scaricarli manualmente dall’ambiente di anteprima e ricaricarli nell’ambiente di produzione. Se desideri scaricare e caricare documenti in blocco, devi richiedere un ripristino dei dati da Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni necessarie per il ripristino dei dati

Una volta stabilito che un oggetto eliminato deve essere ripristinato dal nostro team di database, raccogli tutte le informazioni che hai su di esso. Per trovare l&#39;oggetto e avviare il ripristino, gli amministratori del database devono disporre delle seguenti informazioni:

* Nome oggetto
* Tipo di oggetto (attività, problema, progetto, ecc.)
* Data e ora stimate per l’eliminazione
* GUID oggetto (se possibile)

  Quando si individua il GUID di un oggetto, fare riferimento alle informazioni seguenti:

   * Il GUID può essere trovato facendo riferimento a notifiche e-mail attivate interagendo con l’oggetto (assegnazioni a, commenti su, ecc.)
   * Esempio di GUID trovato alla fine di un URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Una volta raccolte queste informazioni o se hai bisogno di assistenza, chiama il nostro team di assistenza clienti al numero 844-306-HELP(4357) o invia un ticket online.

## Processo di ripristino dei dati

1. Una volta ricevute le informazioni, il team di assistenza clienti le invierà al team di assistenza clienti.
1. Il nostro team di assistenza clienti contatterà il nostro team di database.
1. Una volta che il team del database ha avuto la possibilità di esaminare i dati da ripristinare, è possibile fornire una stima più accurata per l’ETA. Un ripristino richiede generalmente tre giorni, ma può richiedere più tempo a seconda del tipo e del volume di dati da ripristinare.
1. Il team del database ripristinerà le informazioni nell’ambiente Sandbox di anteprima in cui potrai esaminare i dati ripristinati. Il nostro team di assistenza clienti ti informerà quando i dati saranno disponibili nella Sandbox di anteprima.
1. Quando sei soddisfatto del ripristino nella sandbox, informa il team di assistenza clienti che contatterà il team del database per informarlo che può ripristinare i dati nell’ambiente di produzione.
1. Avrai la possibilità di rivedere i dati ripristinati prima che la richiesta venga chiusa.
