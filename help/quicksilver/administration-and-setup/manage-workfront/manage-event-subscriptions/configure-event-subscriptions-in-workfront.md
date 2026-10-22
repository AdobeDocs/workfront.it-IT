---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configurare le sottoscrizioni di eventi in Workfront
description: Gli amministratori di Workfront possono creare, visualizzare ed eliminare sottoscrizioni di eventi da Configurazione. Gli utenti con l’accesso richiesto possono anche gestire le sottoscrizioni di eventi all’interno dell’ambito consentito dalle loro autorizzazioni e dalla configurazione del sistema.
feature: System Setup and Administration
role: Admin
author: Becky
source-git-commit: 35d1ee552feec33f3f2ae17dff12601ab0d90951
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 8%
---

# Configurare le sottoscrizioni di eventi in Workfront

In qualità di amministratore di Adobe Workfront, puoi creare, visualizzare ed eliminare sottoscrizioni di eventi dall’area Configurazione. Le sottoscrizioni di eventi inviano informazioni sull’evento Workfront a un endpoint esterno quando si verificano eventi specifici.

Puoi creare ed eliminare sottoscrizioni di eventi in Workfront, ma non puoi modificare una sottoscrizione esistente. Se devi modificare un abbonamento, eliminalo e creane uno nuovo.

Gli utenti che dispongono dell’accesso richiesto possono anche gestire gli abbonamenti agli eventi in Workfront, ma solo entro l’ambito consentito dalle loro autorizzazioni e dalla configurazione del sistema. Per ulteriori informazioni, vedere [Gestire le sottoscrizioni di eventi come utente non amministratore](/help/quicksilver/wf-api/general/event-subs-non-admin.md).

Per ulteriori informazioni sulle sottoscrizioni di eventi, vedere gli articoli in [Sottoscrizioni di eventi](/help/quicksilver/wf-api/api/event-subscriptions.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Pacchetto Adobe Workfront</td>
   <td>Qualsiasi</td>
  </tr>
  <tr>
   <td role="rowheader">Licenza di Adobe Workfront</td>
   <td>
    <p>Standard</p>
    <p>Piano</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurazioni del livello di accesso</td>
   <td>
    <p>Devi disporre dell’accesso appropriato per gestire gli abbonamenti agli eventi.</p>
    <p>Gli utenti non amministratori possono accedere solo all’interno dell’ambito consentito dalle loro autorizzazioni e dalla configurazione del sistema.</p>
   </td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una sottoscrizione di evento

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **Sistema**, quindi su **Sottoscrizioni eventi**.
1. Fai clic su **Nuova sottoscrizione evento**.
1. Nel campo **Oggetto** selezionare l&#39;oggetto Workfront che si desidera monitorare.
1. Nel campo **Tipo evento**, selezionare se si desidera che la sottoscrizione dell&#39;evento venga attivata quando l&#39;oggetto viene creato, aggiornato, eliminato o condiviso.
1. Nel campo **URL webhook**, immettere l&#39;endpoint che deve ricevere il payload dell&#39;evento.
1. Nel campo **Token di autenticazione**, immetti il token utilizzato per autenticare la richiesta nell&#39;endpoint.
1. Se desideri che Workfront codifichi il payload prima di inviarlo, abilita l’opzione per inviare il payload come Base64.
1. Se necessario, aggiungi uno o più filtri per limitare gli eventi che attivano l’abbonamento. I filtri disponibili si basano sull’oggetto selezionato.
1. Fai clic su **Crea**.

Per informazioni sui requisiti dell&#39;endpoint, vedere [Requisiti di consegna per abbonamento eventi](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## Visualizza sottoscrizioni eventi

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **Sistema**, quindi su **Sottoscrizioni eventi**.

Dalla pagina Sottoscrizioni eventi, puoi esaminare le sottoscrizioni configurate per il tuo ambiente. Puoi anche vedere quanti abbonamenti totali ha la tua organizzazione e quanti di questi sono attivi, disabilitati o congelati.

* **Sottoscrizioni disabilitate**: queste sottoscrizioni sono state disabilitate automaticamente a causa di ripetuti errori di consegna.
* **Abbonamenti bloccati**: questi abbonamenti sono temporaneamente bloccati a causa di problemi di consegna.

## Eliminare una sottoscrizione di evento

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **Sistema**, quindi su **Sottoscrizioni eventi**.
1. Seleziona la sottoscrizione evento da rimuovere.
1. Fai clic su **Elimina**.
