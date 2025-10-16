---
title: Concedi accesso alla gestione delle risorse
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente alla gestione delle risorse in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# Concedere l’accesso alla gestione delle risorse

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente alla gestione delle risorse, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configurare l’accesso degli utenti agli strumenti di gestione delle risorse utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Gestione risorse, quindi seleziona le abilità che desideri concedere in **Ottimizza le impostazioni**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modifica priorità e ore preventivate nella Programmazione</td> 
      <td> <p>Consente agli utenti con questa licenza di effettuare le seguenti operazioni:</p> <p>Assegna la priorità ai progetti nella Programmazione delle risorse.</p> <p>Allocazione del budget per le risorse negli strumenti di pianificazione delle risorse (la sezione Pianificazione risorse e Budget risorse nel caso aziendale di un progetto).</p> <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestisci gruppi di risorse</td> 
      <td> <p>Consente agli utenti con questa licenza di creare, modificare ed eliminare gruppi di risorse. Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Aggiorna le ore pianificate nel Bilanciatore dei carichi di lavoro</span> </td> 
      <td> <p>Consente agli utenti con questa licenza di aggiornare le ore pianificate degli elementi di lavoro quando aggiornano le allocazioni utente nel Bilanciatore dei carichi di lavoro. Il numero totale di ore allocate diventa le ore pianificate degli elementi di lavoro.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> <p> Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni utente nel Bilanciatore dei carichi di lavoro</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso alla gestione delle risorse per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con Gestione risorse, vedere la sezione [Gestione risorse](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai problemi condivisi

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando si condivide un oggetto con un altro utente, i diritti del destinatario per l&#39;allocazione del budget o la visualizzazione dell&#39;allocazione delle risorse su di esso sono determinati da una combinazione di tre elementi:

* Impostazione del livello di accesso del destinatario per Gestione risorse
* Accesso dell&#39;utente ai dati finanziari, come spiegato in [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Qualsiasi autorizzazione concessa dal condivisore ai dati finanziari per l&#39;oggetto

Per informazioni sulle autorizzazioni che gli utenti possono concedere ai dati finanziari su un oggetto durante la condivisione dell&#39;oggetto, vedere [Condividere le autorizzazioni finanziarie su un oggetto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
