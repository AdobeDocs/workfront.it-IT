---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 è obbligatorio in Adobe Workfront
description: Per garantire una sicurezza ottimale, Adobe Workfront richiede che tutte le connessioni browser e le integrazioni API che si basano su TLS 1.0 o versioni precedenti siano aggiornate per utilizzare TLS 1.2. Nell’ambiente di anteprima, TLS 1.0 è già disabilitato.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
TQID: https://experienceleague.adobe.com/23UVEvZitUFvhkTkgOnubLK76Lzl8QKiyz-R4svWcc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 4%

---

# TLS 1.2 è obbligatorio in Adobe Workfront

Per garantire una sicurezza ottimale, Adobe Workfront richiede che tutte le connessioni browser e le integrazioni API che si basano su TLS 1.0 o versioni precedenti siano aggiornate per utilizzare TLS 1.2. Nell’ambiente di anteprima, TLS 1.0 è già disabilitato.

Workfront ha ufficialmente terminato il supporto per TLS 1.0 a marzo 2018. Tutte le integrazioni che sfruttano TLS 1.0 non funzioneranno più dal 9 gennaio 2019.  TLS 1.1 verrà disattivato nel quarto trimestre del 2019.

Le sezioni seguenti forniscono ulteriori dettagli su questi importanti obiettivi intermedi e su come prepararti per questo aggiornamento nella tua organizzazione:

## Workfront termina il supporto ufficiale di TLS 1.0 (5 marzo 2018)

Workfront ha terminato il supporto ufficiale per TLS 1.0 a marzo 2018.

Le connessioni browser e le integrazioni API che sfruttano TLS 1.0 sono ancora operative, ma Workfront non risolve i problemi nell’applicazione Workfront relativi a TLS 1.0.

## Integrazioni Workfront con TLS 1.0 disabilitate (9 gennaio 2019)

Il 9 gennaio 2019, tutte le connessioni al browser Workfront e le integrazioni API che sfruttano TLS 1.0 devono essere aggiornate per utilizzare TLS 1.1 o versione successiva. Le connessioni browser e le integrazioni API che continuano a utilizzare TLS 1.0 (connessioni in entrata o in uscita) non saranno più in grado di comunicare con l’applicazione Workfront dopo questo periodo di tempo. 

## TLS 1.1 da disabilitare nel quarto trimestre 2019

Nell’ambiente di produzione, TLS 1.1 è stato disattivato il 21 ottobre 2019. Trascorso questo periodo, tutte le integrazioni che utilizzano TLS 1.1 non funzioneranno più.

Questa modifica entrerà in vigore negli ambienti di anteprima e sandbox il 7 agosto per aiutare le organizzazioni a prepararsi per lo spegnimento.

## Preparazione per l’aggiornamento TLS

* [Accesso a Workfront tramite il browser](#when-accessing-workfront-via-the-browser)
* [Quando ci si connette a Workfront tramite l’API](#when-connecting-to-workfront-via-the-api)

### Quando si accede a Workfront tramite il browser {#when-accessing-workfront-via-the-browser}

Assicurati che gli utenti della tua organizzazione accedano a Workfront tramite un browser supportato. (Per informazioni sui browser supportati, vedi [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Tutti i browser supportati da Workfront sono compatibili con TLS 1.2.

### Quando ci si connette a Workfront tramite l’API {#when-connecting-to-workfront-via-the-api}

Se stai integrando applicazioni di terze parti in Workfront tramite l’API (in entrata o in uscita), assicurati che TLS 1.2 (e i protocolli di crittografia TLS 1.2) siano abilitati nelle integrazioni.
