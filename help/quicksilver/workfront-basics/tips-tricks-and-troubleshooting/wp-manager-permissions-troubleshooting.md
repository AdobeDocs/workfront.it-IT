---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Risoluzione dei problemi relativi alle autorizzazioni di Workfront Proof Manager
description: I profili di autorizzazione disponibili in [!DNL Adobe] I Workfront per gli utenti di verifica sono Amministratore, Supervisore e Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Gestione bozze] risoluzione dei problemi relativi alle autorizzazioni

Di seguito sono riportati i profili di autorizzazione disponibili in [!DNL Adobe Workfront] per gli utenti di verifica:

* [!UICONTROL Amministratore]
* [!UICONTROL Supervisore]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Quando si concede un utente [!UICONTROL Manager] autorizzazioni, sono disponibili le seguenti informazioni per la risoluzione dei problemi:

* **PROBLEMA:** Utenti con [!UICONTROL Manager] Le autorizzazioni di non possono visualizzare le bozze create da altri utenti. Invece, visualizzano [!UICONTROL Accesso negato] schermo.

   ![](assets/access-denied-350x161.png)

   **SOLUZIONE:** Utenti con [!UICONTROL Manager] Le autorizzazioni di devono essere aggiunte esplicitamente alle bozze. Le bozze devono sempre essere create tramite [!UICONTROL Opzioni di verifica avanzate] e gli utenti devono sempre essere aggiunti tramite questa opzione.

* **PROBLEMA:** Utenti con [!UICONTROL Manager] Le autorizzazioni non possono aggiungere versioni di bozze alle bozze create da altri utenti (potrebbero potenzialmente inviare una bozza nel set di documenti, ma le versioni NON sarebbero connesse al set originale creato da un altro utente).\
   **SOLUZIONE:** Utenti con [!UICONTROL Manager] Le autorizzazioni di possono inviare le versioni alla bozza di un altro utente solo se l’utente con [!UICONTROL Manager] autorizzazioni quando:

   * Aggiunto esplicitamente alle bozze
   * Imposta come [!UICONTROL Autori] (ruolo bozza) sulle bozze

* **PROBLEMA:** Utenti con [!UICONTROL Manager] le autorizzazioni non possono modificare i commenti di altri utenti su una bozza di cui non sono proprietari o che non hanno creato.\
   **SOLUZIONE:** Se gli utenti con [!UICONTROL Manager] le autorizzazioni non sono proprietarie delle bozze, ma devono poter modificare i commenti e aggiungerli come [!UICONTROL Autori] (o [!UICONTROL Moderatori]).\
   Questi tre tipi di autorizzazioni sono disponibili in [!DNL Workfront] per [!UICONTROL Planner], [!UICONTROL Lavoratore], [!UICONTROL Richiessore], [!UICONTROL Revisore] digitare le licenze. Amministratore di sistema o Amministratore utenti in [!DNL Workfront] può modificare i profili degli utenti e regolare [!DNL Workfront Proof] autorizzazioni da lì.
