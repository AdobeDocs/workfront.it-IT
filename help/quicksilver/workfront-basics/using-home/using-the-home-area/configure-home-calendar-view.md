---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurare le impostazioni di visualizzazione del calendario principale
description: È possibile configurare le impostazioni del calendario principale per l'integrazione con una versione di Outlook basata sul Web e consentire di tenere traccia del carico di lavoro rispetto alle ore lavorative disponibili.
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Configura le [!UICONTROL Calendario Home] visualizza impostazioni

Puoi configurare le [!UICONTROL Calendario Home] per eseguire le seguenti operazioni:

* Effettua l’integrazione con una versione basata sul web di [!DNL Outlook] in hosting sul cloud [!DNL Office 365] o [!DNL Outlook Live]. È possibile visualizzare tutti gli eventi dal calendario di Outlook e tutti i calendari associati selezionati, ad esempio i calendari di compleanno e di vacanza, nel [!UICONTROL Calendario Home].
* Consente di tenere traccia del carico di lavoro rispetto alle ore di lavoro disponibili [!UICONTROL Allocazione] bar.

Per ulteriori informazioni sul Calendario Home, vedi [[!UICONTROL Calendario Home] visualizzare](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Informazioni sull’integrazione [!DNL Microsoft Outlook] calendari

Quando configuri il tuo Calendario Home con il tuo [!DNL Microsoft Outlook] calendario:

* È possibile integrare solo una versione basata sul Web di [!DNL Outlook] in hosting sul cloud [!DNL Office 365] o [!DNL Outlook Live].

   Presso i locali [!DNL Outlook] e [!DNL Outlook] su un’azienda basata su cloud [!DNL Exchange] server non supportati.

   Se l’organizzazione utilizza l’accesso single sign-on, è necessario [!DNL Microsoft 365 E3] o [!DNL E5].

* Allegati associati al [!DNL Outlook] gli eventi non sono collegati al [!DNL Outlook] eventi nel calendario principale.
* Integrazione con un [!DNL Outlook] Il calendario deve essere completato singolarmente per ogni utente.
* Eventi visualizzati nella [!UICONTROL Scadenza] la barra non viene visualizzata sul [!DNL Microsoft] calendario a meno che non siano stati trascinati dal [!UICONTROL Elenco lavori] al tuo [!DNL Adobe Workfront] Calendario. Per ulteriori informazioni, consulta [[!UICONTROL Scadenza] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Elenco di lavoro [!UICONTROL Calendario Home]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Calendario Home] visualizzare](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Quando abiliti l’integrazione con [!DNL Outlook], solo gli elementi di lavoro trascinati sul [!UICONTROL Calendario Home] da quel momento in avanti si sincronizzerà. Gli elementi presenti nel Calendario principale prima di abilitare l&#39;integrazione non verranno visualizzati e dovrai trascinarli nuovamente nel Calendario principale se desideri che vengano visualizzati in [!DNL Outlook].
* Quando condividi (o annulla condivisione) un [!DNL Outlook] calendario con altre persone o quando si modifica il livello di autorizzazione per un calendario condiviso con altri, questa modifica non influisce sui calendari per circa 30 minuti (per ulteriori informazioni, consultare il [!DNL Microsoft Outlook] documentazione).\
   Di conseguenza, quando si integra [!DNL Workfront] Calendario con un [!DNL Outlook] calendario condiviso con altri utenti, non visualizzeranno il tuo [!DNL Workfront] Elementi calendario per circa 30 minuti.

>[!NOTE]
>
>La [!DNL Outlook] la configurazione del calendario è completamente separata dalla [!DNL Outlook] Add-in ([!UICONTROL [!DNL Outlook] Integrazione] o [!DNL Workfront Outlook]). Non è necessaria alcuna installazione per configurare il calendario, ma è necessaria un’installazione per il [!DNL Outlook] Componente aggiuntivo. Per ulteriori informazioni sulla [!DNL Outlook] Add-in vedi [Configurazione [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configura le [!UICONTROL Calendario Home] visualizza impostazioni

1. In [!UICONTROL Calendario Home] visualizzazione, fai clic su **[!UICONTROL Impostazioni]** icona ingranaggio ![Calendar_Settings_ingran_icon.png](assets/calendar-settings-gear-icon.png) nell&#39;angolo in alto a destra per aprire **[!UICONTROL Impostazioni del calendario]** sul lato destro della finestra.

   Se hai bisogno di informazioni sull&#39;accesso al [!UICONTROL Calendario Home] visualizza, vedi [Visualizza la [!UICONTROL Calendario Home]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facoltativo) Per integrare [!DNL Microsoft Outlook] calendario, fai clic su **[!UICONTROL Aggiungi account]** nell&#39;angolo superiore destro del **[!UICONTROL Impostazioni del calendario]** pannello. Quindi, se ti viene richiesto di farlo, immetti il tuo [!DNL Microsoft Outlook] informazioni di accesso. È possibile ripetere questo passaggio per aggiungere più [!DNL Outlook] conti.

   >[!NOTE]
   >
   >Devi dare [!DNL Workfront] autorizzazione ad accedere al tuo [!DNL Outlook] calendario. La concessione del permesso di soggiorno permette [!DNL Workfront] per mantenere l&#39;accesso ai dati del calendario, leggi [!DNL outlook] e leggi e aggiorna il tuo profilo [!DNL Microsoft] calendario.

1. Aggiorna la finestra del browser per visualizzare le informazioni dal tuo [!DNL Outlook] nel calendario e nel [!UICONTROL Impostazioni del calendario] pannello.
1. Fai clic sul pulsante **[!UICONTROL Impostazioni]** icona ingranaggio nuovamente nell&#39;angolo superiore destro per aprire **[!UICONTROL Impostazioni del calendario]** pannello. ![Calendar_Settings_ingran_icon.png](assets/calendar-settings-gear-icon.png)

1. (Facoltativo) Sotto ogni [!DNL Microsoft] account aggiunto nel passaggio precedente, seleziona **[!UICONTROL Visualizza]** o **[!UICONTROL Sincronizzazione]**:

   * **[!UICONTROL Visualizza]**: Questa è un&#39;opzione di sola lettura che viene visualizzata [!DNL Microsoft] eventi di calendario [!UICONTROL Calendario Home].
   * **[!UICONTROL Sincronizzazione]**: Questa opzione consente una sincronizzazione bidirezionale tra [!DNL Microsoft] e [!UICONTROL Pagina principale] calendari. In altre parole, [!DNL Workfront] [!UICONTROL Calendario Home] articoli esportati nel tuo [!DNL Microsoft] calendario e [!DNL Microsoft] elementi calendario importati in Workfront [!UICONTROL Calendario Home] in tempo reale.

      ![](assets/view-sync-checkboxes-qs.png)

1. (Facoltativo) Sotto il [!DNL Workfront] per un account o un account integrato, selezionare i calendari associati che si desidera visualizzare sul tuo [!UICONTROL Calendario Home] (ad esempio il tuo PTO, i compleanni o il calendario delle vacanze) fai clic sul browser del tuo [!UICONTROL Aggiorna] o [!UICONTROL Ricarica] per visualizzare le modifiche.

1. (Facoltativo) In **[!UICONTROL Generale]** sezione **[!UICONTROL Inizia settimana il]**, selezionare il giorno che si desidera visualizzare come primo giorno della settimana lavorativa nel calendario principale.

1. Configura le seguenti opzioni:

   * **[!UICONTROL Giorni di lavoro]:** Selezionare i giorni lavorativi.
   * **[!UICONTROL Ora di inizio normale]:** Selezionare l&#39;ora di inizio del giorno lavorativo.
   * **[!UICONTROL Ora di fine normale]:** Selezionare l&#39;ora di fine giornata lavorativa.

   [!DNL Workfront] utilizza queste tre impostazioni per calcolare il numero di ore lavorative in una settimana. Questo numero influisce sul [!UICONTROL Allocazione] barra, che consente di tenere traccia del carico di lavoro rispetto alle ore lavorative disponibili. Per ulteriori informazioni, consulta [[!UICONTROL Allocazione] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) nell&#39;articolo [[!UICONTROL Calendario Home] visualizzare](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Fai clic all’esterno del **[!UICONTROL Impostazioni del calendario]** zona per ignorarlo.

   [!DNL Workfront] salva automaticamente le modifiche.

Per informazioni sull&#39;utilizzo del [!UICONTROL Calendario] per gestire le assegnazioni di lavoro e gli eventi di calendario integrati, vedere [Utilizza la [!UICONTROL Calendario Home] visualizzare](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
