---
title: Verifica delle limitazioni della collaborazione con persone esterne all’organizzazione
description: Verifica delle limitazioni della collaborazione con persone esterne all’organizzazione
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Verifica delle limitazioni della collaborazione con persone esterne all’organizzazione

Durante la comunicazione con persone esterne all’organizzazione è necessario tenere presenti alcune limitazioni quando queste vengono aggiunte a una bozza, in particolare se la persona al di fuori dell’organizzazione dispone dell’accesso per le prove in un ambiente separato.

## Contatti con la distinzione di membro

Esistono tre tipi di contatti in un ambiente di correzione:

* **Utenti**: Gli utenti dispongono di un accesso Workfront Proof nell’ambiente della tua organizzazione.
* **Membri**: I membri dispongono del proprio accesso Workfront Proof nell’ambiente di un’altra organizzazione (non il proprio). Non è possibile convertire i membri in utenti nel proprio ambiente.
* **Ospiti**: Gli ospiti non dispongono del proprio accesso Workfront Proof nell’ambiente della tua organizzazione, ma hai aggiunto i loro dettagli al tuo account (ad esempio, revisori ospiti sulle bozze). Puoi convertire gli ospiti in utenti.

Poiché i membri non possono essere convertiti in utenti, la loro capacità di assegnare tag alle persone nei commenti della bozza è limitata agli utenti di *organizzazione originale*.

**Esempio:** La società A invita un utente esterno a rivedere una bozza. Questo utente esiste già in un ambiente di prova separato, la società B.

 

Quando la società A invita l&#39;utente esterno alla bozza, l&#39;utente esterno viene aggiunto all&#39;elenco dei contatti della società A come membro. I revisori nel flusso di lavoro di prova della società A possono assegnare all&#39;utente esterno un tag nei commenti di prova perché si trovano nella directory dei contatti della società A.

 

L&#39;utente esterno non può assegnare tag agli utenti della società A, anche se si trovano nello stesso flusso di lavoro di prova, perché gli utenti della società A non sono stati aggiunti come contatti alla società B.

 

L&#39;utente esterno della società B può assegnare tag ad altri utenti della società B se si trovano nel flusso di lavoro di prova o se dispongono dell&#39;autorizzazione per condividere la bozza con nuovi utenti, perché questi utenti esistono come contatti nella società B.
