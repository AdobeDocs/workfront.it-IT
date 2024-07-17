---
title: 22.2 Miglioramenti alla gestione delle risorse
description: 22.2 Miglioramenti alla gestione delle risorse
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 22.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.2, vedere [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Miglioramenti alla navigazione del Bilanciatore dei carichi di lavoro

Per migliorare la tua esperienza nell’utilizzo del Bilanciatore dei carichi di lavoro, sono stati introdotti i seguenti miglioramenti:

* I pulsanti Annulla e Salva durante la regolazione delle allocazioni sono ora permanenti, anche quando l’attività è più lunga dell’intervallo di tempo incluso sullo schermo o quando viene visualizzato il pannello Riepilogo.
* Il pannello sinistro, in cui vengono visualizzati i nomi degli utenti e degli elementi di lavoro, è ora appiccicoso e consente di scorrere orizzontalmente per intervalli di tempo più lunghi e di leggere comunque i nomi degli elementi elencati nel pannello.
* È possibile comprimere ed espandere tutti gli elementi elencati nel pannello sinistro con un solo clic invece che a livello di utente o progetto.
* Il pannello sinistro è ora ridimensionabile.
* È ora disponibile una modalità a schermo intero per il Bilanciatore dei carichi di lavoro.

Per ulteriori informazioni sulla navigazione nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Accedere alle assegnazioni avanzate nel Bilanciatore dei carichi di lavoro

Per rendere l&#39;assegnazione degli elementi di lavoro più semplice e precisa, è ora possibile effettuare assegnazioni avanzate quando si assegnano gli elementi di lavoro manualmente nel Bilanciatore dei carichi di lavoro. Prima di questo miglioramento, era possibile accedere ad Assegnazioni avanzate durante la modifica di elementi, dalle intestazioni degli elementi o negli elenchi.

Per ulteriori informazioni, consulta [Assegnare il lavoro manualmente utilizzando il Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nuova formula per il calcolo della disponibilità utente quando è selezionata la preferenza Pianificazione predefinita

Per fornire informazioni più precise negli strumenti di gestione delle risorse, è stata modificata la formula utilizzata da Workfront per calcolare la disponibilità dell&#39;utente quando l&#39;amministratore di Workfront seleziona La pianificazione predefinita nelle preferenze di gestione delle risorse. Con il nuovo aggiornamento, Workfront utilizza la seguente formula per calcolare la disponibilità dell’utente:

Ore disponibili utente = (Ore programmate predefinite - Eccezioni) &#42; FTE - Ore di inattività

Prima di questo aggiornamento, Workfront utilizzava la formula seguente per calcolare la disponibilità dell&#39;utente quando veniva selezionata la pianificazione predefinita:

Ore disponibili utente = (Ore programmate predefinite - (Eccezioni programmate + Ore di inattività)) &#42; Valore FTE utente

Per ulteriori informazioni, vedere [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

