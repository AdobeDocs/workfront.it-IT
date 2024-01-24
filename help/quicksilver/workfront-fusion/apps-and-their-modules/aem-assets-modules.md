---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Experience Manager Assets
description: Con il [!DNL Adobe Experience Manager Assets] connettore per [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] creare, caricare e aggiornare le risorse, nonché copiare o spostare cartelle e risorse.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] moduli

Con il [!DNL Adobe Experience Manager Assets] connettore per [!DNL Adobe Workfront Fusion], puoi avviare uno scenario basato sugli eventi nel tuo [!DNL Adobe Experience Manager Assets] creare, caricare e aggiornare le risorse, nonché copiare o spostare cartelle e risorse.

Per un’introduzione al connettore Adobe Experience Manager Assets, consulta:

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

* Devi avere un [!DNL Adobe Experience Manager Assets] per utilizzare questi moduli.
* È necessario configurare [!UICONTROL Server-to-server] flusso in [!DNL Adobe Developer console].

  Per istruzioni sull&#39;impostazione [!UICONTROL Server-to-server] flusso in [!DNL Adobe Developer console], vedi [Generazione dei token di accesso per le API lato server](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Per creare una connessione per [!DNL Adobe Experience Manager Assets] moduli:

1. Clic [!UICONTROL Aggiungi] accanto al [!UICONTROL Connessione] casella.

2. Selezionare il tipo di connessione che si sta creando:

   * **[!DNL AEM Assets as a Cloud Service]**

     Questa configurazione richiede informazioni da [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Questa configurazione richiede un nome utente e una password.

3. Compila i campi per il tipo di connessione che stai creando.

   Per [!DNL AEM Assets as a Cloud Service], vedi [Configurare la connessione per [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Per [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]), vedi [Configurare la connessione per [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.


### Configurare la connessione per [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>Le informazioni per questi campi vengono generate durante la configurazione di [!UICONTROL Server-to-server] flusso sul [!DNL Adobe Developer Console]. Questi valori si trovano nel file JSON delle credenziali del servizio generato come parte di tale configurazione.
>
>Per istruzioni sull&#39;impostazione [!UICONTROL Server-to-server] flusso sul [!UICONTROL Console Adobe Developer], vedi [Generazione dei token di accesso per le API lato server](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


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
                  <td role="rowheader">[!UICONTROL URL istanza senza una barra finale]</td>
                  <td>Immetti l’URL per il tuo [!DNL Adobe Experience Manager] dell'istanza. Non includere una barra <code>/</code> alla fine dell’URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID client]</td>
                  <td>Immettere l'ID client generato nell'installazione di [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Segreto client]</td>
                  <td>Immettere il segreto client generato nell'installazione di [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID account tecnico]</td>
                  <td>Immetti l’ID dell’account tecnico. Campo "[!UICONTROL id]" nel file JSON delle credenziali client.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID organizzazione]</td>
                  <td class="">Immetti l’ID della tua organizzazione. Campo "[!UICONTROL org]" nel file JSON delle credenziali client.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta Ambiti]</td>
                  <td>Immettere i metadati generati nella configurazione di [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Chiave privata]</td>
                  <td>Immetti la chiave privata generata per vincere l'installazione di [!UICONTROL Server-to-Server]. Per estrarre la chiave privata, fare clic su [!UICONTROL Extract], quindi immettere il file da estrarre e la password per il file.</td>
              </tr>
          </tbody>
      </table>


### Configurare la connessione per [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

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
                <td role="rowheader">[!UICONTROL URL istanza senza una barra finale]</td>
                <td>Immetti l’URL per il tuo [!DNL Adobe Experience Manager] dell'istanza. Non includere una barra <code>/</code> alla fine dell’URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Immetti il nome utente per [!DNL AEM Assets] account utilizzato da questa connessione.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Immetti la password per [!DNL AEM Assets] account utilizzato da questa connessione.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] moduli e relativi campi

Quando si configura [!DNL Adobe Experience Manager Essentials] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Experience Manager Essentials] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copiare una cartella o una risorsa]

