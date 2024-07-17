---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Modifica in blocco altri gruppi dell'utente
description: Durante la modifica in blocco ho tentato di aggiungere un singolo Altri gruppi a numerosi utenti. Dopo il salvataggio delle modifiche, tutti gli altri gruppi esistenti sono stati rimossi e solo il nuovo Altro gruppo è rimasto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Modifica in blocco altri gruppi dell&#39;utente

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

## Problema:

Durante la modifica in blocco ho tentato di aggiungere un singolo Altri gruppi a numerosi utenti.
Dopo il salvataggio delle modifiche, tutti gli altri gruppi esistenti sono stati rimossi e solo il nuovo Altro gruppo è rimasto.

## Risposta:

Il comportamento risultante dipende dall&#39;appartenenza al gruppo corrente degli utenti selezionati:

* Se tutti gli utenti selezionati l&#39;appartenenza ad altri gruppi corrisponde esattamente...
Dopo aver selezionato gli utenti e aver selezionato [!UICONTROL modifica], nel campo [!UICONTROL Altri gruppi] verrà visualizzato l&#39;elenco completo
di tutti i gruppi a cui appartengono questi utenti.

* Se gli utenti selezionati hanno appartenenze ad altri gruppi diverse...
Dopo aver selezionato gli utenti e aver fatto clic su [!UICONTROL Modifica], il campo [!UICONTROL Altri gruppi] sarà vuoto.

Quando fai clic su **[!UICONTROL Salva modifiche]**, viene salvato tutto ciò che viene visualizzato nel campo Altri gruppi.

I contenuti precedenti del campo vengono sovrascritti.
