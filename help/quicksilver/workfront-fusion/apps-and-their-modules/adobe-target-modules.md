---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Adobe Target
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] I moduli consentono di creare, leggere, aggiornare o eliminare record, elencare tutti i record di un determinato tipo, cercare i record in base ai criteri specificati o eseguire una chiamata API personalizzata al [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 51db439995430dad86e41190520824743216df69
workflow-type: tm+mt
source-wordcount: '2646'
ht-degree: 0%

---

# [!DNL Adobe Target] Moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Target], oltre a collegarlo a più applicazioni e servizi di terze parti. [!DNL Adobe Target] I moduli consentono di creare, leggere, aggiornare o eliminare record, elencare tutti i record di un determinato tipo, cercare i record in base ai criteri specificati o eseguire una chiamata API personalizzata al [!DNL Adobe Target] API.


Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
      <td>
        <p>[!UICONTROL Pro] o versione successiva</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
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
    </tr>
  </tbody>
</table>


Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Prima di utilizzare il [!DNL Adobe Target] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* È necessario disporre di un [!DNL Adobe Target] account.

## Creare una connessione a [!DNL Adobe Target]

Per creare una connessione per [!DNL Adobe Target] moduli:

1. Clic **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
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
        <td role="rowheader">[!UICONTROL ID organizzazione]</td>
        <td>Immetti il [!DNL Adobe] ID organizzazione. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Immetti il [!DNL Adobe] ID account tecnico. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Per individuare il tenant, accedi a [!DNL Adobe Experience Cloud], aperto [!DNL Target], quindi fare clic su [!DNL Target] Card. Utilizza il valore ID tenant indicato nel sottodominio URL.</p>
          <p>Ad esempio, se l’URL di è stato registrato in [!DNL Adobe Target] è <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> quindi il tuo ID tenant è "mia azienda".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Ambiti]</td>
        <td>Invio <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Immetti la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
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
    </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## [!DNL Adobe Target] moduli e relativi campi

Quando si configura [!DNL Adobe Target] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Target] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)

* [Ricerche](#searches)


### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)

* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)

