---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi
description: Se sei un amministratore di Adobe Workfront, puoi sbloccare o bloccare nuovamente la possibilità per gli amministratori di gruppi di configurare una notifica di evento per i gruppi di livello superiore che gestiscono. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 325fb9e58d32d1b6cfa1035cd4a25da4b66f6955
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi

Se sei un amministratore di Adobe Workfront, puoi sbloccare o bloccare nuovamente la possibilità per gli amministratori di gruppi di configurare una notifica di evento per i gruppi di livello superiore che gestiscono. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Quando un amministratore configura una notifica di evento per un gruppo, la configurazione influisce sugli utenti per i quali tale gruppo, o uno dei suoi sottogruppi, è il proprio Gruppo predefinito. Nei profili utente, questi utenti visualizzano le notifiche degli eventi attivate per il proprio Gruppo predefinito anziché le notifiche degli eventi attivate a livello di sistema. Per ulteriori informazioni, consulta [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un amministratore di Workfront può sbloccare e bloccare nuovamente la configurazione per una notifica di evento sia in Adobe Workfront Classic che nella nuova esperienza Adobe Workfront. Tuttavia, un amministratore di gruppo può configurare tale notifica di evento per un gruppo solo nella nuova esperienza Adobe Workfront. Gli amministratori di gruppi che utilizzano Adobe Workfront Classic possono passare alla nuova esperienza Adobe Workfront per configurare le notifiche degli eventi sbloccati per un gruppo, quindi tornare a Adobe Workfront Classic per visualizzare le modifiche in vigore.
>* I sottogruppi ereditano le configurazioni di notifica degli eventi a livello di gruppo dai gruppi di livello superiore.
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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sblocca o riblocca la possibilità di configurare una notifica di evento

>[!IMPORTANT]
>
>Quando si blocca nuovamente una notifica, tutti i gruppi nel sistema ereditano la notifica esattamente come è stata impostata. In questo modo si ignorano eventuali modifiche apportate dagli amministratori dei gruppi ai propri gruppi. È quindi consigliabile consultarli prima.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **E-mail** > **Notifiche**.

1. Assicurati che le **Notifiche evento** è aperta.
1. Fai clic sull’icona a destra della notifica per passare al bloccato ![Icona Blocca](assets/lock-toggle-button.png) o sbloccato ![Icona Sblocca](assets/unlock-toggle-button.png) posizione.

   Oppure

   Se desideri sbloccare o bloccare più notifiche contemporaneamente, selezionale, quindi fai clic su Sblocca ![Icona Sblocca](assets/unlock-icon-toolbar.png) o Blocco ![Icona Blocca](assets/lock-icon-locked-qs.png) che viene visualizzato nella barra degli strumenti sopra l’elenco.

1. Fai clic su **Salva**.
1. (Facoltativo) Se si desidera configurare la notifica dell&#39;evento per un gruppo di livello superiore invece di lasciare questa attività all&#39;amministratore del gruppo, è possibile effettuare una delle seguenti operazioni:

   * Elimina **Notifiche eventi di sistema** nella casella di ricerca sopra l’elenco delle notifiche, cerca e seleziona il nome del gruppo di livello superiore per elencare le notifiche, quindi attiva o disattiva le notifiche sbloccate nell’elenco visualizzato.
   * Clic **Gruppi** nel menu sinistro fare clic sul nome del gruppo di primo livello. Clic **Notifiche evento** nel pannello a sinistra, quindi configura la notifica dell’evento sbloccato, come spiegato in [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
