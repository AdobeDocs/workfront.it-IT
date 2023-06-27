---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhook
description: Un webhook è una chiamata HTTP attivata da un evento. Puoi utilizzare i webhook per attivare moduli di attivazione istantanea. Qualsiasi applicazione connessa a Internet e che consenta le richieste HTTP può inviare webhook ad Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Webhook

Un webhook è una chiamata HTTP attivata da un evento. Puoi utilizzare i webhook per attivare moduli di attivazione istantanea. Qualsiasi applicazione connessa a Internet e che consenta le richieste HTTP può inviare webhook ad Adobe Workfront Fusion.

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

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Utilizzare un webhook in [!DNL Workfront Fusion]

>[!NOTE]
>
>Per chiamare un webhook di terze parti (un webhook in uscita) utilizza uno dei moduli HTTP. Per ulteriori informazioni, consulta [Moduli HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Per utilizzare un webhook per connettere un’app a [!DNL Workfront Fusion]:

1. Aggiungi il **[!UICONTROL Webhook]** >**[!UICONTROL Webhook personalizzato]** modulo di attivazione istantanea per lo scenario.

1. Clic **[!UICONTROL Aggiungi]** accanto al campo webhook e immettere un nome per il nuovo webhook.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**.
1. In **[!UICONTROL Restrizioni IP]** , inserisci un elenco separato da virgole degli indirizzi IP da cui il modulo può accettare i dati.
1. Fai clic su **[!UICONTROL Salva]**

Dopo aver creato un webhook, viene visualizzato un URL univoco. Questo è l’indirizzo a cui il webhook invia i dati. Workfront Fusion convalida i dati inviati a questo indirizzo, quindi li trasmette per l’elaborazione nello scenario.

>[!NOTE]
>
>Una volta creato un webhook, puoi utilizzarlo in più scenari alla volta.

### Configurare la struttura dati del webhook {#configure-the-webhook-s-data-structure}

Al fine di riconoscere la struttura dati del payload in ingresso, [!DNL Workfront Fusion] analizza i dati di esempio inviati all&#39;indirizzo visualizzato. Puoi fornire i dati di esempio apportando una modifica al servizio o all’app che farà sì che il servizio o l’app chiamino il webhook. Ad esempio, puoi rimuovere un file.

Oppure puoi seguire i passaggi seguenti per inviare i dati di esempio tramite il [!UICONTROL HTTP] > [!UICONTROL Fai una richiesta] modulo.

1. Crea un nuovo scenario con **[!UICONTROL HTTP]** > **[!UICONTROL Fai una richiesta]** modulo

1. Configura il modulo con i seguenti valori:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Immetti l’URL del webhook. È possibile trovare questo URL nel modulo [!UICONTROL Webhooks] utilizzato per configurare il webhook.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di corpo]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di contenuto]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contenuto richiesta]</td> 
      <td><p>JSON non elaborato previsto nel webhook</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Apri lo scenario con [!UICONTROL Webhook] in una scheda o finestra del browser separata.
1. Nel modulo webhooks, fai clic su **[!UICONTROL Rideterminare la struttura dei dati]**.

   Non è necessario scollegare altri moduli dal modulo webhooks.

1. Passa allo scenario con [!UICONTROL HTTP] ed eseguirlo.
1. Torna allo scenario con il modulo Webhooks.

   A &quot;[!UICONTROL Determinato correttamente]Il messaggio &quot;indica che il modulo ha determinato correttamente la struttura dati.

   ![](assets/successfully-determined-350x175.png)

1. Clic **[!UICONTROL OK]** per salvare la struttura dati.

   Gli elementi del webhook sono ora disponibili nel pannello di mappatura per l’utilizzo con i moduli successivi nello scenario.

## Coda

Se un webhook riceve dati e non esiste uno scenario attivo che preveda tali dati, questi vengono memorizzati nella coda. Una volta attivato lo scenario, elabora in sequenza tutti i bundle in attesa nella coda.

>[!IMPORTANT]
>
>Le code dei webhook sono condivise tra scenari che utilizzano lo stesso webhook. Se uno degli scenari è disattivato, tutti i dati in arrivo vengono mantenuti nella coda.

## Formati di dati in arrivo supportati

[!DNL Workfront Fusion] supporta 3 formati di dati in arrivo: [!UICONTROL Stringa di query], [!UICONTROL Dati modulo] e [!UICONTROL JSON].

[!DNL Workfront Fusion] convalida tutti i dati in arrivo in base alla struttura dati selezionata. Quindi, a seconda delle impostazioni dello scenario, i dati vengono memorizzati nella coda per l’elaborazione o vengono elaborati immediatamente.

Se una parte qualsiasi dei dati non supera la convalida, [!DNL Workfront Fusion] restituisce un codice di stato HTTP 400 e specifica, nel corpo della risposta HTTP, il motivo per cui i controlli di convalida dei dati in arrivo non sono riusciti. Se la convalida dei dati in arrivo ha esito positivo, Workfront Fusion restituisce un &quot;[!UICONTROL 200 accettati]&quot;.

* [[!UICONTROL Stringa di query]](#query-string)
* [[!UICONTROL Dati modulo]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Stringa di query]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Dati modulo]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Dati modulo multipart

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