* [[!UICONTROL Eliminare un record]](#delete-a-record)

* [[!UICONTROL Leggi un record]](#read-a-record)

* [[!UICONTROL Aggiornare un record]](#update-a-record)


#### [!UICONTROL Creare un record]

Questo modulo di azione crea un’attività AB o XT, un’offerta o un pubblico.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo di record]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Selezionare il tipo di record da creare.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continua con <a href="#ab-activity-fields" class="MCXref xref" >Campi attività AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Continua con <a href="#xt-activity-fields" class="MCXref xref" >Campi di attività XT</a>.</p>
        </li>
        <li>
          <p>Offerta [!UICONTROL]</p>
          <p>Continua con <a href="#offer-fields" class="MCXref xref" >Campi offerta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Continua con <a href="#audience-fields" class="MCXref xref" >Campi del pubblico</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### Campi attività AB

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per questa attività. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>Per ogni opzione che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e compilare i campi seguenti:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tenere traccia dell’opzione nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per l’opzione. Il nome non può contenere più di 250 caratteri.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID offerta]</b>
            </p>
          </li>
          <li>
            <p>Seleziona o mappa l’Offerta associata all’opzione.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Percorsi]</td>
      <td>
        <p>Per ogni Mbox che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e compilare i campi seguenti:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID pubblico]</p>
            <p>Per ogni pubblico che desideri aggiungere alla Mbox, fai clic su <b>[!UICONTROL Add item]</b> e seleziona l’ID pubblico.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per monitorare la posizione nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per la posizione. Il nome non può contenere più di 250 caratteri.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Esperienze]</td>
      <td>
        <p>Un elenco di posizioni sulla pagina in cui viene distribuita l’offerta di contenuti. Una posizione contiene quanto segue:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID Experience Local]</b>
            </p>
            <p>Inserisci o mappa l'ID dell'esperienza</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Inserisci o mappa il nome dell’esperienza

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Per ogni pubblico a cui desideri mostrare l’esperienza, fai clic su <b>[!UICONTROL Add item]</b> e inserisci l’ID pubblico.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Percentuale Visitatori]</b>
            </p>
            <p>Immetti o mappa la percentuale di visitatori allocata all'esperienza</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Immetti o mappa un ID per identificare questa attività. Puoi scegliere questo ID. Questo ID non deve essere lo stesso di un’altra attività e non può superare i 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL inizia da]</td>
      <td>Immetti o mappa la data e l’ora di inizio dell’attività nel formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina alle]</td>
      <td>Immetti o mappa la data e l’ora in cui terminare l’attività nel formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Inserisci o mappa lo stato dell’attività.</p>
        <ul>
          <li>
            <p>[!UICONTROL approvato]</p>
          </li>
          <li>
            <p>[!UICONTROL Disattivato]</p>
          </li>
          <li>
            <p>[!UICONTROL In Pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Salvato] </p>
          </li>
          <li>
            <p>[!UICONTROL eliminato]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Priorità [!UICONTROL]</td>
      <td>Immetti un numero che definisce la priorità dell’attività. I numeri più alti hanno priorità più alta. Questo valore deve essere compreso tra 0 e 999. Il valore predefinito è 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Allocazione automatica traffico]</td>
      <td>
        <p>Abilita questa opzione per allocare automaticamente il traffico. L’allocazione automatica invia più traffico all’esperienza di maggior successo.</p>
        <p>Seleziona o mappa i criteri di valutazione in base ai quali giudicare quale esperienza ha più successo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Inserisci o mappa l’area di lavoro a cui è associata l’attività</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID proprietà] </td>
      <td>Per ogni proprietà che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e seleziona o mappa l’ID della proprietà.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipi di pubblico per reportistica]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Per ogni pubblico di reportistica che si desidera aggiungere all'attività, fare clic su [!UICONTROL Aggiungi elemento] e immettere le informazioni seguenti:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per monitorare il pubblico di reportistica nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID pubblico]</b>
            </p>
            <p>Inserisci o mappa il segmento da utilizzare nel reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric Local ID]</b>
            </p>
            <p>Inserisci o mappa una stringa da utilizzare per monitorare la metrica nelle richieste API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campi di attività XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per questa attività. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>Per ogni opzione che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e compilare i campi seguenti:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tenere traccia dell’opzione nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per l’opzione. Il nome non può contenere più di 250 caratteri.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID offerta]</b>
            </p>
          </li>
          <li>
            <p>Seleziona o mappa l’Offerta associata all’opzione.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Percorsi]</td>
      <td>
        <p>Per ogni Mbox che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e compilare i campi seguenti:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID pubblico]</p>
            <p>Per ogni pubblico che desideri aggiungere alla Mbox, fai clic su <b>[!UICONTROL Add item]</b> e seleziona l’ID pubblico.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per monitorare la posizione nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per la posizione. Il nome non può contenere più di 250 caratteri.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Esperienze]</td>
      <td>
        <p>Un elenco di posizioni sulla pagina in cui viene distribuita l’offerta di contenuti. Una posizione contiene quanto segue:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID Experience Local]</b>
            </p>
            <p>Inserisci o mappa l'ID dell'esperienza</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Inserisci o mappa il nome dell’esperienza

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Per ogni pubblico a cui desideri mostrare l’esperienza, fai clic su <b>[!UICONTROL Add item]</b> e inserisci l’ID pubblico.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Percentuale Visitatori]</b>
            </p>
            <p>Immetti o mappa la percentuale di visitatori allocata all'esperienza</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Immetti o mappa un ID per identificare questa attività. Puoi scegliere questo ID. Questo ID non deve essere lo stesso di un’altra attività e non può superare i 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL inizia da]</td>
      <td>Immetti o mappa la data e l’ora di inizio dell’attività nel formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina alle]</td>
      <td>Immetti o mappa la data e l’ora in cui terminare l’attività nel formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Inserisci o mappa lo stato dell’attività.</p>
        <ul>
          <li>
            <p>[!UICONTROL approvato]</p>
          </li>
          <li>
            <p>[!UICONTROL Disattivato]</p>
          </li>
          <li>
            <p>[!UICONTROL In Pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Salvato] </p>
          </li>
          <li>
            <p>[!UICONTROL eliminato]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Priorità [!UICONTROL]</td>
      <td>Immetti un numero che definisce la priorità dell’attività. I numeri più alti hanno priorità più alta. Questo valore deve essere compreso tra 0 e 999. Il valore predefinito è 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Allocazione automatica traffico]</td>
      <td>
        <p>Abilita questa opzione per allocare automaticamente il traffico. L’allocazione automatica invia più traffico all’esperienza di maggior successo.</p>
        <p>Seleziona o mappa i criteri di valutazione in base ai quali giudicare quale esperienza ha più successo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Inserisci o mappa l’area di lavoro a cui è associata l’attività</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID proprietà] </td>
      <td>Per ogni proprietà che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Add item]</b> e seleziona o mappa l’ID della proprietà.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipi di pubblico per reportistica]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Per ogni pubblico di reportistica che si desidera aggiungere all'attività, fare clic su [!UICONTROL Aggiungi elemento] e immettere le informazioni seguenti:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience Local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per monitorare il pubblico di reportistica nelle diverse richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID pubblico]</b>
            </p>
            <p>Inserisci o mappa il segmento da utilizzare nel reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric Local ID]</b>
            </p>
            <p>Inserisci o mappa una stringa da utilizzare per monitorare la metrica nelle richieste API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campi offerta

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per questa attività. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Inserisci o mappa il contenuto dell’offerta che verrà mostrato all’utente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Inserisci o mappa l’ID dell’area di lavoro associata all’offerta. Se non specificata, l’offerta viene associata all’area di lavoro predefinita dell’account. Questa funzionalità si applica solo a [!DNL Target] Account Premium.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Campi del pubblico

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per questo pubblico. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Inserisci o mappa una descrizione del pubblico.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Regola di destinazione [!UICONTROL]</td>
      <td>
        <p>Attiva l’interruttore per creare regole E, ovvero, tutte le regole devono essere applicate.</p>
        <p>Per ogni regola che desideri applicare al pubblico, fai clic su <b>[!UICONTROL Add item]</b> e inserisci il JSON della regola da applicare. </p>
        <div class="example"><span class="autonumber"><span><b>Esempio: </b></span></span>
          <p>Esempi:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Inserisci o mappa l’ID dell’area di lavoro associata al pubblico. Se non specificata, l’offerta viene associata all’area di lavoro predefinita dell’account. Questa funzionalità si applica solo a [!DNL Target Premium] account.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo effettua una chiamata API personalizzata al [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] URL di base]</td>
      <td>Inserisci o mappa il tuo [!DNL Target] URL di base.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Inserisci un percorso relativo a {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione e le intestazioni x-api-key.</p>
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
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina una singola attività AB, un’attività XT, un’offerta o un pubblico.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record che si desidera eliminare.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID record]</td>
    <td>Immettere o mappare l'ID del record che si desidera eliminare.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione recupera i dati per una singola attività, offerta, pubblico, proprietà o rapporto.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record che si desidera leggere.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID record]</td>
    <td>Immetti o mappa l’ID del record da leggere.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un’attività, un’offerta o un pubblico.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di record]</td>
      <td>
        <p>Selezionare il tipo di record da aggiornare.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Vedi le descrizioni dei campi in <a href="#ab-activity-fields" class="MCXref xref" >Campi attività AB</a> in <a href="#create-a-record" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>Vedi le descrizioni dei campi in <a href="#xt-activity-fields" class="MCXref xref" >Campi di attività XT</a> in <a href="#create-a-record" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Altra Attività]</b>
            </p>
            <p>Selezionare il campo per il quale si desidera aggiornare un valore, quindi immettere il nuovo valore per il campo.</p>
          </li>
          <li>
            <p><b>Offerta [!UICONTROL]</b>
            </p>
            <p>Vedi le descrizioni dei campi in <a href="#offer-fields" class="MCXref xref" >Campi offerta</a> in <a href="#create-a-record" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Vedi le descrizioni dei campi in <a href="#audience-fields" class="MCXref xref" >Campi del pubblico</a> in <a href="#create-a-record" class="MCXref xref" >Creare un record</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID record]</td>
      <td>Immetti o mappa l’ID del record da aggiornare.</td>
    </tr>
  </tbody>
