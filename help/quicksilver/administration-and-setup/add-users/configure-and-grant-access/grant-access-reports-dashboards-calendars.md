---
title: Consentire l’accesso a report, dashboard e calendari
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
source-wordcount: '602'
ht-degree: 0%

---

# Consentire l’accesso a report, dashboard e calendari

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente a rapporti, dashboard e calendari, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Questo accesso include anche l’accesso alle pagine esterne. Per informazioni sulle pagine esterne, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Se desideri concedere agli utenti l’accesso a rapporti, dashboard e calendari, devi anche consentire loro di accedere a filtri, visualizzazioni e raggruppamenti. Per istruzioni, consulta [Consentire l’accesso a filtri, visualizzazioni e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Quando un utente condivide un report, un dashboard o un calendario con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi: Impostazione del livello di accesso del destinatario per report, dashboard e calendari _e_ autorizzazioni concesse dall&#39;utente condiviso per il report, il dashboard o il calendario
>
>Per informazioni sulle autorizzazioni che gli utenti possono concedere su un report, dashboard o calendario durante la condivisione, consulta [Condividere rapporti, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso degli utenti a rapporti, dashboard e calendari utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Report, quindi seleziona le capacità che desideri concedere in **Ottimizzare le impostazioni**.

   ![reports_access.png](assets/reports-access.png)

   Le seguenti opzioni sono abilitate per impostazione predefinita:

   * **Crea**
   * **Elimina**
   * **Visualizzare i rapporti incorporati**: Questa opzione deve essere selezionata per visualizzare i report generati da Workfront.
   * **Condividi**
   * **Condividere i rapporti pubblicamente**: I rapporti possono essere condivisi pubblicamente, condividendo un link pubblico al rapporto con chiunque non abbia un account Workfront. Questa opzione deve essere selezionata per consentire questo livello di condivisione.
   * **Condividi a livello di sistema**: I rapporti possono essere condivisi con tutti gli utenti del sistema che dispongono di una licenza Workfront. Questa opzione deve essere selezionata per consentire questo livello di condivisione.

      Per informazioni sulla condivisione di rapporti, dashboard e calendari, consulta [Condividere rapporti, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso a report, dashboard e calendari per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i problemi, consulta la sezione . [Rapporti](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso a rapporti condivisi, dashboard e calendari condivisi

In qualità di proprietario o creatore di un report, dashboard o calendario, puoi condividerlo con altri utenti concedendo loro autorizzazioni, come spiegato in [Condividere rapporti, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
