---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Sostituisci il pulsante Lavoraci con un pulsante Start
description: La configurazione predefinita di Adobe Workfront include un pulsante Lavoraci per le attività e i problemi visualizzati per gli elementi assegnati.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Sostituisci il pulsante [!UICONTROL Lavoraci] con un pulsante [!UICONTROL Avvia]

La configurazione predefinita di [!DNL Adobe Workfront] include un pulsante [!UICONTROL Lavoraci] per le attività e i problemi visualizzati per gli elementi assegnati. Quando fai clic su [!UICONTROL Lavoraci] sugli elementi che ti sono stati assegnati, segnali ad altri utenti che hai ricevuto il lavoro e confermi che ci lavorerai. Tuttavia, il pulsante [!DNL Work On It] non aggiorna lo stato dell&#39;attività o del problema per segnalare che il lavoro è effettivamente iniziato.

È possibile sostituire il pulsante [!DNL Work On It] con un pulsante [!UICONTROL Inizia] per un team a cui si appartiene. In questo caso, si fa clic sul pulsante [!UICONTROL Inizio] invece di [!UICONTROL Lavoraci], che aggiorna automaticamente lo stato e la [!UICONTROL Data di inizio effettiva] dell&#39;elemento di lavoro, segnalando che hai iniziato a lavorare. Per informazioni sull&#39;impostazione di quale team potrebbe influire sulle modifiche nel pulsante [!UICONTROL Lavoraci], vedere la sezione [Configurare il pulsante [!UICONTROL Avvia]](#configure-the-uicontrol-start-button) in questo articolo.

>[!IMPORTANT]
>
>Facendo clic sul pulsante [!UICONTROL Inizio], lo stato e la data di inizio effettiva dell&#39;elemento vengono modificati . Se un altro utente ha iniziato a lavorare su un&#39;attività o un problema (che ha cambiato lo stato in [!UICONTROL In corso] e ha popolato la [!UICONTROL Data di inizio effettiva]), il pulsante per l&#39;elemento viene visualizzato come [!UICONTROL Lavoraci] anche quando un team a cui appartieni ha fatto sostituire il pulsante con un pulsante [!UICONTROL Inizia].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura il pulsante [!UICONTROL Avvia]

Se disponi di una licenza [!UICONTROL Plan], puoi configurare il pulsante [!UICONTROL Start] per un team nella finestra [!UICONTROL Edit] team. Di seguito è riportato il funzionamento del pulsante dopo che è stato abilitato per un team:

* **Il team è assegnato a un elemento di lavoro**: se un team è assegnato all&#39;elemento di lavoro, i membri del team visualizzano il pulsante [!UICONTROL Avvia] e gli stati configurati per il team.
* **L&#39;utente appartiene a un team predefinito**: se nessun team è assegnato all&#39;elemento di lavoro ma l&#39;utente è assegnato a un team predefinito nel suo profilo, l&#39;utente visualizza il pulsante [!UICONTROL Avvia] e gli stati configurati per tale team. Questo è lo scenario consigliato se si desidera che gli utenti utilizzino spesso il pulsante [!UICONTROL Avvia].
* **L&#39;utente è assegnato a un elemento di lavoro**: se all&#39;elemento di lavoro non è assegnato alcun team e all&#39;utente non è assegnato alcun team predefinito ma l&#39;utente è assegnato all&#39;elemento di lavoro, l&#39;utente visualizza il pulsante [!UICONTROL Avvia] e gli stati combinati configurati per tutti i team a cui sono assegnati.
* **L&#39;utente non è assegnato ad alcun team:** Se all&#39;elemento di lavoro non è assegnato alcun team e non è assegnato alcun team per l&#39;utente, incluso il team predefinito, e l&#39;elemento è assegnato all&#39;utente, verrà visualizzato il pulsante [!UICONTROL Lavoraci].

>[!NOTE]
>
>Questa funzione non è attualmente disponibile in
>
>* L&#39;app mobile [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notifiche e-mail
>

Per configurare il pulsante Start:

{{step1-to-team}}

1. Nel menu a discesa **[!UICONTROL Team]**, seleziona un team.\
   oppure\
   Fare clic su **[!UICONTROL Crea nuovo team]**.

1. Fai clic sull&#39;icona **[!UICONTROL Altro]** ![](assets/more-icon.png), quindi fai clic su **[!UICONTROL Modifica]**.

1. Trova la sezione del pulsante **[!UICONTROL Lavoraci]** nella parte inferiore della pagina [!UICONTROL Modifica team].
1. Selezionare la casella di controllo **[!UICONTROL Cambia il pulsante Lavoraci in pulsante Avvia per aggiornare automaticamente lo stato di un elemento]**.
1. Selezionare uno o più stati per ogni tipo di elemento di lavoro. Se si selezionano più stati, quando si fa clic su [!UICONTROL Inizio] viene visualizzato un menu a discesa in cui è possibile scegliere lo stato desiderato.
1. Fai clic su **[!UICONTROL Salva modifiche]**. Gli utenti ora visualizzano un pulsante [!UICONTROL Avvia attività] o [!UICONTROL Avvia problema] invece del pulsante [!UICONTROL Lavoraci] quando ricevono un elemento di lavoro.

   >[!NOTE]
   >
   >È consigliabile impostare il team come team predefinito di un utente in modo che il pulsante di avvio venga visualizzato su tutti gli elementi di lavoro assegnati. Vedi [Associa utenti a un team predefinito](#associate-users-with-a-home-team) di seguito.

## Associa utenti a un team predefinito

Per associare utenti a un team predefinito:

{{step-1-to-users}}

1. Selezionare l&#39;utente o gli utenti che si desidera associare a un team predefinito.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Nella sezione **[!UICONTROL Organizzazione]**, seleziona il campo **[!UICONTROL Team predefinito]**. Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fare clic sul nome del team quando viene visualizzato nell&#39;elenco.

1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team predefinito.

   Tutte le impostazioni del team, inclusi gli stati associati al pulsante [!UICONTROL Fine], sono ora visibili a questi utenti.

