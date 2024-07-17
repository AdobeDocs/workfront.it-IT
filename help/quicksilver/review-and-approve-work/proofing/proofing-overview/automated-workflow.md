---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Panoramica del flusso di lavoro automatizzato
description: I flussi di lavoro automatizzati consentono di creare una serie di fasi di revisione sequenziale o parallela, stabilire dipendenze tra queste fasi e limitarne la visibilità a determinati utenti. Se nel processo di revisione sono presenti fasi interdipendenti, i flussi di lavoro automatizzati spostano automaticamente la bozza nelle varie fasi, inviando una notifica ai revisori e agli approvatori interessati.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Panoramica del flusso di lavoro automatizzato

<!-- Audited: 01/2024 -->

I flussi di lavoro automatizzati consentono di creare una serie di fasi di revisione sequenziale o parallela, stabilire dipendenze tra queste fasi e limitarne la visibilità a determinati utenti. Se nel processo di revisione sono presenti fasi interdipendenti, i flussi di lavoro automatizzati spostano automaticamente la bozza nelle varie fasi, inviando una notifica ai revisori e agli approvatori interessati. Per informazioni sulla configurazione di un flusso di lavoro automatico, vedere [Creare una bozza avanzata con un flusso di lavoro automatico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Esempi:** i flussi di lavoro automatizzati consentono di gestire processi di revisione delle bozze complessi come:

* Quando diversi gruppi o revisori devono rivedere il contenuto in un determinato ordine
* In presenza di dipendenze tra l’attività degli utenti durante la revisione del contenuto
* Quando il contenuto viene rivisto regolarmente dagli stessi gruppi di persone
* Quando si desidera controllare il periodo di tempo in cui i revisori esaminano il contenuto
* Quando desideri mantenere privata un&#39;attività di revisione

## Fasi

Per ogni fase del flusso di lavoro automatizzato, puoi configurare impostazioni quali una scadenza per la fase, un blocco su una fase, un revisore impostato come responsabile delle decisioni per la fase e un’impostazione di privacy che consente solo a determinate persone di visualizzare i commenti del revisore sulla fase.

Le fasi possono essere attivate manualmente, al momento della creazione della bozza, al raggiungimento di una scadenza, in una data e un’ora specifiche o quando viene presa una decisione sulla fase principale.

Le fasi possono essere bloccate manualmente, così come quando inizia la fase successiva o quando tutte le decisioni vengono prese sulla fase. È inoltre possibile scegliere di non bloccare mai un palco.

È possibile nominare un responsabile delle decisioni principale per una fase. La decisione di questa persona rende superflue tutte le altre decisioni per la fase.

Allo stesso modo, puoi scegliere di richiedere una sola decisione per una fase. In questo caso, il processo di revisione per la fase viene contrassegnato come completato dopo che uno dei destinatari ha preso la sua decisione sulla fase.

È possibile che tutti i revisori ricevano una notifica relativa all&#39;invito a rivedere il contenuto all&#39;inizio del processo di revisione oppure che ogni revisore riceva una notifica solo quando la fase è attivata.

## Fasi private

Per impostazione predefinita, i commenti lasciati dai revisori in tutte le fasi sono visibili a tutti coloro che stanno esaminando il contenuto e ricevono notifiche e-mail e riepiloghi di commenti sul processo di revisione.

Se si desidera impedire ad alcuni gruppi di revisori di visualizzare i commenti di altri revisori, è possibile creare fasi private.

Le fasi private sono visibili solo ai revisori aggiunti a tali fasi. Sono visibili anche agli utenti che dispongono dei diritti di modifica per la bozza o i diritti di modifica per tutti gli elementi creati nell’account Adobe Workfront della tua organizzazione (Supervisore e versioni successive, oppure agli utenti con profili personalizzati per i quali è abilitata la modifica delle informazioni di altri utenti).

I commenti aggiunti dai partecipanti alla fase privata non vengono inclusi nelle notifiche e-mail e nei riepiloghi dei commenti della bozza richiesti da chiunque non abbia i diritti per visualizzarli.

## Diagramma del flusso di lavoro

Il diagramma del flusso di lavoro è una rappresentazione visiva del processo di revisione della bozza. Mostra l’ordine delle fasi e le dipendenze tra le fasi durante la creazione o la visualizzazione dei dettagli di una bozza. Tutte le fasi private vengono visualizzate con un simbolo di chiave.

![intro-to-aw-example-diagram.png](assets/intro-to-aw-example-diagram-350x199.png)

Nelle bozze live, le dipendenze degli stadi vengono visualizzate con una linea grigia tratteggiata per gli stadi inattivi o una linea nera continua per gli stadi attivi. Le fasi vengono visualizzate in verde se il processo di approvazione è stato completato entro la scadenza specificata. Gli stadi che si avvicinano alle rispettive scadenze vengono visualizzati in arancione mentre quelli che superano le rispettive scadenze vengono visualizzati in rosso.

![workflow_2.png](assets/workflow-2-350x183.png)

## Modelli di flusso di lavoro automatizzato

Se la tua organizzazione utilizza lo stesso processo di revisione per più bozze, l’amministratore di Workfront può creare modelli di flusso di lavoro automatizzati per semplificare notevolmente la creazione delle bozze. Puoi scegliere un modello di flusso di lavoro automatico durante la configurazione di una bozza per aggiungere le fasi e i revisori in tale modello alla bozza. Puoi modificare il modello applicato alla bozza in base alle esigenze prima e dopo aver creato la bozza.

L’amministratore di Workfront può creare un numero illimitato di modelli in base alle esigenze della tua azienda.

Per ulteriori informazioni sulla creazione, l’utilizzo e la gestione dei modelli, rivolgiti al tuo amministratore Workfront.
