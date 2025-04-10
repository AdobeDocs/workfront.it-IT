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
source-git-commit: 5ff071a6e0af93f5280225355edad1d0dde42b3f
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 1%

---

# Configurare le integrazioni di documenti

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

In qualità di amministratore di [!DNL Adobe Workfront], puoi configurare le integrazioni di documenti per gestire i documenti in [!UICONTROL Workfront]. È inoltre possibile configurare [!UICONTROL Workfront] in modo che i documenti vengano archiviati solo nelle applicazioni Document Services e non in [!UICONTROL Workfront]. Per ulteriori informazioni, vedere [Aggiornare e collegare un documento da [!UICONTROL Workfront] a un provider di cloud esterno](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Per consentire la comunicazione aperta tra [!DNL Workfront Proof] e i server [!DNL Workfront], potrebbe essere necessario aggiungere determinati indirizzi IP al inserisco nell&#39;elenco Consentiti di. Per ulteriori informazioni, vedere [Configurare il inserisco nell&#39;elenco Consentiti di protezione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrazioni supportate

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puoi configurare le seguenti integrazioni per la gestione dei documenti:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Il collegamento delle bozze da [!DNL Workfront Proof] consente di rendere disponibili in [!DNL Workfront] le bozze create in origine in [!DNL Workfront Proof]. Per i piani correnti, è necessario un piano [!UICONTROL Pro] [!DNL Workfront] o superiore per utilizzare questa funzione. Per i nuovi piani, questa funzione è disponibile con tutti i piani. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Per informazioni sull&#39;integrazione con [!DNL SharePoint], vedere [Configurare l&#39;integrazione [!DNL SharePoint] ](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Provider di documenti cloud di terze parti:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Unità Google]
   * Quip

  >[!TIP]
  >
  >È possibile verificare e approvare i documenti collegati da un provider cloud esterno nello stesso modo in cui si esegue la verifica e l&#39;approvazione dei documenti caricati direttamente in [!DNL Workfront].

* Altri provider di documenti (tramite integrazioni di documenti personalizzate).

  Per i piani attuali, è necessario un [!UICONTROL Pro] [!DNL Workfront] piano o superiore per utilizzare questa funzione. Per i nuovi piani, questa funzione è disponibile con tutti i piani. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani](https://www.workfront.com/plans) di Workfront.

Inoltre, è possibile migliorare l&#39;esperienza del documento [!DNL Workfront] con integrazioni DAM di terze parti. Gli amministratori devono abilitare queste funzionalità affinché gli utenti possano collegare il servizio al proprio account [!DNL Workfront].

## Configurare le integrazioni per gestire i documenti

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider di cloud].**

1. (Facoltativo) Per archiviare i documenti in un applicazione di Document Services e non in [!DNL Workfront], selezionare **[!UICONTROL Impedisci agli utenti di archiviare documenti in [!DNL Workfront]].**

1. Seleziona le integrazioni che desideri abilitare.
1. Fai clic su **[!UICONTROL Salva]**.

