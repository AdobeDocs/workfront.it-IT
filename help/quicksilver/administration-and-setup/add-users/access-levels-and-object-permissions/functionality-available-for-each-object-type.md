---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accesso, modello, funnel, diagramma, livelli, autorizzazioni
navigation-topic: access-levels
title: Funzionalità disponibile per ogni tipo di oggetto per vari livelli di accesso
description: Nella tabella seguente sono elencate le funzionalità disponibili per ogni tipo di oggetto nei vari livelli di accesso.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 11%

---

# Funzionalità disponibile per ogni tipo di oggetto per vari livelli di accesso

Nella tabella seguente sono elencate le funzionalità disponibili per ogni tipo di oggetto nei vari livelli di accesso.

Indica inoltre quali azioni possono essere disabilitate o abilitate dagli amministratori di Workfront utilizzando un livello di accesso.

## Progetti

Solo gli utenti con una licenza Plan possono avere accesso completo ai progetti.

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; |   |   |   |   |
| Copia | ✓&#42; |   |   |   |   |
| Elimina | ✓&#42; |   |   |   |   |
| Condividi | ✓&#42; | ✓&#42; |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Aggiungere un modulo personalizzato | ✓ |   |   |   |   |
| Aggiorna campi personalizzati | ✓ | ✓ |   |   |   |
| Aggiungi un processo di approvazione | ✓ |   |   |   |   |
| Approvare un progetto | ✓ | ✓ | ✓ |   |   |
| Aggiungi documento | ✓ | ✓ | ✓ |   |   |
| Aggiungi problema | ✓ | ✓ |   |   |   |
| Aggiungi  attività | ✓ | ✓ |   |   |   |
| Aggiornamenti/commenti | ✓ | ✓ | ✓ |   |   |
| Cambia stato | ✓ |   |   |   |   |
| Ore di log | ✓ | ✓ |   |   |   |
| Modifica assegnazioni | ✓ | ✓ |   |   |   |
| Gestire una baseline | ✓ |   |   |   |   |
| Gestire i rischi | ✓ |   |   |   |   |
| Gestire i finanziamenti | ✓ |   |   |   |   |
| Aggiungi/modifica spese | ✓ | ✓ |   |   |   |
| Allega modelli | ✓ |   |   |   |   |
| Salva come modello | ✓ |   |   |   |   |
| Aggiungi/modifica un caso aziendale | ✓ |   |   |   |   |
| Modificare i dettagli del progetto | ✓ |   |   |   |   |
| Modifica del personale | ✓ |   |   |   |   |
| Esporta in MS Project | ✓ | ✓ | ✓ |   |   |
| Ricalcola finanza/timeline | ✓ |   |   |   |   |
| Impostare le proprietà della coda | ✓ |   |   |   |   |



&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Attività

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; | ✓&#42; |   |   |   |
| Elimina | ✓&#42; | ✓&#42; |   |   |   |
| Condividi | ✓&#42; | ✓&#42; |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Aggiungi predecessori | ✓ | ✓ |   |   |   |
| Aggiungi  problemi | ✓ | ✓ |   |   |   |
| Modificare un’attività (escluso lo stato) | ✓ | ✓ |   |   |   |
| Modifica stato attività | ✓ | ✓ |   |   |   |
| Aggiungi documenti | ✓ | ✓ | ✓ |   |   |
| Copiare un’attività | ✓ | ✓ |   |   |   |
| Spostare un’attività | ✓ | ✓ |   |   |   |
| Ore di log | ✓ | ✓ |   |   |   |
| Accettare un&#39;assegnazione | ✓ | ✓ |   |   |   |
| Creare un&#39;assegnazione | ✓ | ✓ | Solo modifica in linea | Solo modifica in linea |   |
| Allegare un modulo personalizzato | ✓ | ✓ |   |   |   |
| Modificare campi personalizzati | ✓ | ✓ |   |   |   |
| Creazione di un processo di approvazione | ✓ | ✓ |   |   |   |
| Approvare un’attività | ✓ | ✓ | ✓ |   |   |
| Modifica delle finanze | ✓ |   |   |   |   |
| Aggiungi/modifica spese | ✓ | ✓ |   |   |   |
| Visualizza finanza | ✓ | ✓ | ✓ |   |   |
| Aggiornamenti/commenti | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemi

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Modifica | ✓ | ✓ | ✓ | ✓ |   |
| Elimina | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Condividi | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Allegare moduli personalizzati | ✓ | ✓ | ✓ | ✓ |   |
| Modificare campi personalizzati | ✓ | ✓ | ✓ | ✓ |   |
| Approvare i problemi | ✓ | ✓ | ✓ | ✓ |   |
| Aggiungi un processo di approvazione | ✓ | ✓ | ✓ | ✓ |   |
| Aggiungi documenti | ✓ | ✓ | ✓ | ✓ |   |
| Copia i problemi | ✓ | ✓ | ✓ | ✓ |   |
| Sposta i problemi | ✓ | ✓ | ✓ | ✓ |   |
| Ore di log | ✓ | ✓ |   |   |   |
| Convertire un problema in un progetto | ✓ | ✓ |   |   |   |
| Convertire un problema in un&#39;attività | ✓ |   |   |   |   |
| Accetta assegnazioni | ✓ | ✓ |   |   |   |
| Assegna assegnazioni | ✓ | ✓ |   |   |   |
| Aggiungere aggiornamenti e commenti | ✓ | ✓ | ✓ | ✓ |   |



