---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhook
description: Un webhook è una chiamata HTTP attivata da un evento. È possibile utilizzare i webhook per attivare moduli di trigger istantanei. Qualsiasi applicazione connessa a Internet e che consente richieste HTTP può inviare webhook ad Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1391'
ht-degree: 0%

---

# Webhook

Un webhook è una chiamata HTTP attivata da un evento. È possibile utilizzare i webhook per attivare moduli di trigger istantanei. Qualsiasi applicazione connessa a Internet e che consente richieste HTTP può inviare webhook ad Adobe Workfront Fusion.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Usa un webhook in [!DNL Workfront Fusion]

>[!NOTE]
>
>Per chiamare un webhook di terze parti (un webhook in uscita) utilizzare uno dei moduli HTTP. Per ulteriori informazioni, consulta [Moduli HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Per utilizzare un webhook per collegare un&#39;app a [!DNL Workfront Fusion]:

1. Aggiungi il **[!UICONTROL Webhook]** >**[!UICONTROL Webhook personalizzato]** modulo trigger istantaneo al tuo scenario.

1. Fai clic su **[!UICONTROL Aggiungi]** accanto al campo Webhook e immettere un nome per il nuovo webhook.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**.
1. In **[!UICONTROL Restrizioni IP]** immetti un elenco separato da virgole degli indirizzi IP da cui il modulo può accettare i dati.
1. Fai clic su **[!UICONTROL Salva]**

Dopo aver creato un webhook, viene visualizzato un URL univoco. Questo è l&#39;indirizzo dove il webhook invia dati. Workfront Fusion convalida i dati inviati a questo indirizzo, quindi li trasmette per l&#39;elaborazione nello scenario.

>[!NOTE]
>
>Una volta creato un webhook, puoi utilizzarlo in più scenari alla volta.

### Configurare la struttura dati del webhook {#configure-the-webhook-s-data-structure}

Al fine di riconoscere la struttura dei dati del payload in arrivo, [!DNL Workfront Fusion] analizza i dati di esempio inviati all’indirizzo visualizzato. Puoi fornire i dati di esempio effettuando una modifica nel servizio o nell’app che renderà quel servizio o l’app chiamata il webhook. Ad esempio, è possibile rimuovere un file.

Oppure puoi seguire i passaggi seguenti per inviare i dati di esempio tramite il [!UICONTROL HTTP] > [!UICONTROL Fai una richiesta] modulo .

1. Crea un nuovo scenario con il **[!UICONTROL HTTP]** > **[!UICONTROL Fai una richiesta]** modulo

1. Configura il modulo con i seguenti valori:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Inserisci l'URL del webhook. Puoi trovare questo URL nel modulo Webhook che hai usato per configurare il webhook.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL, Metodo] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di contenuto]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Richiedi contenuto]</td> 
      <td><p>JSON non elaborato previsto nel webhook</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Apri lo scenario con il [!UICONTROL Webhook] in una scheda o in una finestra del browser separata.
1. Nel modulo dei webhook, fai clic su **[!UICONTROL Rideterminare la struttura dati]**.

   Non è necessario scollegare altri moduli dal modulo webhooks.

1. Passa allo scenario con [!UICONTROL HTTP] modulo ed eseguilo.
1. Torna allo scenario con il modulo Webhooks.

   A &quot;[!UICONTROL Determinato]&quot; messaggio significa che il modulo ha determinato correttamente la struttura dei dati.

   ![](assets/successfully-determined-350x175.png)

1. Fai clic su **[!UICONTROL OK]** per salvare la struttura dati.

   Gli elementi del webhook sono ora disponibili nel pannello di mappatura per l’utilizzo con i moduli successivi nello scenario.

## Coda

Se un webhook riceve i dati e non c&#39;è uno scenario attivo che prevede tali dati, i dati vengono memorizzati nella coda. Una volta attivato lo scenario, elabora tutti i bundle in attesa nella coda sequenzialmente.

>[!IMPORTANT]
>
>Le code di Webhook sono condivise tra scenari che utilizzano lo stesso webhook. Se uno degli scenari è disabilitato, tutti i dati in arrivo vengono mantenuti nella coda.

## Formati di dati in arrivo supportati

[!DNL Workfront Fusion] supporta 3 formati di dati in arrivo: [!UICONTROL Stringa query], [!UICONTROL Dati modulo] e [!UICONTROL JSON].

[!DNL Workfront Fusion] convalida tutti i dati in arrivo rispetto alla struttura dati selezionata. Quindi, a seconda delle impostazioni dello scenario, i dati vengono memorizzati nella coda per l’elaborazione, oppure vengono elaborati immediatamente.

Se una parte dei dati non supera la convalida, [!DNL Workfront Fusion] restituisce un codice di stato HTTP 400 e specifica, nel corpo della risposta HTTP, il motivo per cui i dati in arrivo non sono riusciti nei controlli di convalida. Se la convalida dei dati in arrivo ha esito positivo, Workfront Fusion restituisce un &quot;[!UICONTROL 200 accettati]&quot; stato.

* [[!UICONTROL Stringa query]](#query-string)
* [[!UICONTROL Dati modulo]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Stringa query]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Dati modulo]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Dati modulo multiparte

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

Per ricevere i file codificati con `multipart/form-data`, devi configurare una struttura dati con un `collection` campo di testo contenente i campi nidificati `name`, `mime`e `data`. Il campo `name` è un `text` digita e contiene il nome del file caricato. La `mime` è un `text` digita e contiene un file in formato MIME. Il campo `data` è un `buffer` digitare e contiene dati binari per il file che si sta trasferendo.

Per ulteriori informazioni sul formato MIME, vedi [Moduli MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Se desideri accedere al JSON originale, abilita il pass-through JSON durante la configurazione del webhook.
>
>1. Fai clic su **[!UICONTROL Aggiungi]** per aggiungere un nuovo webhook.
>1. Fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.
>1. Fai clic su **[!UICONTROL Passaggio-through JSON]**.

>


## Intestazioni Webhook

Per accedere alle intestazioni del webhook, abilita le intestazioni di richiesta Get durante la configurazione del webhook.

1. Fai clic su **[!UICONTROL Aggiungi]** per aggiungere un nuovo webhook.
1. Fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.
1. Fai clic su **[!UICONTROL Ottieni intestazioni richieste]**.

Puoi estrarre un particolare valore di intestazione con la combinazione di `map()` e `get()` funzioni.

>[!INFO]
>
>**Esempio:**
>
>L&#39;esempio seguente mostra una formula che estrae il valore del `authorization` intestazione dal `Headers[]` array. La formula viene utilizzata in un filtro che confronta il valore estratto con il testo specificato per passare solo i webhook in presenza di una corrispondenza.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Per ulteriori informazioni su come ottenere un elemento di un array con una determinata chiave, vedi [Mappare un elemento di un array con una determinata chiave](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) nell&#39;articolo [Mappare le informazioni da un modulo all&#39;altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Risposta ai webhook

La risposta predefinita a una chiamata webhook è il testo &quot;Accettato&quot;. La risposta viene restituita all&#39;app che ha chiamato il webhook durante l&#39;esecuzione del modulo Custom Webhook.

* [Verifica la risposta a un webhook](#test-the-response-to-a-webhook)
* [Esempio di risposta HTML](#html-response-example)
* [Esempio di reindirizzamento](#redirect-example)

### Verifica la risposta a un webhook

1. Includi il **[!UICONTROL Webhook personalizzato]** nel tuo scenario.
1. Aggiungi un nuovo webhook al modulo.
1. Copia l&#39;URL del webhook negli appunti.
1. Esegui lo scenario.

   Icona del fulmine [!UICONTROL Webhook personalizzato] Il modulo cambia in punti rotanti. Questo mostra che il modulo è in attesa della chiamata webhook.

1. Apri una nuova finestra del browser, incolla l’URL copiato nella barra degli indirizzi e premi **[!UICONTROL Invio]**.

   La [!UICONTROL Webhook personalizzato] Il modulo viene attivato e il browser visualizzerà una nuova pagina.

Se si desidera personalizzare la risposta del webhook, utilizzare il modulo Webhook Response.

La configurazione del modulo contiene due campi: [!UICONTROL Stato] e [!UICONTROL Corpo].

* La [!UICONTROL Stato] il campo contiene codici di stato della risposta HTTP come 2xx per il successo (ad esempio, `200` per OK, 3xx per Reindirizzamento (ad esempio, `307` per il reindirizzamento temporaneo), 4xx per gli errori client (ad esempio, `400` per Bad Request) e così via.

* La [!UICONTROL Corpo] Il campo contiene tutto ciò che verrà accettato dalla chiamata del webhook. Può essere testo semplice, HTML, XML, JSON e così via.

   >[!TIP]
   >
   >Consigliamo di impostare `Content-Type` intestazione del tipo MIME corrispondente: `text/plain` per testo normale, `text/html` per HTML, `application/json` per JSON, `application/xml` per XML e così via. Per ulteriori informazioni sui tipi MIME, vedi [Moduli MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

Il timeout per l’invio di una risposta è di 40 secondi. Se la risposta non è disponibile entro tale periodo, Workfront Fusion restituisce uno stato &#39;200 Accettate&#39;.

### Esempio di risposta HTML

>[!INFO]
>
>**Esempio:**
>
>Configura le [!UICONTROL Risposta Webhook] modulo come segue:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Codice di stato HTTP 2xx con successo, ad esempio 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>Codice HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Chiave</strong>: Tipo di contenuto</li> 
&gt;     <li><strong>Valore</strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Questo produrrà una risposta HTML che verrà visualizzata in un browser Web:
>
>![](assets/html-response-350x70.png)

### Esempio di reindirizzamento

>[!INFO]
>
>**Esempio:** Configura le [!UICONTROL Risposta Webhook] modulo come segue:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Codice di stato HTTP di reindirizzamento 3xx, ad esempio 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Posizione</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: URL a cui si desidera reindirizzare.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Disattivazione Webhook

I webhook vengono disattivati automaticamente se si applica una delle seguenti funzioni:

* Il webhook non è stato collegato ad alcuno scenario per più di 5 giorni
* Il webhook viene utilizzato solo in scenari inattivi, che sono stati inattivi per più di 30 giorni.

I webhook disattivati vengono eliminati e non registrati automaticamente se non sono connessi ad alcuno scenario e sono stati disattivati per più di 30 giorni.


## Risoluzione dei problemi

### Elementi mancanti nel pannello di mappatura

Se mancano alcuni elementi nel pannello di mappatura nella configurazione dei moduli che seguono [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato] modulo, fai clic su **[!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato]** modulo per aprire la configurazione e fare clic su **[!UICONTROL Rideterminazione della struttura dati]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Quindi segui i passaggi descritti nella sezione [Configurare la struttura dati del webhook](#configure-the-webhook-s-data-structure) in questo articolo.
