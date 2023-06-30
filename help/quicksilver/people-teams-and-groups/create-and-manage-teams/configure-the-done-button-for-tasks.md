---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configura il pulsante Fine per le attività
description: Il pulsante Done (Fine) può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un’attività come Completata quando un assegnatario fa clic su Fine sul relativo elemento di lavoro.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Configurare [!UICONTROL Fine] pulsante per le attività

Il [!UICONTROL Fine] può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, [!UICONTROL Adobe Workfront] contrassegna un&#39;attività come [!UICONTROL Completato] quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare [!UICONTROL Fine] per riflettere determinati stati nel sistema. Esistono due modi diversi [!UICONTROL Fine] funziona per le attività in [!UICONTROL Workfront]:

* Se all’utente è assegnato un Team predefinito, viene visualizzato [!DNL Workfront] amministratore o un utente con un [!UICONTROL Piano] la licenza può configurare [!UICONTROL Fine] per riflettere determinati stati per i membri del team. Consulta [Configurare [!UICONTROL Fine] pulsante per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se l’utente non dispone di un’ [!UICONTROL Team predefinito], ma hanno [!UICONTROL Altri team] nel loro profilo, Workfront cerca l’impostazione del [!UICONTROL Fine] su uno dei team associati all’utente. La selezione è casuale e per l’attività viene utilizzato lo stato associato a uno dei team.
* Se all’utente non è assegnato un Team predefinito, il [!UICONTROL Fine] per le attività è associato a uno stato completo. Non sono disponibili opzioni di configurazione in questo scenario. Il [!UICONTROL Fine] viene impostato automaticamente su questo stato.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] piano*</strong></p></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licenza*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare [!DNL Workfront] amministratore.

## Configurare [!UICONTROL Fine] pulsante per un team

È possibile modificare lo stato applicato all&#39;elemento di lavoro con [!UICONTROL Fine] pulsante. È inoltre possibile impostare più stati e consentire all&#39;utente di scegliere lo stato appropriato.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic su **[!UICONTROL Cambia team]** , quindi selezionare un nuovo team dal menu a discesa o cercare un team nella barra di ricerca.
1. Fai clic su **[!UICONTROL Altro]** , quindi fai clic su **[!UICONTROL Modifica]**.
1. Trova il **[!UICONTROL Pulsante Fine]** sezione nella parte inferiore della sezione **[!UICONTROL Impostazioni team]** pagina.

1. Selezionare uno stato o più stati per ogni tipo di elemento di lavoro.

   >[!NOTE]
   >
   >Quando selezioni gli stati per attività o problemi, considera quanto segue:
   >
   >* Quando si seleziona uno stato per ogni tipo di elemento di lavoro, lo stato dell’attività o del problema viene impostato su tale stato quando un utente fa clic su [!UICONTROL Fine] sull&#39;oggetto. Se si impostano più stati per ogni tipo di elemento di lavoro, viene aggiunto un menu a discesa al [!UICONTROL Fine] e l&#39;utente deve scegliere uno stato per modificare lo stato sull&#39;elemento di lavoro.
   >* È possibile associare solo gli stati a livello di sistema al [!UICONTROL Fine] pulsante. Non è possibile associare gli stati specifici del gruppo agli stati degli elementi di lavoro.
   >* Quando un utente assegnato all’elemento lo inserisce nello stato associato all’elemento [!UICONTROL Fine] , l&#39;elemento viene visualizzato come [!UICONTROL Fine] per tale utente indipendentemente dal fatto che lo stato selezionato sia [!UICONTROL Completato] o [!UICONTROL Chiuso] stato o uno stato di lavoro.
   >   
   >   
   >  Ad esempio, associando [!UICONTROL Fine] pulsante con [!UICONTROL In corso] causa la visualizzazione dell&#39;elemento di lavoro come [!UICONTROL Fine] per l’utente che modifica lo stato da [!UICONTROL Nuovo] a [!UICONTROL In corso].
   >   
   >* I tipi di problema sono personalizzabili e possono avere nomi diversi da quelli elencati di seguito nel tuo ambiente.\
   >  Di seguito sono elencati i tipi di problemi e le attività predefiniti:
   >     
   >   * [!UICONTROL Attività]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Richiesta]
   >   * [!UICONTROL Richiesta di Modifica]
   >   * [!UICONTROL Segnalazione Bug]

   Se l’attività o il problema è assegnato a più utenti, viene visualizzato un messaggio &quot;[!UICONTROL Fine con la mia parte]&quot; nel menu a discesa, oltre ai diversi stati scelti per il team.

1. Clic **[!UICONTROL Salva modifiche]**.

## Associa utenti a un team predefinito

Per apportare le modifiche al [!UICONTROL Fine] funzionalità pulsante visibile agli utenti, è possibile rendere il team di cui sono state modificate le impostazioni il Team predefinito degli utenti.

Per associare utenti a un team predefinito:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].

1. Clic **[!UICONTROL Utenti]**, quindi selezionare l&#39;utente o gli utenti che si desidera associare a un team predefinito.
1. Fai clic su **[!UICONTROL Altro]** , quindi seleziona **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In **[!UICONTROL Organizzazione]** , seleziona la sezione **[!UICONTROL Team predefinito]** campo. Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fare clic sul nome del team quando viene visualizzato nell&#39;elenco.

1. Clic **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team predefinito.
Tutte le impostazioni del team, inclusi gli stati associati al [!UICONTROL Fine] sono ora visibili a questi utenti.