&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfolio

Solo gli utenti con una licenza Plan possono avere accesso completo ai portfolio.

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; |   |   |   |   |
| Elimina | ✓&#42; |   |   |   |   |
| Condividi | ✓&#42; |   |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Modifica dettagli | ✓ |   |   |   |   |
| Allegare moduli personalizzati | ✓ |   |   |   |   |
| Modificare campi personalizzati | ✓ |   |   |   |   |
| Aggiungere e rimuovere progetti | ✓ |   |   |   |   |
| Approvare progetti | ✓ |   |   |   |   |
| Ottimizzazione del Portfolio | ✓ |   |   |   |   |
| Aggiungi documenti | ✓ | ✓ | ✓ |   |   |
| Aggiungere aggiornamenti e commenti | ✓ | ✓ | ✓ |   |   |



&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programmi

Solo gli utenti con una licenza Plan possono avere accesso completo ai programmi.

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; |   |   |   |   |
| Elimina | ✓&#42; |   |   |   |   |
| Condividi | ✓&#42; |   |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Modifica dettagli | ✓ |   |   |   |   |
| Allegare moduli personalizzati | ✓ |   |   |   |   |
| Modificare campi personalizzati | ✓ |   |   |   |   |
| Aggiungere e rimuovere progetti | ✓ |   |   |   |   |
| Approvare progetti | ✓ |   |   |   |   |
| Ottimizzazione Portfolio | ✓ |   |   |   |   |
| Aggiungi documenti | ✓ | ✓ | ✓ |   |   |
| Aggiungi aggiornamenti e commenti | ✓ | ✓ | ✓ |   |   |



&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Report, dashboard e calendari

Gli utenti con una licenza Plan possono avere accesso completo ai report. Tutti gli altri livelli di accesso hanno accesso a Visualizza rapporti.

| Azione | Pianificatore | Collaboratore | Revisore | Richiesta | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; |   |   |   |   |
| Elimina | ✓&#42; |   |   |   |   |
| Visualizzare i rapporti incorporati | ✓&#42; |   |   |   |   |
| Condividi | ✓&#42; | ✓ | ✓ |   |   |
| Condividere calendari e rapporti pubblicamente | ✓&#42; |   |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Modifica | ✓ |   |   |   |   |
| Copia | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>I richiedenti possono visualizzare solo i rapporti condivisi con loro

