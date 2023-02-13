---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configura il pulsante Fine per i problemi
description: Il pulsante Fine consente di impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un problema come Risolto quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Configura le [!UICONTROL Fine] pulsante per problemi

La [!UICONTROL Fine] può impostare automaticamente lo stato di un&#39;attività o di un problema. Per impostazione predefinita, [!DNL Adobe Workfront] contrassegna un problema come [!UICONTROL Risolto] quando un assegnatario fa clic su [!UICONTROL Fine] sul loro lavoro.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare le [!UICONTROL Fine] per riflettere alcuni stati del sistema. Ci sono 3 modi diversi [!UICONTROL Fine] funziona per i problemi in [!DNL Workfront]:

* Se l’utente ha una [!UICONTROL Team principale], [!DNL Workfront] un amministratore o un utente con un [!UICONTROL Pianificare] la licenza può configurare [!UICONTROL Fine] per riflettere alcuni stati per i membri del team. Vedi [Configura le [!UICONTROL Fine] pulsante per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se l’utente non ha un [!UICONTROL Team principale] assegnato, [!UICONTROL Fine] per problemi è legato a un [!UICONTROL Risolto] stato con codice a tre lettere [!UICONTROL RLV]. In questo scenario non sono disponibili opzioni di configurazione. La [!UICONTROL Fine] per impostazione predefinita questo stato viene impostato automaticamente su pulsante.
* Se la [!UICONTROL Risolto] ([!UICONTROL RLV]) viene eliminato e l&#39;utente contrassegna il problema come [!UICONTROL Fine] non [!UICONTROL Team principale], lo stato predefinito del problema è associato a qualsiasi valore impostato come predefinito per [!UICONTROL Chiuso] per il gruppo assegnato al progetto a cui appartiene il problema. L’amministratore di Workfront può configurare un’impostazione predefinita a livello di sistema per il gruppo. Vedi [Configura le [!UICONTROL Fine] quando [!UICONTROL Risolto] stato eliminato](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in questo articolo.

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
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td>L'accesso dell'amministratore di sistema è necessario per configurare il pulsante [!UICONTROL Done] quando lo stato [!UICONTROL Resolved] viene eliminato</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

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
   >  Ad esempio, l&#39;associazione [!UICONTROL Fine] Il pulsante In corso causa la visualizzazione dell&#39;elemento di lavoro come [!UICONTROL Fine] per l’utente che cambia lo stato da Nuovo a In corso.
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

## Configura le [!UICONTROL Fine] quando [!UICONTROL Risolto] stato eliminato

Se un utente non dispone di un team principale e l&#39;impostazione predefinita a livello di sistema per [!UICONTROL Risolto] ([!UICONTROL RLV]) è stato eliminato, un [!DNL Workfront] l&#39;amministratore può configurare le [!UICONTROL Chiuso] stato del gruppo sul progetto. [!DNL Workfront] seleziona questo stato per un problema chiuso quando l&#39;utente fa clic sul pulsante [!DNL Done] pulsante .

### Trova il gruppo associato al progetto

Quando un utente crea un progetto, il relativo Gruppo Home viene assegnato automaticamente al progetto. Utenti con [!UICONTROL Gestisci] l&#39;accesso al progetto può modificare questo gruppo nel [!UICONTROL Dettagli progetto] in qualsiasi momento. Per capire quale stato [!DNL Workfront] utilizza per un problema completato in questo caso, devi capire quale gruppo è associato al progetto su cui si trova il problema e per quale stato predefinito [!UICONTROL Chiuso] questo gruppo ha problemi.

Per trovare il gruppo associato al progetto:

1. Vai a un progetto.
1. Sul lato sinistro della pagina, fai clic su **[!UICONTROL Dettagli progetto]**.
1. Individua il **[!UICONTROL Associazione dei progetti]** sezione , quindi trova **[!UICONTROL Gruppo]**.\
   Questo è il nome del gruppo da utilizzare per controllare lo stato nell&#39;area Configurazione. Per istruzioni su come aggiornare lo stato predefinito di un gruppo specifico, consulta la sezione seguente.

### Aggiorna lo stato predefinito per un gruppo specifico

Come [!UICONTROL Workfront] amministratore, puoi aggiornare lo stato di un gruppo specifico:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze del progetto]**, quindi **[!UICONTROL Stati]**.

1. Fai clic su **[!UICONTROL Problemi]**, quindi digita il nome del gruppo nel **[!UICONTROL Stati del sistema]** casella di ricerca a destra.

1. Selezionare il gruppo.
1. Fai clic sul pulsante **[!UICONTROL Imposta stati predefiniti]** menu a discesa, quindi scegliere uno stato predefinito per [!UICONTROL Chiuso]. [!DNL Workfront] utilizza questo stato per un problema chiuso quando un utente fa clic sul pulsante [!UICONTROL Fine] pulsante .

   >[!IMPORTANT]
   >
   >Questo stato viene utilizzato solo quando l&#39;utente non ha un Home Team assegnato e il [!UICONTROL RLV] stato eliminato.

1. Fai clic su **[!UICONTROL Salva]**.
