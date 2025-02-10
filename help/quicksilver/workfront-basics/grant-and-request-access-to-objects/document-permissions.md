---
title: Condividere un documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: L'amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano livelli di accesso, come spiegato in Concedere l'accesso ai documenti.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 3bd377ba2dec29bb956632cf3e9e3e33afe4305d
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# Condividere un documento

L&#39;amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano i livelli di accesso, come spiegato in [Concedere l&#39;accesso ai documenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Il livello di accesso concesso dall&#39;amministratore di Workfront agli utenti consente loro di visualizzare o modificare i documenti. Inoltre, altri utenti possono concedere ad altri utenti le autorizzazioni per visualizzare o gestire documenti specifici che hanno caricato personalmente o che possono condividere.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento. Per informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per impostazione predefinita, l’utente che carica un documento in Workfront dispone delle autorizzazioni di gestione per tale documento.

Per informazioni sulla condivisione di un&#39;intera cartella documenti, vedere [Condividere una cartella documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Considerazioni sulla condivisione di documenti

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

* La condivisione di un documento è simile alla condivisione di qualsiasi altro oggetto in Workfront. Per informazioni sulla condivisione di documenti in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* È possibile concedere le seguenti autorizzazioni ai documenti:

   * Visualizza
   * Gestire

* È inoltre possibile condividere un documento pubblicamente o a livello di sistema.

  >[!CAUTION]
  >
  >Si consiglia di usare cautela quando si condivide con utenti esterni un oggetto contenente informazioni riservate. Questo consente loro di visualizzare le informazioni senza essere utenti di Workfront o parte dell’organizzazione.

* È possibile condividere un documento con un utente che non dispone di un account Workfront aggiungendo il proprio indirizzo di posta elettronica nel campo Concedi accesso al documento.
* Quando si condivide un documento, gli utenti hanno lo stesso accesso a tutte le versioni del documento e a tutte le bozze del documento.\
  Per ulteriori informazioni sulla verifica in Workfront, vedere la sezione [Verifica](../../review-and-approve-work/proofing/proofing.md).

* È possibile ereditare le autorizzazioni per i documenti dagli oggetti a cui sono associati. L&#39;amministratore di Workfront può limitare l&#39;ereditarietà delle autorizzazioni per i documenti nel proprio livello di accesso.

  Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  È possibile rimuovere manualmente le autorizzazioni ereditate dai documenti. Per ulteriori informazioni, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un documento allegato eredita le autorizzazioni solo dall&#39;oggetto a cui è stato associato. Se si crea una cartella sull&#39;oggetto e si sposta il documento nella cartella, questa eredita le autorizzazioni della cartella. Tuttavia, se si crea una cartella su un oggetto padre o padre e si sposta il documento in tale cartella, questa non eredita le autorizzazioni della cartella.

## Autorizzazioni documento

Nella tabella seguente vengono indicate le autorizzazioni che è possibile concedere agli utenti quando si consente loro di visualizzare o gestire documenti:

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
   <td scope="row">Scarica</td> 
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
   <td scope="row">Sposta in (oggetto)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Invia a (integrazione)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiornamenti/Commenti</td> 
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
   <td scope="row">Genera bozza**</td> 
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

L&#39;azione &#42; è condivisa sia da Cartelle documenti che da Cartelle documenti.

&#42;&#42; Per eseguire la verifica dei documenti è necessario disporre di una licenza di verifica separata associata al proprio account Workfront. Contatta il tuo account manager per ottenere una licenza di verifica. Per ulteriori informazioni sulla verifica in Workfront, vedere [Verifica](../../review-and-approve-work/proofing/proofing.md).
