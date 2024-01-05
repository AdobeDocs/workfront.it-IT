---
title: Configurare le integrazioni dei documenti
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: In qualità di amministratore di Adobe Workfront, puoi configurare le integrazioni di documenti per gestire i documenti in Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# Configurare le integrazioni dei documenti

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Come un [!DNL Adobe Workfront] amministratore, puoi configurare le integrazioni di documenti per gestire i documenti in [!UICONTROL Workfront]. Puoi anche configurare [!UICONTROL Workfront] in modo che i documenti vengano archiviati solo nelle applicazioni di servizi documentali e non in [!UICONTROL Workfront] stesso. Per ulteriori informazioni, consulta [Aggiornare e collegare un documento da [!UICONTROL Workfront] a un provider cloud esterno](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Per consentire la comunicazione aperta tra [!DNL Workfront Proof] e [!DNL Workfront] server, potrebbe essere necessario aggiungere determinati indirizzi IP al inserisco nell&#39;elenco Consentiti di. Per ulteriori informazioni, consulta [Configurare il inserisco nell&#39;elenco Consentiti di configurazione del firewall per l’accesso a un sistema di protezione da attacchi di tipo](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
       <p>oppure</p>
       <p>Corrente: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Integrazioni supportate

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puoi configurare le seguenti integrazioni per la gestione dei documenti:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Collegamento delle bozze da [!DNL Workfront Proof] consente di creare bozze che sono state originariamente create in [!DNL Workfront Proof] disponibile in [!DNL Workfront]. Per i piani correnti, [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario un piano o versione successiva. Per i nuovi piani, questa funzione è disponibile con tutti i piani. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Per informazioni sull’integrazione con [!DNL SharePoint], vedi [Configurare [!DNL SharePoint] integrazione](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Provider di documenti cloud di terze parti:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Unità Google]

     <!--Quip-->
  >[!TIP]
  >
  >Puoi verificare e approvare i documenti collegati da un provider cloud esterno nello stesso modo in cui esegui la verifica e l’approvazione dei documenti caricati direttamente in [!DNL Workfront].

* Altri provider di documenti (tramite integrazioni di documenti personalizzate).

  Per i piani correnti, [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario un piano o versione successiva. Per i nuovi piani, questa funzione è disponibile con tutti i piani. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

Inoltre, puoi migliorare i [!DNL Workfront] documenta l’esperienza con un sistema Digital Asset Management (DAM) nativo o con integrazioni DAM di terze parti. Gli amministratori devono abilitare queste funzioni affinché gli utenti possano collegare il servizio al proprio [!DNL Workfront] account. Per ulteriori informazioni su Workfront DAM, consulta [Gestione dei documenti con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurare le integrazioni per gestire i documenti

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider cloud].**

1. (Facoltativo) Per memorizzare i documenti in un&#39;applicazione di servizi documentali e non in [!DNL Workfront], seleziona **[!UICONTROL Impedisci agli utenti di archiviare i documenti in [!DNL Workfront]].**

1. Seleziona le integrazioni da abilitare.
1. Fai clic su **[!UICONTROL Salva]**.

Se imposti integrazioni con [!DNL Workfront DAM], è possibile abilitare [!DNL Workfront] per includere metadati nei documenti. Per informazioni sulla mappatura dei metadati, consulta [Impostare la mappatura dei metadati](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurare le integrazioni di documenti personalizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

L’integrazione di un documento personalizzato consente [!DNL Workfront] utenti in cui collegare i file [!DNL Workfront] praticamente da qualsiasi sistema, a condizione che il sistema sia progettato per funzionare con [!DNL Workfront].

Per rendere l’integrazione personalizzata disponibile agli utenti, devi innanzitutto generarla. Per informazioni su come creare integrazioni da utilizzare con [!DNL Workfront], vedi [API dei webhook dei documenti](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Dopo aver creato l&#39;integrazione del documento personalizzato, è possibile renderla disponibile agli utenti del sito.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata]**.

1. Clic **[!UICONTROL Aggiungi integrazione personalizzata]**.
1. Immetti le seguenti informazioni per configurare l’integrazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Nome dell’integrazione personalizzata. Questo è il nome visualizzato dagli utenti quando utilizzano l’integrazione all’interno di Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL API di base] </td> 
      <td>L’URL HTTP di base o sicuro per le chiamate API. Ad esempio: <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Il metodo di autenticazione da utilizzare quando si effettuano chiamate API autorizzate all’integrazione personalizzata.</p> 
       <ul> 
        <li>Se si sceglie <strong>[!UICONTROL OAuth]</strong>, continuare con il passaggio 5.</li> 
        <li>Se si sceglie <strong>[!UICONTROL ApiKey]</strong>, continuare con il passaggio 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se hai selezionato **[!UICONTROL OAuth]** autenticazione per **[!UICONTROL Tipo di autenticazione]**, immetti le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL autenticazione]</td> 
      <td>L’URL completo utilizzato per l’autenticazione dell’utente. [!DNL Workfront] passa a questo indirizzo come parte del processo di provisioning OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL endpoint token]</td> 
      <td>L'URL API completo utilizzato per recuperare i token OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td>ID client OAut per questa integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td>Il segreto client OAut per questa integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parametri di richiesta]</td> 
      <td> <p>Inserisci i valori facoltativi da aggiungere alla stringa di query di ogni chiamata API. Ad esempio, tipo_di_accesso=offline.</p> <p>Per aggiungere più parametri di richiesta, fai clic su <strong>+Aggiungi parametro richiesta</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Il [!DNL Workfront] URI di reindirizzamento visualizzato nella parte inferiore della [!UICONTROL Integrazione personalizzata] pagina elenca l’URI utilizzato per registrare questa integrazione con il provider di documenti esterno.

1. (Condizionale) Se hai selezionato **[!UICONTROL ApiKey]** autenticazione per **[!UICONTROL Tipo di autenticazione]**, immetti la chiave API rilasciata dal provider di documenti personalizzato.

   [!DNL Workfront] utilizza questa chiave API per effettuare chiamate API autorizzate al provider di documenti.

1. Clic **[!UICONTROL Salva]** per creare l’integrazione.

## Utilizzare le integrazioni dei documenti

Per informazioni su come gli utenti possono utilizzare [!DNL Workfront DAM], vedi [Gestione dei documenti con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Per informazioni sull&#39;utilizzo della verifica da parte degli utenti, vedere [Creare le bozze](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Per informazioni su come gli utenti possono utilizzare integrazioni di documenti di terze parti dopo averle configurate, consulta [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configura [!DNL Workfront] per inviare metadati a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Quando si invia un documento da [!DNL Workfront] a [!DNL Workfront DAM], è inoltre possibile inviare informazioni associate a tale documento. Informazioni sul documento mappate a [!DNL Workfront DAM] come metadati.

Le informazioni sono mappate solo unidirezionale, da [!DNL Workfront] a [!DNL Workfront DAM] e viene trasferito solo quando il documento viene caricato in [!DNL Workfront DAM]. Eventuali modifiche future nei campi Workfront non aggiorneranno i campi di metadati in [!DNL Workfront DAM] dopo il caricamento del documento.\
Puoi mappare lo stesso [!DNL Workfront] campo a vari [!DNL Workfront DAM] , ma non puoi utilizzare lo stesso [!DNL Workfront DAM] campo per più [!DNL Workfront] campi.

Se devi configurare più [!DNL Workfront] campi da esportare in uno [!DNL Workfront DAM] , crea un campo personalizzato calcolato in [!DNL Workfront] per visualizzare tutti i singoli campi personalizzati di un oggetto. Quindi, mappa il valore calcolato [!DNL Workfront] campo a uno [!DNL Workfront DAM] campo.\
Per ulteriori informazioni sui campi personalizzati calcolati, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

La mappatura influisce su tutti i documenti caricati da qualsiasi utente da [!DNL Workfront] a [!UICONTROL Workfront] DAM

As a [!DNL Workfront] amministratore, devi abilitare [!DNL Workfront DAM] in Workfront prima di poter mappare i campi per il processo di mappatura dei metadati.

Per configurare [!DNL Workfront] per inviare metadati a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Clic **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

1. In **[!UICONTROL Seleziona campo di origine per la mappatura]** , inizia a digitare il nome del campo Workfront a cui si desidera eseguire il mapping [!DNL Workfront DAM], quindi selezionala quando la visualizzi nell&#39;elenco.
1. In **[!UICONTROL Seleziona campo di destinazione per la mappatura]**, seleziona la [!DNL Workfront DAM] campo da compilare con le informazioni nel campo selezionato [!DNL Workfront] campo.

   >[!NOTE]
   >
   > Tutti i documenti inviati a [!DNL Workfront DAM] da parte degli utenti che dispongono dei diritti per farlo, i loro metadati vengano aggiornati con [!DNL Workfront] campi qui mappati, quando vengono caricati in [!DNL Workfront DAM].

1. Clic **[!UICONTROL Aggiungi mappatura]**.

1. Continua ad aggiungere altri [!UICONTROL Workfront] campi e corrispondenti [!DNL Workfront DAM] campi.

### Elimina campi mappati

{{step-1-to-setup}}

1. Espandi **[!UICONTROL Documenti]**, quindi fai clic su **[!UICONTROL Mappatura metadati]**.

1. Nell&#39;elenco dei campi selezionare i campi che si desidera rimuovere dalla mappatura dei metadati.
1. Clic **[!UICONTROL Elimina]**.

   I campi vengono rimossi dalla mappatura dei metadati e le informazioni in essi contenute non vengono trasferite a [!DNL Workfront DAM] con i documenti caricati.
