---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Risoluzione dei problemi relativi alle autorizzazioni di Workfront Proof Manager
description: I profili di autorizzazione disponibili in [!DNL Adobe] Workfront per gli utenti di verifica sono Amministratore, Supervisore e Manager.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Risoluzione dei problemi relativi alle autorizzazioni di [!UICONTROL [!DNL Workfront] Proof Manager]

Di seguito sono riportati i profili di autorizzazione disponibili in [!DNL Adobe Workfront] per gli utenti di verifica:

* [!UICONTROL Amministratore]
* [!UICONTROL Supervisore]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Quando si concedono a un utente le autorizzazioni [!UICONTROL Manager], sono disponibili le seguenti informazioni per la risoluzione dei problemi:

* **PROBLEMA:** gli utenti con autorizzazioni [!UICONTROL Manager] non possono visualizzare le bozze create da altri utenti. Viene invece visualizzata la schermata [!UICONTROL Accesso negato].

  ![](assets/access-denied-350x161.png)

  **SOLUZIONE:** Gli utenti con autorizzazioni [!UICONTROL Manager] devono essere aggiunti in modo esplicito alle bozze. Le bozze devono sempre essere create tramite la finestra [!UICONTROL Opzioni di bozza avanzate] e gli utenti devono sempre essere aggiunti tramite questa opzione.

* **PROBLEMA:** Gli utenti con autorizzazioni [!UICONTROL Manager] non possono aggiungere versioni delle bozze alle bozze create da altri utenti. Potrebbero inviare una bozza nel set di documenti, ma le versioni NON sarebbero connesse al set originale creato da un altro utente.\
   **SOLUZIONE:** Gli utenti con autorizzazioni [!UICONTROL Manager] possono inviare le versioni alla bozza di un altro utente solo se l&#39;utente con autorizzazioni [!UICONTROL Manager] dispone di entrambe le seguenti autorizzazioni:

   * Aggiunto esplicitamente alle bozze
   * Imposta come [!UICONTROL Autori] (ruolo bozza) sulle bozze

* **PROBLEMA:** Gli utenti con autorizzazioni [!UICONTROL Manager] non possono modificare i commenti di altri utenti su una bozza di cui non sono proprietari o che non hanno creato.\
   **SOLUZIONE:** Se gli utenti con autorizzazioni [!UICONTROL Manager] non sono proprietari delle bozze, ma devono essere in grado di modificare i commenti, aggiungerli come [!UICONTROL Autori] (o [!UICONTROL Moderatori]).\
   Questi tre tipi di autorizzazioni sono disponibili in [!DNL Workfront] per le licenze di tipo [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Richiedente], [!UICONTROL Revisore]. L&#39;amministratore di sistema o l&#39;amministratore utenti in [!DNL Workfront] può modificare i profili degli utenti e modificare le autorizzazioni di [!DNL Workfront Proof] da tale posizione.
