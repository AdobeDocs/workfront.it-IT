---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Decisione approvatore mostra un trattino nel rapporto Proof Approval (Approvazione bozza)
description: Un trattino nel campo Decisione approvatore del rapporto Approvazione bozza indica che un destinatario non è più in un ruolo decisionale sulla bozza.
author: Courtney
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 73c78912e15a03bfd09c127e39d94bf5af42b8e2
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# Decisione approvatore mostra un trattino nel rapporto Proof Approval (Approvazione bozza)

## Problema

Nel rapporto Proof Approval (Approvazione della bozza), il campo Decisione approvatore di un destinatario mostra un trattino (-) anche se il campo Data decisione mostra una data e In attesa di decisione è False.

![La decisione dell&#39;approvatore mostra un trattino nel report Approvazione bozza](assets/approver-decision-hyphen.png)

## Causa

Un trattino nel campo Decisione approvatore indica che il destinatario non è più in un ruolo decisionale sulla bozza. Ciò può verificarsi quando:

* Il destinatario è stato aggiunto alla bozza, ha preso una decisione ed è stato successivamente rimosso dal flusso di lavoro. Se il destinatario rivede la bozza, il sistema di verifica registra la visita come una modifica della decisione. Poiché il destinatario non è più un approvatore, il sistema registra la nuova decisione sotto forma di trattino.
* Il ruolo bozza del destinatario è stato modificato in uno che non include i diritti di approvazione, ad esempio Revisore. Per informazioni sulle azioni che ogni ruolo può eseguire su una bozza, consulta [Panoramica sui ruoli della bozza](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* Il profilo di autorizzazione della bozza del destinatario è stato ridotto dopo la sua decisione.

## Cosa significa questo nei rapporti

Il trattino è intenzionale. Indica che il sistema non attende l’approvazione della bozza da parte del destinatario e che quest’ultimo non ha più un ruolo decisionale sulla bozza.

Il campo Data decisione mostra ancora la data dell’attività di decisione più recente del destinatario, ma la decisione del destinatario non viene più conteggiata nel rapporto.

Per informazioni sulla creazione e l&#39;utilizzo del report Approvazione bozza, vedere [Utilizzare il report Approvazione bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).




