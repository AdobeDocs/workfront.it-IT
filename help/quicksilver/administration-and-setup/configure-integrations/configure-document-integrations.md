---
title: Configurare le integrazioni di documenti
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Configurare le integrazioni di documenti
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# Configurare le integrazioni di documenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Come [!DNL Adobe Workfront] amministratore, puoi configurare le integrazioni documenti per gestire i documenti in [!UICONTROL Workfront]. Puoi anche configurare [!UICONTROL Workfront] in modo che i documenti siano archiviati solo nelle applicazioni document services e non in [!UICONTROL Workfront] stesso. Per ulteriori informazioni, consulta [Aggiornare e collegare un documento da [!UICONTROL Workfront] a un provider cloud esterno](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Per consentire una comunicazione aperta tra [!DNL Workfront Proof] e [!DNL Workfront] server, potrebbe essere necessario aggiungere alcuni indirizzi IP al inserire nell&#39;elenco Consentiti. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Integrazioni supportate

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puoi configurare le seguenti integrazioni per la gestione dei documenti:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Collegamento delle bozze da [!DNL Workfront Proof] consente di creare bozze originariamente create in [!DNL Workfront Proof] disponibile all&#39;interno di [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare o eseguire operazioni successive. Per ulteriori informazioni sui vari piani disponibili, vedi [Piani Workfront.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Per informazioni sull&#39;integrazione con [!DNL SharePoint], vedi [Configura le [!DNL SharePoint] integrazione](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Provider di documenti cloud di terze parti:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >È possibile verificare e approvare i documenti collegati da un provider cloud esterno nello stesso modo in cui vengono verificati e approvati i documenti caricati direttamente in [!DNL Workfront].