</table>

### Ricerche

* [[!UICONTROL Ottieni record]](#get-records)

* [[!UICONTROL Ricerca]](#search)


#### [!UICONTROL Ottieni record]

Questo modulo di ricerca recupera un elenco di record del tipo selezionato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di record]</td>
      <td>Selezionare il tipo di record da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordina per]</td>
      <td>Per ogni campo in base al quale si desidera ordinare, fare clic su <b>[!UICONTROL Add item]</b> e seleziona il campo e specifica se i risultati restituiti devono essere crescenti o decrescenti.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inizia Da]</td>
      <td>
        <p>Immettere la prima data per la quale si desidera recuperare i record. </p>
        <p>Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina A]</td>
      <td>
        <p>Immettere l'ultima data per la quale si desidera recuperare i record. </p>
        <p>Per un elenco dei formati di data e ora supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ricerca]

Questo modulo di ricerca cerca attività, offerte o tipi di pubblico in base ai criteri specificati.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Target], vedi <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record da aggiornare.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Ordina per]</td>
    <td>Per ogni campo in base al quale si desidera ordinare, fare clic su <b>[!UICONTROL Add item]</b> e seleziona il campo e specifica se i risultati restituiti devono essere crescenti o decrescenti.</td>
  </tr>
  <tr>
    <td role="rowheader">Criteri di ricerca di [!UICONTROL]</td>
    <td>Per ogni regola che desideri impostare, seleziona il campo, l’operatore e il valore. Clic <b>[!UICONTROL Aggiungi regola AND]</b> per creare regole aggiuntive.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Immettere il numero della prima risposta che si desidera venga restituita dal modulo. La prima risposta restituita ha uno scostamento di <code>0</code>. Utilizza questo campo in combinazione con il campo [!UICONTROL Numero massimo di risultati restituiti] per impaginare le risposte.</p>
      <p>Ad esempio, per visualizzare la terza pagina di risposte, quando ogni pagina ha dieci risposte, impostare [!UICONTROL Offset] su 20 e [!UICONTROL Numero massimo di risultati restituiti] su 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario. Utilizzare questo campo in combinazione con il campo [!UICONTROL Offset] per impaginare le risposte.</p>
      <p>Ad esempio, per visualizzare la terza pagina di risposte, quando ogni pagina ha dieci risposte, impostare [!UICONTROL Offset] su 20 e [!UICONTROL Numero massimo di risultati restituiti] su 10.</p>
    </td>
  </tr>
</tbody>
</table>
