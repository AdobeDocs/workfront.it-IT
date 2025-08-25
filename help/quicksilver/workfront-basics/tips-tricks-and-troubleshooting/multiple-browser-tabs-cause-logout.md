---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Più schede del browser causano la disconnessione di Workfront
description: Quando un utente ha più schede del browser aperte, Workfront potrebbe disconnettersi automaticamente.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 29%

---

# Più schede del browser causano la disconnessione di Workfront

>[!IMPORTANT]
>
>Questo problema è presente solo per le organizzazioni che sono state caricate in Adobe IMS.

## Problema

Quando un utente apre più schede del browser e fa clic su una scheda che è stata inattiva per un certo periodo di tempo, la sessione della scheda è scaduta. L’utente non può visualizzare la pagina che aveva aperto e visualizza invece il seguente messaggio:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Motivo

Questo comportamento è dovuto all’autenticazione basata su criteri (PBA, Policy-Based Authentication), una misura di sicurezza configurata dall’organizzazione. Quando una scheda è rimasta inattiva per più del limite di tempo impostato nella configurazione PBA della tua organizzazione, la sessione di scheda scade.

## Soluzione

La soluzione dipende dal fatto che tu sia stato attivo o meno in un’altra scheda che ha effettuato l’accesso a Workfront.

* Se una scheda Workfront attiva è aperta, ricarica la scheda scaduta. Tornerà alla pagina aperta prima della scadenza.

* Se non hai una scheda Workfront attiva aperta, accedi nuovamente a Workfront.
