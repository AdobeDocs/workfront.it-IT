---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurare il pulsante Fine per i problemi
description: Il pulsante Done (Fine) può impostare automaticamente lo stato di un’attività o di un problema. Per impostazione predefinita, Adobe Workfront contrassegna un problema come Risolto quando un assegnatario fa clic su Fine sul proprio elemento di lavoro.
author: Jenny
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 1%

---

# Configura il pulsante [!UICONTROL Fine] per i problemi

Il pulsante [!UICONTROL Fine] può impostare automaticamente lo stato di un&#39;attività o di un problema. Per impostazione predefinita, [!DNL Adobe Workfront] contrassegna un problema come [!UICONTROL Risolto] quando un assegnatario fa clic su [!UICONTROL Fine] sul proprio elemento di lavoro.

>[!NOTE]
>
>Il pulsante Done (Fine) viene visualizzato come Mark as done (Contrassegna come completato) in tutte le aree di Workfront.

## Panoramica

Gli utenti con determinate autorizzazioni possono configurare il pulsante [!UICONTROL Fine] per riflettere determinati stati nel sistema. Il pulsante [!UICONTROL Fine] funziona in 3 modi diversi per i problemi in [!DNL Workfront]:

* Se all&#39;utente è assegnato un [!UICONTROL Team predefinito], un amministratore [!DNL Workfront] o un utente con una licenza [!UICONTROL Plan] può configurare il pulsante [!UICONTROL Done] per riflettere determinati stati per i membri del team. Vedi [Configurare il pulsante [!UICONTROL Fine] per un team](#configure-the-uicontrol-done-button-for-a-team) in questo articolo.
* Se l&#39;utente non ha un [!UICONTROL Team predefinito], ma ha [!UICONTROL Altri team] nel suo profilo, Workfront cerca l&#39;impostazione del pulsante [!UICONTROL Fine] su uno qualsiasi dei team associati all&#39;utente. La selezione è casuale e lo stato associato a uno qualsiasi dei team viene utilizzato per il problema.
* Se all&#39;utente non è assegnato un [!UICONTROL Team predefinito], il pulsante [!UICONTROL Fine] per i problemi è associato a uno stato [!UICONTROL Risolto] generato dal sistema con codice di tre lettere [!UICONTROL RLV]. Non sono disponibili opzioni di configurazione in questo scenario. Il pulsante [!UICONTROL Fine] viene impostato automaticamente su questo stato.
* Se lo stato [!UICONTROL Risolto] ([!UICONTROL RLV]) viene eliminato e l&#39;utente che contrassegna il problema come [!UICONTROL Completato] non dispone di [!UICONTROL Team predefinito], lo stato del problema predefinito è associato a quello impostato come predefinito per [!UICONTROL Chiuso] per il gruppo assegnato al progetto a cui appartiene il problema. L’amministratore di Workfront può configurare un’impostazione predefinita a livello di sistema per il gruppo. Consulta [Configurare il pulsante [!UICONTROL Fine] quando lo stato [!UICONTROL Risolto] è stato eliminato](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in questo articolo.

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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per configurare il pulsante Fine quando lo stato Risolto viene eliminato, è necessario disporre dell'accesso come amministratore di sistema</p> </td> 
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
   >  Se ad esempio si associa il pulsante [!UICONTROL Fine] a In corso, l&#39;elemento di lavoro verrà visualizzato come [!UICONTROL Fine] per l&#39;utente che modifica lo stato da Nuovo a In corso.
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
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Nella sezione **[!UICONTROL Organizzazione]**, seleziona il campo **[!UICONTROL Team predefinito]**. Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fare clic sul nome del team quando viene visualizzato nell&#39;elenco.

1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team predefinito.
Tutte le impostazioni del team, inclusi gli stati associati al pulsante [!UICONTROL Fine], sono ora visibili a questi utenti.

## Configura il pulsante [!UICONTROL Fine] quando lo stato [!UICONTROL Risolto] è stato eliminato

Se un utente non dispone di un team predefinito e l&#39;impostazione predefinita a livello di sistema per [!UICONTROL Risolto] ([!UICONTROL RLV]) è stata eliminata, un amministratore [!DNL Workfront] può configurare lo stato [!UICONTROL Chiuso] per il gruppo sul progetto. [!DNL Workfront] seleziona questo stato per un problema chiuso quando l&#39;utente fa clic sul pulsante [!DNL Done].

### Trova il gruppo associato al progetto

Quando un utente crea un progetto, il suo Gruppo Predefinito viene assegnato automaticamente al progetto. Gli utenti con l&#39;accesso [!UICONTROL Gestione] al progetto possono cambiare questo gruppo nella sezione [!UICONTROL Dettagli progetto] in qualsiasi momento. Per capire lo stato utilizzato da [!DNL Workfront] per un problema completato in questo caso, è necessario capire quale gruppo è associato al progetto in cui si trova il problema e quale stato predefinito ha per [!UICONTROL Chiuso] questo gruppo per i problemi.

Per trovare il gruppo associato al progetto:

1. Vai a un progetto.
1. Sul lato sinistro della pagina, fare clic su **[!UICONTROL Dettagli progetto]**.
1. Individua la sezione **[!UICONTROL Associazione progetto]**, quindi trova **[!UICONTROL Gruppo]**.\
   Questo è il nome del gruppo che devi usare per controllare lo stato nell’area Configura. Consulta la sezione seguente per istruzioni su come aggiornare lo stato predefinito per un gruppo specifico.

### Aggiornare lo stato predefinito per un gruppo specifico

In qualità di amministratore [!UICONTROL Workfront], puoi aggiornare lo stato per un gruppo specifico:

1. Fai clic sull&#39;icona **[!UICONTROL del]** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze progetto]**, quindi su **[!UICONTROL Stati]**.

1. Fai clic su **[!UICONTROL Problemi]**, quindi digita il nome del gruppo nella casella di ricerca **[!UICONTROL Stati di sistema]** a destra.

1. Selezionare il gruppo.
1. Fai clic sul menu a discesa **[!UICONTROL Imposta stati predefiniti]**, quindi scegli uno stato predefinito per [!UICONTROL Chiuso]. [!DNL Workfront] utilizza questo stato per un problema chiuso quando un utente fa clic sul pulsante [!UICONTROL Fine].

   >[!IMPORTANT]
   >
   >Questo stato viene utilizzato solo quando all&#39;utente non è assegnato alcun team predefinito e lo stato [!UICONTROL RLV] è stato eliminato.

1. Fai clic su **[!UICONTROL Salva]**.
