---
product-area: documents
navigation-topic: approvals
title: Richiedi approvazione documento legacy
description: Puoi richiedere l’approvazione dei manager o di altri utenti per un documento in Adobe Workfront. È inoltre possibile richiedere l'approvazione dei documenti a persone senza account Workfront se l'amministratore di Workfront ha abilitato questa funzionalità, come descritto in Configurare le preferenze di protezione del sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
TQID: https://experienceleague.adobe.com/NQgXFcbc-4DiObeNE2nRgaW9iKeCKRD5v7J1PRfHkHU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 6%

---

# Richiedi approvazione documento legacy

Puoi richiedere l’approvazione dei manager o di altri utenti per un documento in Adobe Workfront. È inoltre possibile richiedere l&#39;approvazione dei documenti a persone senza account Workfront se l&#39;amministratore di Workfront ha abilitato questa funzionalità, come descritto in [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

>[!NOTE]
>
>Le informazioni contenute in questo articolo si riferiscono alle approvazioni di documenti legacy. <br>
>Per informazioni sulla nuova revisione e approvazione unificate, vedere [Panoramica sulla revisione e sull&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
   <p>Contributo o superiore</p>
   <p>Revisione o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard e calendari, documenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Richiedi approvazione documento

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trovare il documento necessario.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel Riepilogo e inizia a digitare nella casella di testo **Aggiungi approvatore**. Puoi aggiungere utenti Workfront per nome o utenti esterni tramite e-mail.

1. Se l&#39;amministratore di Adobe Workfront ha abilitato la funzionalità di collaborazione con persone che non utilizzano Workfront, come descritto in [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), è possibile digitare i propri indirizzi di posta elettronica per includerli.

   Non puoi richiedere l’approvazione di team o gruppi.

1. Ripeti il passaggio precedente per aggiungere altri approvatori.

## Invia nuovamente un’approvazione per una nuova versione

Le decisioni di approvazione dei documenti non vengono reimpostate automaticamente quando si carica una nuova versione. Ad esempio, se il documento viene approvato con modifiche, nella decisione vengono visualizzate le &quot;modifiche&quot; come decisione, anche se si carica una nuova versione con le modifiche specificate. Se invii nuovamente l’approvazione manualmente, puoi annullare la decisione relativa a una nuova versione.

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trovare il documento necessario.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel riepilogo, fai clic sull&#39;icona Altro, quindi fai clic su Invia di nuovo.

   ![Invia di nuovo l&#39;approvazione](assets/nwe-resubmit-approval-350x149.png)

## Eliminare una richiesta di approvazione documento

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trovare il documento necessario.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel riepilogo, quindi fai clic sul menu **Altro** in linea con il nome dell&#39;approvatore e seleziona **Elimina**.

   La richiesta di approvazione viene rimossa e l’approvatore riceve una notifica che indica che la sua approvazione non è più necessaria. Viene rimosso anche l’accesso condiviso relativo all’approvazione.

## Invia un promemoria a un approvatore

È possibile inviare un messaggio per ricordare a un approvatore di essere in attesa del suo feedback.

1. Vai al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trovare il documento necessario.

1. Scorri verso il basso fino alla sezione **Approvazioni** nel riepilogo, quindi fai clic sul menu **Altro** in linea con il nome dell&#39;approvatore e seleziona **Ricorda**.

   L&#39;approvatore riceve una notifica che informa che l&#39;approvazione è ancora in sospeso. Se attivato, può anche ricevere un promemoria e-mail.
