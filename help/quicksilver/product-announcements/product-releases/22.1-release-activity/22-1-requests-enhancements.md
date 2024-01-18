---
title: 22.1 Richieste di miglioramenti
description: 22.1 Richieste di miglioramenti
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1 Richieste di miglioramenti

Questa pagina descrive tutti i miglioramenti apportati con la versione 22.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 17 gennaio 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.1, consulta [Panoramica sulla versione 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Miglioramento dell’interfaccia per gli utenti che non hanno accesso per creare richieste

Per migliorare l’esperienza degli utenti che lavorano con le richieste, è stato introdotto un miglioramento all’interfaccia che indica all’utente connesso di non avere accesso per creare richieste. Grazie a questo miglioramento, il pulsante New request (Nuova richiesta) diventa inattivo per gli utenti che non hanno accesso a per creare problemi. Passando il puntatore del mouse sul pulsante sfumato viene visualizzata una descrizione comando che spiega come l’amministratore di Workfront abbia limitato l’accesso dell’utente corrente per la creazione delle richieste.

Prima di questo miglioramento, il pulsante Nuova richiesta non veniva visualizzato nell’area Richieste per questi utenti. È inoltre limitato copiare e inviare una richiesta come nuova.

Per ulteriori informazioni sulla creazione delle richieste, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiare e inviare richieste

Per ottimizzare il processo di invio delle richieste, stiamo introducendo una nuova funzionalità che consente di copiare una richiesta esistente e inviarla come nuova richiesta. Questa funzione è utile quando si inviano spesso richieste simili. In questo caso, puoi riutilizzare una richiesta esistente, apportare alcune modifiche e inviarla come nuova richiesta.

Con questa modifica, anche gli utenti che possono visualizzare le richieste inviate da altri possono copiare le richieste e inviarle come nuove. Per evitare che ciò si verifichi, aggiorna la seguente impostazione nel progetto della coda richieste: Persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste.

>[!NOTE]
>
>Non è possibile copiare e inviare nuovamente i problemi inviati a una coda di richieste senza un argomento della coda prima del rilascio di questa funzionalità.

Per ulteriori informazioni, consulta [Copiare e inviare richieste](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Esperienza aggiornata del pannello Riepilogo nella sezione Inviata dell’area Richieste

>[!NOTE]
>
>Questa funzione è stata temporaneamente rimossa dall’ambiente di anteprima il 12 novembre 2021. Sarà aggiunto di nuovo in un secondo momento.

Per migliorare la visibilità e l’interazione con il pannello Riepilogo, è stata aggiunta un’etichetta all’icona Apri riepilogo nella sezione Inviata dell’area Richieste. L’etichetta ora è dinamica e si aggiorna a seconda che il pannello sia aperto o chiuso.

Quando si apre il pannello Riepilogo senza prima selezionare una richiesta, ora viene visualizzata un’immagine più semplice che indica chiaramente all’utente di selezionare un elemento prima di aprire il pannello. Per ulteriori informazioni, consulta [Individuare le richieste inviate](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Con questa modifica, è stato aggiornato anche il pannello Riepilogo per attività, problemi e documenti. Per informazioni sul pannello Riepilogo, consulta [Panoramica di riepilogo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
