---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhook
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# Webhook



>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili negli articoli:
>
>* [Webhook](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/webhooks-updated.html)
>* [Configurare un webhook per un servizio Web senza un connettore](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

&#42;&#42;Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Utilizza un webhook in [!DNL Workfront Fusion]

>[!NOTE]
>
>Per chiamare un webhook di terze parti (un webhook in uscita) utilizza uno dei moduli HTTP. Per ulteriori informazioni, vedere [Moduli HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Per utilizzare un webhook per connettere un&#39;app a [!DNL Workfront Fusion]:

1. Aggiungi il modulo di attivazione immediata **[!UICONTROL Webhook]** >**[!UICONTROL Webhook personalizzato]** allo scenario.

1. Fai clic su **[!UICONTROL Aggiungi]** accanto al campo Webhook e immetti un nome per il nuovo webhook.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**.
1. Nel campo **[!UICONTROL Restrizioni IP]**, inserisci un elenco separato da virgole degli indirizzi IP da cui il modulo può accettare i dati.
1. Fai clic su **[!UICONTROL Salva]**

Dopo aver creato un webhook, viene visualizzato un URL univoco. Questo è l’indirizzo a cui il webhook invia i dati. Workfront Fusion convalida i dati inviati a questo indirizzo, quindi li trasmette per l’elaborazione nello scenario.

>[!NOTE]
>
>Una volta creato un webhook, puoi utilizzarlo in più scenari alla volta.

### Configurare la struttura dati del webhook {#configure-the-webhook-s-data-structure}

Per riconoscere la struttura dati del payload in ingresso, [!DNL Workfront Fusion] analizza i dati di esempio inviati all&#39;indirizzo visualizzato. Puoi fornire i dati di esempio apportando una modifica al servizio o all’app che farà sì che il servizio o l’app chiamino il webhook. Ad esempio, puoi rimuovere un file.

Oppure puoi seguire i passaggi seguenti per inviare i dati di esempio tramite il modulo [!UICONTROL HTTP] > [!UICONTROL Fai una richiesta].

1. Crea un nuovo scenario con il modulo **[!UICONTROL HTTP]** > **[!UICONTROL Invia una richiesta]**

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

1. Apri lo scenario con il modulo [!UICONTROL Webhooks] in una scheda o finestra del browser separata.
1. Nel modulo webhooks fare clic su **[!UICONTROL Ridetermina la struttura dati]**.

   Non è necessario scollegare altri moduli dal modulo webhooks.

1. Passa allo scenario con il modulo [!UICONTROL HTTP] ed eseguilo.
1. Torna allo scenario con il modulo Webhooks.

   Un messaggio &quot;[!UICONTROL correttamente determinato]&quot; indica che il modulo ha determinato correttamente la struttura dati.

   ![](assets/successfully-determined-350x175.png)

1. Fare clic su **[!UICONTROL OK]** per salvare la struttura dati.

   Gli elementi del webhook sono ora disponibili nel pannello di mappatura per l’utilizzo con i moduli successivi nello scenario.

## La coda del webhook

Se un webhook riceve dati e non esiste uno scenario attivo che preveda tali dati, questi vengono memorizzati nella coda. Una volta attivato lo scenario, elabora in sequenza tutti i bundle in attesa nella coda.

>[!IMPORTANT]
>
>Le code dei webhook sono condivise tra scenari che utilizzano lo stesso webhook. Se uno degli scenari è disattivato, tutti i dati in arrivo vengono mantenuti nella coda.

## Formati di dati in arrivo supportati

[!DNL Workfront Fusion] supporta 3 formati di dati in ingresso: [!UICONTROL Stringa query], [!UICONTROL Dati modulo] e [!UICONTROL JSON].

[!DNL Workfront Fusion] convalida tutti i dati in arrivo in base alla struttura dati selezionata. Quindi, a seconda delle impostazioni dello scenario, i dati vengono memorizzati nella coda per l’elaborazione o vengono elaborati immediatamente.

Se una parte qualsiasi dei dati non supera la convalida, [!DNL Workfront Fusion] restituisce un codice di stato HTTP 400 e specifica, nel corpo della risposta HTTP, il motivo per cui i dati in arrivo non hanno superato i controlli di convalida. Se la convalida dei dati in arrivo viene eseguita correttamente, Workfront Fusion restituirà lo stato &quot;[!UICONTROL 200 Accepted]&quot;.

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

Per ricevere i file codificati con `multipart/form-data`, è necessario configurare una struttura di dati con un campo di tipo `collection` contenente i campi nidificati `name`, `mime` e `data`. Il campo `name` è di tipo `text` e contiene il nome del file caricato. `mime` è un tipo `text` e contiene un file in formato MIME. Il campo `data` è di tipo `buffer` e contiene dati binari per il file da trasferire.

Per ulteriori informazioni sul formato MIME, vedere [Moduli MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

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
>1. Fare clic su **[!UICONTROL Mostra impostazioni avanzate]**.
>1. Fare clic su **[!UICONTROL pass-through JSON]**.
>

## Intestazioni webhook

Per accedere alle intestazioni del webhook, abilita Ottieni intestazioni di richiesta durante la configurazione del webhook.

1. Fai clic su **[!UICONTROL Aggiungi]** per aggiungere un nuovo webhook.
1. Fare clic su **[!UICONTROL Mostra impostazioni avanzate]**.
1. Fai clic su **[!UICONTROL Ottieni intestazioni richiesta]**.

È possibile estrarre un particolare valore di intestazione con la combinazione di `map()` e `get()` funzioni.

>[!INFO]
>
>**Esempio:**
>
>L&#39;esempio seguente mostra una formula che estrae il valore dell&#39;intestazione `authorization` dall&#39;array `Headers[]`. La formula viene utilizzata in un filtro che confronta il valore estratto con il testo specificato per trasmettere solo i webhook in caso di corrispondenza.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Per ulteriori informazioni su come ottenere un elemento di un array con una determinata chiave, vedere [Mappare l&#39;elemento di un array con una determinata chiave](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) nell&#39;articolo [Mappare le informazioni da un modulo all&#39;altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Risposta ai webhook

La risposta predefinita a una chiamata al webhook è il testo &quot;Accepted&quot; (Accettato). La risposta viene restituita all’app che ha chiamato il webhook durante l’esecuzione del modulo Webhook personalizzato.

* [Verifica la risposta a un webhook](#test-the-response-to-a-webhook)
* [Esempio di risposta HTML](#html-response-example)
* [Esempio di reindirizzamento](#redirect-example)

### Verificare la risposta a un webhook

1. Includi il modulo **[!UICONTROL Webhook personalizzato]** nello scenario.
1. Aggiungi un nuovo webhook al modulo.
1. Copia l’URL del webhook negli Appunti.
1. Esegui lo scenario.

   L&#39;icona del fulmine nel modulo [!UICONTROL Webhook personalizzato] diventa un punto in rotazione. Questo mostra che il modulo è ora in attesa della chiamata del webhook.

1. Apri una nuova finestra del browser, incolla l&#39;URL copiato nella barra degli indirizzi e premi **[!UICONTROL Invio]**.

   Il modulo [!UICONTROL Webhook personalizzato] è attivato e nel browser verrà visualizzata una nuova pagina.

Se desideri personalizzare la risposta del webhook, utilizza il modulo Risposta del webhook.

La configurazione del modulo contiene due campi: [!UICONTROL Stato] e [!UICONTROL Corpo].

* Il campo [!UICONTROL Stato] contiene codici di stato di risposta HTTP come 2xx per Completato (ad esempio, `200` per OK), 3xx per Reindirizzamento (ad esempio, `307` per Reindirizzamento temporaneo), 4xx per Errori client (ad esempio, `400` per Richiesta non valida) e così via.

* Il campo [!UICONTROL Corpo] contiene qualsiasi elemento che verrà accettato dalla chiamata del webhook. Può essere testo semplice, HTML, XML, JSON e così via.

  >[!TIP]
  >
  >È consigliabile impostare l&#39;intestazione `Content-Type` sul tipo MIME corrispondente: `text/plain` per il testo normale, `text/html` per HTML, `application/json` per JSON, `application/xml` per XML e così via. Per ulteriori informazioni sui tipi MIME, vedere [Moduli MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

Il timeout per l’invio di una risposta è di 40 secondi. Se la risposta non è disponibile entro tale periodo, Workfront Fusion restituisce lo stato &quot;200 Accepted&quot; (Accettato).

### Esempio di risposta HTML

>[!INFO]
>
>**Esempio:**
>
>Configura il modulo [!UICONTROL Risposta webhook] come segue:
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
&gt;     <li><strong>Valore</strong>: text/html</li> 
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
>**Esempio:** Configura il modulo [!UICONTROL Risposta webhook] come segue:
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
&gt;     <li><strong>[!UICONTROL Key]</strong>: Location</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: l'URL a cui si desidera reindirizzare.</li> 
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

Se nel pannello di mappatura mancano alcuni elementi nella configurazione dei moduli che seguono il modulo [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato], fai clic sul modulo **[!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato]** per aprirne la configurazione e fai clic su **[!UICONTROL Ridetermina la struttura dati]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Segui quindi i passaggi descritti nella sezione [Configurare la struttura dati del webhook](#configure-the-webhook-s-data-structure) in questo articolo.
