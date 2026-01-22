---
title: Condividere un documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: L'amministratore di Adobe Systems Workfront concede agli utenti accesso di visualizzare o modificare i documenti quando assegnano accesso livelli, come spiegato in Concedere accesso ai documenti.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 5%

---

# Condividere un documento

L&#39;amministratore di Workfront controlla chi può visualizzare o modificare i documenti nell&#39;area Livelli di accesso nel programma di installazione. Per ulteriori informazioni, vedere [Concedere accesso ai documenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Gli utenti possono anche condividere i documenti che hanno caricato o accesso, dando ad altri autorizzazione per visualizzarli o gestire loro.

* Le autorizzazioni si applicano ai singoli elementi e definiscono le azioni che un utente può intraprendere.
* La persona che carica un documento ottiene automaticamente il pieno controllo (Gestisci autorizzazioni).
* Per condividere un&#39;intera cartella, vedere [Condividere una cartella](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) di documenti.

>[!NOTE]
>
>Se il istanza di Workfront utilizza Adobe Systems archiviazione aziendale, non è possibile condividere singoli documenti. Al contrario, è possibile concedere accesso a livello di progetto. Tieni presente che la condivisione del progetto può concedere accesso a informazioni sensibili del progetto like finanziamenti a seconda del livello di autorizzazione scelto.



## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Visualizza accesso o superiore agli oggetti che desideri condividere</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) di Workfront.

+++



## Condividere un documento

Il utente che carica un documento su Workfront dispone delle autorizzazioni di gestione per impostazione predefinita.

{{step1-to-documents}}

1. **Nella pagina Documenti**, passa il puntatore del mouse sul documento da condividere e fai clic sulla collegare Dettagli **documento** visualizzata. Viene visualizzata la pagina Dettagli **documento**.

   ![Dettagli documento collegare](assets/document-details-link.png)

1. Fai clic sull&#39;icona Altro a **destra del nome del documento, quindi fai clic su** Condividi![.](assets/more-icon.png) **** Viene visualizzata la **finestra di dialogo Condividi [nome]** documento.

   ![Condividere un documento](assets/share-a-document-350x160.png)

1. **Nel campo Grant Document accesso to**, iniziare a digitare il nome del utente, team, ruolo, gruppo o società con cui si desidera condividere il documento, quindi fare clic sul nome visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >È possibile condividere un documento solo con utenti, team, ruoli o società attivi.


