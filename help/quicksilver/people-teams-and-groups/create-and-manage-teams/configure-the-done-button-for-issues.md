---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configura il pulsante Fine per i problemi
description: Il pulsante Done (Fine) può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un problema come Risolto quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 0%

---

# Configurare [!UICONTROL Fine] pulsante per problemi

Il [!UICONTROL Fine] può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, [!DNL Adobe Workfront] contrassegna un problema come [!UICONTROL Risolto] quando un assegnatario fa clic su [!UICONTROL Fine] sull&#39;elemento di lavoro.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare [!UICONTROL Fine] per riflettere determinati stati nel sistema. Esistono 3 modi diversi per [!UICONTROL Fine] funziona per i problemi in [!DNL Workfront]:

* Se all’utente è stato assegnato un [!UICONTROL Team predefinito], a [!DNL Workfront] amministratore o un utente con un [!UICONTROL Piano] la licenza può configurare [!UICONTROL Fine] per riflettere determinati stati per i membri del team. Consulta [Configurare [!UICONTROL Fine] pulsante per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se l’utente non dispone di un’ [!UICONTROL Team predefinito], ma hanno [!UICONTROL Altri team] nel loro profilo, Workfront cerca l’impostazione del [!UICONTROL Fine] su uno dei team associati all’utente. La selezione è casuale e lo stato associato a uno qualsiasi dei team viene utilizzato per il problema.
* Se l’utente non dispone di un’ [!UICONTROL Team predefinito] assegnato, il [!UICONTROL Fine] per i problemi è associato a un pulsante generato dal sistema [!UICONTROL Risolto] stato con codice di tre lettere [!UICONTROL RLV]. Non sono disponibili opzioni di configurazione in questo scenario. Il [!UICONTROL Fine] viene impostato automaticamente su questo stato.
* Se il [!UICONTROL Risolto] ([!UICONTROL RLV]) viene eliminato e l&#39;utente contrassegna il problema come [!UICONTROL Fine] non ha [!UICONTROL Team predefinito], lo stato predefinito del problema è associato a ciò che è impostato come predefinito per [!UICONTROL Chiuso] per il gruppo assegnato al progetto a cui appartiene il problema. L’amministratore di Workfront può configurare un’impostazione predefinita a livello di sistema per il gruppo. Consulta [Configurare [!UICONTROL Fine] quando [!UICONTROL Risolto] lo stato è stato eliminato](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in questo articolo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td>Per configurare il pulsante [!UICONTROL Done] è necessario disporre dell'accesso come amministratore di sistema quando viene eliminato lo stato [!UICONTROL Resolved]</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

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
   >  Ad esempio, associando [!UICONTROL Fine] con In corso, l&#39;elemento di lavoro viene visualizzato come [!UICONTROL Fine] per l’utente che modifica lo stato da Nuovo a In corso.
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
Tutte le impostazioni del team, inclusi gli stati associati al [!UICONTROL Fine] , sono ora visibili a questi utenti.

## Configurare [!UICONTROL Fine] quando [!UICONTROL Risolto] lo stato è stato eliminato

Se un utente non dispone di un team predefinito e l’impostazione predefinita a livello di sistema per [!UICONTROL Risolto] ([!UICONTROL RLV]) è stato eliminato, un [!DNL Workfront] può configurare [!UICONTROL Chiuso] stato del gruppo sul progetto. [!DNL Workfront] seleziona questo stato per un problema chiuso quando l’utente fa clic su [!DNL Done] pulsante.

### Trova il gruppo associato al progetto

Quando un utente crea un progetto, il suo Gruppo Predefinito viene assegnato automaticamente al progetto. Utenti con [!UICONTROL Gestisci] l’accesso al progetto può modificare questo gruppo nel [!UICONTROL Dettagli progetto] sezione in qualsiasi momento. Per capire quale stato [!DNL Workfront] utilizza per un problema completato in questo caso, è necessario comprendere a quale gruppo è associato il progetto in cui si trova il problema e per quale stato predefinito [!UICONTROL Chiuso] questo gruppo ha per problemi.

Per trovare il gruppo associato al progetto:

1. Vai a un progetto.
1. Sul lato sinistro della pagina, fai clic su **[!UICONTROL Dettagli progetto]**.
1. Individua il **[!UICONTROL Associazione progetto]** , quindi trova **[!UICONTROL Gruppo]**.\
   Questo è il nome del gruppo che devi usare per controllare lo stato nell’area Configura. Consulta la sezione seguente per istruzioni su come aggiornare lo stato predefinito per un gruppo specifico.

### Aggiornare lo stato predefinito per un gruppo specifico

As a [!UICONTROL Workfront] amministratore, puoi aggiornare lo stato per un gruppo specifico:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze progetto]**, quindi **[!UICONTROL Stati]**.

1. Clic **[!UICONTROL Problemi]**, quindi digitare il nome del gruppo nel **[!UICONTROL Stati del sistema]** casella di ricerca a destra.

1. Selezionare il gruppo.
1. Fai clic su **[!UICONTROL Imposta stati predefiniti]** menu a discesa, quindi scegliere uno stato predefinito per [!UICONTROL Chiuso]. [!DNL Workfront] utilizza questo stato per un problema chiuso quando un utente fa clic su [!UICONTROL Fine] pulsante.

   >[!IMPORTANT]
   >
   >Questo stato viene utilizzato solo quando all’utente non è assegnato alcun Team predefinito e il [!UICONTROL RLV] lo stato è stato eliminato.

1. Fai clic su **[!UICONTROL Salva]**.
