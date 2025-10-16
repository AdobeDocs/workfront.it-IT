---
title: Concedere l’accesso alle attività
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente alle attività in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aafa8886-82e2-41c4-8fcb-cbb9df2d55dd
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Concedere l’accesso alle attività

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente alle attività, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Per informazioni sull&#39;utilizzo dei livelli di accesso personalizzati per gestire l&#39;accesso degli utenti ad altri tipi di oggetti in Workfront, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare l’accesso degli utenti alle attività utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Attività, quindi seleziona le abilità che desideri concedere in **Ottimizza le impostazioni**.

   ![ottimizzazione impostazioni attività](assets/fine-tune-tasks.png)

   >[!NOTE]
   >
   >Quando si configura un&#39;impostazione del livello di accesso per un determinato tipo di oggetto, tale configurazione non influisce sull&#39;accesso degli utenti agli oggetti di livello inferiore. Ad esempio, è possibile impedire agli utenti di eliminare le attività nel loro livello di accesso, ma ciò non impedisce loro di eliminare i problemi, che sono di livello inferiore rispetto alle attività.Per ulteriori informazioni sulla gerarchia degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Informazioni sugli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facoltativo) Per limitare le autorizzazioni ereditate per le attività da oggetti di classificazione superiore, fare clic su **Imposta restrizioni aggiuntive**, quindi selezionare **Non ereditare mai l&#39;accesso ai documenti da progetti, attività, problemi, ecc**.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso alle attività per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con le attività, vedere la sezione [Attività](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#tasks) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso alle attività condivise

In qualità di proprietario o creatore di un problema, puoi condividere con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere un&#39;attività](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

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
