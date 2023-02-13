---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Adobe Target
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] I moduli ti consentono di creare, leggere, aggiornare o eliminare record, elencare tutti i record di un determinato tipo, cercare record in base ai criteri specificati o eseguire una chiamata API personalizzata per [!DNL Adobe Target] API.
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# [!DNL Adobe Target] Moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Target], nonché collegarlo a più applicazioni e servizi di terze parti. [!DNL Adobe Target] i moduli ti consentono di creare, leggere, aggiornare o eliminare record, elencare tutti i record di un determinato tipo, cercare record in base ai criteri specificati o eseguire una chiamata API personalizzata per [!DNL Adobe Target] API.


Se hai bisogno di istruzioni su come creare uno scenario, vedi [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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
        <p>[!UICONTROL Pro] o superiore</p>
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
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Prodotto</td>
      <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td>
    </tr>
    </tr>
  </tbody>
</table>


Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Prima di poter utilizzare il [!DNL Adobe Target] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* Devi avere un attivo [!DNL Adobe Target] conto.

## Creare una connessione a [!DNL Adobe Target]

Per creare una connessione per [!DNL Adobe Target] moduli:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

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
        <td role="rowheader">ID client [!UICONTROL]</td>
        <td>Inserisci il tuo [!DNL Adobe] ID client. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Inserisci il tuo [!DNL Adobe] Segreto client. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Inserisci il tuo [!DNL Adobe] ID organizzazione. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Inserisci il tuo [!DNL Adobe] ID account tecnico. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Per individuare il tenant, accedi al [!DNL Adobe Experience Cloud], apri [!DNL Target], quindi fai clic su [!DNL Target] il Card. Utilizza il valore ID tenant come indicato nel sottodominio URL.</p>
          <p>Ad esempio, se l'URL al momento dell'accesso a [!DNL Adobe Target] è <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> il tuo ID tenant è quindi "la mia azienda".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta-ambito]</td>
        <td>Invio <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Immetti la chiave privata generata al momento della creazione delle credenziali nel [!DNL Adobe Developer Console]. </p>
          <p>Per estrarre la chiave privata o il certificato:</p>
          <ol>
            <li value="1">
              <p>Fai clic su <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selezionare il tipo di file da estrarre.</p>
            </li>
            <li value="3">
              <p>Selezionare il file contenente la chiave privata o il certificato.</p>
            </li>
            <li value="4">
              <p>Immetti la password del file.</p>
            </li>
            <li value="5">
              <p>Fai clic su <b>[!UICONTROL Save]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo .

## [!DNL Adobe Target] moduli e relativi campi

