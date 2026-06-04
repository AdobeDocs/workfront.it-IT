---
title: 22.2 - Miglioramenti per la gestione delle risorse
description: 22.2 - Miglioramenti per la gestione delle risorse
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
TQID: https://experienceleague.adobe.com/X2dBmB8Qyiwg9hM60af6GRBDGT4KkH6Jjs2A-S-TWVg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 5%

---

# 22.2 - Miglioramenti per la gestione delle risorse

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

Per ulteriori informazioni, consulta [Configurare le preferenze di gestione delle risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

