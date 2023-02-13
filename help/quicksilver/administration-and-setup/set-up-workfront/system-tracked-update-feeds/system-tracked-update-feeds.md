---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Aggiornamenti tracciati dal sistema
description: Adobe Workfront acquisisce l’attività che si svolge su determinati oggetti registrando le informazioni sullo stato nel [!UICONTROL Aggiornamenti] area.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Aggiornamenti tracciati dal sistema

[!DNL Adobe Workfront] acquisisce l&#39;attività che si svolge su determinati oggetti registrando le informazioni sullo stato nel [!UICONTROL Aggiornamenti] area.

La [!UICONTROL Aggiornamenti] l’area include i seguenti tipi di aggiornamenti:

* **Aggiornamenti utente:** Inserito manualmente dagli utenti. Denominati anche osservazioni, risposte e note.

   ![](assets/updates-qs-350x125.png)

* **Aggiornamenti di sistema:** Effettuata automaticamente dal sistema. Un aggiornamento del sistema include una breve nota che descrive il tipo di modifica apportata all&#39;elemento.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Gli aggiornamenti possono essere apportati ai seguenti oggetti:

* Progetto
* Attività
* Problema
* Portfolio
* Programma
* Utente
* Modelli
* Attività del modello
* Documenti
* Schede orario

Le [!DNL Workfront] la licenza determina se gli aggiornamenti del sistema vengono visualizzati per impostazione predefinita nel [!UICONTROL Aggiornamenti] area degli oggetti. [!DNL Workfront] utenti con un [!UICONTROL Pianificare] la licenza visualizza gli aggiornamenti di sistema nella [!UICONTROL Aggiornamenti] area per impostazione predefinita. Tuttavia, gli utenti possono filtrare gli aggiornamenti di sistema, come descritto in [[!UICONTROL Abilita] o disattiva gli aggiornamenti del sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) sezione [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Tutti gli altri [!DNL Workfront] per impostazione predefinita, gli aggiornamenti del sistema del filtro licenze vengono filtrati.

[!DNL Workfront] gli amministratori possono definire il tipo di modifiche che il sistema deve monitorare nel [!UICONTROL Aggiornamenti] area. Non tutti gli oggetti sono configurabili [!UICONTROL update] feed di stato. I seguenti oggetti hanno un [!UICONTROL Aggiornamenti] area che acquisisce i feed di aggiornamento tracciati dal sistema, ma che non dispone di feed di stato di aggiornamento configurabili:

* Modelli
* Attività del modello
* Documenti
* Schede orario

Per ulteriori informazioni sui feed di aggiornamento del sistema e su come attivarli, consulta [Configurare gli aggiornamenti di sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Per ulteriori informazioni sulla configurazione degli aggiornamenti utente, consulta [Configurare le preferenze per gli aggiornamenti utente](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
