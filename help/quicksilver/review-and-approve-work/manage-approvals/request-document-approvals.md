---
product-area: documents
navigation-topic: approvals
title: Richiedere le approvazioni dei documenti
description: Puoi richiedere l’approvazione dei manager o di altri utenti per un documento in Adobe Workfront. È inoltre possibile richiedere l'approvazione dei documenti a persone senza account Workfront se l'amministratore di Workfront ha abilitato questa funzionalità, come descritto in Configurare le preferenze di protezione del sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 1%

---

# Richiedere le approvazioni dei documenti

Puoi richiedere l’approvazione dei manager o di altri utenti per un documento in Adobe Workfront. È inoltre possibile richiedere l&#39;approvazione dei documenti a persone senza account Workfront se l&#39;amministratore di Workfront ha abilitato questa funzionalità, come descritto in [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso a progetti, attività, problemi, modelli, Portfoli, programmi, report, dashboard e calendari, documenti o versioni successive</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta di accesso o approvazione </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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

   ![](assets/nwe-resubmit-approval-350x149.png)

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
