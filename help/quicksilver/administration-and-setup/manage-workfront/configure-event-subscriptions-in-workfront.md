---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configurare le sottoscrizioni di eventi in Workfront
description: In qualità di amministratore di Adobe Workfront, puoi creare, visualizzare ed eliminare sottoscrizioni di eventi dall’area Configurazione per inviare eventi Workfront a un endpoint esterno.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 9%
---

# Configurare le sottoscrizioni di eventi in Workfront

{{highlighted-preview-article-level}}

In qualità di amministratore di Adobe Workfront, puoi creare, visualizzare ed eliminare sottoscrizioni di eventi dall’area Configurazione. Le sottoscrizioni di eventi inviano informazioni sull’evento Workfront a un endpoint esterno quando si verificano eventi specifici.

Puoi creare ed eliminare sottoscrizioni di eventi in Workfront, ma non puoi modificare una sottoscrizione esistente. Se devi modificare un abbonamento, eliminalo e creane uno nuovo.

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
   <td>Devi essere un amministratore di Workfront.</td>
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
