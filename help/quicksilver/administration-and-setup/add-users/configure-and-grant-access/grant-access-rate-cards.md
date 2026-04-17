---
title: Concedi l'accesso alle schede tariffa
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi definire l’accesso di un utente ai dati finanziari in Workfront tramite il suo livello di accesso.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 10%

---

# Concedere l’accesso alle schede tariffa

In qualità di amministratore di Adobe Workfront, puoi definire l&#39;accesso di un utente alle schede di valutazione attraverso il suo livello di accesso, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Per informazioni sulle schede di tariffa, consulta [Gestire le schede di tariffa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per la concessione dell’accesso alle schede tariffarie

Quando consenti agli utenti di accedere alle schede delle tariffe in Workfront, tieni presente quanto segue:

* Gli utenti devono disporre dell&#39;accesso in modifica a schede tariffe, progetti e dati finanziari per associare una scheda tariffa a un progetto.
* Gli utenti che non hanno accesso alle schede tariffarie e accesso in modifica ai dati finanziari non possono allegare una scheda tariffaria a un progetto, ma possono modificare altre tariffe di fatturazione sul progetto provenienti da altre origini.

## Configurare l’accesso degli utenti alle schede di classificazione utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Biglietti da visita, quindi seleziona le abilità che desideri concedere in **Ottimizza le impostazioni**.

   ![Ottimizzare l&#39;accesso alle schede](assets/rate-card-access-fine-tune.png)

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedere l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso alle schede di tariffa condivisa

Puoi condividere una scheda tariffaria con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere una scheda tariffaria](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

Quando si condivide un oggetto con un altro utente, i diritti del destinatario su di esso sono determinati da una combinazione di due fattori:

* Autorizzazioni concesse al destinatario per l&#39;oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
