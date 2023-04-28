---
title: Miglioramenti a Gestione risorse 22.1
description: Miglioramenti a Gestione risorse 22.1
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 513e0831-5571-4432-ade3-4f11b7e97266
source-git-commit: e0a8093be33773a8b801567cfbe90f67701f9ff3
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Miglioramenti a Gestione risorse 22.1

Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 22.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, vedi [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Miglioramenti al pannello Impostazioni e alla capacità di colorare i progetti e le loro attività nel workload Balancer

Per migliorare la tua esperienza quando utilizzi il servizio di bilanciamento del carico di lavoro, sono stati introdotti i seguenti miglioramenti:

* Il pannello Impostazioni è stato riprogettato per includere opzioni precedentemente presenti nella barra degli strumenti. Questo migliora l’utilizzo dello spazio nella barra degli strumenti.
* Aggiunta la possibilità di personalizzare il tema del colore in base a Progetto. Quando si sceglie di colorare il codice in base a Progetto, ogni progetto e i relativi elementi di lavoro vengono visualizzati con lo stesso colore. I colori sono unici per ogni progetto. Prima di questo miglioramento, era possibile usare solo il codice a colori in base allo stato del progetto.

Per ulteriori informazioni, consulta [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Assegnare il lavoro in blocco utilizzando il bilanciamento del carico di lavoro

Continuando il nostro sforzo per deprecare gli strumenti di programmazione e sostituirli con il load Balancer, abbiamo aggiunto la possibilità di gestire le assegnazioni in blocco. È ora possibile assegnare più elementi di lavoro alla volta a più utenti, sostituire gli utenti di più elementi di lavoro con altri utenti e annullare l&#39;assegnazione degli utenti da più elementi contemporaneamente. Puoi eseguire tutte queste operazioni con una sola azione utilizzando la nuova funzionalità Assegnazione in blocco nel servizio di bilanciamento del carico di lavoro.

Prima di questo miglioramento, era possibile assegnare un solo utente a un elemento di lavoro manualmente o trascinandolo e rilasciandolo.

Le nuove assegnazioni in blocco includono anche nuove funzionalità di filtro per Stato progetto e attività, oltre a Nome.

Per ulteriori informazioni, consulta [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Ignora valuta durante la gestione dei ruoli del lavoro

Per aiutarti a gestire facilmente i tassi di costo e fatturazione tra le organizzazioni globali, abbiamo implementato la sostituzione della valuta di un ruolo di lavoro. Utilizzando questa funzione, è ora possibile impostare i tassi di costo e fatturazione per i ruoli di lavoro nella valuta che corrisponde alla posizione del ruolo di lavoro. In questo modo verrà ignorata la valuta del sistema in tutti i calcoli finanziari per il ruolo di lavoro.

Per informazioni, consulta [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

