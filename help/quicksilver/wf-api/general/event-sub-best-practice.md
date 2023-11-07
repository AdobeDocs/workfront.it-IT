---
content-type: api
navigation-topic: general-api
title: Best practice per l’abbonamento agli eventi
description: Best practice per l’abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Best practice per l’abbonamento agli eventi

I messaggi di abbonamento agli eventi di Adobe Workfront vengono inviati automaticamente da Workfront dopo che hai configurato correttamente il servizio e creato un abbonamento agli eventi per attivare le consegne dei messaggi. Per ulteriori informazioni sulla corretta configurazione delle sottoscrizioni agli eventi, consulta [Requisiti di consegna dell’abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).


Di seguito sono elencate alcune best practice per creare in modo efficace gli abbonamenti agli eventi.

## Fornisci tutti i campi obbligatori del corpo della richiesta

Assicurati che tutti i campi obbligatori del corpo della richiesta siano forniti all’API. Per informazioni su tutti gli attributi di richiesta richiesti, consulta [API di abbonamento agli eventi](../../wf-api/general/event-subs-api.md).

## Evita di includere campi corpo aggiuntivi

Non includere campi corpo aggiuntivi nella richiesta, in quanto l’API non sarà in grado di creare una sottoscrizione.

## Completa il test entro il periodo di tolleranza

Prova a eseguire tutti i test di abbonamento entro il periodo di tolleranza di 100 messaggi. Per ulteriori informazioni su questo periodo di tolleranza, consulta [Domande frequenti - Abbonamenti agli eventi](../../wf-api/general/event-subs-faq.md).

## Soddisfa i requisiti standard per la consegna dei messaggi di abbonamento agli eventi

Assicurati che l’endpoint di abbonamento sia conforme ai requisiti di consegna dei messaggi di abbonamento agli eventi standard. Per informazioni su questi requisiti, consulta [Requisiti di consegna dell’abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).

## Inserire nell&#39;elenco Consentiti indirizzi IP per area geografica globale

Inserire nell&#39;elenco Consentiti Per ricevere i payload degli abbonamenti agli eventi tramite il firewall, è necessario aggiungere gli indirizzi IP all’di riferimento per area globale. Per ulteriori informazioni, consulta [API di abbonamento agli eventi](../../wf-api/general/event-subs-api.md).

## Avere il giusto livello di accesso e una chiave API

Per creare, eseguire query o eliminare un abbonamento a un evento, è necessario che l’utente di Workfront:

* Un livello di accesso di **Amministratore di sistema**
Per ulteriori informazioni, consulta [Concedere a un utente l&#39;accesso amministrativo completo](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Una chiave API

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
