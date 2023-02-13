---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Sostituire il pulsante Work On It con un pulsante Start
description: La configurazione predefinita di Adobe Workfront include un pulsante Lavora su di esso per le attività e i problemi che vengono visualizzati per gli elementi a cui sei stato assegnato.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Sostituisci il [!UICONTROL Lavorare] pulsante con un [!UICONTROL Inizio] pulsante

[!DNL Adobe Workfront]La configurazione predefinita include un [!UICONTROL Lavorare] pulsante per le attività e i problemi che vengono visualizzati per gli elementi a cui sei stato assegnato. Quando fai clic su [!UICONTROL Lavorare] sugli elementi assegnati, segnala ad altri utenti che hai ricevuto il lavoro e riconosce che lavorerai a esso. Tuttavia, [!DNL Work On It] pulsante non aggiorna l&#39;attività o lo stato del problema per segnalare che il lavoro è effettivamente iniziato.

È possibile sostituire [!DNL Work On It] pulsante con un [!UICONTROL Inizio] pulsante per un team a cui appartieni. In questo caso, fai clic sul pulsante [!UICONTROL Inizio] al posto di [!UICONTROL Lavorare], che aggiorna automaticamente lo stato e la [!UICONTROL Data di inizio effettiva] dell&#39;elemento di lavoro, segnalando che hai iniziato a lavorare. Per informazioni sull&#39;impostazione di quale team potrebbe influenzare le modifiche nel [!UICONTROL Lavorare] , vedi la sezione [Configura le [!UICONTROL Inizio] pulsante](#configure-the-uicontrol-start-button) in questo articolo.

>[!IMPORTANT]
>
>Fai clic su [!UICONTROL Inizio] cambia lo stato dell&#39;elemento e [!UICONTROL Data di inizio effettiva]. Se un altro utente ha iniziato a lavorare su un&#39;attività o su un problema (che ha modificato lo stato in [!UICONTROL In corso] e ha popolato [!UICONTROL Data di inizio effettiva]), il pulsante relativo all’elemento viene visualizzato come [!UICONTROL Lavorare] anche quando una squadra a cui appartieni ha fatto sostituire il pulsante con un [!UICONTROL Inizio] pulsante .

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
   <td> <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Configura le [!UICONTROL Inizio] pulsante

Se hai [!UICONTROL Pianificare] è possibile configurare la [!UICONTROL Inizio] per un team in [!UICONTROL Modifica] finestra del team. Di seguito viene illustrato il funzionamento del pulsante dopo l’abilitazione di un team:

* **Il team viene assegnato a un elemento di lavoro**: Se un team viene assegnato all&#39;elemento di lavoro, i membri del team visualizzano il [!UICONTROL Inizio] e gli stati configurati per quel team.
* **L&#39;utente appartiene a un team principale**: Se nessun team viene assegnato all&#39;elemento di lavoro ma l&#39;utente viene assegnato a un team principale nel suo profilo, l&#39;utente visualizza il [!UICONTROL Inizio] e gli stati configurati per quel team. Questo è lo scenario consigliato se desideri che gli utenti utilizzino il [!UICONTROL Inizio] spesso.
* **L&#39;utente viene assegnato a un elemento di lavoro**: Se all&#39;elemento di lavoro non è assegnato alcun team e all&#39;utente non è assegnato alcun team, ma l&#39;utente è assegnato all&#39;elemento di lavoro, l&#39;utente visualizza il [!UICONTROL Inizio] e gli stati combinati configurati per tutti i team a cui sono assegnati.
* **L’utente non viene assegnato ad alcun team:** Se all&#39;utente non è assegnato alcun team e nessun team per l&#39;utente, incluso il team principale, e l&#39;elemento viene assegnato all&#39;utente, l&#39;utente sembra che l&#39;utente [!UICONTROL Lavorare] pulsante .

>[!NOTE]
>
>Questa funzione non è attualmente disponibile in
>
>* La [!DNL Workfront] app mobile
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notifiche e-mail
>


Per configurare il pulsante Start:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Team]**.

1. In **[!UICONTROL Team]** selezionare un team dal menu a discesa.\
   oppure\
   Fai clic su **[!UICONTROL Crea team]**.

1. Fai clic sul pulsante **[!UICONTROL Altro]** icona ![](assets/more-icon.png), quindi fai clic su **[!UICONTROL Modifica]**.

1. Trova il **[!UICONTROL Lavorare]** sezione pulsante vicino alla parte inferiore del [!UICONTROL Modifica team] pagina.
1. Seleziona la **[!UICONTROL Per aggiornare automaticamente lo stato di un elemento, cambiare il pulsante Work On It in un pulsante Start]** casella di controllo.
1. Selezionare uno o più stati per ogni tipo di elemento di lavoro. Se selezioni più di uno stato, quando fai clic su viene visualizzato un menu a discesa [!UICONTROL Inizio] dove puoi scegliere lo stato desiderato.
1. Fai clic su **[!UICONTROL Salva modifiche]**. Gli utenti ora visualizzano un [!UICONTROL Avvia attività] o [!UICONTROL Problema iniziale] al posto del [!UICONTROL Lavorare] quando gli viene assegnato un elemento di lavoro.

   >[!NOTE]
   >
   >È consigliabile impostare il team come Home Team dell&#39;utente in modo che il pulsante di avvio venga visualizzato su tutti gli elementi di lavoro assegnati. Vedi [Associare gli utenti a un team principale](#associate-users-with-a-home-team) sotto.

## Associare gli utenti a un team principale

Per associare gli utenti a un team principale:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront].

1. Fai clic su **[!UICONTROL Utenti]**, quindi selezionare l&#39;utente o gli utenti che si desidera associare a un Home Team.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In **[!UICONTROL Organizzazione]** seleziona la sezione **[!UICONTROL Team principale]** campo . Inizia a digitare il nome del team di cui desideri associare le impostazioni agli utenti. Fai clic sul nome del team quando lo trovi nell’elenco.

1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   Gli utenti selezionati sono ora associati a un team principale.

   Tutte le impostazioni del team, inclusi gli stati associati all&#39;azione [!UICONTROL Fine] sono ora visibili a questi utenti.

