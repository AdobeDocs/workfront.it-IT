---
title: Verifica dei limiti di collaborazione con persone esterne all’organizzazione
description: Verifica dei limiti di collaborazione con persone esterne all’organizzazione
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Verifica dei limiti di collaborazione con persone esterne all’organizzazione

Esistono alcune limitazioni di cui tenere conto nelle comunicazioni con persone esterne all’organizzazione quando vengono aggiunte a una bozza, in particolare se la persona esterna all’organizzazione dispone dell’accesso alle bozze in un ambiente separato.

## Contatti con la distinzione degli Stati membri

In un ambiente di verifica esistono tre tipi di contatti:

* **Utenti**: gli utenti dispongono di un accesso a Workfront Proof nell&#39;ambiente della tua organizzazione.
* **Membri**: i membri dispongono del proprio accesso a Workfront Proof nell&#39;ambiente di un&#39;altra organizzazione (non nel proprio). Non è possibile convertire i membri in utenti nell&#39;ambiente.
* **Ospiti**: gli ospiti non dispongono del proprio accesso a Workfront Proof nell&#39;ambiente della tua organizzazione, ma hai aggiunto i loro dettagli al tuo account (ad esempio, i revisori ospiti sulle bozze). Puoi convertire gli ospiti in utenti.

Poiché i membri non possono essere convertiti in utenti, la possibilità di assegnare tag alle persone nei commenti della bozza è limitata agli utenti della *organizzazione originale*.

**Esempio:** la società A invita un utente esterno a rivedere una bozza. Questo utente esiste già in un ambiente di bozza separato, Società B.

 

Quando la società A invita l’utente esterno alla bozza, quest’ultimo viene aggiunto all’elenco dei contatti della società A in qualità di membro. I revisori nel flusso di lavoro delle bozze dalla società A possono assegnare tag all’utente esterno nei commenti della bozza perché si trovano ora nella directory dei contatti della società A.

 

L’utente esterno non può assegnare tag agli utenti della società A, anche se si trovano nello stesso flusso di lavoro della bozza, perché gli utenti della società A non sono stati aggiunti come contatti alla società B.

 

L’utente esterno della Società B può assegnare tag ad altri utenti della Società B se si trovano nel flusso di lavoro della bozza o se dispone dell’autorizzazione per condividere la bozza con i nuovi utenti, in quanto tali utenti esistono come contatti nella Società B.
