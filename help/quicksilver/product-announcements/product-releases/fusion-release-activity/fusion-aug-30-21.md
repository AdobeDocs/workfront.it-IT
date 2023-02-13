---
title: Attività di rilascio di Workfront Fusion:&nbsp;Settimana del 30 agosto 2021
description: Attività di rilascio di Workfront Fusion:&nbsp;Settimana del 30 agosto 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana 30 agosto 2021

Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion nella settimana del 30 agosto 2021.

Per un elenco di tutte le modifiche recenti, vedi [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedi [Aggiornamenti alla manutenzione di Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e controlla eventuali aggiornamenti etichettati Workfront Fusion Maintenance Update.

## Filtrare gli eventi che attivano il modulo eventi Workfront > Watch

1. Imposta un filtro personalizzato per gli eventi che attivano il modulo Workfront > Guarda eventi

   Per ridurre il numero di esecuzioni di scenari non necessari, abbiamo aggiornato il modulo Workfront > Watch records per abilitare il filtro degli eventi. Ora puoi impostare un filtro quando crei un webhook. Questo consente allo scenario di attivarsi solo quando l’evento soddisfa determinati criteri.

   Il filtro eventi offre attualmente le seguenti operazioni:

   * Uguale a: Attiva uno scenario solo quando un evento corrisponde alle condizioni del filtro. Ad esempio, puoi impostare un filtro che attiva uno scenario solo se l’evento si verifica in un progetto specifico.
   * Diverso: Attiva uno scenario solo se un evento non corrisponde alle condizioni del filtro. Ad esempio, puoi creare un filtro che attivi uno scenario solo se il problema si verifica in non ha lo stato Chiuso.

   In precedenza, il modulo dei record Watch recuperava tutti i record. Gli utenti potevano filtrare solo impostando i filtri in un secondo momento nello scenario.

   Per sfruttare il filtro degli eventi, crea un nuovo webhook nel modulo degli eventi Watch. Al momento non è possibile modificare i webhook esistenti per includere questa funzionalità. È consigliabile creare nuovi webhook utilizzando filtri evento per gli scenari esistenti.

1. Filtrare gli eventi attivati dalla connessione corrente.

   Per semplificare la configurazione dei tuoi webhook per il modulo Workfront > Guarda eventi, abbiamo incluso il filtro eventi più comune. Ora, il webhook dispone di un&#39;opzione per filtrare tutte le modifiche apportate dai moduli utilizzando la connessione specificata per il modulo Eventi Watch. In altre parole, con questo filtro abilitato, qualsiasi modifica apportata dall’utente Workfront associato a tale connessione non può attivare lo scenario.

   In precedenza, questo filtro non era disponibile. Pertanto, era più facile per le modifiche apportate nei moduli Workfront attivare scenari contenenti tali moduli, potenzialmente causando scenari da attivare in un ciclo infinito.

Per ulteriori informazioni sui filtri eventi nel modulo Workfront > Guarda eventi , vedi [Moduli Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

