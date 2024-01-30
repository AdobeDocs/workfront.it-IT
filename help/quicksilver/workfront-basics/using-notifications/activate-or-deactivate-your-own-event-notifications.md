---
product-area: setup
navigation-topic: notifications
keywords: modifica,e-mail,notifica,impostazioni
title: Modifica le tue notifiche e-mail
description: Questo articolo descrive come gestire le notifiche e-mail nel profilo utente.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Modifica le tue notifiche e-mail

<!-- Audited: 1/2024 -->

Adobe [!DNL Workfront] l’amministratore configura le notifiche e-mail ricevute dagli utenti quando si verificano eventi in Workfront (come descritto in [[!UICONTROL Configura evento] notifiche per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

L’amministratore del gruppo può anche configurare quali notifiche vengono attivate per te e per gli utenti nel tuo [!UICONTROL Gruppo Predefinito]. Se il [!UICONTROL Gruppo Predefinito] è un sottogruppo, ricevi le notifiche attivate per il gruppo di livello superiore rispetto al tuo gruppo.

Puoi personalizzare ulteriormente questa impostazione configurando le notifiche che ricevi. Puoi anche scegliere se ricevere le notifiche quando gli eventi si verificano o in un’e-mail di riepilogo giornaliera.

Per ulteriori informazioni sulle notifiche e-mail, consulta [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Se si attiva un tipo di notifica e successivamente si scopre che non vengono ricevute notifiche di quel tipo, è possibile che tale tipo non sia applicabile al ruolo.
>* Il [!DNL Workfront] un amministratore o un amministratore gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Per ulteriori informazioni sulle notifiche, vedere [!DNL Workfront] l&#39;amministratore può configurare, vedi [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Per informazioni sulla configurazione di singole notifiche per [!DNL Workfront Goals] continua a leggere questo articolo.
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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td>  <p>Nuovo:</p> 
   <ul><li>Collaboratore o versione successiva</li></ul>
   <p>Corrente:</p>
   <ul><li>Request or Higher</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Visualizzare e modificare le impostazioni delle notifiche e-mail

{{step1-click-profile-pic}}

1. Fai clic su **[!UICONTROL Altro]** icona ![](assets/more-icon.png) accanto al tuo nome, quindi fai clic su **[!UICONTROL Modifica]**.

1. In **[!UICONTROL Modifica persona]** che viene visualizzata, passa alla **[!UICONTROL Notifiche]** sezione.

1. Fare clic su una categoria per visualizzare le impostazioni di notifica correlate a tale categoria.

   ![](assets/my-profile-notifications.png)

1. Selezionare o deselezionare le caselle di controllo sulla destra per specificare se si desidera ricevere o meno notifiche ogni giorno, all&#39;istante o entrambe.

   È inoltre possibile utilizzare le caselle di controllo di una categoria per attivare o disattivare tutte le notifiche della categoria.

   >[!NOTE]
   >
   >I membri del team di un progetto continuano a ricevere notifiche e-mail finché non vengono rimossi dal team, anche se non hanno più accesso al progetto. Per istruzioni sulla rimozione di utenti da un team, vedi [Rimuovere utenti dai progetti](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Per **[!UICONTROL Comunicazione]** categoria, puoi selezionare singole notifiche solo per la consegna immediata. Affinché le notifiche vengano recapitate in un riepilogo giornaliero, è necessario selezionarle tutte.

   Se tutte le notifiche e-mail per una determinata categoria sono attivate, la casella nel titolo della categoria viene visualizzata come selezionata. Se tutte le notifiche e-mail in una determinata categoria sono disattivate, la casella viene deselezionata. Se alcune notifiche sono attivate e altre sono disattivate, la casella di controllo della categoria viene visualizzata come una linea retta.\
   Quando modifichi un’impostazione di notifica, l’etichetta **[!UICONTROL Modificato]** per l&#39;impostazione di notifica, per comunicare che l&#39;impostazione di notifica è stata modificata.

1. Se hai selezionato delle notifiche da inviare come riepilogo giornaliero, seleziona l’ora del giorno in cui desideri riceverla nella parte superiore della **[!UICONTROL Notifiche]** sezione nella sezione **[!UICONTROL Invia digest tramite e-mail ogni giorno dopo]** menu.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   Il riepilogo giornaliero include gli eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Ricevi un’e-mail di riepilogo giornaliero per ogni tipo di notifica.\
   Il riepilogo giornaliero può arrivare dopo l’orario selezionato, a seconda di quante e-mail sono in coda per la consegna nel sistema. L’ora indicata corrisponde all’ora locale specificata nelle impostazioni del browser.

1. (Condizionale e facoltativo) Quando modifichi le impostazioni delle notifiche e-mail nell’ambiente di anteprima, abilita **[!UICONTROL Ricevi e-mail da questo ambiente di test]** impostazione per la ricezione di e-mail. Le e-mail non vengono generate automaticamente dall’ambiente di anteprima.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Clic **[!UICONTROL Salva modifiche]**.
