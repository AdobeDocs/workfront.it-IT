---
title: Concedere l’accesso ai progetti
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai progetti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Concedere l’accesso ai progetti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai progetti, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configurare l’accesso utente ai progetti tramite un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Progetti, quindi seleziona le capacità che desideri concedere in **Ottimizzare le impostazioni**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Gli utenti con una licenza di lavoro dispongono di diritti di progetto limitati. Possono contribuire a un progetto, ma non gestirlo.
   >* Gli utenti con una licenza di revisione dispongono dei diritti di visualizzazione sui progetti derivanti da problemi di conversione, ma i loro diritti di visualizzazione sono limitati.
   >* Per informazioni sulle autorizzazioni che gli utenti possono concedere quando condividono progetti con altri, consulta [Condivisione di un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Quando si configura un&#39;impostazione del livello di accesso per un determinato tipo di oggetto, tale configurazione non influisce sull&#39;accesso degli utenti agli oggetti con un livello inferiore. Ad esempio, è possibile impedire agli utenti di eliminare i progetti nel loro livello di accesso, ma ciò non impedisce loro di eliminare le attività, che sono di livello inferiore rispetto ai progetti.Per ulteriori informazioni sulla gerarchia degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).


1. (Facoltativo) Fai clic su **imposta valori predefiniti di condivisione** a destra dell’opzione Crea , quindi **Aggiungi regola** per aggiungere una regola di condivisione per i nuovi progetti.

   Quando l’utente con questo livello di accesso crea un progetto, questo viene condiviso automaticamente con gli utenti selezionati nel menu a sinistra.

   ![](assets/project-sharing-menu.png)

   Nel menu a destra, specifica come condividere il progetto con tali utenti:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Se un utente con questo livello di accesso utilizza un modello di accesso al progetto, questo sostituisce le impostazioni di condivisione a livello di accesso. Per informazioni sui modelli di accesso ai progetti, consulta [Condivisione di un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   Puoi ripetere questo passaggio per aggiungere tutte le regole di condivisione del progetto necessarie per il livello di accesso.

1. Fai clic sulla X per chiudere la **Ottimizzare le impostazioni** scatola.
1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso a report, dashboard e calendari per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i problemi, consulta la sezione . [Progetti](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai progetti condivisi

In qualità di proprietario o creatore di un problema, puoi condividerlo con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condivisione di un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
