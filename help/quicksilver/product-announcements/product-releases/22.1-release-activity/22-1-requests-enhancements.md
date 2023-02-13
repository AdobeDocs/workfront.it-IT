---
title: Miglioramenti alle richieste 22.1
description: Miglioramenti alle richieste 22.1
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Miglioramenti alle richieste 22.1

Questa pagina descrive tutti i miglioramenti delle richieste effettuati con la versione 22.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, vedi [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Miglioramento dell’interfaccia per gli utenti che non hanno accesso per creare richieste

Per migliorare l’esperienza degli utenti quando lavorano con le richieste, abbiamo introdotto un miglioramento all’interfaccia che indica all’utente connesso che non ha accesso per creare richieste. Con questo miglioramento, il pulsante Nuova richiesta è disattivato per gli utenti che non hanno accesso a creare problemi. Passando il puntatore del mouse sul pulsante disattivato viene visualizzata una descrizione che spiega che l’amministratore di Workfront ha limitato l’accesso dell’utente corrente alla creazione di richieste.

Prima di questo miglioramento, il pulsante Nuova richiesta non veniva visualizzato nell’area Richieste per questi utenti. Anche la copia e l’invio di una richiesta come nuova è soggetta a restrizioni.

Per ulteriori informazioni sulla creazione delle richieste, vedi [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copia e invia richieste

Per ottimizzare il processo di invio delle richieste, stiamo introducendo una nuova funzionalità che ti consente di copiare una richiesta esistente e inviarla come nuova richiesta. Questa funzione è utile quando si inviano spesso richieste simili. In questo caso, puoi riutilizzare una richiesta esistente, apportare alcune modifiche e quindi inviarla come nuova richiesta.

Con questa modifica, gli utenti che possono visualizzare le richieste inviate da altri possono anche copiare tali richieste e inviarle come nuove. Per evitare che ciò si verifichi, aggiorna la seguente impostazione nel progetto di coda delle richieste: le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste.

>[!NOTE]
>
>Non è possibile copiare e inviare nuovamente i problemi inviati a una coda di richieste senza un argomento della coda prima del rilascio di questa funzionalità.

Per ulteriori informazioni, consulta [Copia e invia richieste](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Aggiornamento dell’esperienza del pannello Riepilogo nella sezione Inviato dell’area Richieste

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di anteprima il 12 novembre 2021. Verrà riaggiunto in una data successiva.

Per migliorare la visibilità e l’interazione con il pannello Riepilogo, abbiamo aggiunto un’etichetta all’icona Apri riepilogo nella sezione Inviato dell’area Richieste. L’etichetta è ora dinamica e viene aggiornata a seconda che il pannello sia aperto o chiuso.

Quando si apre il pannello Riepilogo senza prima selezionare una richiesta, ora viene visualizzata un’immagine più intuitiva per istruire chiaramente l’utente a selezionare un elemento prima di aprire il pannello. Per ulteriori informazioni, consulta [Individua richieste inviate](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Con questa modifica è stato aggiornato anche il pannello Riepilogo per attività, problemi e documenti. Per informazioni sul pannello Riepilogo, consulta [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