Se stai configurando integrazioni con [!DNL Workfront DAM], puoi abilitare per includere [!DNL Workfront] metadati con i documenti. Per informazioni sulla mappatura dei metadati, vedere [Configurazione metadati mappatura](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurare integrazioni di documenti personalizzati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Un&#39;integrazione personalizzata dei documenti consente a [!DNL Workfront] utenti di collegare i file in [!DNL Workfront] da qualsiasi sistema, a condizione che il sistema funzioni con [!DNL Workfront].

Per rendere l’integrazione personalizzata disponibile agli utenti, devi innanzitutto generarla. Per informazioni su come creare integrazioni da utilizzare con [!DNL Workfront], vedere [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Dopo aver creato l&#39;integrazione del documento personalizzato, è possibile renderla disponibile agli utenti del sito.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata]**.

1. Fare clic su **[!UICONTROL Aggiungi integrazione personalizzata]**.
1. Immetti le seguenti informazioni per configurare l’integrazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[! Nome UICONTROL]</td> 
      <td>Nome dell'integrazione personalizzata. Questo è il nome che gli utenti vedono quando utilizzano l'integrazione all'interno di Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! UICONTROL Base API URL] </td> 
      <td>Il URL HTTP di base o HTTP sicuro per le chiamate API. Ad esempio: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! Tipo Authentication UICONTROL]</td> 
      <td> <p>Metodo di autenticazione da utilizzare quando si effettuano chiamate API autorizzate all'integrazione personalizzata.</p> 
       <ul> 
        <li>Se scegli <strong>[! UICONTROL OAuth]</strong>, continua con il passaggio 5.</li> 
        <li>Se scegli <strong>[! UICONTROL ApiKey],</strong> continuare con il passaggio 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se hai selezionato **[!UICONTROL Autenticazione OAuth]** per Tipo **[!UICONTROL Authentication]**, immetti le seguenti informazioni:

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
      <td> <p>Inserisci i valori facoltativi da aggiungere alla stringa di query di ogni chiamata API. Ad esempio, tipo_di_accesso=offline.</p> <p>Per aggiungere più parametri di richiesta, fare clic su <strong>+Aggiungi parametro di richiesta</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >L&#39;URI di reindirizzamento [!DNL Workfront] visualizzato nella parte inferiore della pagina [!UICONTROL Integrazione personalizzata] elenca l&#39;URI utilizzato per registrare questa integrazione con il provider di documenti esterno.

1. (Condizionale) Se hai selezionato l&#39;autenticazione **[!UICONTROL ApiKey]** per il **[!UICONTROL tipo di autenticazione]**, immetti la chiave API rilasciata dal provider di documenti personalizzato.

   [!DNL Workfront] utilizza questa chiave API per effettuare chiamate API autorizzate al provider di documenti.

1. Fai clic su **[!UICONTROL Salva]** per creare l&#39;integrazione.

## Utilizzare le integrazioni dei documenti

Per informazioni su come gli utenti possono utilizzare la verifica, consulta [Creare bozze](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Per informazioni su come gli utenti possono utilizzare integrazioni di documenti di terze parti dopo averle configurate, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configura [!DNL Workfront] per inviare metadati a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Quando si invia un documento da [!DNL Workfront] a [!DNL Workfront DAM], è anche possibile inviare informazioni associate a tale documento. Le informazioni sul documento sono mappate a [!DNL Workfront DAM] come metadati.

Le informazioni sono mappate solo unidirezionale, da [!DNL Workfront] a [!DNL Workfront DAM] e vengono trasferite solo quando il documento viene caricato in [!DNL Workfront DAM]. Eventuali modifiche future nei campi di Workfront non aggiorneranno i campi di metadati in [!DNL Workfront DAM] dopo il caricamento del documento.\
È possibile mappare lo stesso campo [!DNL Workfront] a vari campi [!DNL Workfront DAM], ma non è possibile utilizzare lo stesso campo [!DNL Workfront DAM] per più campi [!DNL Workfront].

Se è necessario configurare più campi [!DNL Workfront] da esportare in un campo [!DNL Workfront DAM], creare innanzitutto un campo personalizzato calcolato in [!DNL Workfront] per visualizzare tutti i singoli campi personalizzati di un oggetto. Quindi, mappare il campo [!DNL Workfront] calcolato a un campo [!DNL Workfront DAM].\
Per ulteriori informazioni sui campi personalizzati calcolati, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

La mappatura interessa tutti i documenti caricati da qualsiasi utente da [!DNL Workfront] a [!UICONTROL Workfront] DAM.

In qualità di amministratore di [!DNL Workfront], è necessario abilitare [!DNL Workfront DAM] in Workfront prima di poter mappare i campi per il processo di mappatura dei metadati.

Per configurare [!DNL Workfront] per l&#39;invio di metadati a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

1. Nel campo **[!UICONTROL Seleziona campo Source per mappatura]**, inizia a digitare il nome del campo Workfront che desideri mappare a [!DNL Workfront DAM], quindi selezionalo quando lo visualizzi nell&#39;elenco.
1. In **[!UICONTROL Seleziona campo di destinazione per mappatura]**, selezionare il campo [!DNL Workfront DAM] che si desidera compilare con le informazioni nel campo [!DNL Workfront] selezionato.

   >[!NOTE]
   >
   > Tutti i documenti inviati a [!DNL Workfront DAM] da utenti che dispongono dei diritti per farlo vengono aggiornati con i campi [!DNL Workfront] qui mappati, quando vengono caricati in [!DNL Workfront DAM].

1. Fare clic su **[!UICONTROL Aggiungi mappatura]**.

1. Continua l&#39;aggiunta di ulteriori [!UICONTROL campi Workfront] e campi corrispondenti [!DNL Workfront DAM] .

### Elimina campi mappati

{{step-1-to-setup}}

1. Espandi **[!UICONTROL Documenti]**, quindi fai clic su **[!UICONTROL Mappatura metadati]**.

1. Nell&#39;elenco dei campi selezionare i campi che si desidera rimuovere dalla mappatura dei metadati.
1. Fare clic su **[!UICONTROL Elimina]**.

   I campi vengono rimossi dalla mappatura dei metadati e le informazioni in essi contenute non vengono trasferite a [!DNL Workfront DAM] con i documenti caricati.


## Limitazioni

* L&#39;integrazione dei documenti di Google Drive supporta l&#39;aggiunta di cartelle e immagini dall&#39;area My Drive dell&#39;unità Google. Impossibile aggiungere cartelle o immagini da un&#39;unità condivisa. Ulteriori informazioni sulle [unità condivise di Google](https://support.google.com/a/users/answer/7212025?hl=en).