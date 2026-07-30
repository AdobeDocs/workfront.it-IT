---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Collegare contenuti e cartelle da Experience Manager Assets con l’archiviazione cloud Adobe
description: Se la tua organizzazione utilizza l’archiviazione cloud di Adobe, puoi collegare contenuti e cartelle da Experience Manager Assets a qualsiasi oggetto Adobe Workfront che supporti i documenti.
author: Courtney
source-git-commit: 805cc8dfaa17438eb1d454d00d5f7986540379b3
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 7%

---

# Collegare contenuti e cartelle da Experience Manager Assets con l’archiviazione cloud Adobe

Se la tua organizzazione utilizza l’archiviazione cloud di Adobe, puoi collegare contenuti e cartelle da Experience Manager Assets a Workfront. Una volta effettuato il collegamento, puoi visualizzare e gestire il contenuto in Workfront; eventuali modifiche apportate al contenuto in Experience Manager Assets verranno applicate anche in Workfront.

>[!IMPORTANT]
>
>Se l&#39;organizzazione rifiuta di firmare l&#39;accordo GenAI Rider, è comunque possibile utilizzare Contenuto verificato per scegliere risorse e cartelle in Experience Manager Assets, ma non sarà possibile accedere alle funzioni basate sull&#39;intelligenza artificiale, ad esempio Ricerca IA, suggerimenti avanzati o analisi delle descrizioni delle campagne.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Devi disporre di Experience Manager as a Cloud Service e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni Experience Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare:

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Utilizzare Adobe Experience Manager con l’integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Per utilizzare i suggerimenti avanzati o la funzionalità Brief campagna, è necessario firmare un Rider GenAI. Per ulteriori informazioni, vedere [Utilizzare Contenuto verificato per accedere al contenuto di AEM nelle applicazioni Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).

## Collega contenuto da Experience Manager Assets

Per collegare il contenuto:

1. Vai all’oggetto Workfront in cui desideri collegare il contenuto.
1. Fai clic sulla sezione **Documenti** nel pannello a sinistra.
1. Fai clic su **Nuovo** sul lato destro della pagina, quindi fai clic su **File AEM** per collegare una singola risorsa.
   ![Aggiungi file AEM all&#39;area documenti](assets/aem-files.png)

1. Contenuto verificato consente di:

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Cerca risorse tramite Ricerca IA.</strong> Utilizza la ricerca basata sull’intelligenza artificiale per comprendere il significato e le intenzioni alla base delle query, supportando più lingue, errori di battitura e sinonimi.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Ricerche IA per un'individuazione più intelligente delle risorse</a>.</td>
      </tr>
      <tr>
         <td><strong>Visualizza suggerimenti avanzati in base al contesto e all'intento.</strong> Scopri le risorse che sono in linea con le tue esigenze di contenuto utilizzando i consigli in base al contesto forniti dall’applicazione host di Adobe.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Suggerimenti avanzati basati su contesto e intento</a>.</td>
      </tr>
      <tr>
         <td><strong>Carica una descrizione della campagna per individuare le risorse rilevanti.</strong> Caricare un documento di descrizione di una campagna PDF, DOCX o TXT in modo che Contenuto verificato possa analizzarlo e consigliare le risorse pertinenti.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Documenti informativi sulla campagna per individuare le risorse rilevanti</a>.</td>
      </tr>
      <tr>
         <td><strong>Visualizza e seleziona rappresentazioni risorse Dynamic Media.</strong> Sfoglia le rappresentazioni ottimizzate per il canale, inclusi i predefiniti immagine, ritagli avanzati e tipi di formato, e applica i modificatori Dynamic Media per le regolazioni di anteprima in tempo reale.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendering delle risorse Dynamic Media disponibili per l'uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Applica modificatori Dynamic Media alle rappresentazioni.</strong> Aggiungi modificatori per trasformare le rappresentazioni delle risorse in tempo reale e visualizzare in anteprima i risultati prima di selezionare una rappresentazione per l’applicazione host.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendering delle risorse Dynamic Media disponibili per l'uso</a>.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>Accedere ai metadati delle risorse.</strong> Rivedi le proprietà della risorsa come titolo, descrizione, formato, dimensione e altre schede di metadati (Prodotto, Campagna, Tag) coerenti con la vista Assets.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Accedere ai metadati delle risorse coerenti con la vista Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrare le risorse utilizzando filtri predefiniti.</strong> Ottimizza i risultati delle risorse utilizzando filtri come Tipo file, Formato file, Stato risorsa, Dimensione file, Larghezza immagine, Altezza immagine, Data di modifica e Data di creazione.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Filtri di accesso coerenti con la visualizzazione Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Salvare e riutilizzare le ricerche.</strong> Per creare ricerche salvate, specifica un termine di ricerca e le opzioni di filtro, quindi riutilizzale in Experience Manager Assets e altre applicazioni Adobe.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Accedere e riutilizzare ricerche recenti e salvate</a>.</td>
      </tr>
      <tr>
         <td><strong>Cerca le risorse tra e all'interno delle raccolte.</strong> Cerca risorse o raccolte in tutte le raccolte oppure limita la ricerca a una raccolta specifica.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Cercare risorse in e all'interno di raccolte</a>.</td>
      </tr>
   </tbody>
   </table>

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## Considerazioni

* I flussi di lavoro di revisione e approvazione non sono supportati per le risorse AEM collegate.
* I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets. Se l&#39;amministratore di Workfront ha attivato la sincronizzazione dei metadati dell&#39;oggetto, i campi rimangono aggiornati se vengono modificati in una delle applicazioni.
