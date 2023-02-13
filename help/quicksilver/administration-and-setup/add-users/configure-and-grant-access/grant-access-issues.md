---
title: Concedere l’accesso ai problemi
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai problemi di Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Concedere l’accesso ai problemi

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai problemi, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Per informazioni sull&#39;utilizzo dei livelli di accesso personalizzati per gestire l&#39;accesso degli utenti ad altri tipi di oggetto in Workfront, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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

## Consentire agli utenti di accedere ai problemi utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Issues, quindi seleziona le capacità che desideri concedere in **Ottimizzare le impostazioni**.

1. (Facoltativo) Per limitare le autorizzazioni ereditate per i problemi derivanti da oggetti di classificazione superiore, fare clic su **Imposta restrizioni aggiuntive**, quindi seleziona **Non ereditare mai l’accesso ai documenti da progetti, attività, problemi e così via**.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso ai problemi per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i problemi, consulta la sezione . [Problemi](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai problemi condivisi

In qualità di proprietario o creatore di un problema, puoi condividerlo con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto

Inoltre, se consentito dal livello di accesso, gli utenti possono accedere a un problema tramite la gerarchia degli oggetti: se un utente dispone già dell&#39;autorizzazione per un progetto o un&#39;attività padre di un problema, dispone anche dell&#39;autorizzazione per il problema (vedi il passaggio 3 sopra). Quando condividi un problema, puoi visualizzare un elenco degli utenti che hanno ereditato l’autorizzazione.

![](assets/inherited-permissions.png)
