---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurare il pulsante Fine per le attività
description: Il pulsante Done (Fine) può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un’attività come Completata quando un assegnatario fa clic su Fine sul relativo elemento di lavoro.
author: Jenny
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 2%

---

# Configura il pulsante [!UICONTROL Fine] per le attività

Il pulsante [!UICONTROL Fine] può impostare automaticamente lo stato di un&#39;attività o di un problema. Per impostazione predefinita, [!UICONTROL Adobe Workfront] contrassegna un&#39;attività come [!UICONTROL Completata] quando un assegnatario fa clic su Contrassegna come completata sul proprio elemento di lavoro.

>[!NOTE]
>
>Il pulsante Done (Fine) viene visualizzato come Mark as done (Contrassegna come completato) in tutte le aree di Workfront.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare il pulsante [!UICONTROL Fine] per associarlo a determinati stati nel sistema. Il pulsante [!UICONTROL Fine] funziona in due modi diversi per le attività in [!UICONTROL Workfront]:

* Se all&#39;utente è assegnato un team predefinito, un amministratore [!DNL Workfront] o un utente con una licenza [!UICONTROL Plan] può configurare il pulsante [!UICONTROL Done] per riflettere determinati stati per i membri del team. Vedi [Configurare il pulsante [!UICONTROL Fine] per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se l&#39;utente non ha un [!UICONTROL Team predefinito], ma ha [!UICONTROL Altri team] nel suo profilo, Workfront cerca l&#39;impostazione del pulsante [!UICONTROL Fine] su uno qualsiasi dei team associati all&#39;utente. La selezione è casuale e per l’attività viene utilizzato lo stato associato a uno dei team.
* Se all&#39;utente non è assegnato un team predefinito, il pulsante [!UICONTROL Fine] per le attività è associato a uno stato completo. Non sono disponibili opzioni di configurazione in questo scenario. Il pulsante [!UICONTROL Fine] viene impostato automaticamente su questo stato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Pacchetto Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura il pulsante [!UICONTROL Fine] per un team

È possibile cambiare lo stato applicato all&#39;elemento di lavoro con il pulsante [!UICONTROL Fine]. È inoltre possibile impostare più stati e consentire all&#39;utente di scegliere lo stato appropriato.

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]**, quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi fai clic su **[!UICONTROL Modifica]**.
1. Trova la sezione **[!UICONTROL Pulsante completato]** nella parte inferiore della pagina **[!UICONTROL Impostazioni team]**.

1. Selezionare uno stato o più stati per ogni tipo di elemento di lavoro.

   >[!NOTE]
   >
   >Quando selezioni gli stati per attività o problemi, considera quanto segue:
   >
   >* Quando si seleziona uno stato per ogni tipo di elemento di lavoro, lo stato dell&#39;attività o del problema viene impostato su tale stato quando un utente fa clic su [!UICONTROL Fine] sul relativo elemento. Se si impostano più stati per ogni tipo di elemento di lavoro, al pulsante [!UICONTROL Fine] viene aggiunto un menu a discesa e l&#39;utente deve scegliere uno stato per modificare lo stato dell&#39;elemento di lavoro.
   >* È possibile associare solo gli stati a livello di sistema al pulsante [!UICONTROL Fine]. Non è possibile associare gli stati specifici del gruppo agli stati degli elementi di lavoro.
   >* Quando un utente assegnato all&#39;elemento inserisce l&#39;elemento nello stato associato al pulsante [!UICONTROL Fine], l&#39;elemento viene visualizzato come [!UICONTROL Fine] per tale utente indipendentemente dal fatto che lo stato selezionato sia [!UICONTROL Completato] o [!UICONTROL Chiuso] o uno stato funzionante.
   >   
   >   
   >  Ad esempio, se si associa il pulsante [!UICONTROL Fine] a [!UICONTROL In corso], l&#39;elemento di lavoro verrà visualizzato come [!UICONTROL Fine] per l&#39;utente che modifica lo stato da [!UICONTROL Nuovo] a [!UICONTROL In corso].
   >   
   >* I tipi di problema sono personalizzabili e possono avere nomi diversi da quelli elencati di seguito nel tuo ambiente.\
   >  Di seguito sono elencati i tipi di problemi e le attività predefiniti:
   >     
   >   * [!UICONTROL Attività]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Richiesta]
   >   * [!UICONTROL Richiesta di Modifica]
   >   * [!UICONTROL Segnalazione Bug]

   Se l&#39;attività o il problema è assegnato a più utenti, nel menu a discesa viene visualizzata l&#39;opzione &quot;[!UICONTROL Fine con la parte &#x200B;]&quot;, oltre ai diversi stati scelti per il team.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Associa utenti a un team predefinito

Per rendere visibili agli utenti le modifiche apportate alla funzionalità del pulsante [!UICONTROL Fine], è possibile rendere il team di cui sono state modificate le impostazioni il team predefinito degli utenti.

Per associare utenti a un team predefinito:

1. Fai clic sull&#39;icona **[!UICONTROL del]** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].

1. Fare clic su **[!UICONTROL Utenti]**, quindi selezionare l&#39;utente o gli utenti che si desidera associare a un team predefinito.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi fai clic su **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Nella sezione **[!UICONTROL Organizzazione]**, seleziona il campo **[!UICONTROL Team predefinito]**. Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fare clic sul nome del team quando viene visualizzato nell&#39;elenco.

1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team predefinito.
Tutte le impostazioni del team, inclusi gli stati associati al pulsante [!UICONTROL Fine], sono ora visibili a questi utenti.
