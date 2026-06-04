---
title: Altri miglioramenti durante l’arco temporale di rilascio del secondo trimestre 2025
description: Altri miglioramenti durante il periodo di rilascio del secondo trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/s8T1ziXqzEOn8yipB5UdM-nShwJhYbCPNfIycC3GjYw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 27%

---

# Altri miglioramenti durante l’arco temporale di rilascio del secondo trimestre 2025

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del secondo trimestre 2025. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del secondo trimestre 2025, consulta [Panoramica sulla versione del secondo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Effettua l’aggiornamento alla nuova versione dell’abbonamento agli eventi con gli endpoint di aggiornamento della versione

>[!NOTE]
>
>Produzione per tutti i clienti: 6 marzo 2025

Workfront ora dispone di versioni delle sottoscrizioni agli eventi. Questa nuova versione non cambia l’API Workfront, ma la funzionalità di sottoscrizione eventi.

La possibilità di aggiornare o eseguire il downgrade delle sottoscrizioni eventi assicura che, quando vengono apportate modifiche alla struttura degli eventi, le sottoscrizioni esistenti non vengano interrotte, consentendo di testarle e aggiornarle alla nuova versione senza interruzioni nella sottoscrizione eventi.

Per ulteriori informazioni sulle differenze tra le due versioni, vedere l&#39;articolo [Controllo delle versioni delle sottoscrizioni di eventi](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Per informazioni sugli endpoint utilizzati per aggiornare o effettuare il downgrade di una sottoscrizione di eventi tra versioni, vedere la sezione [Controllo delle versioni delle sottoscrizioni di eventi](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) nell&#39;articolo API delle sottoscrizioni di eventi.

## Rappresenta le modifiche utente di Adobe Admin Console come &quot;System&quot; nel feed di aggiornamento di Workfront

>[!NOTE]
>
>Versione di anteprima: 23 gennaio 2025; produzione per rilascio rapido: con la versione 25.2 (13 febbraio 2025); produzione per rilascio trimestrale: con la versione 25.4 (aprile 2025)

Ora, quando l’amministratore di Adobe Admin Console apporta una modifica alle informazioni utente di un utente Workfront, Workfront registra tale modifica nella scheda Attività di sistema dell’area Aggiornamenti dell’utente come appartenente al &quot;Sistema&quot;. Si riferisce all’amministratore di Adobe Admin Console.

Prima di questo aggiornamento, le modifiche apportate dall’amministratore di Admin Console venivano registrate in base alle istruzioni dell’amministratore di sistema principale di Workfront.

Per informazioni sulla gestione degli utenti in Adobe Admin Console, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
