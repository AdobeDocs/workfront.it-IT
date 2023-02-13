---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Adobe Experience Manager Assets
description: Con la [!DNL Adobe Experience Manager Assets] connettore per [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] , creare, caricare e aggiornare le risorse e copiare o spostare cartelle e risorse.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] moduli

Con la [!DNL Adobe Experience Manager Assets] connettore per [!DNL Adobe Workfront Fusion], puoi avviare uno scenario basato sugli eventi nel [!DNL Adobe Experience Manager Assets] , creare, caricare e aggiornare le risorse e copiare o spostare cartelle e risorse.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

* Devi avere un [!DNL Adobe Experience Manager Assets] per utilizzare questi moduli.
* Devi configurare [!UICONTROL Server-to-server] flusso [!DNL Adobe Developer console].

   Per istruzioni sulla configurazione [!UICONTROL Server-to-server] flusso [!DNL Adobe Developer console], vedi [Generazione dei token di accesso per le API lato server](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Per creare una connessione per [!DNL Adobe Experience Manager Assets] moduli:

1. Fai clic su [!UICONTROL Aggiungi] accanto al [!UICONTROL Connessione] scatola.

2. Selezionare il tipo di connessione che si sta creando:

   * **[!DNL AEM Assets as a Cloud Service]**

      Questa configurazione richiede informazioni dal [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      Questa configurazione richiede un nome utente e una password.

3. Compila i campi per il tipo di connessione che stai creando.

   Per [!DNL AEM Assets as a Cloud Service], vedi [Configura la connessione per [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Per [!UICONTROL AEM Assets Basic], vedi [Configura la connessione per [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo .


### Configura la connessione per [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>Le informazioni relative a questi campi vengono generate come parte della configurazione [!UICONTROL Server-to-server] flusso [!DNL Adobe Developer Console]. Puoi trovare questi valori nel file JSON delle credenziali del servizio generato come parte di tale configurazione.
>
>Per istruzioni sulla configurazione [!UICONTROL Server-to-server] flusso [!UICONTROL Console Adobe Developer], vedi [Generazione dei token di accesso per le API lato server](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Nome connessione]</td>
                  <td>
                      <p>Immettere un nome per la connessione</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL URL dell'istanza senza barra finale]</td>
                  <td>Immetti l’URL per il tuo [!DNL Adobe Experience Manager] istanza. Non includere una barra <code>/</code> alla fine dell’URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">ID client [!UICONTROL]</td>
                  <td>Immetti l’ID client generato nell’impostazione server-to-server.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Segreto client]</td>
                  <td>Immetti il Segreto client generato nella configurazione [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID account tecnico]</td>
                  <td>Immetti l’ID dell’account tecnico. Questo è il campo "[!UICONTROL id]" nel file JSON delle credenziali client.</td>
              </tr>
              <tr>
                  <td role="rowheader">ID organizzazione [!UICONTROL]</td>
                  <td class="">Immetti l'ID della tua organizzazione. Questo è il campo "[!UICONTROL org]" nel file JSON delle credenziali client.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta-ambito]</td>
                  <td>Immetti i Meta-ambiti generati nell'installazione di [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Chiave privata]</td>
                  <td>Immetti la chiave privata generata vince la configurazione [!UICONTROL Server-to-server]. Per estrarre la chiave privata, fai clic su [!UICONTROL Extract], quindi immetti il file da estrarre e la password per il file.</td>
              </tr>
          </tbody>
      </table>


### Configura la connessione per [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Nome connessione]</td>
                <td>
                    <p>Immettere un nome per la connessione</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL dell'istanza senza barra finale]</td>
                <td>Immetti l’URL per il tuo [!DNL Adobe Experience Manager] istanza. Non includere una barra <code>/</code> alla fine dell’URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Immetti il nome utente per il [!DNL AEM Assets] account utilizzato da questa connessione.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Immetti la password per il [!DNL AEM Assets] account utilizzato da questa connessione.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] moduli e relativi campi

Quando si configura [!DNL Adobe Experience Manager Essentials] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Experience Manager Essentials] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copiare una cartella o una risorsa]

Questo modulo di azione copia una cartella o una risorsa in un’altra posizione nel tuo account Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se vuoi copiare una cartella o una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella] / [!UICONTROL Selezione risorse]</td> 
   <td>Seleziona o mappa la cartella o la risorsa da copiare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percorso di Destinazione]</td> 
   <td>Seleziona o mappa il percorso della nuova cartella o risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome della cartella copiata] / [!UICONTROL risorsa]</td> 
   <td>Immetti un nome per la nuova cartella o risorsa. Nome della cartella visualizzato in [!DNL Adobe Experience Manager Assets] è uguale al nome originale. Il nome immesso viene visualizzato nell’URL della nuova cartella o risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia elementi figlio]</td> 
   <td>Abilita questa opzione per copiare le sottocartelle o le risorse all’interno della cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sovrascrivi]</td> 
   <td>Abilita questa opzione per sovrascrivere qualsiasi cartella o risorsa nella posizione di destinazione con lo stesso nome della cartella o della risorsa da copiare.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare un record]