* Altri provider di documenti (tramite integrazioni personalizzate di documenti).

   A [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare o eseguire operazioni successive. Per ulteriori informazioni sui vari piani disponibili, vedi [[!DNL Workfront] Piani.](https://www.workfront.com/plans)

Inoltre, è possibile migliorare [!DNL Workfront] documenta l’esperienza con un sistema DAM (Digital Asset Management) nativo o con integrazioni DAM di terze parti. Gli amministratori devono abilitare queste funzioni affinché gli utenti possano collegare il servizio ai propri [!DNL Workfront] conto. Per ulteriori informazioni su Workfront DAM, vedi [Gestione dei documenti con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurare le integrazioni per gestire i documenti

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider cloud].**

1. (Facoltativo) Per memorizzare documenti in un&#39;applicazione Document Services e non in [!DNL Workfront], seleziona **[!UICONTROL Impedisci agli utenti di archiviare documenti in [!DNL Workfront]].**

1. Seleziona le integrazioni da abilitare.
1. Fai clic su **[!UICONTROL Salva]**.

Se configuri integrazioni con [!DNL Workfront DAM], puoi abilitare [!DNL Workfront] per includere metadati con documenti. Per informazioni sulla mappatura dei metadati, consulta [Impostare la mappatura dei metadati](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurare integrazioni di documenti personalizzate

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Un’integrazione personalizzata dei documenti consente di: [!DNL Workfront] utenti per collegare file in [!DNL Workfront] praticamente da qualsiasi sistema, a condizione che il sistema sia utilizzato [!DNL Workfront].

Per rendere l’integrazione personalizzata disponibile agli utenti, devi innanzitutto creare l’integrazione . Per informazioni su come creare integrazioni con cui utilizzare [!DNL Workfront], vedi [API per i webhook dei documenti](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Dopo la creazione dell’integrazione dei documenti personalizzata, puoi renderli disponibili agli utenti del sito.

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata].**

1. Fai clic su **[!UICONTROL Aggiungi integrazione personalizzata]**.
1. Specifica le seguenti informazioni per configurare l’integrazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Nome dell’integrazione personalizzata. Questo è il nome visualizzato dagli utenti quando si utilizza l’integrazione in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>L’URL HTTP di base o HTTP protetto per le chiamate API. Ad esempio: <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Il metodo di autenticazione da utilizzare per effettuare chiamate API autorizzate all’integrazione personalizzata.</p> 
       <ul> 
        <li>Se scegli <strong>[!UICONTROL OAuth]</strong>, continua con il passaggio 6.</li> 
        <li>Se scegli <strong>[!UICONTROL ApiKey]</strong>, continua con il passaggio 7.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se hai selezionato **[!UICONTROL OAuth]** autenticazione per **[!UICONTROL Tipo di autenticazione]**, specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>L’URL completo utilizzato per l’autenticazione dell’utente. [!DNL Workfront] sposta gli utenti a questo indirizzo come parte del processo di provisioning di OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>L'URL API completo utilizzato per recuperare i token OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL]</td> 
      <td>ID client OAut per questa integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td>Segreto client OAut per questa integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parametri di richiesta]</td> 
      <td> <p>Specifica i valori facoltativi da aggiungere alla stringa di query di ogni chiamata API. Ad esempio, access_type=offline.</p> <p>Per aggiungere più parametri di richiesta, fai clic su <strong>+Aggiungi parametro di richiesta</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >La [!DNL Workfront] URI di reindirizzamento visualizzato nella parte inferiore del [!UICONTROL Integrazione personalizzata] in questa pagina è riportato l’URI utilizzato per registrare l’integrazione con il provider di documenti esterno.

1. (Condizionale) Se hai selezionato **[!UICONTROL ApiKey]** autenticazione per **[!UICONTROL Tipo di autenticazione]**, specifica la chiave API rilasciata dal provider di documenti personalizzato.

   [!DNL Workfront] utilizza questa chiave API per effettuare chiamate API autorizzate al provider di documenti.

1. Fai clic su **[!UICONTROL Salva]** per creare l’integrazione.

## Utilizzare integrazioni di documenti

Per informazioni su come gli utenti possono utilizzare [!DNL Workfront DAM], vedi [Gestione dei documenti con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Per informazioni su come gli utenti possono utilizzare la correzione, vedi [Creazione di bozze](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Per informazioni su come gli utenti possono utilizzare le integrazioni di documenti di terze parti dopo averle configurate, consulta [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configura [!DNL Workfront] per inviare metadati a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Quando si invia un documento da [!DNL Workfront] a [!DNL Workfront DAM], puoi anche inviare informazioni associate a quel documento. Informazioni sul documento mappate su [!DNL Workfront DAM] come metadati.

Le informazioni sono mappate solo a senso unico, da [!DNL Workfront] a [!DNL Workfront DAM] e viene trasferito solo quando il documento viene caricato in [!DNL Workfront DAM]. Eventuali modifiche future nei campi di Workfront non aggiorneranno i campi di metadati in [!DNL Workfront DAM] dopo il caricamento del documento.\
Puoi eseguire la stessa mappatura [!DNL Workfront] campo a vari [!DNL Workfront DAM] ma non è possibile utilizzare gli stessi campi [!DNL Workfront DAM] campo per più [!DNL Workfront] campi.

Se è necessario configurare più [!DNL Workfront] campi da esportare in uno [!DNL Workfront DAM] crea innanzitutto un campo personalizzato calcolato in [!DNL Workfront] per visualizzare tutti i singoli campi personalizzati di un oggetto. Quindi, mappa il calcolato [!DNL Workfront] campo a uno [!DNL Workfront DAM] campo .\
Per ulteriori informazioni sui campi personalizzati calcolati, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

La mappatura interessa tutti i documenti caricati da qualsiasi utente da [!DNL Workfront] a [!UICONTROL Workfront] DAM.

Come [!DNL Workfront] amministratore, devi abilitare [!DNL Workfront DAM] in Workfront prima di poter mappare i campi per il processo di mappatura dei metadati. Per ulteriori informazioni su come abilitare [!DNL Workfront DAM], vedi [Configurare Workfront per l’invio dei metadati a [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

Per configurare [!DNL Workfront] per inviare metadati a [!DNL Workfront DAM]:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

1. In **[!UICONTROL Selezionare il campo di origine per la mappatura]** campo , inizia a digitare il nome del campo Workfront a cui si desidera eseguire la mappatura [!DNL Workfront DAM], quindi selezionalo quando lo vedi nell’elenco.
1. In **[!UICONTROL Selezionare il campo di destinazione per la mappatura]**, seleziona [!DNL Workfront DAM] campo da compilare con le informazioni nel campo selezionato [!DNL Workfront] campo .

   >[!NOTE]
   >
   > Tutti i documenti inviati a [!DNL Workfront DAM] dagli utenti che dispongono dei diritti per farlo, i loro metadati vengono aggiornati con [!DNL Workfront] campi mappati qui, quando vengono caricati in [!DNL Workfront DAM].

1. Fai clic su **[!UICONTROL Aggiungi mappatura]**.

1. Continua ad aggiungere altro [!UICONTROL Workfront] campi e corrispondenti [!DNL Workfront DAM] campi.

### Elimina campi mappati

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Espandi **[!UICONTROL Documenti]**, quindi fai clic su **[!UICONTROL Mappatura metadati]**.

1. Nell’elenco dei campi, seleziona uno dei campi da rimuovere dalla mappatura metadati.
1. Fai clic su **[!UICONTROL Elimina]**.

   I campi vengono rimossi dalla mappatura dei metadati e le informazioni in essi contenute non vengono trasferite a [!DNL Workfront DAM] con i documenti caricati.
