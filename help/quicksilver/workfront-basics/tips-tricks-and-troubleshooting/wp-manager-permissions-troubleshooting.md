---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Risoluzione dei problemi relativi alle autorizzazioni di Workfront Proof Manager
description: Di seguito sono riportati i profili di autorizzazione disponibili in [!DNL Adobe] Workfront per la correzione degli utenti - EDIT ME.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Responsabile delle prove] risoluzione dei problemi delle autorizzazioni

Di seguito sono riportati i profili di autorizzazione disponibili in [!DNL Adobe Workfront] per gli utenti di bozze:

* [!UICONTROL Amministratore]
* [!UICONTROL Supervisore]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Quando si concede un utente [!UICONTROL Manager] autorizzazioni, sono disponibili le seguenti informazioni per la risoluzione dei problemi:

* **PROBLEMA:** Utenti con [!UICONTROL Manager] le autorizzazioni non possono visualizzare le bozze create da altri utenti. Invece, vedono la [!UICONTROL Accesso negato] schermo.

   ![](assets/access-denied-350x161.png)

   **SOLUZIONE:** Utenti con [!UICONTROL Manager] le autorizzazioni devono essere aggiunte esplicitamente alle bozze. Le bozze devono sempre essere create tramite il [!UICONTROL Opzioni di correzione avanzate] e gli utenti devono sempre essere aggiunti tramite questa opzione.

* **PROBLEMA:** Utenti con [!UICONTROL Manager] Le autorizzazioni non possono aggiungere versioni di bozza alle bozze create da altri utenti (potrebbero potenzialmente inviare una bozza nel set di documenti, ma le versioni NON sarebbero collegate al set originale creato da un altro utente).\
   **SOLUZIONE:** Utenti con [!UICONTROL Manager] le autorizzazioni possono inviare le versioni alla bozza di un altro utente solo se l&#39;utente con [!UICONTROL Manager] autorizzazioni quando :

   * Aggiunto esplicitamente alle bozze
   * Imposta come [!UICONTROL Autori] (ruolo di prova) sulle prove

* **PROBLEMA:** Utenti con [!UICONTROL Manager] Le autorizzazioni non possono modificare i commenti di altri utenti su una bozza che non possiedono o che non hanno creato.\
   **SOLUZIONE:** Se gli utenti utilizzano [!UICONTROL Manager] le autorizzazioni non possiedono le bozze, ma devono essere in grado di modificare i commenti e aggiungerli come [!UICONTROL Autori] o [!UICONTROL Moderatori]).\
   Questi tre tipi di autorizzazioni sono disponibili in [!DNL Workfront] per [!UICONTROL Planner], [!UICONTROL Lavoratore], [!UICONTROL Richiedente], [!UICONTROL Revisore] licenze di tipo. Amministratore di sistema o amministratore utente in [!DNL Workfront] può modificare i profili degli utenti e regolare [!DNL Workfront Proof] autorizzazioni da lì.
