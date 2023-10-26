---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Aggiornamenti monitorati dal sistema
description: Adobe Workfront acquisisce l’attività che si svolge su determinati oggetti registrando le informazioni sullo stato nel file [!UICONTROL Aggiornamenti] area.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 6%

---

# Aggiornamenti monitorati dal sistema

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] acquisisce l&#39;attività che si svolge su determinati oggetti registrando le informazioni sullo stato nel [!UICONTROL Aggiornamenti] area.

Il [!UICONTROL Aggiornamenti] L&#39;area include i seguenti tipi di aggiornamenti:

* **Aggiornamenti utente:** Inserito manualmente dagli utenti. Denominati anche commenti, risposte e note.

  Per ulteriori informazioni sulla configurazione degli aggiornamenti utente, consulta [Configurare le preferenze per gli aggiornamenti utente](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Aggiornamenti di sistema:** Automaticamente eseguita dal sistema. Un aggiornamento del sistema include una breve nota che descrive il tipo di modifica apportata all&#39;elemento.

  Per ulteriori informazioni sui feed di aggiornamento del sistema e su come attivarli, vedere [Configurare gli aggiornamenti di sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considerazioni sugli aggiornamenti tracciati dal sistema

Gli aggiornamenti tracciati dal sistema non sono disponibili per tutti gli oggetti che dispongono dell&#39;area Aggiornamenti.

* Il [!UICONTROL Aggiornamenti] L&#39;area è disponibile per i seguenti oggetti:

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

     In entrata [!DNL Workfront], una storia è un&#39;attività.
   * [!UICONTROL Iterazione]
   * [!UICONTROL Obiettivo]

     Per accedere alla proprietà è necessaria una licenza aggiuntiva [!UICONTROL Obiettivi] area. Per informazioni, consulta [Requisiti per l’utilizzo degli obiettivi di Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Scheda] su una bacheca

     Per ulteriori informazioni sugli aggiornamenti sulle schede, consulta [Utilizzare le schede collegate sulle bacheche](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] non tiene traccia degli aggiornamenti di sistema per i seguenti oggetti:

   * [!UICONTROL Team]
   * [!UICONTROL Modello]
   * [!UICONTROL Attività modello]
   * Ad hoc [!UICONTROL Scheda]
   * [!UICONTROL Iterazioni]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Di seguito sono riportate le differenze tra la nuova esperienza di commento e quella precedente:

   * Quando si utilizza la nuova esperienza di inserimento di commenti, gli aggiornamenti utente vengono visualizzati nella scheda Commenti e gli aggiornamenti di sistema nella scheda Attività di sistema.

     Per ulteriori informazioni sulla nuova esperienza di aggiunta di commenti, vedi [Nuova esperienza di commento](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * Quando si utilizza l’esperienza di commento legacy, gli aggiornamenti di sistema e utente vengono visualizzati in un unico feed continuo.

   * Quando si utilizza l’esperienza di commento legacy, gli utenti possono visualizzare gli aggiornamenti di sistema per impostazione predefinita o scegliere di non visualizzarli. Non è possibile disabilitare gli aggiornamenti di sistema quando si utilizza la nuova esperienza di aggiunta di commenti.

     Per informazioni sulla disattivazione della visualizzazione degli aggiornamenti di sistema, vedere la sezione [Attivare o disattivare gli aggiornamenti di sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) nell’articolo [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront registra gli aggiornamenti tracciati dal sistema per i seguenti oggetti, ma non è possibile disattivarne la visualizzazione:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programma]
   * [!UICONTROL Iterazione]

* [!DNL Workfront] gli amministratori possono definire il tipo di modifiche che il sistema deve tracciare nel [!UICONTROL Aggiornamenti] area. Non tutti gli oggetti con [!UICONTROL Aggiornamenti] area hanno anche configurato [!UICONTROL aggiorna] feed. I seguenti oggetti hanno un [!UICONTROL Aggiornamenti] area in cui vengono acquisiti i feed di aggiornamento tracciati dal sistema, ma per i quali non sono disponibili feed di aggiornamento configurabili:

   * [!UICONTROL Documento]
   * [!UICONTROL Scheda orario]
   * [!UICONTROL Iterazione]
   * [!UICONTROL Obiettivo]


