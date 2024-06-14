---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurare le impostazioni di visualizzazione Calendario predefinito
description: È possibile configurare le impostazioni del Calendario predefinito per l'integrazione con una versione di Outlook basata sul Web e consentire di tenere traccia del carico di lavoro in base alle ore lavorative disponibili.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Configurare [!UICONTROL Calendario predefinito] impostazioni di visualizzazione

<!--Audited: 01/2024-->

È possibile configurare [!UICONTROL Calendario predefinito] impostazioni per eseguire le operazioni seguenti:

* Integrare con una versione basata sul web di [!DNL Outlook] in [!DNL Office 365] o [!DNL Outlook Live] ospitati nel cloud. È possibile visualizzare tutti gli eventi dal calendario di Outlook e tutti i calendari associati selezionati nel [!UICONTROL Calendario predefinito] in Adobe Workfront.
* Consente di tenere traccia del carico di lavoro rispetto alle ore lavorative disponibili sul [!UICONTROL Allocazione] barra.

Per ulteriori informazioni sul Calendario predefinito, consulta [[!UICONTROL Calendario predefinito] visualizza](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

In questo articolo viene descritto come configurare le impostazioni del Calendario predefinito e integrare il Calendario predefinito con il calendario di Outlook esterno.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>Corrente: [!UICONTROL Work] o versione successiva</p> 
   Oppure
   <p>Nuovo: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Per sapere quale piano o tipo di licenza si dispone, contattare il [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sull’integrazione [!DNL Microsoft Outlook] calendari

Quando configuri il Calendario predefinito con il tuo [!DNL Microsoft Outlook] calendario:

* È possibile integrare solo una versione basata sul Web di [!DNL Outlook] in hosting cloud [!DNL Office 365] o [!DNL Outlook Live].

  On-premise [!DNL Outlook] e [!DNL Outlook] su un&#39;azienda basata su cloud [!DNL Exchange] server non supportati.

  Se l&#39;organizzazione utilizza il Single Sign-On, è necessario [!DNL Microsoft 365 E3] o [!DNL E5].

* Allegati associati al tuo [!DNL Outlook] gli eventi non sono associati al [!DNL Outlook] eventi nel Calendario predefinito.
* Integrazione con un [!DNL Outlook] il calendario deve essere completato singolarmente per ogni utente.
* Eventi visualizzati nel [!UICONTROL Scadenza] non vengono visualizzate sul [!DNL Microsoft] a meno che non siano stati trascinati dal [!UICONTROL Elenco lavori] al tuo [!DNL Adobe Workfront] Calendario. Per ulteriori informazioni, consulta [[!UICONTROL Scadenza] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Elenco lavori sul [!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Calendario predefinito] visualizza](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Quando abiliti l’integrazione con [!DNL Outlook], solo gli elementi di lavoro trascinati nel [!UICONTROL Calendario predefinito] da quel momento in poi si sincronizzerà. Gli elementi presenti nell’Home Calendar prima dell’abilitazione dell’integrazione non verranno visualizzati ed è necessario trascinarli nuovamente nell’Home Calendar per visualizzarli in [!DNL Outlook].
* Quando si condivide (o si annulla la condivisione) un [!DNL Outlook] o quando si modifica il livello di autorizzazione per un calendario condiviso con altri utenti, questa modifica non influisce sui calendari per circa 30 minuti. Per ulteriori informazioni, consultare [!DNL Microsoft Outlook] documentazione.\
   Di conseguenza, quando si integra [!DNL Workfront] Calendario con [!DNL Outlook] che condividi con altri utenti, non vedranno il tuo [!DNL Workfront] Elementi del calendario per circa 30 minuti.

>[!NOTE]
>
>Il [!DNL Outlook] la configurazione del calendario è completamente separata dalla [!DNL Outlook] Componente aggiuntivo ([!UICONTROL [!DNL Outlook] Integrazione] o [!DNL Workfront Outlook]). Non è necessaria alcuna installazione per configurare il calendario, ma è necessaria un&#39;installazione per [!DNL Outlook] Componente aggiuntivo. Per ulteriori informazioni su [!DNL Outlook] Componente aggiuntivo vedere [Configurazione [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configurare [!UICONTROL Calendario predefinito] visualizzare le impostazioni e integrarle con i calendari di Outlook

1. In [!UICONTROL Calendario predefinito] , fare clic sul pulsante **[!UICONTROL Impostazioni]** icona ingranaggio ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) nell&#39;angolo superiore destro per aprire **[!UICONTROL Impostazioni calendario]** sulla destra.

   Se hai bisogno di informazioni sull’accesso a [!UICONTROL Calendario predefinito] visualizza, vedi [Visualizza [!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facoltativo) Per integrare [!DNL Microsoft Outlook] calendario, fai clic su **[!UICONTROL Aggiungi account]** nell&#39;angolo superiore destro del **[!UICONTROL Impostazioni calendario]** pannello. Quindi, se ti viene richiesto di farlo, immetti il [!DNL Microsoft Outlook] informazioni di accesso. È possibile ripetere questo passaggio per aggiungere più [!DNL Outlook] account.

   >[!NOTE]
   >
   >Devi dare [!DNL Workfront] autorizzazione ad accedere al tuo [!DNL Outlook] calendario. La concessione dell’autorizzazione consente [!DNL Workfront] per mantenere l&#39;accesso ai dati del calendario, leggere [!DNL outlook] e leggi e aggiorna i tuoi [!DNL Microsoft] calendario.

1. Aggiorna la finestra del browser per visualizzare le informazioni [!DNL Outlook] account nel calendario e nel [!UICONTROL Impostazioni calendario] pannello.
1. Fai clic su **[!UICONTROL Impostazioni]** icona ingranaggio di nuovo nell&#39;angolo superiore destro per aprire **[!UICONTROL Impostazioni calendario]** pannello. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (Facoltativo) Sotto ogni [!DNL Microsoft] account aggiunto nel passaggio precedente, seleziona **[!UICONTROL Visualizza]** o **[!UICONTROL Sincronizza]**:

   * **[!UICONTROL Visualizza]**: opzione di sola lettura che consente di visualizzare [!DNL Microsoft] eventi calendario sul tuo [!UICONTROL Calendario predefinito].
   * **[!UICONTROL Sincronizza]**: questa opzione consente una sincronizzazione bidirezionale tra [!DNL Microsoft] e [!UICONTROL Home] calendari. In altre parole, [!DNL Workfront] [!UICONTROL Calendario predefinito] elementi esportati nel tuo [!DNL Microsoft] calendario e [!DNL Microsoft] elementi del calendario importati nel Workfront [!UICONTROL Calendario predefinito] in tempo reale.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Facoltativo) Sotto il [!DNL Workfront] o un account integrato, selezionare i calendari associati che si desidera visualizzare sul [!UICONTROL Calendario predefinito] (ad esempio il calendario PTO, Compleanni o Festività), quindi fare clic su [!UICONTROL Aggiorna] o [!UICONTROL Ricarica] per visualizzare le modifiche.

1. (Facoltativo) In **[!UICONTROL Generale]** sezione in **[!UICONTROL Inizio settimana il]**, selezionare il giorno che si desidera visualizzare come primo giorno della settimana lavorativa nel Calendario predefinito.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configura le seguenti opzioni:

   * **[!UICONTROL I miei giorni di lavoro]:** Selezionare i giorni di lavoro.
   * **[!UICONTROL Il mio tempo iniziale normale]:** Selezionare l&#39;ora di inizio della giornata lavorativa.
   * **[!UICONTROL Il mio tempo finale normale]:** Selezionare l&#39;ora di fine della giornata lavorativa.

   [!DNL Workfront] utilizza queste tre impostazioni per calcolare il numero di ore lavorative in una settimana. Questo numero influisce sul [!UICONTROL Allocazione] che consente di tenere traccia del carico di lavoro in base alle ore lavorative disponibili. Per ulteriori informazioni, consulta [[!UICONTROL Allocazione] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) nell’articolo [[!UICONTROL Calendario predefinito] visualizza](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Fai clic all’esterno del **[!UICONTROL Impostazioni calendario]** per chiuderlo.

   [!DNL Workfront] salva automaticamente le modifiche.

Per informazioni sull&#39;utilizzo di [!UICONTROL Calendario] visualizzazione per gestire le assegnazioni di lavoro e gli eventi di calendario integrati, vedere [Utilizza il [!UICONTROL Calendario predefinito] visualizza](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
