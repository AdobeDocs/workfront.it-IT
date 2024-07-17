---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Tipi di ruolo licenze Adobe Workfront e tipi di ruolo DAM Adobe Workfront
description: Gli amministratori di Adobe Workfront utilizzano i livelli di accesso per determinare cosa possono fare gli utenti in un’applicazione.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Tipi di ruolo licenze Adobe Workfront e tipi di ruolo DAM Adobe Workfront

Gli amministratori di Adobe Workfront utilizzano i livelli di accesso per determinare cosa possono fare gli utenti in un’applicazione.

* In Workfront, la gestione delle licenze determina il livello di accesso di un utente.
* In Workfront DAM, i tipi di ruolo definiscono l’accesso degli utenti alle risorse in DAM.

Poiché i tipi di licenza e i tipi di ruolo non sono intercambiabili, un livello di accesso in un&#39;applicazione non implica l&#39;accesso nell&#39;altra applicazione. Ad esempio, a un utente con una licenza Lavoro in Workfront non viene assegnato automaticamente un ruolo Collaboratore in Workfront DAM.

## Tipi di licenze Workfront

In qualità di amministratore di Workfront, puoi definire il livello di accesso di cui dispongono gli utenti assegnando tipi di licenza. Ogni licenza include un set di funzioni di accesso predefinite che è possibile modificare prima di assegnarla all’utente. 

Le licenze vengono utilizzate per determinare cosa un utente può vedere e fare in Workfront. In Workfront sono disponibili cinque tipi di licenze:

* Piano
* Lavoro
* Revisiona
* Richiesta
* Esterno

Per una descrizione dei diversi tipi di licenza in Workfront, consulta [Panoramica licenze legacy](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

## Tipi di ruolo Workfront DAM

In qualità di amministratore di Workfront DAM Workfront, assegni agli utenti i tipi di ruolo per definire l’accesso di cui dispongono alle risorse. Inoltre, i tipi di ruolo specificano le aree in DAM in cui gli utenti possono lavorare.

I tipi di ruolo collaborano con i gruppi quando si stabiliscono i diritti di accesso degli utenti. I gruppi controllano l’accesso degli utenti alle cartelle e alle risorse stesse. I tipi di ruolo determinano le azioni che gli utenti possono intraprendere con le risorse. Tutti gli utenti DAM devono essere associati ad almeno un gruppo. Per ulteriori informazioni sui tipi di ruolo e sulla configurazione degli accessi, consulta la Guida di Workfront DAM.

In Workfront DAM sono disponibili quattro tipi di ruolo distinti:

### Brand Portal

Gli utenti con questo tipo di ruolo possono accedere solo al portale Brand Connect in DAM. All’interno del portale, gli utenti possono visualizzare e scaricare le risorse per le quali dispongono delle autorizzazioni.

Gli utenti di Brand Portal possono collaborare con altri creando e condividendo lightbox.

### Utente normale

Gli utenti con questo tipo di ruolo possono visualizzare e scaricare le risorse da Workfront DAM e dal portale Brand Connect.

Gli utenti normali possono anche collaborare con altri creando e condividendo lightbox.

### Collaboratore

Gli utenti con questo tipo di ruolo possono accedere a Workfront DAM e al portale Brand Connect.

I collaboratori possono visualizzare, scaricare, caricare, modificare, spostare ed eliminare risorse e cartelle a cui hanno accesso. I collaboratori possono inoltre collaborare con altri utenti creando e condividendo lightbox. 

### Amministratore

Gli amministratori di Workfront hanno accesso a tutto ciò che si trova nel portale Brand Connect e in Workfront DAM, comprese le risorse scadute o con stato inattivo.

Per poter accedere come amministratore, gli utenti con il tipo di ruolo Amministratore devono appartenere al gruppo Amministratore.
