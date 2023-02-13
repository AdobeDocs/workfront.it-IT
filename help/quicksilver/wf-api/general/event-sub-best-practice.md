---
content-type: api
navigation-topic: general-api
title: Best practice per l’abbonamento agli eventi
description: Best practice per l’abbonamento agli eventi
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Best practice per l’abbonamento agli eventi

I messaggi di abbonamento agli eventi di Adobe Workfront vengono inviati automaticamente da Workfront dopo che il servizio è stato configurato correttamente e hai creato un abbonamento agli eventi per attivare tali consegne. Per ulteriori informazioni sulla configurazione corretta degli abbonamenti agli eventi, consulta [Requisiti di consegna abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).


Di seguito sono elencate alcune best practice per aiutarti a creare efficacemente sottoscrizioni di eventi.

## Fornisci tutti i campi corpo della richiesta richiesti

Assicurati che tutti i campi del corpo della richiesta richiesti siano forniti all&#39;API. Per informazioni su tutti gli attributi di richiesta richiesti, consulta [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md).

## Evitare di includere campi corpo extra

Non includere ulteriori campi corpo nella richiesta, in quanto ciò causerà l’errore dell’API di creare una sottoscrizione.

## Test completi entro il periodo di tolleranza

Prova a fare tutti i test di abbonamento entro il periodo di tolleranza di 100 messaggi. Per ulteriori informazioni su questo periodo di tolleranza, consulta [Domande frequenti - Abbonamenti agli eventi](../../wf-api/general/event-subs-faq.md).

## Soddisfare i requisiti standard di consegna dei messaggi di abbonamento agli eventi

Assicurati che l’endpoint di sottoscrizione sia conforme ai requisiti standard di consegna dei messaggi di abbonamento agli eventi. Per informazioni su questi requisiti, consulta [Requisiti di consegna abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Inserire nell&#39;elenco Consentiti indirizzi IP per area globale

Per ricevere payload di sottoscrizioni di eventi tramite il firewall, è necessario aggiungere gli indirizzi IP al inserire nell&#39;elenco Consentiti in base all’area geografica globale. Per ulteriori informazioni, consulta [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md).

## Avere il giusto livello di accesso e una chiave API

Per creare, eseguire query o eliminare una sottoscrizione a un evento, l’utente Workfront deve:

* Livello di accesso **Amministratore di sistema**
Per ulteriori informazioni, consulta [Concedere a un utente pieno accesso amministrativo](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Una chiave API

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
