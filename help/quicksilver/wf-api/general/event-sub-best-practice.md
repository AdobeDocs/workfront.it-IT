---
content-type: api
navigation-topic: general-api
title: Best practice per l’abbonamento agli eventi
description: Best practice per l’abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 699ce13472ee70149fba7c8c34dde83c7db5f5de
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Best practice per l’abbonamento agli eventi

I messaggi di abbonamento agli eventi di Adobe Workfront vengono inviati automaticamente da Workfront dopo che hai configurato correttamente il servizio e creato un abbonamento agli eventi per attivare le consegne dei messaggi. Per ulteriori informazioni sulla corretta configurazione delle sottoscrizioni eventi, vedere [Requisiti di consegna delle sottoscrizioni eventi](../../wf-api/general/setup-event-sub-endpoint.md).


Di seguito sono elencate alcune best practice per creare in modo efficace gli abbonamenti agli eventi.

## Fornisci tutti i campi obbligatori del corpo della richiesta

Assicurati che tutti i campi obbligatori del corpo della richiesta siano forniti all’API. Per informazioni su tutti gli attributi di richiesta richiesti, vedere [API sottoscrizione evento](../../wf-api/general/event-subs-api.md).

## Evita di includere campi corpo aggiuntivi

Non includere campi corpo aggiuntivi nella richiesta, in quanto l’API non sarà in grado di creare una sottoscrizione.

## Evita di sovraccaricare le sottoscrizioni di eventi

Il servizio di abbonamento agli eventi è progettato per fornire una consegna affidabile di eventi per tutti gli utenti. A tal fine, sono state introdotte misure di salvaguardia per impedire la produzione di eventi eccessivi da parte di un singolo utente, che potrebbero causare potenziali problemi di qualità del servizio per tutti gli utenti. Di conseguenza, un utente che produce troppi eventi a una velocità elevata in un breve arco di tempo può riscontrare ritardi nella sandboxing e nella consegna degli eventi.

## Completa il test entro il periodo di tolleranza

Prova a eseguire tutti i test di abbonamento entro il periodo di tolleranza di 100 messaggi. Per ulteriori informazioni su questo periodo di tolleranza, consulta [Domande frequenti - Sottoscrizioni eventi](../../wf-api/general/event-subs-faq.md).

## Soddisfa i requisiti standard per la consegna dei messaggi di abbonamento agli eventi

Assicurati che l’endpoint di abbonamento sia conforme ai requisiti di consegna dei messaggi di abbonamento agli eventi standard. Per informazioni su questi requisiti, consulta [Requisiti di consegna per abbonamento eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Inserire nell&#39;elenco Consentiti indirizzi IP per area geografica globale

Per ricevere i payload degli abbonamenti agli eventi tramite il firewall, è necessario aggiungere gli indirizzi IP al, inseriti nell&#39;elenco Consentiti per area globale. Per ulteriori informazioni, vedere [API sottoscrizione eventi](../../wf-api/general/event-subs-api.md).

## Avere il giusto livello di accesso e autenticazione

Per creare, eseguire query o eliminare un abbonamento a un evento, è necessario che l’utente di Workfront:

* Livello di accesso di **Amministratore di sistema**
Per ulteriori informazioni, vedere [Concedere a un utente l&#39;accesso amministrativo completo](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* È necessaria un&#39;intestazione `sessionID` per utilizzare l&#39;API sottoscrizioni eventi

  Per ulteriori informazioni, vedere [Autenticazione](api-basics.md#authentication) in [Nozioni di base sulle API](api-basics.md).