Quando si configura [!DNL Adobe Target] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Target] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
    <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo di record]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Selezionare il tipo di record che si desidera creare.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continua a <a href="#AB%C2%A0Activ" class="MCXref xref" >Campi attività AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Continua a <a href="#XT" class="MCXref xref" >Campi attività XT</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>Continua a <a href="#Offer" class="MCXref xref" >Campi offerta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Continua a <a href="#Audience" class="MCXref xref" >Campi pubblico</a>.</p>
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
      <td role="rowheader">[!UICONTROL Opzioni]</td>
      <td>
        <p>Per ogni opzione che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p>
        <ul>
          <li>
            <p><b>ID locale opzione [!UICONTROL]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare l’opzione tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per l’opzione. Il nome non deve contenere più di 250 caratteri.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Seleziona o mappa l’offerta associata all’opzione .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>Per ogni mbox che desideri aggiungere all'attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>Per ogni pubblico da aggiungere alla mbox, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e seleziona l'ID pubblico.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare la posizione tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Inserisci o mappa un nome per la posizione. Il nome non deve contenere più di 250 caratteri.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Esperienze]</td>
      <td>
        <p>Un elenco delle posizioni nella pagina in cui viene distribuita l’offerta di contenuto. Una posizione contiene quanto segue:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Immetti o mappa l’ID dell’esperienza</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa il nome dell’esperienza

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Per ogni pubblico che desideri visualizzare l’esperienza, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti l'ID pubblico.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Percentuale di visitatori]</b>
            </p>
            <p>Immettere o mappare la percentuale di visitatori allocata all'esperienza</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Metriche [!UICONTROL]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID di terze parti]</td>
      <td>Immetti o mappa un ID per identificare questa attività. Puoi scegliere questo ID. Questo ID non deve essere lo stesso di un'altra attività e non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inizia da]</td>
      <td>Immetti o mappa la data e l’ora di inizio dell’attività nel formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina a]</td>
      <td>Immetti o mappa la data e l’ora di fine dell’attività nel formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Immetti o mappa lo stato dell’attività.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approvato]</p>
          </li>
          <li>
            <p>[!UICONTROL Disattivato]</p>
          </li>
          <li>
            <p>[!UICONTROL Sospeso]</p>
          </li>
          <li>
            <p>[!UICONTROL salvato] </p>
          </li>
          <li>
            <p>[!UICONTROL Eliminato]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Immetti un numero che definisca la priorità dell’attività. I numeri più alti hanno maggiore priorità. Questo valore deve essere compreso tra 0 e 999. Il valore predefinito è 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Allocazione automatica del traffico]</td>
      <td>
        <p>Abilita questa opzione per allocare automaticamente il traffico. L’allocazione automatica invia più traffico all’esperienza più riuscita.</p>
        <p>Seleziona o mappa i criteri di valutazione in base ai quali giudicare quale esperienza ha più successo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Immettere o mappare l'area di lavoro a cui è associata l'attività</td>
    </tr>
    <tr>
      <td role="rowheader">ID proprietà [!UICONTROL] </td>
      <td>Per ogni proprietà che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e seleziona o mappa l’ID della proprietà.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipi di pubblico per reportistica]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Per ogni pubblico di reporting che desideri aggiungere all’attività, fai clic su [!UICONTROL Aggiungi elemento] e immetti le seguenti informazioni:</p>
        <ul>
          <li>
            <p><b>ID locale del pubblico per la generazione di rapporti</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare il pubblico dei rapporti tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Immettere o mappare il segmento da utilizzare nel reporting</p>
          </li>
          <li>
            <p><b>ID locale della metrica [!UICONTROL]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare la metrica tra le richieste API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campi attività XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per questa attività. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opzioni]</td>
      <td>
        <p>Per ogni opzione che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p>
        <ul>
          <li>
            <p><b>ID locale opzione [!UICONTROL]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare l’opzione tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa un nome per l’opzione. Il nome non deve contenere più di 250 caratteri.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Seleziona o mappa l’offerta associata all’opzione .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>Per ogni mbox che desideri aggiungere all'attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e compila i campi seguenti:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>Per ogni pubblico da aggiungere alla mbox, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e seleziona l'ID pubblico.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare la posizione tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Inserisci o mappa un nome per la posizione. Il nome non deve contenere più di 250 caratteri.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Esperienze]</td>
      <td>
        <p>Un elenco delle posizioni nella pagina in cui viene distribuita l’offerta di contenuto. Una posizione contiene quanto segue:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Immetti o mappa l’ID dell’esperienza</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Immetti o mappa il nome dell’esperienza

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Per ogni pubblico che desideri visualizzare l’esperienza, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti l'ID pubblico.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Percentuale di visitatori]</b>
            </p>
            <p>Immettere o mappare la percentuale di visitatori allocata all'esperienza</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Metriche [!UICONTROL]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID di terze parti]</td>
      <td>Immetti o mappa un ID per identificare questa attività. Puoi scegliere questo ID. Questo ID non deve essere lo stesso di un'altra attività e non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inizia da]</td>
      <td>Immetti o mappa la data e l’ora di inizio dell’attività nel formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina a]</td>
      <td>Immetti o mappa la data e l’ora di fine dell’attività nel formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Immetti o mappa lo stato dell’attività.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approvato]</p>
          </li>
          <li>
            <p>[!UICONTROL Disattivato]</p>
          </li>
          <li>
            <p>[!UICONTROL Sospeso]</p>
          </li>
          <li>
            <p>[!UICONTROL salvato] </p>
          </li>
          <li>
            <p>[!UICONTROL Eliminato]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Immetti un numero che definisca la priorità dell’attività. I numeri più alti hanno maggiore priorità. Questo valore deve essere compreso tra 0 e 999. Il valore predefinito è 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Allocazione automatica del traffico]</td>
      <td>
        <p>Abilita questa opzione per allocare automaticamente il traffico. L’allocazione automatica invia più traffico all’esperienza più riuscita.</p>
        <p>Seleziona o mappa i criteri di valutazione in base ai quali giudicare quale esperienza ha più successo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Immettere o mappare l'area di lavoro a cui è associata l'attività</td>
    </tr>
    <tr>
      <td role="rowheader">ID proprietà [!UICONTROL] </td>
      <td>Per ogni proprietà che desideri aggiungere all’attività, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e seleziona o mappa l’ID della proprietà.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipi di pubblico per reportistica]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Per ogni pubblico di reporting che desideri aggiungere all’attività, fai clic su [!UICONTROL Aggiungi elemento] e immetti le seguenti informazioni:</p>
        <ul>
          <li>
            <p><b>ID locale del pubblico per la generazione di rapporti</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare il pubblico dei rapporti tra le richieste API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Immettere o mappare il segmento da utilizzare nel reporting</p>
          </li>
          <li>
            <p><b>ID locale della metrica [!UICONTROL]</b>
            </p>
            <p>Immetti o mappa una stringa da utilizzare per tracciare la metrica tra le richieste API.</p>
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
        <p>Immetti o mappa il contenuto dell’offerta che verrà mostrato all’utente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Immetti o mappa l’ID dell’area di lavoro associata all’offerta. Se lasciata vuota, l’offerta è associata all’area di lavoro predefinita dell’account. Questa funzionalità si applica solo a [!DNL Target] Account Premium.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Campi pubblico

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Immetti o mappa un nome per il pubblico. Il nome non può contenere più di 250 caratteri.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Immetti o mappa una descrizione del pubblico.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Abilita l’opzione per creare regole E, ovvero, tutte le regole devono essere applicate.</p>
        <p>Per ogni regola da applicare al pubblico, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti il JSON della regola che desideri applicare. </p>
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
        <p>Immetti o mappa l’ID dell’area di lavoro associata al pubblico. Se lasciata vuota, l’offerta è associata all’area di lavoro predefinita dell’account. Questa funzionalità si applica solo a [!DNL Target Premium] conti.</p>
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
      <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
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
        <p>Immettere un percorso relativo a {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL, Metodo]</p>
      </td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente intestazioni di autorizzazione e intestazioni x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Immetti la stringa di query della richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina una singola attività AB, attività XT, offerta o pubblico.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record da eliminare.</td>
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
    <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record da leggere.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID record]</td>
    <td>Immettere o mappare l'ID del record che si desidera leggere.</td>
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
      <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di record]</td>
      <td>
        <p>Selezionare il tipo di record da aggiornare.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Consultare le descrizioni dei campi in <a href="#AB%C2%A0Activ" class="MCXref xref" >Campi attività AB</a> sotto <a href="#Create2" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>Consultare le descrizioni dei campi in <a href="#XT" class="MCXref xref" >Campi attività XT</a> sotto <a href="#Create2" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Altra attività]</b>
            </p>
            <p>Selezionare il campo per il quale si desidera aggiornare un valore, quindi immettere il nuovo valore per il campo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>Consultare le descrizioni dei campi in <a href="#Offer" class="MCXref xref" >Campi offerta</a> sotto <a href="#Create2" class="MCXref xref" >Creare un record</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Consultare le descrizioni dei campi in <a href="#Audience" class="MCXref xref" >Campi pubblico</a> sotto <a href="#Create2" class="MCXref xref" >Creare un record</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID record]</td>
      <td>Immettere o mappare l'ID del record che si desidera aggiornare.</td>
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
      <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo di record]</td>
      <td>Selezionare il tipo di record da aggiornare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordina per]</td>
      <td>Per ogni campo di cui si desidera eseguire l'ordinamento, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e selezionare il campo e se i risultati restituiti devono essere in ascesa o in discesa.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inizia Da]</td>
      <td>
        <p>Immettere la data più recente per la quale si desidera recuperare i record. </p>
        <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina A]</td>
      <td>
        <p>Immettere la data più recente per la quale si desidera recuperare i record. </p>
        <p>Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ricerca]

