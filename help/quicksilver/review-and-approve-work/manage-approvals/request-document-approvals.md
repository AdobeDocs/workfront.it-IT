---
product-area: documents
navigation-topic: approvals
title: Richiedere l'approvazione del documento
description: Puoi richiedere l’approvazione dei responsabili o di altri utenti per un documento in Adobe Workfront. È inoltre possibile richiedere l’approvazione dei documenti da parte di persone senza account Workfront se l’amministratore Workfront ha abilitato questa funzionalità, come descritto in Configurare le preferenze di sicurezza del sistema.
author: Courtney
feature: Work Management
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Richiedere l&#39;approvazione del documento

Puoi richiedere l’approvazione dei responsabili o di altri utenti per un documento in Adobe Workfront. Se l’amministratore Workfront ha abilitato questa funzionalità, puoi anche richiedere l’approvazione dei documenti alle persone senza account Workfront [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti, attività, problemi, modelli, Portfoli, programmi, rapporti, dashboard e calendari, documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzazione o accesso superiore all'oggetto associato alla richiesta di accesso o approvazione </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Richiesta di approvazione di un documento

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trova il documento di cui hai bisogno.

1. Scorri verso il basso fino a **Approvazioni** nella sezione Riepilogo e inizia a digitare nella **Aggiungi approvatore** casella di testo. Puoi aggiungere utenti Workfront per nome o utenti esterni tramite e-mail.

1. Se il tuo amministratore Adobe Workfront ha abilitato la funzionalità di collaborare con persone che non utilizzano Workfront, come descritto in [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), puoi digitare i relativi indirizzi e-mail per includerli.

   Non puoi richiedere l’approvazione da parte di team o gruppi.

1. Ripeti il passaggio precedente per aggiungere altri approvatori.

## Invia nuovamente un&#39;approvazione per una nuova versione

Le decisioni di approvazione dei documenti non vengono reimpostate automaticamente quando si carica una nuova versione. Ad esempio, se il documento viene approvato con modifiche, la decisione mostrerà come decisione &quot;modifiche&quot;, anche se carichi una nuova versione con le modifiche specificate. Se invii manualmente l’approvazione, puoi deselezionare la decisione relativa a una nuova versione.

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trova il documento di cui hai bisogno.

1. Scorri verso il basso fino a **Approvazioni** in Riepilogo, fare clic sull&#39;icona Altro, quindi fare clic su Invia nuovamente.

   ![](assets/nwe-resubmit-approval-350x149.png)

## Eliminare una richiesta di approvazione documento

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trova il documento di cui hai bisogno.

1. Scorri verso il basso fino a **Approvazioni** in Riepilogo, quindi fai clic sul pulsante **Altro** in linea con il nome dell&#39;approvatore e seleziona **Elimina**.

   La richiesta di approvazione viene rimossa e l’approvatore riceve una notifica che attesta che la sua approvazione non è più necessaria. Viene rimosso anche l’accesso alla condivisione relativo all’approvazione.

## Invia un promemoria a un approvatore

È possibile inviare un messaggio per ricordare a un responsabile approvazione di essere in attesa del relativo feedback.

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trova il documento di cui hai bisogno.

1. Scorri verso il basso fino a **Approvazioni** in Riepilogo, quindi fai clic sul pulsante **Altro** in linea con il nome dell&#39;approvatore e seleziona **Ricordare**.

   L&#39;approvatore riceve una notifica che informa che l&#39;approvazione è ancora in sospeso. Possono anche ricevere un promemoria e-mail se lo hanno abilitato.
