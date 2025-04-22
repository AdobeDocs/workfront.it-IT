---
title: Condividere un documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: L'amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano livelli di accesso, come spiegato in Concedere l'accesso ai documenti.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 1%

---

# Condividere un documento

L&#39;amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i documenti quando assegnano i livelli di accesso, come spiegato in [Concedere l&#39;accesso ai documenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Il livello di accesso concesso dall&#39;amministratore di Workfront agli utenti consente loro di visualizzare o modificare i documenti. Inoltre, altri utenti possono concedere ad altri utenti le autorizzazioni per visualizzare o gestire documenti specifici che hanno caricato personalmente o che possono condividere.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento. Per informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Per impostazione predefinita, l’utente che carica un documento in Workfront dispone delle autorizzazioni di gestione per tale documento.

Per informazioni sulla condivisione di un&#39;intera cartella documenti, vedere [Condividere una cartella documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p> 
   Oppure
   <p>Corrente: Lavoro o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti da condividere</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

## Condividere un documento

{{step1-to-documents}}

1. Nella pagina **Documenti**, passa il puntatore del mouse sul documento che desideri condividere e fai clic sul collegamento **Dettagli documento** visualizzato. Viene aperta la pagina **Dettagli documento**.

   ![Collegamento dettagli documento](assets/document-details-link.png)

1. Fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome del documento, quindi fai clic su **Condividi**. Viene visualizzata la finestra di dialogo **Condividi [Nome documento]**.

   ![Condividi documento](assets/share-a-document-350x160.png)

1. Nel campo **Concedi l&#39;accesso al documento**, iniziare a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui si desidera condividere il documento, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >È possibile condividere un documento solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Selezionare l&#39;elenco a discesa **Chi ha accesso** e selezionare il livello di accesso del documento:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati al documento possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare il documento senza un invito.

1. (Facoltativo) Per rendere pubblico il documento, fai clic sull&#39;icona a forma di ingranaggio ![Seleziona l&#39;icona a forma di ingranaggio](assets/gear-icon.png), quindi fai clic sulla casella in linea con **Rendi pubblico questo documento agli utenti esterni**. Il pulsante **Copia collegamento pubblico** viene visualizzato nella parte inferiore della finestra di dialogo.

1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per questo documento:

   * **Visualizzazione**: l&#39;utente può rivedere e condividere il documento.
   * **Gestisci**: l&#39;utente ha accesso completo al documento senza diritti amministrativi, concessi al livello di accesso (include anche tutte le autorizzazioni di visualizzazione).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sul documento.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. (Facoltativo) Per disattivare le autorizzazioni ereditate per gli oggetti figlio del documento, fare clic su **Disattiva** in linea con **Autorizzazioni ereditate**.

1. (Condizionale) Per copiare il collegamento pubblico che ti consente di condividere il documento con utenti esterni, fai clic su **Copia collegamento pubblico**.

   >[!CAUTION]
   >
   >Si consiglia di usare cautela quando si condivide un documento contenente informazioni riservate con utenti esterni. Questo consente loro di visualizzare le informazioni senza essere utenti di Workfront o parte dell’organizzazione.

1. Fai clic su **Salva**.

## Condivisione di documenti in blocco

{{step1-to-documents}}

1. Nella scheda **Tutti i documenti** della pagina **Documenti**, tieni premuto **Comando** (Mac) o **Ctrl** (Windows) sulla tastiera, quindi fai clic su ogni documento che desideri condividere.

1. Nella parte superiore della pagina fare clic sull&#39;icona **Condividi** ![Condividi](assets/share-icon.png). Viene visualizzata la finestra modale di condivisione.

   ![Icona Condividi](assets/share-documents-in-bulk.png)

1. Nel campo **Concedi l&#39;accesso al documento**, iniziare a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui si desidera condividere i documenti, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >È possibile condividere documenti solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Selezionare l&#39;elenco a discesa **Chi ha accesso** e selezionare il livello di accesso dei documenti:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati ai documenti possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare i documenti senza un invito.

1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per i documenti:

   * **Visualizza**: l&#39;utente può esaminare e condividere i documenti.
   * **Gestisci**: l&#39;utente ha accesso completo ai documenti senza diritti amministrativi, che sono concessi al livello di accesso (include anche tutte le autorizzazioni di visualizzazione).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sui documenti.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. Fai clic su **Salva**.


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
