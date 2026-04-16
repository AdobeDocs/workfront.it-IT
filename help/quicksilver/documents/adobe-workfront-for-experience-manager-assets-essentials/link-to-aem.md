---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Collegamento di contenuto e cartelle con Contenuto verificato basato su Experience Manager Assets
description: È possibile utilizzare Contenuto verificato per collegare contenuto o cartelle da Experience Manager Assets a qualsiasi oggetto di Adobe Workfront che supporti i documenti. Contenuto verificato consente l'individuazione intelligente e basata sul contesto direttamente in Workfront, consentendo di trovare rapidamente contenuti pertinenti e approvati.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 5%

---

# Collegare contenuto e cartelle con Contenuto verificato di Experience Manager Assets

Contenuto verificato consente di eseguire il rilevamento intelligente e in base al contesto direttamente in Workfront, consentendo di trovare rapidamente contenuti pertinenti e approvati in base al contesto. Grazie a funzioni quali suggerimenti avanzati, rappresentazioni Dynamic Media e metadati di risorse dettagliati, consente di valutare e riutilizzare in modo efficiente i contenuti senza uscire da Workfront, accelerando la creazione dei contenuti e mantenendo al contempo la coerenza del marchio.

È possibile utilizzare Contenuto verificato per collegare contenuto e cartelle da Experience Manager Assets a Workfront. Una volta effettuato il collegamento, puoi visualizzare e gestire il contenuto in Workfront; eventuali modifiche apportate al contenuto in Experience Manager Assets verranno applicate anche in Workfront.

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
   <td>Devi disporre di Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
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

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Per utilizzare i suggerimenti avanzati o la funzionalità Brief campagna, è necessario firmare un Rider GenAI. Per ulteriori informazioni, vedere [Utilizzare Contenuto verificato per accedere al contenuto di AEM nelle applicazioni Adobe](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Collegare il contenuto da Experience Manager Assets con Contenuto verificato

È ora possibile utilizzare Contenuto verificato per collegare il contenuto da Experience Manager Assets direttamente in Workfront. Contenuto verificato non è disponibile per Assets Essentials.

Per collegare il contenuto:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets.

1. Contenuto verificato consente di:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Cerca le risorse utilizzando la Ricerca IA.</strong> Utilizza la ricerca basata sull'intelligenza artificiale per comprendere il significato e le finalità alla base delle query, supportando più lingue, errori di battitura e sinonimi.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Ricerche IA per un'individuazione più intelligente delle risorse</a>.</td>
      </tr>
      <tr>
         <td><strong>Visualizza suggerimenti avanzati in base al contesto e all'intento.</strong> Scopri le risorse in linea con le tue esigenze di contenuto utilizzando i consigli in base al contesto dell'applicazione host Adobe.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Suggerimenti avanzati basati su contesto e intento</a>.</td>
      </tr>
      <tr>
         <td><strong>Carica una descrizione della campagna per individuare le risorse rilevanti.</strong> Caricare un documento di riepilogo di una campagna PDF, DOCX o TXT in modo che Contenuto verificato possa analizzarlo e consigliare le risorse pertinenti.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Documenti informativi sulla campagna per individuare le risorse rilevanti</a>.</td>
      </tr>
      <tr>
         <td><strong>Visualizza e seleziona le rappresentazioni di risorse Dynamic Media.</strong> Sfoglia le rappresentazioni ottimizzate per il canale, inclusi i predefiniti immagine, ritagli avanzati e tipi di formato, e applica i modificatori Dynamic Media alle regolazioni di anteprima in tempo reale.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendering delle risorse Dynamic Media disponibili per l'uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Applicare i modificatori Dynamic Media alle rappresentazioni.</strong> Aggiungi modificatori per trasformare le rappresentazioni delle risorse in tempo reale e visualizzare l'anteprima dei risultati prima di selezionare una rappresentazione per l'applicazione host.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendering delle risorse Dynamic Media disponibili per l'uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Individuare e sfogliare i frammenti di contenuto.</strong> Effettua ricerche nei frammenti di contenuto, visualizza anteprime di miniature live, controlla lo stato (Bozza, Modificato o Pubblicato) e controlla proprietà dettagliate, riferimenti e varianti.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Individuazione di frammenti di contenuto</a>.</td>
      </tr>
      <tr>
         <td><strong>Accedere ai metadati della risorsa.</strong> Rivedi le proprietà della risorsa come titolo, descrizione, formato, dimensione e altre schede di metadati (prodotto, campagna, tag) coerenti con la vista Assets.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Accedere ai metadati delle risorse coerenti con la vista Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrare le risorse utilizzando filtri predefiniti.</strong> Ottimizza i risultati delle risorse utilizzando filtri come Tipo file, Formato file, Stato risorsa, Dimensione file, Larghezza immagine, Altezza immagine, Data di modifica e Data di creazione.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Filtri di accesso coerenti con la visualizzazione Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Salvare e riutilizzare le ricerche.</strong> Per creare ricerche salvate, specificare un termine di ricerca e le opzioni di filtro, quindi riutilizzarle in Experience Manager Assets e altre applicazioni Adobe.</td>
         <td>Per ulteriori informazioni, vedere <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Accedere e riutilizzare ricerche recenti e salvate</a>.</td>
      </tr>
      <tr>
         <td><strong>Cerca le risorse tra e all'interno delle raccolte.</strong> Cerca risorse o raccolte in tutte le raccolte o limita la ricerca a una raccolta specifica.</td>
         <td>Per ulteriori informazioni, consulta <a href="https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Cercare risorse in e all'interno di raccolte</a>.</td>
      </tr>
   </tbody>
   </table>


### Collegare una nuova versione di Experience Manager Assets con Contenuto verificato

Puoi richiamare nuovi contenuti da Experience Manager Assets o Assets Essentials e aggiungerli a una risorsa esistente come nuova versione. Se il documento è già collegato e viene aggiunta una nuova versione in Experience Manager Assets o Assets Essentials, la nuova versione viene visualizzata automaticamente in Workfront.

Per collegare una nuova versione:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri aggiungere il documento.
1. Seleziona la risorsa da sostituire con una nuova versione. Non puoi creare una nuova versione di una risorsa in una cartella collegata.
1. Seleziona **Aggiungi nuovo** > **Versione**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets.

1. Seleziona il contenuto da collegare:

   * Seleziona la scheda Assets per sfogliare risorse, cartelle o raccolte in Experience Manager Assets o Assets Essentials.

     ![Consulente contenuti](assets/content-advisor-full.png)

   * I frammenti di contenuto non supportano le versioni. Se selezioni un frammento di contenuto, la nuova versione sostituirà il frammento di contenuto esistente invece di creare una nuova versione.

1. Fai clic su **Seleziona**.

## Collegare una cartella da Experience Manager Assets con Contenuto verificato

Le autorizzazioni per visualizzare singole risorse all’interno di una cartella si basano sulle autorizzazioni di Experience Manager Assets.

Per collegare una cartella:

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire la cartella.
1. Seleziona **Aggiungi nuovo**, quindi seleziona l&#39;integrazione Experience Manager configurata dall&#39;amministratore.

   >[!NOTE]
   >
   >L’amministratore di Workfront può scegliere qualsiasi nome per questa integrazione, pertanto potrebbe non menzionare specificamente Experience Manager Assets.

1. Fai clic su **Assets** > **File e cartelle**.

1. Fai clic sull&#39;icona **Filtro**, quindi nella sezione **Tipo risorsa** scegli **Cartelle**.

1. Seleziona la cartella da collegare.

1. Fai clic su **Seleziona**.

## Considerazioni

* La funzionalità Contenuto verificato non è disponibile per gli oggetti che utilizzano Adobe Enterprise Storage. Se la tua organizzazione utilizza lo storage aziendale Adobe, è comunque possibile collegare risorse e cartelle da Experience Manager Assets o Assets Essentials, ma non sarà possibile accedere alle funzioni di Contenuto verificato, ad esempio Ricerche IA, suggerimenti avanzati o rappresentazioni Dynamic Media. Per ulteriori informazioni, consulta [Utilizzare Adobe Experience Manager con l’integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* La funzionalità Contenuto verificato non è disponibile per Assets Essentials. Per collegare risorse e cartelle da Assets Essentials, consulta [Collegare risorse e cartelle da Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets. Se l&#39;amministratore di Workfront ha attivato la sincronizzazione dei metadati dell&#39;oggetto, i campi rimangono aggiornati se vengono modificati in una delle applicazioni.
