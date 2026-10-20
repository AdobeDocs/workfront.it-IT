---
content-type: api
navigation-topic: general-api
title: Gestire le sottoscrizioni di eventi come utente non amministratore
description: Se l'accesso a Workfront lo consente, è possibile creare, visualizzare ed eliminare sottoscrizioni di eventi che rientrano nell'ambito consentito dalle autorizzazioni e dalla configurazione del sistema.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# Gestire le sottoscrizioni di eventi come utente non amministratore

Se l’accesso a Workfront lo consente, puoi creare, visualizzare ed eliminare gli abbonamenti agli eventi dall’area Configurazione. Tuttavia, il tuo accesso è limitato agli abbonamenti e alle azioni autorizzati per il tuo ruolo e dalla configurazione del sistema della tua organizzazione.

Questa funzione non è disponibile per tutti gli utenti allo stesso modo degli amministratori di Workfront. Gli utenti con l’accesso richiesto possono gestire le sottoscrizioni di eventi solo all’interno dell’ambito loro concesso.

Ad esempio, le autorizzazioni possono consentire di gestire solo determinati tipi di oggetti, tipi di eventi o sottoscrizioni per un insieme di lavoro definito. Non puoi gestire le sottoscrizioni di eventi al di fuori dell&#39;ambito consentito dal tuo accesso e dalla tua configurazione.

Per l&#39;installazione gestita dall&#39;amministratore, vedere [Configurare sottoscrizioni di eventi in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

Per informazioni sull&#39;API sottoscrizioni eventi, vedere [API sottoscrizioni eventi](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Gli utenti possono gestire le sottoscrizioni di eventi solo entro l’ambito consentito dalle loro autorizzazioni e dalla configurazione di sistema dell’organizzazione. L&#39;accesso non equivale automaticamente all&#39;accesso amministratore.

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
    <p>Il tuo accesso è limitato agli abbonamenti e alle azioni consentiti dalle tue autorizzazioni e dalla configurazione del sistema della tua organizzazione.</p>
   </td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizzare gli abbonamenti agli eventi

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **Sistema**, quindi su **Sottoscrizioni eventi**.
1. Controlla gli abbonamenti disponibili.
1. Crea, visualizza o elimina solo gli abbonamenti che rientrano nell’ambito autorizzato.

Se non sono visualizzate le opzioni previste o se non è possibile creare o gestire un abbonamento, contattare l&#39;amministratore di Workfront per verificare se l&#39;accesso è limitato da ruoli, autorizzazioni o configurazione di sistema.

## Articoli correlati

* [Configurare le sottoscrizioni di eventi in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [API sottoscrizione a eventi](/help/quicksilver/wf-api/general/event-subs-api.md)