## Filtri, visualizzazioni e raggruppamenti

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Azione</p> </th> 
   <th> <p>Pianificatore</p> </th> 
   <th> <p>Collaboratore</p> </th> 
   <th> <p>Revisore</p> </th> 
   <th> <p>Richiedente</p> </th> 
   <th>Utente esterno<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crea</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Condividi</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Condividi a livello di sistema</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documenti

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Elimina (documenti e cartelle) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Condividi | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Condividi pubblicamente (esternamente) | ✓&#42; |   |   |   |   |
| Condividi a livello di sistema | ✓&#42; | ✓&#42; |   |   |   |
| Visualizza | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Modifica dettagli | ✓ | ✓ | ✓ | ✓ |   |
| Scaricare | ✓ | ✓ | ✓ | ✓ | ✓ |
| Pagamento | ✓ | ✓ | ✓ | ✓ |   |
| Aggiungi approvatori | ✓ | ✓ | ✓ | ✓ |   |
| Approvare documenti | ✓ | ✓ | ✓ | ✓ | ✓ |
| Allegare moduli personalizzati | ✓ | ✓ | ✓ | ✓ |   |
| Modificare campi personalizzati | ✓ | ✓ | ✓ | ✓ |   |
| Sposta a (oggetto) | ✓ | ✓ | ✓ | ✓ |   |
| Invia a (integrazione) | ✓ | ✓ | ✓ | ✓ |   |
| Aggiungere aggiornamenti e commenti | ✓ | ✓ | ✓ | ✓ |   |
| Carica nuova versione | ✓ | ✓ | ✓ | ✓ |   |
| Eliminare una versione | ✓ | ✓ | ✓ | ✓ |   |
| Anteprima | ✓ | ✓ | ✓ | ✓ | ✓ |
|  Bozza | ✓ | ✓ | ✓ | ✓ |   |
| Genera bozza | ✓ | ✓ |   |   |   |
| Rimuovi bozza | ✓ | ✓ | ✓ | ✓ |   |
| Aggiungi/Rimuovi&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Rinomina&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Collegamento (con integrazione) | ✓ | ✓ | ✓ | ✓ |   |
| Scollega (con integrazione) | ✓ | ✓ | ✓ | ✓ |   |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponibile solo per cartelle di documenti, non per documenti

## Utenti

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Azione</p> </th> 
   <th> <p>Pianificatore</p> </th> 
   <th>Collaboratore</th> 
   <th> <p>Revisore</p> </th> 
   <th> <p>Richiedente</p> </th> 
   <th> <p>Utente esterno**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crea</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica, elimina, disattiva, accedi come o reimposta la password per qualsiasi utente</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica, elimina, disattiva, accedi come o reimposta la password per qualsiasi utente di un gruppo che amministra</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizzare gli utenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza informazioni di contatto</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Gli utenti esterni possono cercare solo altri utenti

## Team

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Azione</p> </th> 
   <th> <p>Pianificatore</p> </th> 
   <th>Collaboratore</th> 
   <th> <p>Revisore</p> </th> 
   <th> <p>Richiedente</p> </th> 
   <th> <p>Utente esterno*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crea</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modificare i team su cui sono attivi</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modificare i team in gruppi gestiti</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza tutti i team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizzare i team associati ai relativi gruppi</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Modelli

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Crea | ✓&#42; |   |   |   |   |
| Elimina | ✓&#42; |   |   |   |   |
| Condividi | ✓&#42; |   |   |   |   |
| Condividi a livello di sistema | ✓&#42; |   |   |   |   |
| Visualizza | ✓&#42; |   |   |   |   |
| Copia | ✓ |   |   |   |   |
| Modificare i dettagli del modello | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dati finanziari

Solo gli utenti con una licenza Plan possono avere accesso completo ai dati finanziari.

