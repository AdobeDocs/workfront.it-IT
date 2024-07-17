---
title: Concedere l’accesso a rapporti, dashboard e calendari
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a rapporti, dashboard e calendari in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Concedere l’accesso a rapporti, dashboard e calendari

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente a report, dashboard e calendari, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Questo accesso include anche l’accesso alle Pagine esterne. Per informazioni sulle pagine esterne, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Se si desidera concedere agli utenti l&#39;accesso a report, dashboard e calendari, è necessario concedere a tali utenti anche l&#39;accesso a filtri, visualizzazioni e raggruppamenti. Per istruzioni, vedere [Concedere l&#39;accesso a filtri, visualizzazioni e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Quando un utente condivide un report, un dashboard o un calendario con un altro utente, i diritti del destinatario sono determinati da una combinazione di due fattori: l&#39;impostazione del livello di accesso del destinatario per report, dashboard e calendari _e_ le autorizzazioni concesse dal condivisore per il report, il dashboard o il calendario
>
>Per informazioni sulle autorizzazioni che gli utenti possono concedere a un report, dashboard o calendario durante la condivisione, vedere [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso degli utenti a rapporti, dashboard e calendari utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Rapporti, quindi seleziona le funzionalità che desideri concedere in **Ottimizza le impostazioni**.

   ![reports_access.png](assets/reports-access.png)

   Le seguenti opzioni sono abilitate per impostazione predefinita:

   * **Crea**
   * **Elimina**
   * **Visualizza report incorporati**: è necessario selezionarlo per visualizzare i report generati da Workfront.
   * **Condividi**
   * **Condividi report pubblicamente**: i report possono essere condivisi pubblicamente condividendo un collegamento pubblico al report con chiunque non disponga di un account Workfront. Per consentire questo livello di condivisione, è necessario selezionare questa opzione.
   * **Condividi a livello di sistema**: i report possono essere condivisi con tutti gli utenti del sistema che dispongono di una licenza Workfront. Per consentire questo livello di condivisione, è necessario selezionare questa opzione.

     Per informazioni sulla condivisione di report, dashboard e calendari, vedere [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso a report, dashboard e calendari per tipo di licenza

Per informazioni sulle operazioni che gli utenti possono eseguire con i problemi in ogni livello di accesso, vedere la sezione [Report](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso a report, dashboard e calendari condivisi

In qualità di proprietario o creatore di un report, dashboard o calendario, puoi condividerlo con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Quando si condivide un oggetto con un altro utente, i diritti del destinatario su di esso sono determinati da una combinazione di due fattori:

* Autorizzazioni concesse al destinatario per l&#39;oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
