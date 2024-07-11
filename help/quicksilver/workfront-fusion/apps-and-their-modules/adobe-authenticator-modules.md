---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Modulo Adobe Authenticator
description: Con il modulo Adobe Authenticator, puoi connetterti a qualsiasi prodotto Adobe con un’API, utilizzando una singola connessione.
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 1%

---

# Moduli Adobe Authenticator

Il modulo Adobe Authenticator ti consente di connettersi a qualsiasi API Adobe utilizzando una singola connessione. Ciò consente di connettersi più facilmente a prodotti in Adobe che non dispongono ancora di un connettore Fusion dedicato.

Il vantaggio rispetto ai moduli HTTP è che puoi creare una connessione, come in un’app dedicata.

Per visualizzare un elenco delle API Adobe disponibili, consulta [API ADOBE](https://developer.adobe.com/apis). Puoi utilizzare solo le API a cui sei assegnato.

## Requisiti di accesso

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano</td>
      <td>
        <p>Nuovo: Qualsiasi</p><p>Oppure</p><p>Corrente: [!UICONTROL Pro] o versione successiva</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licenza</td>
      <td>
        <p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza</td>
      <td>
   <p>Requisiti attuali della licenza Fusion: no [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza Fusion legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Prodotto</td>
      <td>
   <p>Nuovo piano Workfront: se hai [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Piano Workfront corrente: l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td>
    </tr>
  </tbody>
</table>

## Prerequisiti

* Devi avere accesso al prodotto di Adobe a cui vuoi collegare il modulo.
* Devi avere accesso a Adobe Developer Console.
* In Adobe Developer Console è necessario disporre di un progetto che includa l’API a cui desideri che il modulo si connetta. È possibile:

   * Crea un nuovo progetto con l’API.

     Oppure
   * Aggiungi l’API a un progetto esistente.

  Per informazioni sulla creazione o l’aggiunta di un’API a un progetto su Adobe Developer Console, consulta [Creare un progetto](https://developer.adobe.com/dep/guides/dev-console/create-project/) nella documentazione di Adobe.

## Creare una connessione

Una connessione Adobe Authenticator si connette a un singolo progetto sul Adobe Developer Console. Per utilizzare la stessa connessione per più API Adobe, aggiungi le API allo stesso progetto e crea una connessione a tale progetto.

Puoi creare connessioni separate a progetti separati, ma non puoi utilizzare una connessione per accedere a un’API che non si trova nel progetto specificato in tale connessione.

>[!IMPORTANT]
>
>Con il connettore Adobe Authenticator puoi scegliere se effettuare una connessione server-to-server OAuth o una connessione con account di servizio (JWT). Adobe ha dichiarato obsolete le credenziali JWT, che cesseranno di funzionare dopo il 1° gennaio 2025. **Pertanto, consigliamo vivamente di creare connessioni OAuth.**
>
>Per ulteriori informazioni su questi tipi di connessioni, vedi [Autenticazione da server a server](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) nella documentazione di Adobe

Per creare una connessione:

1. In qualsiasi modulo di Adobe Authenticator, fai clic su **Aggiungi** accanto al campo Connessione.
1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo di connessione]</td>
        <td>
          <p>Seleziona se desideri creare una connessione server-to-server OAuth o una connessione con un account di servizio (JWT).</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Nome connessione]</td>
        <td>
          <p>Immettere un nome per la connessione.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti il [!DNL Adobe] ID client. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il [!DNL Adobe] Segreto client. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Ambiti]</td>
        <td>Se hai selezionato una connessione OAuth, immetti gli ambiti necessari per questa connessione.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Immetti il [!DNL Adobe] ID account tecnico. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID organizzazione]</td>
        <td>Se hai selezionato una connessione JWT, immetti il tuo [!DNL Adobe] ID organizzazione. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Ambiti]</td>
        <td>Se hai selezionato una connessione JWT, inserisci i meta-ambiti necessari per questa connessione. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Se hai selezionato una connessione JWT, immetti la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
          <p>Per estrarre la chiave privata o il certificato:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selezionare il tipo di file da estrarre.</p>
            </li>
            <li value="3">
              <p>Seleziona il file che contiene la chiave privata o il certificato.</p>
            </li>
            <li value="4">
              <p>Immettere la password per il file.</p>
            </li>
            <li value="5">
              <p>Clic <b>[!UICONTROL Salva]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL di base]</td>
        <td>È necessario aggiungere gli URL di base consentiti dall'autenticatore. Quando utilizzi il modulo di chiamata Make a API personalizzata più avanti nello scenario, aggiungi un percorso relativo all’URL scelto. Immettendo gli URL qui, puoi controllare a cosa può connettersi il modulo di chiamata API Make a, aumentando così la sicurezza.<p>Per ogni URL di base che desideri aggiungere all’autenticatore, fai clic su <b>Aggiungi elemento</b> e inserisci l’URL di base.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL autenticazione]</td>
        <td>Lascia questo campo vuoto per utilizzare l’URL standard di autenticazione Adobe IMS di <code>https://ims-na1.adobelogin.com</code>. Se non utilizzi Adobe IMS per l’autenticazione, immetti l’URL da utilizzare per l’autenticazione.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Seleziona se ti connetti a un ambiente di produzione o non di produzione.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Specificare se ci si connette a un account di servizio o a un account personale.</td>
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## Modulo

### Effettuare una chiamata API personalizzata

Questo modulo di azione ti consente di effettuare una chiamata a qualsiasi API Adobe.

>[!TIP]
>
>Devi immettere l’intero URL per l’API a cui desideri connetterti. Questo modulo non accetta URL relativi.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione al modulo Adobe Authenticator, consulta <a href="#create-a-connection" class="MCXref xref" >Creare una connessione</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Inserisci l’intero URL del punto API a cui desideri connetterti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stringa Di Query]  </td>
      <td>
        <p>Immettere la stringa di query richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere il numero massimo di risultati che il modulo deve restituire in un ciclo di esecuzione.</p>
      </td>
    </tr>
  </tbody>
</table>
