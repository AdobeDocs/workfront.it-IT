---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Tipi di ruolo di licenza Adobe Workfront e tipi di ruolo DAM Adobe Workfront
description: Gli amministratori di Adobe Workfront utilizzano i livelli di accesso per determinare cosa possono fare gli utenti in un'applicazione.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Tipi di ruolo di licenza Adobe Workfront e tipi di ruolo DAM Adobe Workfront

Gli amministratori di Adobe Workfront utilizzano i livelli di accesso per determinare cosa possono fare gli utenti in un&#39;applicazione.

* In Workfront, la licenza determina il livello di accesso di un utente.
* In Workfront DAM, i tipi di ruolo definiscono l’accesso degli utenti alle risorse nel DAM.

Poiché i tipi di licenza e i tipi di ruolo non sono intercambiabili, avere un livello di accesso in un&#39;applicazione non implica l&#39;accesso nell&#39;altra applicazione. Ad esempio, a un utente con una licenza Work in Workfront non viene assegnato automaticamente un ruolo Collaboratore in Workfront DAM.

## Tipi di licenze Workfront

In qualità di amministratore di Workfront, puoi definire il livello di accesso di cui dispongono gli utenti assegnando tipi di licenza. Ogni licenza viene fornita con una serie di funzioni di accesso predefinite che è possibile modificare prima di assegnare la licenza all&#39;utente. 

È possibile utilizzare le licenze per determinare le operazioni che un utente può visualizzare e eseguire in Workfront. In Workfront sono disponibili cinque tipi di licenze:

* Piano
* Lavoro
* Revisiona
* Richiesta
* Esterno

Vedi [Panoramica sulle licenze legacy](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) per una descrizione dei diversi tipi di licenza in Workfront.

## Tipi di ruoli DAM Workfront

In qualità di amministratore di Workfront DAM Workfront, assegni i tipi di ruolo agli utenti per definire l’accesso a cui hanno accesso alle risorse. Inoltre, i tipi di ruolo specificano le aree del DAM in cui gli utenti possono lavorare.

I tipi di ruolo funzionano insieme ai gruppi quando si stabiliscono i diritti di accesso dell’utente. I gruppi controllano l’accesso che gli utenti devono avere alle cartelle e alle risorse stesse. I tipi di ruolo determinano le azioni che gli utenti possono eseguire con le risorse. Tutti gli utenti DAM devono essere associati ad almeno un gruppo. Per ulteriori informazioni sui tipi di ruolo e sulla configurazione dell’accesso, consulta la Guida in linea in Workfront DAM.

In Workfront DAM sono disponibili quattro tipi di ruolo distinti:

### Brand Portal

Gli utenti con questo tipo di ruolo hanno accesso solo al portale Brand Connect nel DAM. All’interno del portale, gli utenti possono visualizzare e scaricare le risorse per le quali dispongono delle autorizzazioni.

Gli utenti di Brand Portal possono collaborare con altri creando e condividendo lightbox.

### Utente regolare

Gli utenti con questo tipo di ruolo possono visualizzare e scaricare risorse da Workfront DAM e dal portale Brand Connect.

Gli utenti regolari possono anche collaborare con altri creando e condividendo lightbox.

### Collaboratore

Gli utenti con questo tipo di ruolo possono accedere a Workfront DAM e al portale Brand Connect.

I collaboratori possono visualizzare, scaricare, caricare, modificare, spostare ed eliminare le risorse e le cartelle a cui hanno accesso. Inoltre, i collaboratori possono collaborare con altri creando e condividendo lightbox. 

### Amministratore

Gli amministratori di Workfront possono accedere a tutto ciò che si trova nel portale di Brand Connect e in Workfront DAM, incluse le risorse scadute o con uno stato inattivo.

Per poter accedere come amministratore, gli utenti con il tipo di ruolo Amministratore devono trovarsi nel gruppo Amministratore.
