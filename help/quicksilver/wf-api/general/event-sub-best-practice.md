---
content-type: api
navigation-topic: general-api
title: Best practice per la sottoscrizione a eventi
description: Best practice per la sottoscrizione a eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
TQID: https://experienceleague.adobe.com/uT7erlnJR5-h-KKGQiuztzZKBtwtEvWQ8U-EUgN4TG4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 23%

---

# Best practice per la sottoscrizione a eventi

I messaggi di abbonamento agli eventi di Adobe Workfront vengono inviati automaticamente da Workfront dopo che hai configurato correttamente il servizio e creato un abbonamento agli eventi per attivare le consegne dei messaggi. Per ulteriori informazioni sulla corretta configurazione delle sottoscrizioni eventi, vedere [Requisiti di consegna delle sottoscrizioni eventi](../../wf-api/general/setup-event-sub-endpoint.md).


Di seguito sono elencate alcune best practice per creare in modo efficace gli abbonamenti agli eventi.

## Fornisci tutti i campi obbligatori del corpo della richiesta

Assicurati che tutti i campi obbligatori del corpo della richiesta siano forniti all’API. Per informazioni su tutti gli attributi di richiesta richiesti, vedere [API sottoscrizione evento](../../wf-api/general/event-subs-api.md).

## Evita di includere campi corpo aggiuntivi

Non includere campi corpo aggiuntivi nella richiesta, in quanto l’API non sarà in grado di creare una sottoscrizione.

## Evitare il sovraccarico delle sottoscrizioni a eventi

Il servizio di sottoscrizione a eventi è progettato per fornire una consegna affidabile di eventi a tutti gli utenti. A tal fine, sono state introdotte misure di protezione per impedire la produzione eccessiva di eventi da parte di un singolo utente, che potrebbero causare potenziali problemi di qualità del servizio per tutti gli altri. Di conseguenza, un utente che produce troppi eventi con frequenza elevata in un breve arco temporale può essere soggetto a sandboxing e a ritardi nella consegna degli eventi.

## Completa il test entro il periodo di tolleranza

Prova a eseguire tutti i test di abbonamento entro il periodo di tolleranza di 100 messaggi. Per ulteriori informazioni su questo periodo di tolleranza, consulta [Domande frequenti - Sottoscrizioni eventi](../../wf-api/general/event-subs-faq.md).

## Soddisfa i requisiti standard per la consegna dei messaggi di abbonamento agli eventi

Assicurati che l’endpoint di abbonamento sia conforme ai requisiti di consegna dei messaggi di abbonamento agli eventi standard. Per informazioni su questi requisiti, consulta [Requisiti di consegna per abbonamento eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Inserire nell&#39;elenco Consentiti indirizzi IP per area geografica globale

Per ricevere i payload degli abbonamenti agli eventi tramite il firewall, è necessario aggiungere gli indirizzi IP all’di riferimento per area globale. Per ulteriori informazioni, vedere [API sottoscrizione eventi](../../wf-api/general/event-subs-api.md).

## Avere il giusto livello di accesso e autenticazione

Per creare, eseguire query o eliminare un abbonamento a un evento, è necessario che l’utente di Workfront:

* Livello di accesso di **Amministratore di sistema**
Per ulteriori informazioni, vedere [Concedere a un utente l&#39;accesso amministrativo completo](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Se la tua organizzazione utilizza Adobe IMS (Identity Management System), includi un token utente IMS passato nell&#39;intestazione `X-User-Token`.
