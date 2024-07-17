---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kick-start, kick-start, kick-start, kick-start
navigation-topic: use-kick-starts
title: Domande frequenti su Kick-Start
description: Risposte alle domande frequenti sull'importazione e l'esportazione di dati Workfront tramite Kick-Start.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Domande frequenti su Kick-Start

Di seguito sono riportate le domande frequenti su Kick-Start:

## Perché ricevo questo errore quando tento di importare un file Kick-Start: &quot;Il file era corretto, ma non è stato importato nulla?&quot;

### Risposta

Nel file Kick-Start potrebbe mancare uno dei tre elementi seguenti:

1. La colonna **isNew** deve essere impostata su **TRUE** per tutti gli elementi che si desidera importare. **isNew** deve essere **TRUE** perché è possibile importare nuovi dati solo con un&#39;istruzione di avvio. Non è possibile modificare i dati esistenti tramite Kick-Start. Nel foglio di calcolo possono essere presenti altre righe con **isNew = FALSE**, ma queste righe non verranno importate.

1. &#x200B;Il file deve avere una riga vuota prima che inizino le intestazioni dei dati.
1. &#x200B;I fogli di Excel devono avere i nomi corretti.

Quando si lavora con Kick-Start, si consiglia di scaricare il modello di Kick-Start, compilarlo manualmente con i dati corretti e quindi importarlo nuovamente in Adobe Workfront.

Per ulteriori informazioni sulla corretta importazione dei dati in Workfront tramite Kick-Start, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Perché ricevo questo errore quando tento di importare ore in Workfront utilizzando un file Kick-Start: &quot;Utente con valori di chiave primaria &quot;null&quot; non trovato?&quot;

### Risposta

L’errore si riferisce al GUID dell’utente associato alle ore.

Per risolvere il problema:

1. Esporta un modello Kick-Start vuoto solo per l&#39;oggetto **Hours**.\
   Per ulteriori informazioni sull&#39;esportazione di un file Kick-Start vuoto, vedere &quot;Esportazione del modello Kick-Start&quot; in [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copiare manualmente i dati dall&#39;avvio originale e incollarli nel file vuoto.\
   Eseguire questa operazione per ogni colonna.
1. Provare a importare di nuovo il nuovo file.\
   Il Kick-Start deve essere importato correttamente.

## Perché il campo del paese non viene popolato nel profilo utente in un’importazione Kick-Start?

### Problema

Quando si importa un avvio utente con il campo **setCountry**, tali dati non vengono trasferiti al paese nel profilo utente.

### Risposta

Se l&#39;utente è abilitato per Unified User Management (UUM) o Adobe Identity Management System (IMS), il campo **Paese** accetta solo i valori del codice paese (ad , US, GB, IN). Verificare che il campo **setCountry** nel modello Kick-Start utilizzi i valori del codice paese prima dell&#39;importazione.

Per ulteriori informazioni sulla corretta importazione dei dati in Workfront tramite Kick-Start, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
