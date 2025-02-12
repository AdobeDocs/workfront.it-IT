---
title: Creare un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato con il progettista del modulo. È possibile allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '6493'
ht-degree: 5%

---

# Creare un modulo personalizzato

Puoi progettare un modulo personalizzato con il progettista del modulo in Adobe Workfront. È possibile allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inizia a progettare un modulo personalizzato

{{step-1-to-setup}}

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

1. Fare clic su **Nuovo modulo personalizzato.**
1. Seleziona i tipi di oggetto a cui vuoi allegare il modulo personalizzato, quindi fai clic su **Continua**.

   ![Scegli il tipo di oggetto](assets/choose-object-type.jpg)

1. Nell&#39;area **Titolo obbligatorio** digitare il titolo del modulo personalizzato.
1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sull&#39;icona **Aggiungi** ![Icona Aggiungi oggetti](assets/add-objects-icon.png) dopo **Tipi di oggetto**, quindi selezionare il tipo desiderato nel menu visualizzato. È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   È inoltre possibile fare clic sulla X su un tipo di oggetto per eliminarlo dal modulo.

   >[!CAUTION]
   >
   >L’eliminazione di un modulo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati sugli oggetti associati al modulo. Non è possibile recuperare i dati eliminati. Valuta invece la possibilità di disattivare un modulo personalizzato: quando disattivi un modulo personalizzato che non utilizzi più, vengono conservati tutti i dati storici associati.
   >
   >Per ulteriori informazioni, vedere [Aggiungere o eliminare tipi di oggetto da un modulo personalizzato esistente](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) e [Disattivare o riattivare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Successivamente, puoi iniziare ad aggiungere campi al modulo personalizzato. Vedere le sezioni seguenti:
   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Note sui nomi e sulle etichette dei campi](#notes-on-field-names-and-labels)
   * [Aggiungi campi di testo](#add-text-fields)
   * [Aggiungere campi calcolati](#add-calculated-fields)
   * [Aggiungi pulsanti di scelta, gruppi di caselle di controllo e elenchi a discesa](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Aggiungere campi di tipo typeahead e date](#add-typeahead-and-date-fields)
   * [Aggiungere campi di ricerca esterni](#add-external-lookup-fields)
   * [Aggiungere immagini, PDF e video](#add-images-pdfs-and-videos)
   * [Aggiungi campi nativi Workfront](#add-workfront-native-fields)
   * [Aggiungere file Adobe XD](#add-adobe-xd-files)
   * [Aggiungi campi di connessione Planning](#add-planning-connection-fields)

## Aggiungere campi nuovi o esistenti al modulo personalizzato

È possibile utilizzare campi nuovi o esistenti durante la progettazione del modulo personalizzato.

I moduli personalizzati sono limitati a 500 campi. Un contatore in basso a sinistra visualizza il numero di campi utilizzati nel modulo, che è sempre visibile durante lo scorrimento all&#39;interno del progettista del modulo.

### Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato

1. Nella parte superiore sinistra dello schermo fare clic su **Libreria campi**.

1. Trascina qui il campo o il widget desiderato nel modulo personalizzato.
1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, il calo delle prestazioni può verificarsi quando in un modulo esistono più di 100 moduli, a seconda della complessità.
   >
   >
   >Esempi di moduli complessi includono moduli con parametri a catena, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Note sui nomi e sulle etichette dei campi {#notes-on-field-names-and-labels}

**label** è disponibile per la maggior parte dei campi. Si tratta di un’etichetta descrittiva visualizzata sopra il campo o il widget nel modulo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.

>[!NOTE]
>
>Evita di usare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.

È necessario un **nome** per ogni campo. Questo nome indica il modo in cui il sistema identifica il campo personalizzato quando lo si aggiunge a varie aree in Workfront, ad esempio report, Home e interazioni API. Quando configuri il campo o il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l&#39;etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.

Ogni nome di campo personalizzato deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo, è possibile riutilizzare un modulo già creato per un altro modulo personalizzato.

>[!NOTE]
>
>Sebbene sia possibile farlo, si consiglia di non modificare questo nome dopo che l’utente o altri utenti hanno iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato a cui potrebbe ora fare riferimento in altre aree di Workfront.
>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e non funzionerà più correttamente a meno che non lo aggiungi nuovamente al rapporto utilizzando il nuovo nome.
>
>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.
>
>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori quando si utilizza il campo in aree diverse di Workfront.

I seguenti caratteri speciali non sono supportati nelle etichette e nei nomi dei campi personalizzati.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Aggiungi campi di testo

È possibile aggiungere diversi campi di testo a un modulo personalizzato.

+++ **Espandi per visualizzare le descrizioni dei campi di testo disponibili**

* **Campo di testo a riga singola**: consente agli utenti di digitare una singola riga di testo nel campo.
* **Campo paragrafo**: consente agli utenti di digitare più righe di testo nel campo.
* **Campo di testo con formattazione**: consente agli utenti di digitare più righe di testo nel campo e di formattare il testo con grassetto, corsivo, sottolineatura, punti elenco, numerazione, collegamenti ipertestuali e virgolette. Un limite di caratteri di 15.000 consente di inserire testo e formattazione in modo molto ampio.

  Questo tipo di campo personalizzato non è supportato nei filtri di elenchi e rapporti.

  Per informazioni sull&#39;accesso a questo campo tramite l&#39;API, vedere [Archiviazione campi in formato Rich Text nell&#39;API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >I campi di testo con formattazione non sono disponibili per le app Workfront per dispositivi mobili (disponibili nelle prossime versioni).

* **Testo descrittivo**: consente di includere istruzioni e collegamenti a pagine esterne a Workfront.

+++

Per aggiungere un campo di testo:

1. Nella parte sinistra dello schermo, individua uno dei campi di testo seguenti e trascinalo in una sezione dell’area di lavoro:

   * Testo su riga singola
   * Paragrafo
   * Testo con formattazione
   * Testo descrittivo

   ![Trascina campo nella sezione](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table>
    <tr>
    <td>Input in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr>
    <td>Dimensione</td>
    <td><p>Modificare le dimensioni dei campi di testo nel modulo.<p>
   </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo con formattazione</li>
    <li>Testo descrittivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etichetta</td>
    <td><p>(Obbligatorio)Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare l’etichetta in qualsiasi momento.<p>
    <p>IMPORTANTE: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p></td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo con formattazione</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nome</td>
    <td><p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p>
    <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p>
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo con formattazione</li>
    <li>Testo descrittivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Istruzioni</td>
    <td>Digitare eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo con formattazione</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formato</td>
    <td><p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p> <p><b>NOTA</b>:   
    <ul> 
    <li>Questo campo non può essere modificato dopo il salvataggio del modulo. Se si desidera utilizzare il campo nei calcoli matematici, assicurarsi di selezionare un formato Numerico o Valuta.</li> 
    <li>Quando selezionate Numero (Number) o Valuta (Currency), il sistema tronca automaticamente i numeri che iniziano con 0.</li>
    <li>Il limite di caratteri per i campi Numero è 16. È inoltre possibile utilizzare un campo Testo per immettere numeri ed evitare il limite.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Tipo di Disposizione</td>
    <td>Passa da un campo di testo a riga singola a un campo di testo di paragrafo e viceversa.</td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Collegamento ipertestuale</td>
    <td> Se si desidera applicare un collegamento ipertestuale al testo descrittivo digitato, aggiungerlo qui. Il testo descrittivo viene visualizzato come collegamento sugli oggetti a cui è allegato il modulo.</td>
    <td><ul><li>Testo descrittivo</li></ul></td>
    </tr>
    <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
    </tr> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungere campi calcolati

In un modulo personalizzato è possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene allegato a un oggetto.

Per aggiungere un campo calcolato, vedere [Aggiungere campi calcolati con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Aggiungi pulsanti di scelta, gruppi di caselle di controllo e elenchi a discesa

In un modulo personalizzato è possibile aggiungere pulsanti di scelta, gruppi di caselle di controllo, elenchi a discesa e elenchi a discesa a selezione multipla.

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Pulsanti di scelta**: richiede agli utenti di selezionare una sola scelta.
* **Gruppo di caselle di controllo**: consente agli utenti di selezionare più scelte.
* **Elenco a discesa a selezione singola**: fornisce un elenco di scelte a discesa.
* **Elenco a discesa a selezione multipla**: consente agli utenti di selezionare più scelte da un elenco a discesa.

+++

>[!NOTE]
>
>I campi che consentono selezioni multiple, come il gruppo di caselle di controllo e il menu a discesa a selezione multipla, sono difficili da tracciare e raggruppare nei rapporti. Per semplificare la creazione di grafici e il raggruppamento nei report, è possibile creare campi separati per ogni scelta, ad esempio un campo di testo a riga singola.

Per aggiungere pulsanti di scelta, gruppi di caselle di controllo e elenchi a discesa:

1. Nella parte sinistra dello schermo, individua uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Pulsanti di opzione
   * Gruppo di caselle di controllo
   * Elenco a discesa a selezione singola
   * Elenco a discesa multi-selezione

   ![Trascinare un campo nell&#39;area di lavoro](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Input in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr> 
     <td role="rowheader">Etichetta</td> 
     <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: </p> <p>Evita di usare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nome</td> 
     <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> 
    <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td>
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Istruzioni</td> 
    <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formato</td> 
    <td> <p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p> <p><b>NOTA</b>:   
     <ul> 
    <li>Questo campo non può essere modificato dopo il salvataggio del modulo. Se si desidera utilizzare il campo nei calcoli matematici, assicurarsi di selezionare un formato Numerico o Valuta.<br></li> 
    <li>Quando selezionate Numero (Number) o Valuta (Currency), il sistema tronca automaticamente i numeri che iniziano con 0.</li>
    <li>Il limite di caratteri per i campi Numero è 16. È inoltre possibile utilizzare un campo Testo per immettere numeri ed evitare il limite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Tipo di Disposizione</td> 
    <td>Passa da un pulsante di opzione all’altro, da un gruppo di caselle di controllo a un altro, da un elenco a discesa a selezione singola o a un elenco a discesa a selezione multipla per il campo.</td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Rendi il campo obbligatorio</td> 
    <td>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Scelte </td> 
    <td> 
    <ol> 
    <li> <p>Fai clic su <b>Opzioni</b>, quindi abilita uno dei seguenti elementi:</p> 
    <ul> 
    <li><strong>Mostra valori</strong>: mostra i valori di ciascuna scelta nel campo. L’etichetta di ciascuna scelta viene visualizzata per impostazione predefinita.</li> 
     <li><strong>Ordina scelte A-Z</strong>: ordina alfabeticamente le scelte aggiunte nel campo.</li> 
    </ul> 
    </li> 
    <li> <p>Per ogni scelta aggiunta per l'utente, fare clic sull'icona a forma di ingranaggio <img src="assets/gear-icon-settings.png">, quindi selezionare una delle opzioni seguenti:</p> 
    <ul> 
    <li><strong>Seleziona per impostazione predefinita</strong>: seleziona la scelta per impostazione predefinita nel campo.</li> 
    <li> <p><strong>Nascondi scelta</strong>: nasconde la scelta nel campo. Le scelte nascoste rimangono accessibili nei rapporti.</p> </li> 
    <li> <p><strong>Rimuovi scelta</strong>: rimuovere la scelta dal campo.</p> <p><b>AVVISO</b>: se sono presenti oggetti correnti che utilizzano questa scelta, non rimuoverla dal campo. Rimuovendola, i dati storici andranno perduti. Al contrario, seleziona l’opzione per nasconderlo, impedendo agli utenti di selezionarlo in futuro.</p> </li> 
    </ul> 
     </li> 
    </ol>

   <p><b>NOTA:</b></p>
    <p>Non esiste alcun limite al numero di scelte selezionabili. </p>    
    </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa multi-selezione</li>
    </ul>
    </td>
     </tr> 
    </tbody> 
    </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungere campi di tipo typeahead e date

È possibile aggiungere campi di tipo typeahead e date a un modulo personalizzato.

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Automatico**: consente agli utenti di digitare il nome di un oggetto esistente in Workfront. Quando l’utente inizia a digitare, viene visualizzato un elenco di suggerimenti. Questo tipo di campo supporta i seguenti oggetti:
   * Utente
   * Gruppo
   * Ruolo
   * Portfolio
   * Programma
   * Progetto
   * Team
   * Modello
   * Azienda
* **Data**: visualizza un calendario in cui gli utenti possono selezionare una data e un&#39;ora.

+++

Per aggiungere campi di tipo typeahead e date:

1. Nella parte sinistra dello schermo, individua uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Automatico
   * Data

   ![Trascina campo nella sezione](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Impostazione campo</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
       <td><ul>
    <li>Automatico</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> 
      <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td>
    <td><ul>
    <li>Automatico</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Automatico</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza ora del giorno</td> 
      <td>Seleziona questa opzione se desideri visualizzare l’ora del giorno insieme alla data nel campo.</td> 
         <td><ul>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto di riferimento</td> 
      <td> <p>Selezionare il tipo di oggetto da associare al campo.</p> <p>Dopo aver fatto clic su Applica o su Salva+Chiudi, non è possibile modificare il tipo di oggetto per il campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se l'amministratore di Workfront ha personalizzato il nome di Portfolio, Programmi o Progetti nell'interfaccia utente di Workfront, in questo elenco a discesa viene visualizzato il nome predefinito di Workfront per l'oggetto, non il nome personalizzato. Se hai bisogno di assistenza, rivolgiti all’amministratore di Workfront.<br></li> 
         <li>Nelle app mobili iOS e Android Workfront sono supportati i seguenti tipi di oggetti: Utente, Società, Gruppo, Mansione, Portfolio, Programma, Progetto e Modello.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Automatico</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Aggiungi filtro</td>
      <td><p>Aggiungi un filtro per un tipo di oggetto per limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul> 
        <li>Appartengono a uno o più gruppi specificati</li> 
        <li>Sono associati a un ruolo o a una mansione specificata</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo</li> 
       </ul> <p>È necessario definire il filtro per il tipo di oggetto selezionato utilizzando la sintassi della modalità testo. Per informazioni sulla creazione di un filtro in modalità testo, vedere <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modificare un filtro in modalità testo</a>.</p>
       <p><b>NOTA</b>:
       <ul> 
        <li>Se si sta modificando un modulo personalizzato esistente, l'aggiunta di un filtro a un campo automatico non rimuove gli oggetti già aggiunti dagli utenti utilizzando il campo al di fuori dell'ambito del filtro.</li> 
        <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo Typeahead, il campo verrà visualizzato sui dispositivi mobili degli utenti che non sono interessati dal filtro.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Automatico</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td> 
      <td>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
       <td><ul>
    <li>Automatico</li>
    <li>Data</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungere campi di ricerca esterni

Un campo di ricerca esterno richiama un’API esterna e restituisce i valori come opzioni in un campo a discesa. Gli utenti che utilizzano l’oggetto a cui è associato il modulo personalizzato possono selezionare una o più di queste opzioni dal menu a discesa. Il campo di ricerca esterno è disponibile anche in elenchi e rapporti.

Per esempi di utilizzo del campo di ricerca esterna per chiamare la stessa istanza di Workfront o un&#39;API pubblica, vedere [Esempi di campo di ricerca esterna in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* I campi di ricerca esterna non sono supportati nel plug-in di Outlook.
>* I campi di ricerca esterni non sono disponibili negli elenchi quando il campo ha una dipendenza da un altro campo.

Per aggiungere una ricerca esterna:

1. Nella parte sinistra dello schermo, trovare **Ricerca esterna** e trascinarlo in una sezione dell&#39;area di lavoro.
1. Sul lato destro della schermata, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p>
      <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td>
     </tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td>
      <td><p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p>
      <p><strong>NOTA:</strong></p>
      <ul><li>È possibile modificare il tipo di formato dopo il salvataggio del modulo, con un limite: tutti i valori esistenti sugli oggetti devono poter essere convertiti nel nuovo tipo. Ad esempio, se il tipo di formato è Testo e un oggetto memorizza il valore "abc", non è possibile convertire il campo e viene visualizzato un errore che indica che il sistema non può convertire "abc" in numero/valuta. Se si desidera utilizzare il campo nei calcoli matematici, assicurarsi di selezionare un formato Numerico o Valuta.</li>
      <li>Quando selezionate Numero (Number) o Valuta (Currency), il sistema tronca automaticamente i numeri che iniziano con 0.</li>
      <li>Il limite di caratteri per i campi Numero è 16. È inoltre possibile utilizzare un campo Testo per immettere numeri ed evitare il limite.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL API base</td> 
      <td><p>Digita o incolla l’URL per l’API.</p><p>L’URL API deve restituire il contenuto JSON delle opzioni che desideri visualizzare nel menu a discesa. Puoi utilizzare il campo Percorso JSON per selezionare i valori specifici dal JSON restituito come opzioni a discesa.</p><p>Quando immetti l’URL API, puoi facoltativamente trasmettere i seguenti valori nell’URL:</p>
      <ul>
      <li>$$HOST - Rappresenta l'host Workfront corrente e può essere utilizzato per effettuare chiamate API /search all'API Workfront. Quando si utilizza questo carattere jolly, l'autenticazione viene gestita e gli utenti non devono inviare intestazioni di autenticazione. Gli utenti, ad esempio, possono cercare le attività utilizzando l'URL di base <code>$$HOST/attask/api/task/search</code> e consentire la ricerca delle attività e la selezione dei valori da un elenco di attività restituito.</li>
      <li><p>$$QUERY - Rappresenta il testo di ricerca digitato dall'utente finale nel campo e consente di implementare il filtro delle query per gli utenti finali. L’utente cercherà il valore nel menu a discesa.</p>
      <p>Se l’API a cui stai facendo riferimento lo consente, puoi anche includere modificatori nella query di ricerca per identificare come dovrebbe funzionare la ricerca. È possibile, ad esempio, utilizzare quanto segue come URL API di base per consentire agli utenti di cercare qualsiasi progetto Workfront contenente testo specifico: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Ulteriori informazioni sui modificatori di ricerca Workfront in <a href="/help/quicksilver/wf-api/general/api-basics.md">Nozioni di base sulle API</a>.</p>
      <p><strong>NOTA:</strong> se non si utilizza $$QUERY e l'utente digita del testo nella casella di ricerca, le scelte già disponibili verranno limitate. Tuttavia, se utilizzi $$QUERY e l’utente digita qualsiasi cosa, viene eseguita una nuova chiamata di rete all’API. Pertanto, se nell’API sono presenti più di 2.000 valori e l’API supporta l’esecuzione di query, puoi utilizzare $$QUERY per eseguire ricerche non solo dai valori esistenti del 2.000, ma dall’API originale con le opzioni ridotte.</p></li>
      <li><p>{fieldName} - Dove fieldName è un campo personalizzato o nativo in Workfront. In questo modo puoi implementare i filtri delle opzioni a discesa a cascata, quando trasmetti il valore di un campo già selezionato al campo di ricerca Esterna per filtrare le opzioni. Ad esempio, il campo Regione esiste già nel modulo e stai restringendo un elenco di paesi dall’API a quelli che si trovano in un’area specifica.</p>
      <p>Per un campo di ricerca esterno che ha una dipendenza da altri campi (utilizzando la sintassi {fieldName}), le opzioni restituite dall'API sono limitate a quelle che corrispondono a eventuali stringhe o valori immessi negli altri campi. Questa funzionalità non è supportata negli elenchi e nei report.</p></li>
      <li>{referenceObject}.{fieldName} - Dove il campo fa parte di un oggetto. Questa sintassi è simile alle espressioni personalizzate. Ad esempio, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>NOTA:</strong> consulta la documentazione dell'API con cui stai lavorando per le query specifiche che puoi definire.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Metodo HTTP</td> 
      <td>Selezionare <strong>Get</strong>, <strong>Post</strong> o <strong>Put</strong> per il metodo.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Percorso JSON</td>
      <td><p>Digita o incolla il percorso JSON per l’API.</p> <p>Questa opzione consente di estrarre i dati dal JSON restituito dall’URL API. Serve come modo per selezionare quali valori dall’interno del JSON appariranno nelle opzioni a discesa.</p><p>Ad esempio, se l'URL API restituisce JSON in questo formato:</br>
      <pre>
      {
       dati: {
         { name: "USA"},
         { name: "Canada"}
       }
      }
      </pre>
      </p>
      <p>quindi puoi utilizzare "$.data[*].name" per selezionare Stati Uniti e Canada come opzioni a discesa.</p> <p>Per ulteriori informazioni sul percorso JSON e sulla verifica della scrittura del percorso JSON corretto, fare riferimento a <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Intestazioni</td>
      <td><p>Fai clic su <strong>Aggiungi intestazione</strong> e digita o incolla la coppia chiave-valore richiesta per l'autenticazione con l'API.</p><p><strong>NOTA:</strong> i campi Intestazione non sono un luogo sicuro in cui archiviare le credenziali. È necessario prestare attenzione a ciò che si immette e si salva.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Elenco a discesa multi-selezione</td>
      <td><p>Seleziona questa opzione per consentire all’utente di selezionare più di un valore nel menu a discesa.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr>       
    </tbody>
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

>[!NOTE]
>
>Gli elementi seguenti sono limitazioni tecniche della chiamata all’API esterna:
>
>* Numero massimo di opzioni: 2000 (vengono visualizzate solo le prime 2000 opzioni univoche del JSON restituito)
>* Timeout: 3 secondi
>* Numero di nuovi tentativi: 3
>* Durata attesa tra nuovi tentativi: 500 ms
>* Stati di risposta previsti: 2xx

### Aggiungere immagini, PDF e video

È possibile aggiungere immagini, PDF e video a un modulo personalizzato. Gli utenti che utilizzano l&#39;oggetto a cui è allegato il modulo personalizzato possono visualizzare l&#39;immagine, il PDF o il video solo nelle seguenti aree:

* L’area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Immagine**: consente agli utenti di aggiungere file di immagine.
* **PDF**: consente agli utenti di aggiungere PDF
* **Video**: consente agli utenti di aggiungere file video.

+++

Per aggiungere immagini, PDF o video:

1. Nella parte sinistra dello schermo, individua uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Immagine
   * PDF
   * Video

   ![Trascina campo nella sezione](assets/drag-field-to-section.png)

1. Digitate o modificate una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla l’URL del widget in cui è memorizzato su Internet.</p> 
      <p>Se stai aggiungendo un widget video, al momento puoi farlo aggiungendo quanto segue nella casella URL:</p> 
      <ul> 
      <li> <p>Collegamento YouTube o Vimeo</p> </li> 
      <li> <p>Collegamento video Google Drive</p> </li> 
      <li> <p>Collegamento a video con estensione MP4 e MOV</p> </li> 
      <li> <p>Collegamento a un video già caricato nell’area Documenti della tua istanza di Workfront. Per istruzioni, vedere <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Aggiungere un widget video a un modulo personalizzato dall'area Documenti</a> in questo articolo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>Modifica le dimensioni di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

#### Aggiungere un video a un modulo personalizzato dall’area Documenti{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Quando si aggiunge un video a un modulo personalizzato in questo modo, le autorizzazioni impostate nell&#39;area Documenti vengono applicate al video quando gli utenti accedono al modulo su un oggetto.

1. Vai al video nell&#39;area Documenti e genera una bozza per esso, come descritto in [Crea una bozza interattiva per un sito Web o altro contenuto Web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Apri la bozza.
1. Fai clic con il pulsante destro del mouse in un punto qualsiasi del video, quindi seleziona **Copia indirizzo video**.
1. Nel modulo personalizzato in cui stai aggiungendo il widget video, incolla l&#39;indirizzo copiato nella casella **URL**.
1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungi campi nativi Workfront

Puoi aggiungere campi nativi di Workfront ai moduli personalizzati. Quando il modulo personalizzato viene allegato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, il campo Description (Descrizione) in un modulo personalizzato allegato a un progetto estrae la descrizione del progetto. (Il campo può mostrare &quot;N/D&quot; se non sono disponibili dati).

+++ **Espandi per visualizzare l&#39;elenco dei campi nativi supportati**

In questa tabella sono elencati i campi nativi disponibili per oggetti Workfront specifici in un modulo personalizzato.

| Nome campo | Progetto | Attività | Problema | Modello | Attività modello | Portfolio | Programma | Gruppo |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Data di completamento effettiva | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durata Reale | ✓ |   |   |   |   |   |   |   |
| Ore effettive | ✓ |   | ✓ |   |   |   |   |   |
| Data di inizio effettiva | ✓ | ✓ | ✓ |   |   |   |   |   |
| Azienda | ✓ |   |   | ✓ |   |   |   |   |
| Condizione | ✓ | ✓ | ✓ |   |   |   |   |   |
| Tipo di condizione | ✓ |   |   | ✓ |   |   |   |   |
| Descrizione | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Durata |   | ✓ |   |   | ✓ |   |   |   |
| Tipo di Durata |   | ✓ |   |   | ✓ |   |   |   |
| Unità di Durata |   | ✓ |   |   | ✓ |   |   |   |
| Immesso da | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Data inserimento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Gruppo | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Ultimo aggiornamento di | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Data ultimo aggiornamento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Nome | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Proprietario | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Data di completamento Pianificata | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durata Pianificata | ✓ |   |   | ✓ |   |   |   |   |
| Lavoro Necessario | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Data di inizio pianificata | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Priorità | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programma | ✓ |   |   | ✓ |   |   |   |   |
| Data di completamento Previsto | ✓ | ✓ |   |   |   |   |   |   |
| Durata prevista in minuti |   | ✓ |   |   |   |   |   |   |
| Data di inizio prevista | ✓ | ✓ |   |   |   |   |   |   |
| Numero di riferimento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Modalità pianificazione | ✓ |   |   | ✓ |   |   |   |   |
| Gravità |   |   | ✓ |   |   |   |   |   |
| Sponsor | ✓ |   |   | ✓ |   |   |   |   |
| Stato | ✓ | ✓ |   |   |   |   |   |   |
| Punti storia |   | ✓ |   |   |   |   |   |   |
| Modello | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. Nella parte sinistra della schermata, trova **Riferimento campo nativo** e trascinalo in una sezione dell&#39;area di lavoro.
1. Sul lato destro della schermata, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td>
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p>
      <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digitare eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo di riferimento</td> 
      <td><p>(Obbligatorio) Seleziona un campo nativo di Workfront.<p><p>Sono disponibili solo campi nativi per gli oggetti del modulo. Se ad esempio l'elenco Tipi di oggetto nella parte superiore del progettista del modulo mostra Project, sarà possibile selezionare campi nativi per i progetti ma non campi specifici delle attività.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Aggiungi filtro</td>
      <td><p>Aggiungi un filtro per il campo di riferimento per limitare l’elenco di elementi tra cui gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul>
        <li>Appartengono a uno o più gruppi specificati</li> 
        <li>Sono associati a un ruolo o a una mansione specificata</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo</li> 
       </ul>
       <p>È necessario definire il filtro per il campo di riferimento selezionato utilizzando la sintassi in modalità testo. Per informazioni sulla creazione di un filtro in modalità testo, vedere <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modificare un filtro in modalità testo</a>.</p>
       <p><b>NOTA</b>:
       <ul> 
        <li>L’opzione filtro è disponibile solo quando si fa riferimento a un campo typeahead nativo, ad esempio Portfolio, Company o Owner.</li>
        <li>Se si sta modificando un modulo personalizzato esistente, l'aggiunta di un filtro a un campo nativo non rimuove gli oggetti già aggiunti dagli utenti utilizzando il campo, al di fuori dell'ambito del filtro.</li> 
        <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo nativo, il campo verrà visualizzato sui dispositivi mobili degli utenti non interessati dal filtro.</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del campo in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungere file Adobe XD

Puoi aggiungere un prototipo Adobe XD direttamente a un modulo personalizzato. Gli utenti che utilizzano l’oggetto a cui è allegato il modulo personalizzato possono visualizzare il file Adobe XD solo nelle seguenti aree:

* L’area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività)

Per aggiungere un file Adobe XD:

1. Sul lato sinistro della schermata, trovare **Adobe XD** e trascinarlo in una sezione dell&#39;area di lavoro.
1. Digitate o modificate una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evitare di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p>
    <p>Per ulteriori informazioni, vedere <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla un collegamento valido per il prototipo di XD.</p> 
      <p>Nota: l’impostazione Accesso link nella scheda Condividi di Adobe XD deve essere impostata su Chiunque abbia il link. In caso contrario, gli utenti non potranno visualizzare il prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

### Aggiungi campi di connessione Planning

>[!IMPORTANT]
>
>Le informazioni presenti in questa sezione si riferiscono ad Adobe Workfront Planning, una funzionalità aggiuntiva di Adobe Workfront.
>
>Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:
>
>* Un nuovo piano e una nuova licenza Workfront. Workfront Planning non è disponibile per i piani o le licenze legacy di Workfront.
>* Pacchetto aggiuntivo per Workfront Planning.
>* L’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.
>
> Per un elenco completo dei requisiti per accedere a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Per ulteriori informazioni su Workfront Planning, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

È possibile visualizzare i record connessi da Workfront Planning in un campo personalizzato di un oggetto Workfront aggiungendo un campo personalizzato della connessione Planning al modulo personalizzato di un oggetto.

È possibile aggiungere il campo Connessione Planning ai moduli personalizzati di tutti gli oggetti. È tuttavia possibile visualizzare i record connessi solo nei moduli personalizzati associati agli oggetti di Workfront che possono essere connessi da Workfront Planning.

>[!NOTE]
>
>Gli utenti che visualizzano le informazioni nel campo personalizzato devono avere accesso a Workfront Planning e alle aree di lavoro che contengono i tipi di record connessi agli oggetti di Workfront.

Per aggiungere un campo di connessione Planning:

1. Sul lato sinistro della schermata, trovare **Connessione Planning** e trascinarla in una sezione dell&#39;area di lavoro.
1. Sul lato destro della schermata, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>:</p> <p>Evita di usare caratteri speciali in questa etichetta.</p> 
      <p>È consigliabile scegliere un'etichetta che consenta di identificare facilmente la provenienza del record di Planning. Aggiungere informazioni quali il nome dell'area di lavoro o il nome del tipo di record. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td>
      <td> <p>(Obbligatorio) Il nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>(Consigliato) Inserisci eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p>
      <p>Qui è possibile aggiungere informazioni esplicite sul record e sugli oggetti che si stanno connettendo. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo oggetto</td> 
      <td><p>(Obbligatorio) Selezionare un tipo di oggetto Workfront connesso a un tipo di record in Workfront Planning.</p>
      È possibile selezionare uno dei seguenti tipi di oggetto:
      <ul><li> Progetto</li>
      <li> Portfolio</li><li> Programma</li><li> Azienda</li><li> Gruppo</li></ul>
       <p>Sono disponibili solo i tipi di oggetto di Workfront per i tipi di oggetto del modulo.</p> <p> Se, ad esempio, nell'elenco Tipi di oggetto nella parte superiore del progettista del modulo è visualizzato Progetto, in questo campo è possibile selezionare solo Progetto e non Portfolio, anche se i portfolio possono essere collegati anche ai tipi di record.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Area di lavoro</td> 
      <td> <p>(Obbligatorio) Selezionare l'area di lavoro di Planning da cui provengono i record che si desidera visualizzare in Workfront.</p> <p> Vengono visualizzate solo le aree di lavoro connesse ai tipi di oggetto selezionati nel campo Tipo oggetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di record</td> 
      <td><p>(Obbligatorio) Selezionare il tipo di record Workfront Planning che presenta una connessione con il tipo di oggetto Workfront.</p><p>Vengono visualizzati solo i tipi di record con connessioni al tipo di oggetto selezionato nel campo Tipo oggetto. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Campo connessione</td> 
      <td><p>(Obbligatorio) Selezionare il campo di connessione tra il tipo di record Planning selezionato che si desidera visualizzare sugli oggetti Workfront e il tipo di oggetto Workfront. </p> <p> <b>NOTA</b></p><p>È possibile avere più campi di connessione tra lo stesso oggetto e tipi di record, ma è possibile selezionare un solo campo.</p>  </td> 
     </tr>
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere altri campi.

   oppure

   Per copiare un campo, posiziona il cursore del mouse su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fare clic su **Salva e chiudi**.

   È ora possibile allegare il modulo a un oggetto connesso da Workfront Planning ed eseguire una delle operazioni seguenti:

   * Visualizzare i tipi di record di Workfront Planning connessi all&#39;oggetto Workfront, se presenti.
   * Connettere o disconnettere i record dall&#39;oggetto Workfront.

   Per ulteriori informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

## Organizzare e visualizzare in anteprima un modulo con il progettista del modulo

Per informazioni su come organizzare un modulo personalizzato con interruzioni di sezione e visualizzare un&#39;anteprima del modulo, vedere [Organizzare e visualizzare in anteprima un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
