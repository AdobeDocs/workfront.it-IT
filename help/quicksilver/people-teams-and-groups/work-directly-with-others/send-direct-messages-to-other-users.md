---
content-type: reference
product-area: user-management
navigation-topic: people-teams-and-groups
title: Inviare messaggi diretti ad altri utenti
description: Adobe Workfront consente di inviare in modo rapido e semplice messaggi non correlati a qualsiasi elemento di lavoro direttamente ad altri utenti di Workfront.
author: Lisa
feature: People Teams and Groups
exl-id: 82a1c304-176a-48c5-809d-40663ee768b7
source-git-commit: 52d722932b6b445bc8ee08a706e4e53765776bf7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Inviare messaggi diretti ad altri utenti

{{highlighted-preview}}

[!DNL Adobe Workfront] consente di inviare in modo rapido e semplice messaggi non correlati ad alcun elemento di lavoro direttamente ad altri utenti di [!DNL Workfront]. I messaggi inviati come descritto in questa sezione vengono visualizzati nella scheda [!UICONTROL Aggiornamenti] nella pagina del profilo dell&#39;utente e sono visibili a tutti gli utenti. Per ulteriori informazioni sugli aggiornamenti, vedere [Aggiorna elementi di lavoro e visualizza aggiornamenti: indice articolo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work-items-and-view-updates.md).

Quando si invia un messaggio come descritto in questa sezione, l&#39;utente a cui viene inviato il messaggio riceve i seguenti tipi di notifiche:

* Una notifica in-app, come descritto in [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)
* Una notifica e-mail

  Questo dipende dai tipi di notifiche e-mail che l’utente è configurato per ricevere. Per ulteriori informazioni, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md), [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md) e [Modificare le notifiche e-mail personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Per inviare un messaggio dalla pagina del profilo utente, è necessario disporre di:<br>
   Nuovo: Chiaro o superiore<br>
   o<br>
   Corrente: revisione o versione successiva</p>
   <p>Per inviare un messaggio dall'elenco utenti, è necessario disporre di:<br>
   Nuovo: Standard<br>
   o<br>
   Corrente: Lavoro o versione successiva</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inviare un messaggio non correlato a un elemento di lavoro a un altro utente dalla pagina del profilo

1. Vai alla pagina del profilo dell’utente a cui desideri inviare un messaggio.

   Per passare alla pagina del profilo di un utente, fare clic sul nome collegato dell&#39;utente visualizzato in qualsiasi punto dell&#39;interfaccia [!DNL Workfront]. I nomi utente vengono visualizzati in molte aree, ad esempio in un commento dell’utente.

1. Nella scheda **[!UICONTROL Aggiornamenti]**, fare clic nel campo della casella di testo.

   ![Invia un messaggio all&#39;utente nella scheda [!UICONTROL Aggiornamenti]](assets/send-message-to-user-on-updates-tab.png)

1. Digita il messaggio.
1. (Facoltativo) Fai clic sul campo **[!UICONTROL Notify]**, quindi inizia a digitare il nome di un altro utente che desideri includere nel messaggio.

1. (Facoltativo) Seleziona **[!UICONTROL Privato per la mia azienda]** per rendere questo messaggio visibile solo agli altri utenti della tua azienda.

1. Fai clic su **[!UICONTROL Aggiorna].**
Il messaggio viene pubblicato nella parte superiore dell&#39;elenco dei messaggi nella scheda **[!UICONTROL Aggiornamenti]** della pagina del profilo dell&#39;utente.

## Invia un messaggio a uno o più utenti dall&#39;elenco Utenti

Questa opzione è disponibile solo se si dispone di una licenza Standard, Pianificazione o Lavoro.

{{step-1-to-users}}

1. Selezionare l&#39;utente o gli utenti a cui si desidera inviare un messaggio e fare clic su [!UICONTROL **Invia aggiornamento all&#39;utente**].
1. Digita il messaggio nella finestra [!UICONTROL Invia aggiornamento all&#39;utente]. Utilizza le opzioni di formattazione del testo in base alle esigenze. Per ulteriori informazioni, vedere [Utilizzare Rich Text in un commento di Workfront](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md#use-rich-text-in-a-workfront-comment) nell&#39;articolo [Aggiornare il lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:</span>
   ![Invia messaggio all&#39;utente nella finestra Invia aggiornamento all&#39;utente](assets/send-update-to-user-072825.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Invia messaggio all&#39;utente nella finestra Invia aggiornamento all&#39;utente](assets/send-message-to-user-dialog-from-user-list.png)

1. <span class="preview">(Facoltativo) Fai clic su **Assegna tag alle persone** per assegnare tag ad altri utenti nel messaggio. Per ulteriori informazioni, consulta [Assegnare tag ad altri in occasione di aggiornamenti](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).</span>
1. (Facoltativo) Nell’ambiente di produzione, cerca eventuali altri utenti a cui assegnare il tag nel messaggio. Non è necessario assegnare tag agli utenti già selezionati nell’elenco di utenti.
1. (Facoltativo) Seleziona **[!UICONTROL Privato per la mia azienda]** per rendere questo messaggio visibile solo agli altri utenti della tua azienda.
1. Fai clic su [!UICONTROL **Invia**].
Il messaggio viene pubblicato nella parte superiore dell&#39;elenco dei messaggi nella scheda **[!UICONTROL Aggiornamenti]** della pagina del profilo di ogni utente taggato.
