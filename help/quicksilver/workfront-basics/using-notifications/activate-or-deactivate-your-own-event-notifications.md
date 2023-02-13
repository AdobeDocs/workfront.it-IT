---
product-area: setup
navigation-topic: notifications
title: Attivare o disattivare le notifiche degli eventi personali
description: L’amministratore di Adobe Workfront configura le notifiche degli eventi che gli utenti ricevono quando si verificano eventi in Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Attivare o disattivare le notifiche degli eventi personali

Il tuo Adobe [!DNL Workfront] l&#39;amministratore configura le notifiche degli eventi che gli utenti ricevono quando si verificano eventi in Workfront (come descritto in [[!UICONTROL Configura evento] notifiche per tutti nel sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

L’amministratore del gruppo può anche configurare quali notifiche di evento vengono attivate per te e per gli utenti del gruppo Home. Se [!UICONTROL Gruppo Home] è un sottogruppo, ricevi le notifiche dell’evento attivate per il gruppo di primo livello sopra il gruppo.

Puoi personalizzare ulteriormente questo aspetto configurando le notifiche ricevute. Puoi anche scegliere se desideri ricevere notifiche mentre si verificano eventi o in un’e-mail digest giornaliera.

Per informazioni sulle notifiche e-mail, vedi [[!DNL Adobe Workfront] Notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Se attivi un tipo di notifica e poi scopri che non ricevi notifiche di quel tipo, potrebbe essere perché quel tipo non si applica al tuo ruolo.
>* La [!DNL Workfront] l&#39;amministratore o un amministratore di gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Per ulteriori informazioni sulle notifiche di [!DNL Workfront] l&#39;amministratore può configurare, consulta [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Per informazioni sulla configurazione di singole notifiche per [!DNL Workfront Goals] continua a leggere questo articolo.
>


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

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Visualizza e modifica le impostazioni delle notifiche e-mail

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic sul nome utente accanto all’immagine del profilo.

1. Fai clic sul pulsante **[!UICONTROL Altro]** icona ![](assets/more-icon.png) , quindi fai clic su **[!UICONTROL Modifica]**.

1. In **[!UICONTROL Modifica persona]** nella casella visualizzata, passare alla **[!UICONTROL Notifiche]** sezione .

1. Fai clic su una categoria per visualizzare le impostazioni di notifica relative a tale categoria.

   ![](assets/my-profile-notifications.png)

1. Seleziona o deseleziona le caselle di controllo a destra per specificare se desideri ricevere o meno notifiche giornaliere, istantaneamente o entrambe.

   È inoltre possibile utilizzare le caselle di controllo relative a una categoria per attivare o disattivare tutte le notifiche presenti nella categoria.

   >[!NOTE]
   >
   >Se sei membro del team per un progetto, continua a ricevere notifiche e-mail finché non vieni rimosso dal team, anche se non hai più accesso al progetto. Per istruzioni sulla rimozione degli utenti da un team, consulta [Rimuovere utenti dai progetti](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Per **[!UICONTROL Comunicazione]** categoria , puoi selezionare singole notifiche solo per la consegna istantanea. Per ricevere le notifiche in un riepilogo giornaliero, devi selezionarle tutte.

   Se vengono attivate tutte le notifiche e-mail per una determinata categoria, la casella nel titolo della categoria viene visualizzata come selezionata. Se tutte le notifiche e-mail in una determinata categoria sono disattivate, la casella viene deselezionata. Se alcune notifiche vengono attivate e altre disattivate, la casella di controllo della categoria viene visualizzata come una linea retta.\
   Quando modifichi un’impostazione di notifica, l’etichetta **[!UICONTROL Modificato]** viene visualizzata per tale impostazione di notifica, per informarti che l’impostazione di notifica è stata modificata.

1. Se hai selezionato le notifiche da inviare come riepilogo giornaliero, seleziona l’ora del giorno in cui desideri riceverle nella parte superiore della **[!UICONTROL Notifiche]** nella sezione **[!UICONTROL Digest giornaliero e-mail dopo]** menu.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   Il riepilogo giornaliero include eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Ricevi un’e-mail digest giornaliera per ogni tipo di notifica.\
   Il riepilogo giornaliero potrebbe arrivare dopo il tempo selezionato, a seconda del numero di e-mail che vengono messe in coda per la consegna nel sistema. L&#39;ora indicata è l&#39;ora locale specificata nelle impostazioni del browser.

1. (Condizionale e facoltativo) Quando modifichi le impostazioni delle notifiche e-mail nell’ambiente di anteprima, abilita l’ **[!UICONTROL Ricevi e-mail da questo ambiente di test]** impostazione per la ricezione di e-mail. Le e-mail non vengono generate automaticamente dall’ambiente di anteprima.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Fai clic su **[!UICONTROL Salva modifiche]**.