Questo modulo di azione copia una cartella o una risorsa in un’altra posizione nell’account Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se desideri copiare una cartella o una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>Seleziona o mappa la cartella o la risorsa da copiare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percorso di destinazione]</td> 
   <td>Seleziona o mappa il percorso della nuova cartella o risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome della cartella copiata] / [!UICONTROL risorsa]</td> 
   <td>Immetti un nome per la nuova cartella o risorsa. Nome della cartella visualizzato in [!DNL Adobe Experience Manager Assets] corrisponde al nome originale. Il nome immesso viene visualizzato nell’URL della nuova cartella o risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia elementi figlio]</td> 
   <td>Abilita questa opzione per copiare eventuali sottocartelle o risorse all’interno della cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Abilita questa opzione per sovrascrivere eventuali cartelle o risorse nella posizione di destinazione con lo stesso nome della cartella o risorsa da copiare.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare un record]

Questo modulo di azione crea una cartella o un commento alla risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di oggetto]</td> 
   <td> <p>Seleziona se desideri creare una cartella o un commento su una risorsa.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Immettere un nome per la cartella. Questo nome verrà visualizzato nel percorso del file, pertanto non deve includere spazi o altri caratteri. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Immetti un titolo per la cartella, che può essere visualizzato al posto del nome.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Commento risorsa]</p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p>[!UICONTROL Selezione risorsa]</p> <p>Seleziona o mappa l’ID della risorsa a cui desideri aggiungere un commento.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>Immettere il testo del commento.</p> </li> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se desideri eliminare una cartella, una risorsa o una rappresentazione.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Seleziona la cartella da eliminare selezionando le cartelle nel relativo percorso.</p> </li> 
     <li> <p>[!UICONTROL Risorsa] </p> <p>Seleziona la risorsa selezionando le cartelle nel suo percorso, quindi la risorsa da eliminare.</p> </li> 
     <li> <p>[!UICONTROL Rendering]</p> <p>Seleziona la rappresentazione selezionando le cartelle nel relativo percorso.</p> <p>Immettere o mappare il nome della rappresentazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ottieni un elenco di cartelle]

Questo modulo di azione recupera una rappresentazione di una cartella esistente e delle relative entità secondarie (cartelle o risorse).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Seleziona o mappa la cartella da recuperare. Per aggiungere sottocartelle al percorso, fare clic sull'icona più e selezionare la sottocartella.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immetti un percorso relativo al [!DNL Adobe Experience Manager] URL di base.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query] </td> 
   <td> <p>Immettere la stringa di query richiesta. Per ogni coppia chiave/valore, fai clic su <b>[!UICONTROL Add item]</b> e immettere la chiave [!UICONTROL] e il valore [!UICONTROL].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se desideri spostare una cartella o una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Assets]</td> 
   <td>Seleziona o mappa la cartella o la risorsa da spostare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percorso di destinazione]</td> 
   <td>Seleziona o mappa il percorso del percorso in cui desideri spostare la cartella o la risorsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome della cartella spostata] / [!UICONTROL risorsa]</td> 
   <td>Immetti un nuovo nome per la cartella o la risorsa spostata. Nome della cartella visualizzato in [!DNL Adobe Experience Manager Assets] corrisponde al nome originale. Il nome immesso viene visualizzato nell’URL della cartella o della risorsa spostata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Abilita questa opzione per sovrascrivere eventuali cartelle o risorse nella posizione di destinazione con lo stesso nome della cartella o risorsa da copiare.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona se desideri eliminare i metadati di una risorsa o il rendering di una risorsa.</p> 
    <ul> 
     <li> <p>[!UICONTROL Metadati risorsa]</p> 
      <ul> 
       <li> <p>Seleziona la risorsa per la quale desideri aggiornare i metadati.</p> </li> 
       <li> <p>Immetti il nuovo titolo della risorsa.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Rendering risorsa]</p> 
      <ul> 
       <li> <p>Seleziona la risorsa per la quale desideri aggiornare la rappresentazione.</p> </li> 
       <li> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Caricare una risorsa]

Questo modulo di azione carica una risorsa sul tuo [!DNL Adobe Experience Manager Assets] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Adobe Experience Manager Assets] account a [!DNL Workfront Fusion], vedi <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Adobe Experience Manager Assets] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination]</td> 
   <td> <p>Seleziona la cartella in cui desideri caricare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Immettere o mappare il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>
