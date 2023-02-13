---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi
description: Se sei un amministratore di Adobe Workfront, puoi sbloccare o ribloccare la possibilità per gli amministratori di gruppo di configurare una notifica evento per i gruppi di primo livello che gestiscono. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi

Se sei un amministratore di Adobe Workfront, puoi sbloccare o ribloccare la possibilità per gli amministratori di gruppo di configurare una notifica evento per i gruppi di primo livello che gestiscono. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Quando un amministratore configura una notifica evento per un gruppo, la configurazione ha effetto sugli utenti per i quali tale gruppo, o uno dei suoi sottogruppi, è il gruppo principale. Nei loro profili utente, questi utenti visualizzano le notifiche degli eventi che vengono attivate per il loro gruppo principale invece delle notifiche degli eventi che vengono attivate a livello di sistema. Per ulteriori informazioni, consulta [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un amministratore Workfront può sbloccare e bloccare nuovamente la configurazione per una notifica di evento sia in Adobe Workfront Classic che nella nuova esperienza Adobe Workfront. Tuttavia, un amministratore di gruppo può configurare tale notifica evento per un gruppo solo nella nuova esperienza Adobe Workfront. Gli amministratori di gruppo che utilizzano Adobe Workfront Classic possono passare alla nuova esperienza Adobe Workfront per configurare le notifiche degli eventi sbloccati per un gruppo, quindi tornare ad Adobe Workfront Classic per vedere le modifiche effettive.
>* I sottogruppi ereditano le configurazioni di notifica degli eventi a livello di gruppo dai gruppi di livello superiore sopra di essi.
>


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sblocca o blocca nuovamente la possibilità di configurare una notifica evento

>[!IMPORTANT]
>
>Quando blocchi di nuovo una notifica, tutti i gruppi nel sistema ereditano la notifica esattamente come la imposti. In questo modo vengono ignorate tutte le modifiche che gli amministratori di gruppo potrebbero aver apportato ai propri gruppi, pertanto è consigliabile consultare prima con loro.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **E-mail** > **Notifiche**.

1. Assicurati che **Notifiche degli eventi** è aperta la scheda .
1. Fai clic sull’icona a destra della notifica per passare alla notifica sbloccata ![](assets/lock-toggle-button.png) o bloccato ![](assets/unlock-toggle-button.png) posizione.

   Oppure

   Se desideri sbloccare o bloccare più notifiche contemporaneamente, selezionale, quindi fai clic su Sblocca ![](assets/unlock-icon-toolbar.png) o Blocca ![](assets/lock-icon-locked-qs.png) che viene visualizzato nella barra degli strumenti sopra l’elenco.

1. Fai clic su **Salva**.
1. (Facoltativo) Se desideri configurare la notifica dell&#39;evento per un gruppo di livello principale invece di lasciare questa attività all&#39;amministratore del gruppo, puoi effettuare una delle seguenti operazioni:

   * Elimina **Notifiche degli eventi di sistema** nella casella di ricerca sopra l’elenco delle notifiche, cerca e seleziona il nome del gruppo di livello principale per elencare le relative notifiche, quindi attiva o disattiva le notifiche sbloccate nell’elenco visualizzato.
   * Fai clic su **Gruppi** nel menu a sinistra, fai clic sul nome del gruppo di livello principale. Fai clic su **Notifiche degli eventi** nel pannello a sinistra, configura la notifica dell’evento sbloccato, come spiegato in [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
