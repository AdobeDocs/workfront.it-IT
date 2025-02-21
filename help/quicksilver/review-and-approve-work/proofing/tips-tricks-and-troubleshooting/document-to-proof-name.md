---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Il nome del documento è stato modificato dopo il caricamento e contiene un carattere non valido
description: Alcuni documenti non possono essere convertiti in bozze.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Il nome del documento è stato modificato dopo il caricamento e contiene un carattere non valido

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
