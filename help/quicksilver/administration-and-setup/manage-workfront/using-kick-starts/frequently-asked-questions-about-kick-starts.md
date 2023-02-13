---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart, calcio d'inizio, kickstart, calcio d'inizio
navigation-topic: use-kick-starts
title: Domande frequenti su Kick-Starts
description: Trova le risposte alle domande più frequenti sull’importazione e l’esportazione di dati Workfront tramite Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Domande frequenti su Kick-Starts

Di seguito sono riportate le domande frequenti su Kick-Starts:

## Perché ricevo questo errore quando si tenta di importare un file Kick-Start: &quot;Il tuo file era corretto, ma non è stato importato nulla?&quot;

### Risposta

Nel file Kick-Start potrebbe mancare uno dei tre elementi seguenti:

1. La **isNew** deve essere impostato su **TRUE** per tutti gli elementi da importare. **isNew** devono **TRUE** perché è possibile importare solo i nuovi dati con un Kick-Start. Non è possibile modificare i dati esistenti tramite Kick-Start. Puoi avere altre righe nel foglio di calcolo con **isNew = FALSE** ma queste righe non verranno importate.

1. &#x200B; Il file deve avere una riga vuota prima che le intestazioni dei dati inizino.
1. &#x200B; I fogli Excel devono avere i nomi corretti.

Quando si lavora con Kick-Starts, è consigliabile prima scaricare il modello Kick-start, compilarlo manualmente con i dati corretti e quindi importarlo nuovamente in Adobe Workfront.

Per ulteriori informazioni sulla corretta importazione dei dati in Workfront tramite Kick-Starts, vedi [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Perché ricevo questo errore quando si tenta di importare ore in Workfront utilizzando un file Kick-Start: &quot;Utente con valori di chiave primaria &quot;null&quot; non trovato?&quot;

### Risposta

L&#39;errore si riferisce al GUID dell&#39;utente associato alle ore.

Per risolvere il problema:

1. Esporta un modello Kick-Start vuoto per **Ore** solo oggetto.\
   Per ulteriori informazioni sull&#39;esportazione di un file Kick-Start vuoto, vedere &quot;Esportazione del modello Kick-Start&quot; in  [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copiare manualmente i dati dal collegamento iniziale e incollarli nel file vuoto.\
   Esegui questa operazione per ogni colonna.
1. Provare a importare nuovamente il nuovo file.\
   L&#39;importazione di Kick-Start deve essere completata.

## Perché il campo Paese non viene popolato sul profilo utente in un’importazione Click-Start?

### Problema

Quando si importa un clic utente con il pulsante Start del mouse con il campo **setCountry**, tali dati non vengono inviati al paese nel profilo utente.

### Risposta

Se l’utente è abilitato per Unified User Management (UUM) o Adobe Identity Management System (IMS), la variabile **Paese** accetta solo i valori del codice del paese (ad esempio, US, GB, IN). Verifica che **setCountry** nel modello Click-Start vengono utilizzati i valori del codice del paese prima dell’importazione.

Per ulteriori informazioni sulla corretta importazione dei dati in Workfront tramite Kick-Starts, vedi [Importare dati in Adobe Workfront utilizzando un modello Click-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
