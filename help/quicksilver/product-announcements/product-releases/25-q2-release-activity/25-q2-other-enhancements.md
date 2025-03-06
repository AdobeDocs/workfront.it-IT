---
title: Altri miglioramenti durante il periodo di rilascio del secondo trimestre 2025
description: Altri miglioramenti durante il periodo di rilascio del secondo trimestre 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Altri miglioramenti durante il periodo di rilascio del secondo trimestre 2025

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del secondo trimestre 2025. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del secondo trimestre 2025, consulta [Panoramica sulla versione del secondo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Effettua l’aggiornamento alla nuova versione dell’abbonamento agli eventi con gli endpoint di aggiornamento della versione

>[!NOTE]
>
>Produzione per tutti i clienti: 6 marzo 2025

Workfront ora dispone di versioni delle sottoscrizioni agli eventi. La nuova versione non è una modifica all’API Workfront, ma piuttosto una modifica alla funzionalità di abbonamento agli eventi.

La possibilità di aggiornare o effettuare il downgrade degli abbonamenti agli eventi assicura che, quando vengono apportate modifiche alla struttura degli eventi, gli abbonamenti esistenti non si interrompano, consentendo di testare e aggiornare alla nuova versione senza interruzioni nell’abbonamento agli eventi.

Per ulteriori informazioni sulle differenze tra le due versioni, vedere l&#39;articolo [Controllo delle versioni delle sottoscrizioni di eventi](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Per informazioni sugli endpoint utilizzati per aggiornare o effettuare il downgrade di una sottoscrizione di eventi tra versioni, vedere la sezione [Controllo delle versioni delle sottoscrizioni di eventi](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) nell&#39;articolo API delle sottoscrizioni di eventi.

## Rappresenta le modifiche utente di Adobe Admin Console come &quot;System&quot; nel feed di aggiornamento di Workfront

>[!NOTE]
>
>Versione di anteprima: 23 gennaio 2025; produzione per rilascio rapido: con la versione 25.2 (13 febbraio 2025); produzione per rilascio trimestrale: con la versione 25.4 (aprile 2025)

Ora, quando l’amministratore di Adobe Admin Console apporta una modifica alle informazioni utente di un utente Workfront, Workfront registra tale modifica nella scheda Attività di sistema dell’area Aggiornamenti dell’utente come appartenente al &quot;Sistema&quot;. Si riferisce all’amministratore di Adobe Admin Console.

Prima di questo aggiornamento, le modifiche apportate dall’amministratore di Admin Console venivano registrate in base alle istruzioni dell’amministratore di sistema principale di Workfront.

Per informazioni sulla gestione degli utenti in Adobe Admin Console, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
