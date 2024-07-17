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

# Configura le impostazioni di visualizzazione del [!UICONTROL Calendario predefinito]

<!--Audited: 01/2024-->

È possibile configurare le impostazioni del [!UICONTROL Calendario predefinito] per eseguire le operazioni seguenti:

* Integrare con una versione basata sul web di [!DNL Outlook] in [!DNL Office 365] o [!DNL Outlook Live] ospitati nel cloud. È possibile visualizzare tutti gli eventi dal calendario di Outlook e tutti i calendari associati selezionati nel [!UICONTROL Calendario predefinito] in Adobe Workfront.
* Puoi tenere traccia del carico di lavoro rispetto alle ore lavorative disponibili sulla barra [!UICONTROL Allocazione].

Per ulteriori informazioni sul Calendario predefinito, vedere [[!UICONTROL Calendario predefinito] visualizzazione](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

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

*Per sapere quale piano o tipo di licenza si dispone, contattare l&#39;amministratore [!DNL Workfront]. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sull&#39;integrazione di [!DNL Microsoft Outlook] calendari

Durante la configurazione del Calendario predefinito con il calendario [!DNL Microsoft Outlook], tenere presente quanto segue:

* È possibile integrare solo una versione basata sul Web di [!DNL Outlook] in [!DNL Office 365] o [!DNL Outlook Live] ospitato dal cloud.

  I server [!DNL Outlook] e [!DNL Outlook] locali in un server [!DNL Exchange] aziendale basato su cloud non sono supportati.

  Se l&#39;organizzazione utilizza il Single Sign-On, sono necessari [!DNL Microsoft 365 E3] o [!DNL E5].

* Gli allegati associati agli eventi [!DNL Outlook] non sono allegati agli eventi [!DNL Outlook] nel Calendario predefinito.
* L&#39;integrazione con un calendario [!DNL Outlook] deve essere completata per ogni singolo utente.
* Gli eventi visualizzati nella barra [!UICONTROL Scadenza] non vengono visualizzati nel calendario [!DNL Microsoft] a meno che non siano stati trascinati dal [!UICONTROL Elenco lavori] al calendario [!DNL Adobe Workfront]. Per ulteriori informazioni, vedere [[!UICONTROL Scadenza] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Elenco lavori nel [!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) nella visualizzazione [[!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Quando abiliti l&#39;integrazione con [!DNL Outlook], verranno sincronizzati solo gli elementi di lavoro trascinati nel [!UICONTROL Calendario predefinito] da quel momento in poi. Gli elementi presenti nel Calendario predefinito prima dell&#39;abilitazione dell&#39;integrazione non verranno visualizzati e sarà necessario trascinarli nuovamente nel Calendario predefinito se si desidera visualizzarli in [!DNL Outlook].
* Quando si condivide o si annulla la condivisione di un calendario [!DNL Outlook] con altri utenti o quando si modifica il livello di autorizzazione per un calendario condiviso con altri utenti, questa modifica non influisce sui calendari per circa 30 minuti. Per ulteriori informazioni, consultare la documentazione di [!DNL Microsoft Outlook].\
   Di conseguenza, quando si integra il Calendario [!DNL Workfront] con un calendario [!DNL Outlook] condiviso con altri utenti, questi non vedranno gli elementi del Calendario [!DNL Workfront] per circa 30 minuti.

>[!NOTE]
>
>La configurazione del calendario [!DNL Outlook] è completamente separata dal componente aggiuntivo [!DNL Outlook] ([!UICONTROL [!DNL Outlook] integrazione] o [!DNL Workfront Outlook]). Non è necessaria alcuna installazione per configurare il calendario, ma è necessaria un&#39;installazione per il componente aggiuntivo [!DNL Outlook]. Per ulteriori informazioni sul componente aggiuntivo [!DNL Outlook], vedere [Configurazione [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configura le impostazioni di visualizzazione del [!UICONTROL Calendario predefinito] e integralo con i calendari di Outlook

1. Nella visualizzazione [!UICONTROL Calendario predefinito], fai clic sull&#39;icona a forma di ingranaggio ![Calendario_Impostazioni_icona_ingranaggio.png](assets/calendar-settings-gear-icon.png) nell&#39;angolo superiore destro per aprire il pannello **[!UICONTROL Impostazioni calendario]** a destra.****

   Per informazioni sull&#39;accesso alla visualizzazione [!UICONTROL Calendario predefinito], vedere [Visualizza il [!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facoltativo) Per integrare il calendario [!DNL Microsoft Outlook], fai clic su **[!UICONTROL Aggiungi account]** nell&#39;angolo superiore destro del pannello **[!UICONTROL Impostazioni calendario]**. Quindi, se ti viene richiesto di farlo, immetti le informazioni di accesso a [!DNL Microsoft Outlook]. È possibile ripetere questo passaggio per aggiungere più account [!DNL Outlook].

   >[!NOTE]
   >
   >È necessario concedere a [!DNL Workfront] l&#39;autorizzazione per accedere al calendario [!DNL Outlook]. La concessione dell&#39;autorizzazione consente a [!DNL Workfront] di mantenere l&#39;accesso ai dati del calendario, di leggere il tuo profilo [!DNL outlook] e di leggere e aggiornare il tuo calendario [!DNL Microsoft].

1. Aggiorna la finestra del browser per visualizzare le informazioni dell&#39;account [!DNL Outlook] nel calendario e nel pannello [!UICONTROL Impostazioni calendario].
1. Fai di nuovo clic sull&#39;icona a forma di ingranaggio **[!UICONTROL Impostazioni]** nell&#39;angolo superiore destro per aprire il pannello **[!UICONTROL Impostazioni calendario]**. ![Impostazioni_Calendario_icona_ingranaggio.png](assets/calendar-settings-gear-icon.png)

1. (Facoltativo) Sotto ogni account [!DNL Microsoft] aggiunto nel passaggio precedente, seleziona **[!UICONTROL Visualizza]** o **[!UICONTROL Sincronizza]**:

   * **[!UICONTROL Visualizza]**: opzione di sola lettura che consente di visualizzare [!DNL Microsoft] eventi del calendario nel [!UICONTROL Calendario predefinito].
   * **[!UICONTROL Sincronizzazione]**: questa opzione consente la sincronizzazione bidirezionale tra i calendari [!DNL Microsoft] e [!UICONTROL Home]. In altre parole, [!DNL Workfront] [!UICONTROL Calendario predefinito] elementi vengono esportati nel calendario [!DNL Microsoft] e [!DNL Microsoft] elementi vengono importati nel [!UICONTROL Calendario predefinito] di Workfront in tempo reale.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Facoltativo) Sotto l&#39;account [!DNL Workfront] o un account integrato, seleziona i calendari associati che desideri visualizzare nel [!UICONTROL Calendario predefinito] (ad esempio il tuo PTO, i compleanni o il calendario festivo), quindi fai clic sul pulsante [!UICONTROL Aggiorna] o [!UICONTROL Ricarica] del browser per visualizzare le modifiche.

1. (Facoltativo) Nella sezione **[!UICONTROL Generale]** in **[!UICONTROL Settimana inizio il]**, selezionare il giorno che si desidera visualizzare come primo giorno della settimana lavorativa nel Calendario predefinito.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configura le seguenti opzioni:

   * **[!UICONTROL I miei giorni lavorativi]:** Seleziona i giorni di lavoro.
   * **[!UICONTROL Ora di inizio abituale]:** Seleziona l&#39;ora di inizio del giorno lavorativo.
   * **[!UICONTROL Ora di fine abituale]:** Seleziona l&#39;ora di fine del giorno lavorativo.

   [!DNL Workfront] utilizza queste tre impostazioni per calcolare il numero di ore lavorative in una settimana. Questo numero influisce sulla barra [!UICONTROL Allocazione], che consente di tenere traccia del carico di lavoro rispetto alle ore lavorative disponibili. Per ulteriori informazioni, vedere [[!UICONTROL Allocazione] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) nell&#39;articolo [[!UICONTROL Calendario predefinito] visualizzazione](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Fare clic all&#39;esterno dell&#39;area **[!UICONTROL Impostazioni calendario]** per chiuderla.

   [!DNL Workfront] salva automaticamente le modifiche.

Per informazioni sull&#39;utilizzo della visualizzazione [!UICONTROL Calendario] per gestire le assegnazioni di lavoro e gli eventi di calendario integrati, vedere [Utilizzare la visualizzazione [!UICONTROL Calendario predefinito]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
