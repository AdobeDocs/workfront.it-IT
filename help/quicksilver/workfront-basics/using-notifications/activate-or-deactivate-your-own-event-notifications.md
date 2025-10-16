---
product-area: setup
navigation-topic: notifications
keywords: modifica,e-mail,notifica,impostazioni
title: Modifica le tue notifiche e-mail
description: Questo articolo descrive come gestire le notifiche e-mail nel profilo utente.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Modifica le tue notifiche e-mail

<!-- Audited: 1/2024 -->

L&#39;amministratore di Adobe [!DNL Workfront] configura le notifiche e-mail ricevute dagli utenti quando si verificano eventi in Workfront (come descritto in [[!UICONTROL Configurare le notifiche evento] per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

L&#39;amministratore del gruppo può anche configurare le notifiche attivate per te e per gli utenti del [!UICONTROL Gruppo predefinito]. Se il [!UICONTROL Gruppo predefinito] è un sottogruppo, riceverai le notifiche attivate per il gruppo di primo livello al di sopra del gruppo.

Puoi personalizzare ulteriormente questa impostazione configurando le notifiche che ricevi. Puoi anche scegliere se ricevere le notifiche quando gli eventi si verificano o in un’e-mail di riepilogo giornaliera.

Per ulteriori informazioni sulle notifiche e-mail, vedi [[!DNL Adobe Workfront] notifiche](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Se si attiva un tipo di notifica e successivamente si scopre che non vengono ricevute notifiche di quel tipo, è possibile che tale tipo non sia applicabile al ruolo.
>* L&#39;amministratore di [!DNL Workfront] o un amministratore gruppo non può configurare le notifiche per [!DNL Workfront Goals]. Per ulteriori informazioni sulle notifiche configurabili dall&#39;amministratore [!DNL Workfront], vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Per informazioni sulla configurazione di singole notifiche per [!DNL Workfront Goals], continuare a leggere questo articolo.
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Request or Higher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e modificare le impostazioni delle notifiche e-mail

{{step1-click-profile-pic}}

1. Fai clic sull&#39;icona **[!UICONTROL Altro]** ![Altro icona](assets/more-icon.png) accanto al tuo nome, quindi fai clic su **[!UICONTROL Modifica]**.

1. Nella casella **[!UICONTROL Modifica persona]** visualizzata, vai alla sezione **[!UICONTROL Notifiche]**.

1. Fare clic su una categoria per visualizzare le impostazioni di notifica correlate a tale categoria.

   ![Notifiche del mio profilo](assets/my-profile-notifications.png)

1. Selezionare o deselezionare le caselle di controllo sulla destra per specificare se si desidera ricevere o meno notifiche ogni giorno, all&#39;istante o entrambe.

   È inoltre possibile utilizzare le caselle di controllo di una categoria per attivare o disattivare tutte le notifiche della categoria.

   >[!NOTE]
   >
   >I membri del team di un progetto continuano a ricevere notifiche e-mail finché non vengono rimossi dal team, anche se non hanno più accesso al progetto. Per istruzioni sulla rimozione degli utenti da un team, vedere [Rimuovere gli utenti dai progetti](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Per la categoria **[!UICONTROL Comunicazione]**, è possibile selezionare singole notifiche solo per la consegna immediata. Affinché le notifiche vengano recapitate in un riepilogo giornaliero, è necessario selezionarle tutte.

   Se tutte le notifiche e-mail per una determinata categoria sono attivate, la casella nel titolo della categoria viene visualizzata come selezionata. Se tutte le notifiche e-mail in una determinata categoria sono disattivate, la casella viene deselezionata. Se alcune notifiche sono attivate e altre sono disattivate, la casella di controllo della categoria viene visualizzata come una linea retta.\
   Quando modifichi un&#39;impostazione di notifica, viene visualizzata l&#39;etichetta **[!UICONTROL Modificato]** per tale impostazione di notifica, per informarti che l&#39;impostazione di notifica è stata modificata.

1. Se hai selezionato delle notifiche da inviare come riepilogo giornaliero, seleziona l&#39;ora del giorno in cui desideri riceverla nella parte superiore della sezione **[!UICONTROL Notifiche]** nel menu **[!UICONTROL Invia riepilogo giornaliero tramite posta elettronica dopo]**.

   ![Digest giornaliero: scegli ora del giorno](assets/digest-time-stamp-my-settings-350x78.png)

   Il riepilogo giornaliero include gli eventi che soddisfano i criteri delle notifiche 24 ore prima dell’ora selezionata. Ricevi un’e-mail di riepilogo giornaliero per ogni tipo di notifica.\
   Il riepilogo giornaliero può arrivare dopo l’orario selezionato, a seconda di quante e-mail sono in coda per la consegna nel sistema. L’ora indicata corrisponde all’ora locale specificata nelle impostazioni del browser.

1. (Condizionale e facoltativo) Quando modifichi le impostazioni delle notifiche e-mail nell&#39;ambiente di anteprima, abilita l&#39;impostazione **[!UICONTROL Ricevi e-mail da questo ambiente di test]** per ricevere e-mail. Le e-mail non vengono generate automaticamente dall’ambiente di anteprima.

   ![Ricevi e-mail da sndbox](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Fai clic su **[!UICONTROL Salva modifiche]**.
