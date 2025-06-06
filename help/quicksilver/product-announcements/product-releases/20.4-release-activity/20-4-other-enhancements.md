---
title: 20.4 Altri miglioramenti
description: 20.4 Altri miglioramenti
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 20.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione nella settimana del 9 novembre 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.4, consulta la [panoramica sulla versione 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novità per gli amministratori: opzione di ambiente Switch Workfront disponibile

Per un’esperienza più efficiente e pratica, gli amministratori di gruppi e gli amministratori di Workfront possono ora passare rapidamente da un ambiente Workfront all’altro da qualsiasi pagina di Workfront senza dover disconnettersi.

Nella nuova esperienza Workfront, nel menu principale viene visualizzata l’opzione Passa a Classic.

In Workfront Classic, l’opzione Passa alla nuova esperienza viene visualizzata nel menu visualizzato quando si fa clic sull’immagine del profilo nell’angolo in alto a destra della barra di navigazione globale.

Questa funzionalità è ora inclusa in [Nozioni di base per gli amministratori, parte 1, percorso di apprendimento](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## Crittografia migliorata per Workfront Proof

Stiamo apportando alcune modifiche per migliorare la forza della crittografia dei dati in movimento dell’applicazione di verifica Workfront. Le crittografie TLS deboli diventeranno obsolete l’11 novembre 2020.

Assicurati di utilizzare un browser supportato per accedere a Workfront. Per ulteriori informazioni sui browser supportati, vedere [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nuovo aspetto per 3 modelli e-mail

Per migliorare la leggibilità e l’esperienza complessiva, i seguenti modelli e-mail hanno un nuovo aspetto:

* Nuova richiesta di lavoro
* Un&#39;attività dipendente a cui sei assegnato è pronta per iniziare
* Notifica e-mail team con predecessore completo

Per abilitare l&#39;e-mail a scopo di test nell&#39;ambiente di anteprima, consulta la sezione Gestione delle e-mail nell&#39;anteprima in [Modifica le tue notifiche e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nuove notifiche e-mail per i team

Abbiamo aggiunto la seguente notifica e-mail per i team:

* Un predecessore di un&#39;attività assegnata al mio team è completato: il team assegnato riceve una notifica e-mail quando un predecessore di una delle loro attività è contrassegnato come completato.
* Tutti i predecessori di un&#39;attività assegnata al mio team sono completati: il team assegnato riceve una notifica e-mail per ogni predecessore contrassegnato come completato.

Per ulteriori informazioni, vedere [Notifiche: informazioni sul lavoro assegnato a me](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Novità per gli amministratori: miglioramenti alle notifiche e-mail

Ora, con un solo clic, puoi abilitare o disabilitare una notifica e-mail di evento in Configurazione. Fare clic sull&#39;interruttore On/Off accanto al nome della notifica.

Inoltre, nota il nostro stile moderno che ora migliora l’esperienza di configurazione delle notifiche degli eventi nell’area Notifiche e-mail.

Per informazioni sulla configurazione delle notifiche e-mail, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Questa funzionalità è ora inclusa nel percorso di apprendimento [Notifiche e-mail e in-app](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home) in Workfront One.

## Nuovi oggetti API che attivano gli aggiornamenti delle sottoscrizioni di eventi

Sono stati creati due nuovi oggetti API, documentVersion e proofApproval, configurati per attivare gli aggiornamenti delle sottoscrizioni di eventi quando un documento viene sottoposto a controllo delle versioni o approvato.

Per un elenco completo dei campi associati a ciascun oggetto, vedere [Campi risorse sottoscrizione evento](../../../wf-api/api/event-sub-resource-fields.md).
