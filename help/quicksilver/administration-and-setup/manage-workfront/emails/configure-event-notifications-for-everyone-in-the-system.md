---
title: Configurare le notifiche degli eventi per tutti gli utenti del sistema
description: Le notifiche degli eventi attivano le e-mail agli utenti quando si verifica un determinato evento. In qualità di amministratore Adobe Workfront o di utente con un livello di accesso Planner, puoi configurare una notifica evento per tutti gli utenti del sistema. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Configurare le notifiche degli eventi per tutti gli utenti del sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Le notifiche degli eventi attivano le e-mail agli utenti quando si verifica un determinato evento. In qualità di amministratore Adobe Workfront o di utente con un livello di accesso Planner, puoi configurare una notifica evento per tutti gli utenti del sistema. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

A seconda dell’evento che abiliti e l’utente continua a essere abilitato sul proprio profilo, gli utenti ricevono notifiche e-mail istantanee, giornaliere o sia istantanee che giornaliere quando si verifica un evento.

Devi innanzitutto specificare quali notifiche desideri ricevere tutti gli utenti nell’area Configurazione dell’istanza di Workfront. Dopo aver attivato una notifica nell’area Configurazione, questa viene visualizzata come attivata per ogni utente nella relativa pagina del profilo.

Dopo che le notifiche vengono attivate nell’area Configurazione e visualizzate nelle pagine dei profili degli utenti, i singoli utenti o un altro utente con una licenza Plan possono anche configurare le notifiche attivate in un profilo utente per controllare quali notifiche riceve e con quale frequenza un utente specifico. Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Per un elenco di tutte le notifiche di evento attivabili e disattivabili, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Per informazioni sullo sblocco di una notifica evento in modo che gli amministratori di gruppo possano configurarla per i propri gruppi, consulta [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) e [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Planner o superiore, con accesso amministrativo alle notifiche di promemoria</p> <p>Per informazioni su come concedere a un utente del piano l'accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare le notifiche degli eventi per tutti gli utenti

È necessario abilitare le notifiche nell’area Configurazione di Workfront prima che gli utenti possano attivarle o disattivarle nei loro profili.

>[!TIP]
>
>Non è possibile attivare le notifiche per obiettivi Workfront dall&#39;area Configurazione. Gli utenti possono attivare queste notifiche solo nei loro profili. Gli utenti con licenze Pianifica possono attivarle per altri utenti. Per informazioni sull&#39;abilitazione delle notifiche relative agli obiettivi di Workfront per gli utenti, vedi [Notifiche: Obiettivi](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **E-mail** > **Notifiche**.

1. Assicurati che **Notifiche degli eventi** è aperta la scheda .
1. Fare clic sull&#39;interruttore a sinistra del nome dell&#39;evento per attivarlo o disattivarlo.

   Per visualizzare lo stato predefinito della notifica per un evento, vedi [Notifiche degli eventi](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Facoltativo) Fai clic sul nome di una notifica evento per personalizzare l’oggetto della notifica e-mail.

   Per ulteriori informazioni sulla personalizzazione dell’oggetto delle notifiche e-mail, consulta [Personalizzare gli oggetti e-mail per le notifiche degli eventi](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Facoltativo) Se desideri sbloccare la configurazione di una notifica e-mail in modo che gli amministratori dei gruppi possano configurarla separatamente per i loro gruppi, fai clic sul pulsante ![](assets/lock-toggle-button.png) a destra della notifica per passare alla posizione sbloccata ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Questa funzionalità è inizialmente disponibile solo per i clienti del cluster 4 come parte di un rollout graduale. Sarà disponibile per altri cluster a breve. Questo articolo verrà aggiornato man mano che si verifica.

   Per ulteriori informazioni, consulta [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
