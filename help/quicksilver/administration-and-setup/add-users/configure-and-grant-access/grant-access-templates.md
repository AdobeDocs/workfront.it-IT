---
title: Concedere l’accesso ai modelli
user-type: administrator
product-area: system-administration;templates
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai modelli in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c8e6af1b-8cf3-4522-b0eb-7e5f2d34f5a9
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Concedere l’accesso ai modelli

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai modelli, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Solo gli utenti con una licenza Plan possono avere accesso completo ai modelli.

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

## Configurare l’accesso utente ai modelli utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Templates, quindi selezionare le capacità che si desidera concedere in **Ottimizzare le impostazioni**.

   ![](assets/access-level-to-templates-with-edit-expanded-1.png)

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso ai modelli per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i modelli, consulta la sezione . [Modelli](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#template) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai modelli condivisi

In qualità di proprietario o creatore di un problema, puoi condividerlo con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