Per ricevere i file codificati con `multipart/form-data`, è necessario configurare una struttura dati con `collection` campo di tipo contenente i campi nidificati `name`, `mime`, e `data`. Il campo `name` è un `text` e contiene il nome del file caricato. Il `mime` è un `text` e contiene un file in formato MIME. Il campo `data` è un `buffer` e contiene dati binari per il file da trasferire.

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
>1. Clic **[!UICONTROL Aggiungi]** per aggiungere un nuovo webhook.
>1. Clic **[!UICONTROL Mostra impostazioni avanzate]**.
>1. Clic **[!UICONTROL Pass-through JSON]**.
>

## Intestazioni webhook

Per accedere alle intestazioni del webhook, abilita Ottieni intestazioni di richiesta durante la configurazione del webhook.

1. Clic **[!UICONTROL Aggiungi]** per aggiungere un nuovo webhook.
1. Clic **[!UICONTROL Mostra impostazioni avanzate]**.
1. Clic **[!UICONTROL Ottieni intestazioni richiesta]**.

Puoi estrarre un particolare valore di intestazione con la combinazione di `map()` e `get()` funzioni.

>[!INFO]
>
>**Esempio:**
>
>L’esempio seguente mostra una formula che estrae il valore del `authorization` intestazione da `Headers[]` array. La formula viene utilizzata in un filtro che confronta il valore estratto con il testo specificato per trasmettere solo i webhook in caso di corrispondenza.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Per ulteriori informazioni su come ottenere un elemento di un array con una determinata chiave, consulta [Mappare l’elemento di un array con una determinata chiave](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) nell’articolo [Mappare le informazioni da un modulo all’altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Risposta ai webhook

La risposta predefinita a una chiamata al webhook è il testo &quot;Accepted&quot; (Accettato). La risposta viene restituita all’app che ha chiamato il webhook durante l’esecuzione del modulo Webhook personalizzato.

* [Verificare la risposta a un webhook](#test-the-response-to-a-webhook)
* [Esempio di risposta HTML](#html-response-example)
* [Esempio di reindirizzamento](#redirect-example)

### Verificare la risposta a un webhook

1. Includi **[!UICONTROL Webhook personalizzato]** nel tuo scenario.
1. Aggiungi un nuovo webhook al modulo.
1. Copia l’URL del webhook negli Appunti.
1. Esegui lo scenario.

   L&#39;icona del fulmine sul [!UICONTROL Webhook personalizzato] Il modulo diventa un punto in rotazione. Questo mostra che il modulo è ora in attesa della chiamata del webhook.

1. Apri una nuova finestra del browser, incolla l’URL copiato nella barra degli indirizzi e premi **[!UICONTROL Invio]**.

   Il [!UICONTROL Webhook personalizzato] viene attivato e il browser visualizza una nuova pagina.

Se desideri personalizzare la risposta del webhook, utilizza il modulo Risposta del webhook.

La configurazione del modulo contiene due campi: [!UICONTROL Stato] e [!UICONTROL Corpo].

* Il [!UICONTROL Stato] contiene codici di stato di risposta HTTP come 2xx per il successo (ad esempio, `200` per OK), 3xx per Redirection (ad esempio, `307` per il reindirizzamento temporaneo), 4xx per gli errori del client (ad esempio, `400` per la richiesta non valida) e così via.

* Il [!UICONTROL Corpo] contiene tutto ciò che verrà accettato dalla chiamata del webhook. Può essere testo semplice, HTML, XML, JSON e così via.

  >[!TIP]
  >
  >È consigliabile impostare `Content-Type` intestazione al tipo MIME corrispondente: `text/plain` per il testo normale, `text/html` per HTML, `application/json` per JSON, `application/xml` per XML e così via. Per ulteriori informazioni sui tipi MIME, vedi [Moduli MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

Il timeout per l’invio di una risposta è di 40 secondi. Se la risposta non è disponibile entro tale periodo, Workfront Fusion restituisce lo stato &quot;200 Accepted&quot; (Accettato).

### Esempio di risposta HTML

>[!INFO]
>
>**Esempio:**
>
>Configurare [!UICONTROL Risposta webhook] come segue:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Stato] </td> 
&gt;   <td> <p>Codice di stato HTTP 2xx, ad esempio 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>Codice HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Chiave</strong>: tipo di contenuto</li> 
&gt;     <li><strong>Valore</strong>: testo/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>In questo modo viene generata una risposta di HTML che viene visualizzata in un browser web:
>
>![](assets/html-response-350x70.png)

### Esempio di reindirizzamento

>[!INFO]
>
>**Esempio:** Configurare [!UICONTROL Risposta webhook] come segue:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Stato] </td> 
&gt;   <td> <p>Codice di stato HTTP del reindirizzamento 3xx, ad esempio 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Posizione</li> 
&gt;     <li><strong>Valore [!UICONTROL]</strong>: URL a cui desideri reindirizzare.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Disattivazione webhook

I webhook vengono disattivati automaticamente se si applica una delle seguenti condizioni:

* Il webhook non è stato connesso ad alcuno scenario per più di 5 giorni
* Il webhook viene utilizzato solo in scenari inattivi, che sono stati inattivi per più di 30 giorni.

I webhook disattivati vengono eliminati e annullati automaticamente se non sono connessi ad alcun scenario e se sono in stato disattivato da oltre 30 giorni.


## Risoluzione dei problemi

### Elementi mancanti nel pannello di mappatura

Se nel pannello di mappatura mancano alcuni elementi nella configurazione dei moduli che seguono [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato] , fai clic sul pulsante **[!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato]** per aprire la relativa configurazione e fare clic su **[!UICONTROL Rideterminare la struttura dei dati]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Quindi segui i passaggi descritti nella sezione [Configurare la struttura dati del webhook](#configure-the-webhook-s-data-structure) in questo articolo.
