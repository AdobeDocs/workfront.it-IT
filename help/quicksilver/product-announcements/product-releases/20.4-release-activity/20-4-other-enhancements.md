---
title: 20.4 Altri miglioramenti
description: 20.4 Altri miglioramenti
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati nell’ambiente di anteprima con la versione 20.4. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 9 novembre 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.4, vedi [Panoramica sulla versione 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novità per gli amministratori: opzione di ambiente Switch Workfront disponibile

Per un’esperienza più efficiente e conveniente, gli amministratori di gruppo e gli amministratori di Workfront ora possono passare rapidamente da un ambiente Workfront diverso da qualsiasi pagina in Workfront senza dover disconnettersi.

Nella nuova esperienza Workfront, l&#39;opzione Passa a Classic viene visualizzata nel menu principale.

In Workfront Classic, l&#39;opzione Passa alla nuova esperienza viene visualizzata nel menu visualizzato quando si fa clic sull&#39;immagine del profilo nell&#39;angolo in alto a destra della barra di navigazione globale.

Questa funzione è ora inclusa nella [Nozioni fondamentali sull&#39;amministratore, percorso di apprendimento parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) su Workfront One.

## È stata migliorata la crittografia per la bozza di Workfront

Stiamo apportando alcune modifiche per migliorare l’efficacia della crittografia in movimento dei dati dell’applicazione di correzione Workfront. Le crittografie TLS deboli verranno dichiarate obsolete l’11 novembre 2020.

Assicurati di utilizzare un browser supportato quando accedi a Workfront. Per ulteriori informazioni sui browser supportati, consulta [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nuovo aspetto per 3 modelli e-mail

Per migliorare la leggibilità e l’esperienza complessiva, i seguenti modelli e-mail hanno un nuovo aspetto:

* Nuova richiesta di lavoro
* Un&#39;attività dipendente a cui sei assegnato è ora pronta per l&#39;avvio
* Notifica e-mail del team con predecessore completato

Per abilitare i messaggi e-mail a scopo di test nell’ambiente di anteprima, consulta la sezione Gestione delle e-mail nell’anteprima in [Attivare o disattivare le notifiche degli eventi personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nuove notifiche e-mail per i team

Abbiamo aggiunto la seguente notifica e-mail per i team:

* È stato completato un predecessore di un&#39;attività assegnata al team: Il team assegnato riceve una notifica e-mail quando un predecessore di una delle attività viene contrassegnato come completato.
* Tutti i predecessori di un&#39;attività assegnata al team sono completati: Il team assegnato riceve una notifica e-mail per ogni predecessore contrassegnata come completato.

Per ulteriori informazioni, consulta [Notifiche: Informazioni sul lavoro assegnato](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Novità per gli amministratori: Miglioramenti delle notifiche e-mail

Ora, con un solo clic, puoi abilitare o disabilitare una notifica e-mail dell’evento in Configurazione. Fai clic sull’interruttore On/Off accanto al nome della notifica.

Inoltre, noterai il nostro stile moderno che ora migliora l’esperienza di configurazione delle notifiche degli eventi nell’area Notifiche e-mail.

Per informazioni sulla configurazione delle notifiche e-mail, consulta [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Questa funzione è ora inclusa nella [Percorso di apprendimento per le notifiche e-mail e in-app](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) su Workfront One.

## Nuovi oggetti API che attivano gli aggiornamenti della sottoscrizione degli eventi

Sono stati creati due nuovi oggetti API, documentVersion e proofApproved, configurati per attivare gli aggiornamenti della sottoscrizione degli eventi quando un documento viene sottoposto a versione o approvato.

Per un elenco completo dei campi associati a ciascun oggetto, consultare [Campi delle risorse della sottoscrizione evento](../../../wf-api/api/event-sub-resource-fields.md).