Questo modulo di ricerca cerca le attività, le offerte o i tipi di pubblico in base ai criteri specificati.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Per istruzioni su come creare una connessione a [!DNL Adobe Target], vedi <a href="#Create" class="MCXref xref" >Creare una connessione a [!DNL Adobe Target]</a> in questo articolo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo di record]</td>
    <td>Selezionare il tipo di record da aggiornare.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Ordina per]</td>
    <td>Per ogni campo di cui si desidera eseguire l'ordinamento, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e selezionare il campo e se i risultati restituiti devono essere in ascesa o in discesa.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Criteri di ricerca]</td>
    <td>Per ogni regola da impostare, seleziona il campo, l’operatore e il valore. Fai clic su <b>[!UICONTROL Aggiungi regola AND]</b> per creare regole aggiuntive.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Immettere il numero della prima risposta che si desidera restituire dal modulo. La prima risposta restituita ha un offset di <code>0</code>. Utilizza questo campo in combinazione con il campo [!UICONTROL Numero massimo di risultati restituiti] per impaginare le risposte.</p>
      <p>Ad esempio, per visualizzare la terza pagina di risposte, quando ogni pagina ha dieci risposte, imposta [!UICONTROL Offset] su 20 e [!UICONTROL Numero massimo di risultati restituiti] su 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari. Utilizza questo campo in combinazione con il campo [!UICONTROL Offset] per impaginare le risposte.</p>
      <p>Ad esempio, per visualizzare la terza pagina di risposte, quando ogni pagina ha dieci risposte, imposta [!UICONTROL Offset] su 20 e [!UICONTROL Numero massimo di risultati restituiti] su 10.</p>
    </td>
  </tr>
</tbody>
</table>
