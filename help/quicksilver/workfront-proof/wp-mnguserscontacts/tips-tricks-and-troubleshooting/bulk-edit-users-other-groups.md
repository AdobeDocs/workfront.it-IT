---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Modifica in serie altri gruppi dell'utente
description: Durante la modifica in serie ho tentato di aggiungere un singolo altro gruppo a numerosi utenti. Dopo aver salvato le modifiche, tutti gli altri gruppi esistenti sono stati rimossi e solo il nuovo altro gruppo è rimasto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Modifica in serie altri gruppi dell&#39;utente

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Durante la modifica in serie ho tentato di aggiungere un singolo altro gruppo a numerosi utenti.
Dopo aver salvato le modifiche, tutti gli altri gruppi esistenti sono stati rimossi e solo il nuovo altro gruppo è rimasto.

## Risposta:

Il comportamento risultante dipende dall’appartenenza al gruppo corrente degli utenti selezionati:

* Se tutti gli utenti selezionati Altre appartenenze a gruppi corrispondono esattamente.. Dopo aver selezionato gli utenti e selezionato [!UICONTROL modifica], [!UICONTROL Altri gruppi] Il campo mostrerà l’elenco completo di tutti i gruppi a cui appartengono questi utenti.

* Se gli utenti selezionati hanno appartenenze diverse ad Altri gruppi... Dopo aver selezionato gli utenti e fatto clic su [!UICONTROL Modifica], [!UICONTROL Altri gruppi] Il campo sarà vuoto.

Quando fai clic su **[!UICONTROL Salva modifiche]**, viene salvato tutto ciò che viene visualizzato nel campo Altri gruppi .

Il contenuto precedente del campo viene sovrascritto.
