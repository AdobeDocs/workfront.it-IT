---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Panoramica degli aggiornamenti tracciati dal sistema
description: Adobe Workfront acquisisce l'attività che si svolge su determinati oggetti registrando le informazioni sullo stato nell'area [!UICONTROL Aggiornamenti] dell'oggetto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 4448d2fc6d0230ef2f53ad0ea7ae0f10f52fcac4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Panoramica degli aggiornamenti monitorati dal sistema

<!-- Audited: 06/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront] acquisisce l&#39;attività che si svolge su determinati oggetti registrando le informazioni sullo stato nella sezione [!UICONTROL Aggiornamenti] dell&#39;oggetto.

Per informazioni sulla sezione Aggiornamenti, vedere [Panoramica della sezione Aggiornamenti](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

L&#39;area [!UICONTROL Aggiornamenti] include i seguenti tipi di aggiornamenti:

* **Aggiornamenti utente:** immessi manualmente dagli utenti. Denominati anche commenti, risposte e note. Gli aggiornamenti utente vengono visualizzati nelle schede Commenti e Tutti della sezione Aggiornamenti di un oggetto.

  Per ulteriori informazioni sulla configurazione degli aggiornamenti utente, vedere [Configurare le preferenze per gli aggiornamenti utente](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![Aggiornamenti](assets/updates-qs-350x125.png)

* **Aggiornamenti di sistema:** eseguiti automaticamente dal sistema. Un aggiornamento del sistema include una breve nota che descrive il tipo di modifica apportata all&#39;elemento. Gli aggiornamenti di sistema vengono visualizzati nelle schede Attività di sistema e Tutti nella sezione Aggiornamenti di un oggetto.

  Per ulteriori informazioni sui feed di aggiornamento del sistema e su come attivarli, vedere [Configurare gli aggiornamenti del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![Esempio di aggiornamenti di sistema](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considerazioni sugli aggiornamenti tracciati dal sistema

Gli aggiornamenti tracciati dal sistema non sono disponibili per tutti gli oggetti che dispongono dell&#39;area Aggiornamenti.

* L&#39;area [!UICONTROL Aggiornamenti] è disponibile per i seguenti oggetti:

   * [!UICONTROL Progetto]
   * [!UICONTROL Attività]
   * [!UICONTROL Problema]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programma]
   * [!UICONTROL Utente]
   * [!UICONTROL Modello]
   * [!UICONTROL Attività modello]
   * [!UICONTROL Team]
   * [!UICONTROL Documento]
   * [!UICONTROL Scheda orario]
   * [!UICONTROL Storia]

     In [!DNL Workfront] una storia è un&#39;attività.
   * [!UICONTROL Iterazione]
   * [!UICONTROL Obiettivo]

     Non tutti i pacchetti Workfront includono gli obiettivi di Workfront. Per informazioni, vedere [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Scheda] su una bacheca

     Per ulteriori informazioni sugli aggiornamenti sulle schede, vedere [Utilizzare schede collegate sulle schede](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] non tiene traccia degli aggiornamenti di sistema per i seguenti oggetti:

   * [!UICONTROL Team]
   * [!UICONTROL Modello]
   * [!UICONTROL Attività modello]
   * [!UICONTROL Scheda] ad hoc
   * [!UICONTROL Iterazioni]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Gli aggiornamenti utente vengono visualizzati nella scheda Commenti e gli aggiornamenti di sistema nelle schede Attività di sistema e Tutti.

  Per un elenco degli oggetti che non hanno le schede Attività di sistema o Tutte, vedere [Panoramica della sezione Aggiornamento](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* Impossibile aggiungere una risposta a un aggiornamento del sistema. Tuttavia, tutte le risposte ai record di attività del sistema nell’esperienza di commento legacy precedenti all’11 aprile 2024 sono compilate nella scheda Attività del sistema in sola lettura.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* Gli amministratori di [!DNL Workfront] possono definire il tipo di modifiche che il sistema deve monitorare nell&#39;area [!UICONTROL Aggiornamenti]. Non tutti gli oggetti con un&#39;area [!UICONTROL Aggiornamenti] hanno anche feed [!UICONTROL aggiornamento] configurabili. I seguenti oggetti hanno un&#39;area [!UICONTROL Aggiornamenti] che acquisisce i feed di aggiornamento tracciati dal sistema, ma non dispongono di feed di aggiornamento configurabili:

   * [!UICONTROL Documento]
   * [!UICONTROL Scheda orario]
   * [!UICONTROL Iterazione]
   * [!UICONTROL Obiettivo]


