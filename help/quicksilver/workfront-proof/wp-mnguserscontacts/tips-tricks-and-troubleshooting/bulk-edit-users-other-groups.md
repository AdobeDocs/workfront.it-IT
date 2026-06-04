---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Modifica in blocco di Altri gruppi per più utenti
description: Durante la modifica in blocco ho tentato di aggiungere un singolo Altri gruppi a numerosi utenti. Dopo il salvataggio delle modifiche, tutti gli altri gruppi esistenti sono stati rimossi e solo il nuovo Altro gruppo è rimasto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 5%

---

# Modifica in blocco di Altri gruppi per più utenti

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
