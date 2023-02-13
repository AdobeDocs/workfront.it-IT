---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configura il pulsante Fine per le attività
description: Il pulsante Fine consente di impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un’attività come Completato quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Configura le [!UICONTROL Fine] pulsante per le attività

La [!UICONTROL Fine] può impostare automaticamente lo stato di un&#39;attività o di un problema. Per impostazione predefinita, [!UICONTROL Adobe Workfront] contrassegna un’attività come [!UICONTROL Completato] quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare le [!UICONTROL Fine] per riflettere alcuni stati del sistema. Ci sono due modi diversi per [!UICONTROL Fine] funziona per le attività in [!UICONTROL Workfront]:

* Se l&#39;utente dispone di un Home Team assegnato, un [!DNL Workfront] un amministratore o un utente con un [!UICONTROL Pianificare] la licenza può configurare [!UICONTROL Fine] per riflettere alcuni stati per i membri del team. Vedi [Configura le [!UICONTROL Fine] pulsante per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se all&#39;utente non è assegnato un team principale, il [!UICONTROL Fine] per le attività è associato a uno stato completo. In questo scenario non sono disponibili opzioni di configurazione. La [!UICONTROL Fine] per impostazione predefinita questo stato viene impostato automaticamente su pulsante.

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
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Configura le [!UICONTROL Fine] pulsante per un team

È possibile modificare lo stato applicato all&#39;elemento di lavoro con [!UICONTROL Fine] pulsante . È inoltre possibile impostare più stati e consentire all’utente di scegliere lo stato appropriato.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic sul pulsante **[!UICONTROL Cambia team]** , quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** menu, quindi fai clic su **[!UICONTROL Modifica]**.
1. Trova il **[!UICONTROL Pulsante Fine]** nella parte inferiore del **[!UICONTROL Impostazioni team]** pagina.

1. Selezionare uno stato o più stati per ogni tipo di elemento di lavoro.

   >[!NOTE]
   >
   >Quando selezioni gli stati per le attività o i problemi, considera quanto segue:
   >
   >* Quando si seleziona uno stato per ogni tipo di elemento di lavoro, lo stato dell&#39;attività o del problema viene impostato su tale stato quando l&#39;utente fa clic su [!UICONTROL Fine] sul loro oggetto. Se si impostano più stati per ciascun tipo di elemento di lavoro, viene aggiunto un menu a discesa al [!UICONTROL Fine] e l&#39;utente deve scegliere uno stato per modificare lo stato dell&#39;elemento di lavoro.
   >* È possibile associare solo gli stati a livello di sistema al [!UICONTROL Fine] pulsante . Non è possibile associare gli stati specifici del gruppo con gli stati degli elementi di lavoro.
   >* Quando un utente assegnato all&#39;elemento inserisce l&#39;elemento nello stato associato al [!UICONTROL Fine] l&#39;elemento viene visualizzato come [!UICONTROL Fine] per l&#39;utente indipendentemente dal fatto che lo stato selezionato sia un [!UICONTROL Completato] o [!UICONTROL Chiuso] stato o stato di lavoro.

   >   
   >   
   >  Ad esempio, l&#39;associazione [!UICONTROL Fine] pulsante con [!UICONTROL In corso] determina la visualizzazione dell&#39;elemento di lavoro come [!UICONTROL Fine] per l’utente che modifica lo stato da [!UICONTROL Nuovo] a [!UICONTROL In corso].
   >   
   >* I tipi di problema sono personalizzabili e possono avere nomi diversi rispetto a quelli elencati di seguito nel tuo ambiente.\
      >  Di seguito sono riportate le attività predefinite e i tipi di problemi:
      >     
      >   * [!UICONTROL Attività]
      >   * [!UICONTROL Problema]
      >   * [!UICONTROL Richiesta]
      >   * [!UICONTROL Richiesta di Modifica]
      >   * [!UICONTROL Segnalazione Bug]


   Se l&#39;attività o il problema è assegnato a più utenti, viene visualizzato un &quot;[!UICONTROL Fatto con la mia parte]&quot; nel menu a discesa, oltre ai diversi stati scelti per il team.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Associare gli utenti a un team principale

Per apportare le modifiche al [!UICONTROL Fine] funzionalità pulsante visibile agli utenti, puoi rendere il team di cui hai modificato le impostazioni del team principale degli utenti.

Per associare gli utenti a un team principale:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].

1. Fai clic su **[!UICONTROL Utenti]**, quindi selezionare l&#39;utente o gli utenti che si desidera associare a un Home Team.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In **[!UICONTROL Organizzazione]** seleziona la sezione **[!UICONTROL Team principale]** campo . Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fai clic sul nome del team quando lo trovi nell’elenco.

1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team principale.
Tutte le impostazioni del team, inclusi gli stati associati all&#39;azione [!UICONTROL Fine] sono ora visibili a questi utenti.
