---
title: 22.2 Miglioramenti alla gestione delle risorse
description: 22.2 Miglioramenti alla gestione delle risorse
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 22.2 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.2, vedi [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Miglioramenti alla navigazione del bilanciamento del carico di lavoro

Per migliorare la tua esperienza quando utilizzi il servizio di bilanciamento del carico di lavoro, sono stati introdotti i seguenti miglioramenti:

* I pulsanti Annulla e Salva quando si regolano le allocazioni sono ora permanenti, anche quando l’attività è più lunga dell’intervallo di tempo incluso nella schermata o quando viene visualizzato il pannello Riepilogo .
* Il pannello a sinistra che visualizza i nomi degli utenti e degli elementi di lavoro è ora appiccicoso, consente di scorrere in orizzontale per intervalli di tempo più lunghi e di poter comunque leggere i nomi degli elementi elencati nel pannello.
* Puoi comprimere ed espandere tutti gli elementi elencati nel pannello a sinistra con un solo clic invece che a livello di utente o di progetto.
* È ora possibile ridimensionare anche il pannello a sinistra.
* È ora disponibile una modalità a schermo intero per il bilanciamento del carico di lavoro.

Per ulteriori informazioni sulla navigazione nel servizio di bilanciamento del carico di lavoro, consulta [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Accedere alle assegnazioni avanzate nel load balancer

Per semplificare e rendere più precisa l&#39;assegnazione degli elementi di lavoro, è ora possibile effettuare assegnazioni avanzate quando si assegnano gli elementi di lavoro manualmente nel servizio di bilanciamento del carico di lavoro. Prima di questo miglioramento, era possibile accedere ad Assegnazioni avanzate durante la modifica di elementi, dalle intestazioni degli elementi o negli elenchi.

Per ulteriori informazioni, consulta [Assegnare il lavoro manualmente utilizzando il bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nuova formula per il calcolo della disponibilità dell&#39;utente quando è selezionata la preferenza Pianificazione predefinita

Per fornire informazioni più precise negli strumenti di gestione delle risorse, abbiamo modificato la formula utilizzata da Workfront per calcolare la disponibilità degli utenti quando l’amministratore di Workfront seleziona La pianificazione predefinita nelle preferenze di gestione delle risorse. Con il nuovo aggiornamento, Workfront utilizza la seguente formula per calcolare la disponibilità degli utenti:

Orari disponibili dell&#39;utente = (ore di programmazione predefinite - Eccezioni) &#42; FTE - Tempo di riposo

Prima di questo aggiornamento, Workfront utilizzava la seguente formula per calcolare la disponibilità dell’utente quando era selezionata la pianificazione predefinita:

Orari disponibili dell&#39;utente = (orario di programmazione predefinito - (eccezioni di pianificazione + orario di interruzione) &#42; Valore FTE utente

Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

