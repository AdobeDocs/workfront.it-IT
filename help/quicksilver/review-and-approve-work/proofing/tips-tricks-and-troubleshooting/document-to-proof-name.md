---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Nome del documento modificato dopo il caricamento e contiene un carattere non valido
description: Alcuni documenti non possono essere convertiti in bozze.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 16%

---

# Nome del documento modificato dopo il caricamento e contiene un carattere non valido

## Problema

Alcuni documenti non possono essere convertiti in bozze.

## Causa

I file caricati in Workfront non possono contenere determinati caratteri nei nomi dei file. Se un file contiene uno dei seguenti caratteri nel nome del file, i caratteri vengono rimossi dal nome del file al caricamento: `! # % * \ | ' " / ? < > { } [ ]`.

Se il nome di un documento viene aggiornato in modo da includere un carattere non valido dopo il caricamento iniziale, la generazione della bozza non riuscirà.

## Soluzione

Rimuovi il carattere non valido dal nome del documento:

1. Selezionare il documento, quindi fare clic su **Dettagli documento**.
1. Fare clic sul nome del documento, rimuovere il carattere non valido e premere Invio.

   Caratteri non validi: `! # % * \ | ' " / ? < > { } [ ]`

   ![Nome documento](assets/doc-name.png)

1. Aggiorna la pagina e genera la bozza.
