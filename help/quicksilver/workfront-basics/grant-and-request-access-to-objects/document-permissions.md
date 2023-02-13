---
title: Condividere un documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano livelli di accesso, come spiegato in Concedere l’accesso ai documenti.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# Condividere un documento

L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano livelli di accesso, come spiegato in [Concedere l’accesso ai documenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Il livello di accesso concesso dall’amministratore Workfront agli utenti consente loro di visualizzare o modificare i documenti. Inoltre, altri utenti possono concedere ad altri autorizzazioni per visualizzare o gestire documenti specifici caricati da loro stessi o che hanno accesso alla condivisione.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento. Per informazioni sulle autorizzazioni per gli oggetti, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per impostazione predefinita, l’utente che carica un documento in Workfront dispone delle autorizzazioni di gestione.

Per informazioni sulla condivisione di un&#39;intera cartella di documenti, vedere [Condivisione di una cartella di documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Considerazioni sulla condivisione di documenti

Oltre alle considerazioni seguenti, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

* La condivisione di un documento è simile alla condivisione di qualsiasi altro oggetto in Workfront. Per informazioni su come condividere documenti in Workfront, vedi [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* È possibile concedere le seguenti autorizzazioni ai documenti:

   * Visualizza
   * Gestisci

* È inoltre possibile condividere un documento pubblicamente o a livello di sistema.

   >[!CAUTION]
   >
   >È consigliabile prestare attenzione quando si condivide con utenti esterni un oggetto contenente informazioni confidenziali. Questo consente loro di visualizzare le informazioni senza essere un utente Workfront o parte dell’organizzazione.

* È possibile condividere un documento con un utente che non dispone di un account Workfront, aggiungendo il proprio indirizzo e-mail nel campo Consenti accesso al documento.
* Quando si condivide un documento, gli utenti hanno lo stesso accesso a tutte le versioni del documento e a tutte le bozze del documento.\
   Per ulteriori informazioni sulle bozze in Workfront, consulta la sezione [Copertura](../../review-and-approve-work/proofing/proofing.md) sezione .

* È possibile ereditare le autorizzazioni ai documenti dagli oggetti a cui sono associati. L’amministratore di Workfront può limitare l’ereditarietà delle autorizzazioni per i documenti a livello di accesso.

   Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate ai documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   È possibile rimuovere manualmente le autorizzazioni ereditate sui documenti. Per ulteriori informazioni, consulta [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un documento allegato eredita le autorizzazioni solo dall&#39;oggetto in cui è stato allegato. Se si crea una cartella sull&#39;oggetto e si sposta il documento nella cartella, questa eredita le autorizzazioni della cartella. Tuttavia, se si crea una cartella su un oggetto principale o principale e si sposta il documento in tale cartella, non eredita le autorizzazioni della cartella.

## Autorizzazioni documento

Nella tabella seguente vengono visualizzate le autorizzazioni che è possibile concedere agli utenti per la visualizzazione o la gestione dei documenti:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Azione</strong> </p> </th> 
   <th> <p><strong>Gestisci</strong> </p> </th> 
   <th> <p><strong>Visualizza</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Crea</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica dettagli documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Elimina*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Download</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Pagamento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi approvatori</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approva documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Allega modulo personalizzato</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica campi personalizzati</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Sposta a (oggetto)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Invia a (integrazione)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiornamenti/commenti</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Carica nuova versione</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Elimina versione</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visualizza documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Anteprima</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Bozza**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Crea bozza**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Rimuovi bozza**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi a livello di sistema*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi i documenti pubblicamente*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi con un indirizzo e-mail esterno</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi/Rimuovi</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Rinomina</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Collegamento (con integrazione)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Scollega (con integrazione)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; L&#39;azione è condivisa sia da Documenti che da Cartelle documenti.

&#42;&#42; Per poter provare i documenti, è necessario disporre di una licenza di correzione separata associata al tuo account Workfront. Contatta il tuo account manager per ottenere una licenza di correzione. Per ulteriori informazioni sulle bozze in Workfront, vedi [Copertura](../../review-and-approve-work/proofing/proofing.md).