1. (Facoltativo) Selezionare il menu a **discesa Chi ha accesso** e selezionare il livello di accesso del documento:

   * **Solo gli invitati possono accesso:** solo gli utenti invitati al documento possono accesso tale documento (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare il documento senza un invito.

1. (Facoltativo) Per rendere pubblico il documento, fai clic sull&#39;icona a forma ![di ingranaggio Seleziona l&#39;icona](assets/gear-icon.png) a forma di ingranaggio, quindi fai clic sulla casella in linea con **Rendi pubblico agli utenti esterni**. L&#39;pulsante **Copia collegare** pubblico viene visualizzato nella parte inferiore della finestra di dialogo.

1. Fare clic sull&#39;elenco a discesa a destra del nome del utente e selezionarne il livello di autorizzazione per questo documento:

   * **Visualizza**: l&#39;utente può rivedere e condividere il documento.
   * **Gestisci**: l&#39;utente ha accesso completo al documento senza diritti amministrativi, che sono concessi a livello accesso (include anche tutte le autorizzazioni Visualizza).

1. (Facoltativo) Fai clic sull&#39;icona delle opzioni avanzate accanto al livello di autorizzazione che hai concesso per configurare autorizzazioni specifiche per il documento.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. (Facoltativo) Per disattivare le autorizzazioni ereditate per gli oggetti secondari del documento, fare clic su **Disattiva** in linea con **le autorizzazioni ereditate**.

1. (Condizionale) Per copiare il collegare pubblico che consente di condividere il documento con utenti esterni, fare clic su **Copia collegare** pubblico.

   >[!CAUTION]
   >
   >Si consiglia di prestare attenzione quando si condivide un documento contenente informazioni riservate con utenti esterni. Ciò consente loro di visualizzare le informazioni senza essere un utente di Workfront o parte dell&#39;organizzazione.

1. Fai clic su **Salva**.

## Condividere documenti in blocco

{{step1-to-documents}}

1. Nella scheda Tutti i **documenti** nella **pagina Documenti** , tieni premuto **Comando** (Mac) o **Ctrl** (Windows) sulla tastiera, quindi fai clic su ciascun documento che desideri condividere.

1. Nella parte superiore della pagina, fai clic sull&#39;icona **** Condividi![ Condividi](assets/share-icon.png). Viene visualizzata la modalità di condivisione.

   ![Icona Condividi](assets/share-documents-in-bulk.png)

1. **Nel campo Grant document accesso to**, iniziare a digitare il nome del utente, team, ruolo, gruppo o società con cui si desidera condividere i documenti, quindi fare clic sul nome visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >È possibile condividere documenti solo con utenti, team, ruoli o società attivi.


1. (Facoltativo) Seleziona il menu a **discesa Chi ha accesso** e seleziona il livello di accesso dei documenti:

   * **Solo le persone invitate possono accesso:** solo gli utenti invitati ai documenti possono accesso tale documento (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzarli**: tutti gli utenti del sistema possono visualizzare i documenti senza un invito.

1. Fai clic sul menu a discesa a destra del nome del utente e seleziona il livello di autorizzazione per i documenti:

   * **Visualizza**: l&#39;utente può rivedere e condividere i documenti.
   * **Gestisci**: l&#39;utente ha accesso completa ai documenti senza diritti amministrativi, che sono concessi a livello accesso (include anche tutte le autorizzazioni Visualizza).

1. (Facoltativo) Fai clic sull&#39;icona delle opzioni avanzate accanto al livello di autorizzazione che hai concesso per configurare autorizzazioni specifiche per i documenti.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. Fai clic su **Salva**.

## Condivisione dei documenti con Adobe Systems storage aziendale

Workfront sta passando alla soluzione di storage aziendale Adobe Systems per fornire una maggiore connettività con Adobe Creative Cloud prodotti. I clienti esistenti saranno spostati al nuovo modello in più fasi. Per ulteriori informazioni sui vantaggi dello storage Adobe Systems enterprise, visita [Adobe Systems panoramica](/help/quicksilver/review-and-approve-work/esm-overview.md) dello storage enterprise.

Se il istanza Workfront utilizza Adobe Systems storage aziendale, non è possibile condividere direttamente singoli documenti. È invece necessario concedere accesso a livello di progetto.

>[!IMPORTANT]
>
>La condivisione di un progetto può anche fornire agli utenti accesso a informazioni sensibili del progetto, ad esempio dati finanziari, a seconda del livello di autorizzazione scelto.
>
>Assicurati di controllare attentamente le impostazioni autorizzazione prima di condividere.

## Autorizzazioni documento

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile intraprendere su tale elemento. Per informazioni sulle autorizzazioni per gli oggetti, vedere [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Nella tabella seguente sono indicate le autorizzazioni che è possibile concedere agli utenti quando consentono loro di visualizzare o gestire documenti:

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
   <td scope="row">Dettagli documento Modifica</td> 
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
   <td scope="row">Send To (integrazione)</td> 
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
   <td scope="row">Visualizza Documento/i</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Anteprima</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Prova**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Genera prova**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Prova Rimuovi**</td> 
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
   <td scope="row">Condividi documenti pubblicamente*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi con un indirizzo e-mail esterno</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi/ Rimuovi</td> 
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

&#42;&#42; È necessario disporre di una licenza di correzione separata associata al account di Workfront per poter provare i documenti. Contatta il tuo responsabile account per informazioni sull&#39;acquisizione di una licenza di correzione. Per ulteriori informazioni sulla verifica in Workfront, vedere [Verifica](../../review-and-approve-work/proofing/proofing.md).

## Considerazioni sulla condivisione di documenti

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento nel sistema, per tutti gli utenti, senza essere il proprietario di tali elementi.

* La condivisione di un documento è simile alla condivisione di qualsiasi altro oggetto in Workfront. Per informazioni su come condividere documenti in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* È possibile concedere le seguenti autorizzazioni ai documenti:

   * Visualizzazione
   * Gestione

* È inoltre possibile condividere un documento pubblicamente o a livello di sistema.

  >[!CAUTION]
  >
  >È consigliabile prestare attenzione quando si condivide un oggetto contenente informazioni riservate con utenti esterni. Questo consente loro di visualizzare le informazioni senza essere utenti di Workfront o parte dell’organizzazione.

* È possibile condividere un documento con un utente che non dispone di un account Workfront aggiungendo il proprio indirizzo di posta elettronica nel campo Concedi accesso al documento.
* Quando si condivide un documento, gli utenti hanno lo stesso accesso a tutte le versioni del documento e a tutte le bozze del documento.\
  Per ulteriori informazioni sulla verifica in Workfront, vedere la sezione [Verifica](../../review-and-approve-work/proofing/proofing.md).

* È possibile ereditare le autorizzazioni per i documenti dagli oggetti a cui sono associati. L&#39;amministratore di Workfront può limitare l&#39;ereditarietà delle autorizzazioni per i documenti nel proprio livello di accesso.

  Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate per i documenti, vedere [Crea o modificare i livelli](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) di accesso personalizzati.

  È possibile rimuovere manualmente le autorizzazioni ereditate sui documenti. Per ulteriori informazioni, vedere [Rimuovi autorizzazioni da oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un documento allegato eredita le autorizzazioni solo dall&#39;oggetto in cui è stato allegato. Se si crea una cartella sull&#39;oggetto e si sposta il documento nella cartella, vengono ereditate le autorizzazioni della cartella. Tuttavia, se si crea una cartella su un oggetto padre o nonno e si sposta il documento in tale cartella, non eredita le autorizzazioni di tale cartella.