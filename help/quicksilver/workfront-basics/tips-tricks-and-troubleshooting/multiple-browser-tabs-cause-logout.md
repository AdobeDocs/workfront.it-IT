---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Più schede del browser causano la disconnessione di Workfront
description: Quando un utente ha più schede del browser aperte, Workfront potrebbe disconnettersi automaticamente.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 41%

---

# Più schede del browser causano la disconnessione di Workfront

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