I tipi di licenza Request ed External User non sono inclusi qui perché non hanno accesso a [selezionare un oggetto o un&#39;area].

| Azione | Pianificatore | Collaboratore | Revisore |
|---|---|---|---|
| Modificare la fatturazione dei ruoli e le tariffe dei costi | ✓&#42; |   |   |
| Modificare la fatturazione e le tariffe degli utenti | ✓&#42; |   |   |
| Visualizza la fatturazione dei ruoli e le tariffe dei costi | ✓&#42; |   |   |
| Visualizza la fatturazione e i tassi di costo degli utenti | ✓&#42; |   |   |
| Gestire i record di fatturazione | ✓ |   |   |
| Gestione delle spese | ✓ | ✓ |   |
| Visualizza dati finanziari | ✓&#42; | ✓&#42; | ✓&#42; |
| Visualizzare le informazioni in base al costo negli strumenti di pianificazione delle risorse | ✓ |   |   |
| Risorse di budget negli strumenti di pianificazione delle risorse&#42;&#42; | ✓ |   |   |
| Visualizzare l&#39;allocazione delle risorse negli strumenti di pianificazione delle risorse&#42; | ✓ | ✓ | ✓ |
| Creare rischi sui progetti | ✓ |   |   |
| Visualizza i rischi relativi ai progetti | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Richiede un accesso aggiuntivo a Gestione risorse.

## Gestione risorse

Solo gli utenti con una licenza Plan possono avere accesso completo a [selezionare un oggetto o un&#39;area]. Altri tipi di licenza possono avere accesso limitato o nullo a Gestione risorse in Workfront.

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Modifica priorità e ore preventivate nella Programmazione | ✓&#42; |   |   |   |   |
| Creare, modificare, eliminare i pool di risorse&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| Visualizzare le priorità del progetto nel planner risorse | ✓&#42; |   |   |   |   |
| Visualizzare l&#39;allocazione delle risorse negli strumenti di pianificazione delle risorse | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Visualizza pool di risorse | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Risorse di budget negli strumenti di pianificazione delle risorse&#42;&#42; | ✓ |   |   |   |   |
| Allega pool di risorse a progetti, modelli e utenti | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Utilizzando un livello di accesso, gli amministratori di Workfront possono disabilitare o abilitare questa funzionalità. Per ulteriori informazioni, consulta [Accesso configurabile alla funzionalità per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Richiede un accesso aggiuntivo ai dati finanziari e autorizzazioni per le finanze del progetto. Se si concede l&#39;accesso a Gestione risorse a un utente Planner che non ha accesso ai dati finanziari, l&#39;utente può comunque visualizzare le allocazioni orarie nel Planner risorse, ma non può passare alla visualizzazione Costi o visualizzare il Business Case. Per ulteriori informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Condividere le autorizzazioni finanziarie su un oggetto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Richiede l&#39;autorizzazione per Contribute all&#39;oggetto, con l&#39;opzione Make Assignments abilitata in Impostazioni avanzate. Per informazioni, consulta la sezione . [Comprendere le autorizzazioni ereditate e la gerarchia degli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) nell&#39;articolo [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Area planner dello scenario

| Azione | Pianificatore | Collaboratore | Revisore | Richiedente | Utente esterno |
|---|---|---|---|---|---|
| Creare/modificare piani e iniziative esistenti | ✓ | ✓ | ✓ |   |   |
| Aggiungere o modificare le informazioni sul ruolo del lavoro in piani e iniziative&#42; | ✓ | ✓ | ✓ |   |   |
| Aggiungere o modificare informazioni sui costi relativi a piani e iniziative&#42; | ✓ | ✓ | ✓ |   |   |
| Elimina piani e iniziative | ✓ | ✓ | ✓ |   |   |
| Visualizza scenari nel menu principale ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ |  |   |
| Visualizza piani e iniziative creati dall&#39;utente&#42; | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>Gli utenti possono visualizzare un piano creato da un altro utente solo se con esso è condiviso un collegamento al piano.

&#42; Affinché gli utenti possano visualizzare i dati finanziari in un piano o in un&#39;iniziativa, devono avere accesso ai dati finanziari. Per ulteriori informazioni, consulta [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Area Obiettivi di Workfront

| Azioni | Viste | Modif |
|---|---|---|
| Crea |   | ✓ |
| Modificare/eliminare tutti gli obiettivi |   | ✓ |
| Visualizza obiettivi nel menu principale | ✓ | ✓ |
| Visualizzare l&#39;area Obiettivi da un collegamento condiviso | ✓ | ✓ |
| Visualizza tutti gli obiettivi del sistema | ✓ | ✓ |
| Attivare/disattivare/chiudere tutti gli obiettivi |   | ✓ |
| Creare/modificare/eliminare attività |   | ✓ |
| Creare/modificare/eliminare risultati |   | ✓ |
| Aggiungi un obiettivo allineato |   | ✓ |
| Aggiornare l’avanzamento di un risultato o di un’attività |   | ✓ |
| Possedere un obiettivo, un risultato o un’attività | ✓ | ✓ |
| Commento su un obiettivo | ✓ | ✓ |
| Copia obiettivi |   | ✓ |
| Visualizza la sezione Elenco obiettivi nel pannello a sinistra | ✓ | ✓ |
| Visualizza la sezione Grafici nel pannello a sinistra | ✓ | ✓ |
| Visualizza la sezione Allineamento obiettivo nel pannello a sinistra | ✓ | ✓ |