Questo modulo di azione crea una cartella o un commento di risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di oggetto]</td> 
   <td> <p>Seleziona se desideri creare una cartella o un commento su una risorsa.</p> 
    <ul> 
     <li> <p>[!UICONTROL Cartella]</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Immettere un nome per la cartella. Questo nome verrà visualizzato nel percorso del file, quindi non deve includere spazi o altri caratteri. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Inserisci un titolo per la cartella, che può essere visualizzato al posto del nome.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset comment]</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p>[!UICONTROL Selezione risorse]</p> <p>Seleziona o mappa l’ID della risorsa a cui desideri aggiungere un commento.</p> </li> 
       <li> <p>[!UICONTROL Commento]</p> <p>Inserisci il testo del commento.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina una cartella, una risorsa o un rendering.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se eliminare una cartella, una risorsa o un rendering.</p> 
    <ul> 
     <li> <p>[!UICONTROL Cartella]</p> <p>Selezionare la cartella da eliminare selezionando le cartelle nel relativo percorso.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Seleziona la risorsa selezionando le cartelle nel relativo percorso, quindi la risorsa da eliminare.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Seleziona il rendering selezionando le cartelle nel relativo percorso.</p> <p>Immettere o mappare il nome del rendering.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ottenere un elenco di cartelle]

Questo modulo di azione recupera una rappresentazione di una cartella esistente e delle relative entità secondarie (cartelle o risorse).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Seleziona o mappa la cartella da recuperare. Per aggiungere sottocartelle al percorso, fai clic sull’icona più e seleziona la sottocartella.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo di azione effettua una chiamata API personalizzata al [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo al [!DNL Adobe Experience Manager] URL di base.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Immetti la stringa di query della richiesta. Per ogni coppia chiave/valore, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti la [!UICONTROL Key] e il [!UICONTROL Value].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Spostare una cartella o una risorsa]

Questo modulo di azione sposta la risorsa o la cartella nel percorso specificato in una nuova posizione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se vuoi spostare una cartella o una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella] / [!UICONTROL Risorsa]</td> 
   <td>Seleziona o mappa la cartella o la risorsa da spostare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percorso di Destinazione]</td> 
   <td>Seleziona o mappa il percorso della posizione in cui desideri spostare la cartella o la risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome della cartella spostata] / [!UICONTROL risorsa]</td> 
   <td>Immetti un nuovo nome per la cartella o la risorsa spostata. Nome della cartella visualizzato in [!DNL Adobe Experience Manager Assets] è uguale al nome originale. Il nome immesso viene visualizzato nell’URL della cartella o della risorsa spostata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sovrascrivi]</td> 
   <td>Abilita questa opzione per sovrascrivere qualsiasi cartella o risorsa nella posizione di destinazione con lo stesso nome della cartella o della risorsa da copiare.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un record esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se eliminare i metadati delle risorse o il rendering di una risorsa.</p> 
    <ul> 
     <li> <p>[!UICONTROL Metadati risorsa]</p> 
      <ul> 
       <li> <p>Seleziona la risorsa per la quale vuoi aggiornare i metadati.</p> </li> 
       <li> <p>Inserisci il nuovo titolo della risorsa.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Rendering di risorse]</p> 
      <ul> 
       <li> <p>Seleziona la risorsa per la quale vuoi aggiornare il rendering.</p> </li> 
       <li> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Caricare una risorsa]

Questo modulo di azione carica una risorsa nel tuo [!DNL Adobe Experience Manager Assets] conto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinazione]</td> 
   <td> <p>Seleziona la cartella in cui desideri caricare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Immettere o mappare il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>
