---
title: Creare un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puoi progettare un modulo personalizzato con il designer dei moduli. Puoi allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/9vmobOfSleqLF7HqRnOav5IB1l8C4WPLO0vyEJwmfiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 07a00836f60ce0bb4ee7fb0202c9458b0c1be406
workflow-type: tm+mt
source-wordcount: 7795
ht-degree: 81%

---

# Creare un modulo personalizzato

<!-- Audited: 6/2025 -->

Puoi progettare un modulo personalizzato con il designer dei moduli di Adobe Workfront. Puoi allegare moduli personalizzati a diversi oggetti di Workfront per acquisire dati su tali oggetti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Per creare moduli personalizzati per ruoli, schede di valutazione e assegnazioni: Ultimate del flusso di lavoro</p>
      <p>Per creare moduli personalizzati per tutti gli altri oggetti supportati: qualsiasi pacchetto Workfront o Workflow</p> </td> 
  </tr>  
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai moduli personalizzati</td> 
  </tr>  
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Iniziare a progettare un modulo personalizzato

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Moduli personalizzati**, quindi seleziona **Moduli**.

1. Fai clic su **Nuovo modulo personalizzato.**
1. Seleziona i tipi di oggetto a cui desideri allegare il modulo personalizzato, quindi fai clic su **Continua**.

   ![Scegliere i tipi di oggetto](assets/new-custom-form-select-objects-new-spectrum-icons.png)

   +++ Espandere per visualizzare l&#39;elenco degli oggetti che supportano i moduli personalizzati.

   * Progetto
   * Attività
   * Problema/Richiesta
   * Portfolio
   * Documento
   * Programma
   * Spesa
   * Utente
   * Azienda
   * Iterazione
   * Record della fatturazione
   * Gruppo
   * Team

   Se ti trovi nel pacchetto Workflow Ultimate, puoi anche creare moduli personalizzati per questi oggetti:

   * Mansione
   * Scheda tariffa
   * Assegnazione

   +++

1. Nell’area **Aggiungi nome modulo** digita il titolo del modulo personalizzato.
1. (Facoltativo) Se si desidera aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic su **Tipi di oggetto** nell&#39;intestazione del progettista del modulo. Selezionare i tipi di oggetto che si desidera aggiungere e deselezionare qualsiasi tipo di oggetto che si desidera eliminare dal modulo.

   >[!CAUTION]
   >
   >L’eliminazione di un modulo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati degli oggetti ad esso associati. I dati eliminati non possono essere eliminati. In alternativa, puoi disattivare un modulo personalizzato che non utilizzi più, in modo da conservare tutti i dati storici associati.
   >
   >Per ulteriori informazioni, consulta [Aggiungere o eliminare tipi di oggetto da un modulo personalizzato esistente](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) e [Disattivare o riattivare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Successivamente, puoi iniziare ad aggiungere campi al modulo personalizzato. Per maggiori informazioni, consulta le seguenti sezioni:
   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Note sui nomi e sulle etichette dei campi](#notes-on-field-names-and-labels)
   * [Aggiungere campi di testo](#add-text-fields)
   * [Aggiungere campi calcolati](#add-calculated-fields)
   * [Aggiungere pulsanti di scelta, gruppi di caselle di controllo e menu a discesa](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [Aggiungi campi data](#add-date-fields)
   * [Aggiungere campi di ricerca esterni](#add-external-lookup-fields)
   * [Aggiungere immagini, PDF e video](#add-images-pdfs-and-videos)
   * [Aggiungere campi nativi Workfront](#add-workfront-native-fields)
   * [Aggiungere file Adobe XD](#add-adobe-xd-files)
   * [Aggiungere campi per pianificare una connessione](#add-planning-connection-fields)

## Aggiungere campi nuovi o esistenti al modulo personalizzato

Durante la progettazione di un modulo personalizzato, puoi utilizzare campi nuovi o esistenti.

I moduli personalizzati sono limitati a 500 campi. Un contatore in basso a sinistra mostra il numero di campi utilizzati nel modulo ed è sempre visibile durante lo scorrimento all’interno del designer dei moduli.

### Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato

1. Nella parte superiore a sinistra dello schermo, fai clic su **Libreria campi**.

1. Trascina il campo o il widget desiderato nell’area di lavoro. Ripeti questo passaggio per aggiungere altri campi o widget.

   >[!NOTE]
   >
   >In un singolo modulo personalizzato puoi aggiungere fino a 500 campi. Tuttavia, se in un modulo sono presenti più di 100 campi, potrebbe verificarsi un calo delle prestazioni a seconda della complessità.
   >
   >
   >Esempi di moduli complessi includono moduli con parametri a cascata, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

   >[!NOTE]
   >
   >Contrassegnando un campo esistente come inattivo, lo rende non più disponibile per l&#39;uso negli elementi di reporting e nei moduli personalizzati da quel momento in poi. Se il campo inattivo è attualmente in uso in un rapporto o in un modulo, il campo e i relativi dati storici rimangono invariati.

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Note sui nomi e sulle etichette API dei campi {#notes-on-field-names-and-labels}

* Le etichette sono disponibili per la maggior parte dei campi. Si tratta di etichette descrittive che vengono visualizzate sopra il campo o il widget nel modulo personalizzato. Puoi modificare le etichette in qualsiasi momento.

  >[!NOTE]
  >
  >Evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti.

* È necessario un nome API per ogni campo. Questo nome indica il modo in cui il sistema identifica il campo personalizzato quando viene aggiunto a varie aree di Workfront, ad esempio nei rapporti, nella Home e nelle interazioni API. Quando configuri il campo o il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.

* Ogni nome API per campo personalizzato deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo, puoi riutilizzarne uno che è già stato creato per un altro modulo personalizzato.

* Anche se è possibile farlo, ti consigliamo di non modificare questo nome API dopo che tu o altri utenti avete iniziato a utilizzare il modulo personalizzato in Workfront. Se lo facessi, il sistema non riconoscerebbe più il campo personalizzato nei punti di riferimento in altre aree di Workfront.

  Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome API, Workfront non lo riconosce nel rapporto e non funzionerà più correttamente a meno che non lo aggiungi nuovamente al rapporto utilizzando il nuovo nome.

* Per impostazione predefinita, i nomi API sono di sola lettura. Per rendere modificabile il nome API, fai clic sull&#39;icona **Modifica** accanto al **Nome API**. Digitare quindi **confirm** nella casella di conferma e fare clic su **Rinomina campo**.

* È consigliabile non digitare un nome API già utilizzato per i campi Workfront incorporati.

* È consigliabile non utilizzare il carattere punto/punto nel nome API del campo personalizzato per evitare errori quando si utilizza il campo in aree diverse di Workfront.

* I seguenti caratteri speciali non sono supportati nelle etichette di campo personalizzate e nei nomi API.

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

### Aggiungere campi di testo

In un modulo personalizzato puoi aggiungere diversi campi di testo.

+++ Espandi per visualizzare le descrizioni dei campi di testo disponibili.

* **Campo di testo su riga singola**: consente agli utenti di digitare una singola riga di testo nel campo.
* **Campo paragrafo**: consente agli utenti di digitare più righe di testo nel campo.
* **Testo formattato**: consente agli utenti di digitare più righe di testo nel campo e di formattare il testo con grassetto, corsivo, sottolineatura, punti elenco, numerazione, pedice e apice, collegamenti ipertestuali, virgolette, intestazioni e tabelle. Un limite di caratteri di 15.000 consente di disporre di un ampio spazio per il testo e la formattazione.

  >[!NOTE]
  >
  >Il tipo di campo Rich text sostituisce il tipo di campo Testo con formattazione. Puoi convertire rapidamente il testo esistente con campi di formattazione in testo formattato facendo clic sul pulsante **Converti in testo formattato** nelle opzioni di campo a destra.

<!--

* **Text field with formatting**: Allows users to type multiple lines of text in the field and format the text with bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. A character limit of 15,000 allows for plenty of text and formatting.

    This custom field type is not supported in filters on lists and reports.

    For information about accessing this field through the API, see [Rich text field storage in the API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

-->

* **Testo descrittivo**: consente di includere istruzioni e collegamenti a pagine esterne a Workfront.

+++

Per aggiungere un campo di testo:

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua uno dei campi di testo seguenti e trascinalo in una sezione dell’area di lavoro:

   * Testo su riga singola
   * Paragrafo
   * Testo formattato
   * Testo descrittivo
     <!--Text with formatting-->

   ![Trascina il campo nella sezione](assets/drag-field-to-section.png)

1. Sul lato a destra della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table>
    <tr>
    <td>Input in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr>
    <td>Dimensione</td>
    <td><p>(Facoltativo) Cambia le dimensioni dei campi di testo nel modulo.<p>
   </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo formattato</li>
    <li>Testo descrittivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etichetta</td>
    <td><p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare le etichette in qualsiasi momento.<p>
    <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p></td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo formattato</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nome API</td>
    <td><p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p>
    <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p>
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo formattato</li>
    <li>Testo descrittivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Istruzioni</td>
    <td>Digita eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo formattato</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formato</td>
    <td><p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p> <p><b>Nota</b>:   
    <ul> 
    <li>Questo campo non può essere modificato dopo il salvataggio del modulo. Se intendi utilizzare il campo in calcoli matematici, assicurati di selezionare il formato Numero o Valuta.</li> 
    <li>Quando selezioni Numero o Valuta, il sistema tronca automaticamente i numeri che iniziano con 0.</li>
    <li>Il limite di caratteri per i campi Numero è 16. Inoltre puoi utilizzare un campo Testo per inserire numeri ed evitare il limite.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    </ul></td>
    </tr>
    <tr>
      <td>Tipo di autorizzazione finanziaria</td>
      <td><p>Selezionare il tipo di autorizzazione per la contabilità che gli utenti devono avere prima di poter visualizzare o modificare questo campo personalizzato. Selezionare il formato Valuta.</p>
      <ul>
      <li><p><strong>Nessuna autorizzazione richiesta:</strong> Tutti gli utenti possono visualizzare questo campo</p></li>
      <li><p><strong>Generale:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le informazioni di contabilità generale</p></li>
      <li><p><strong>Fatturazione:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe di fatturazione</p></li>
      <li><p><strong>Costo:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe</p></li>
      </ul>
      <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md">Limitare l'accesso ai dati finanziari nei campi personalizzati</a>.</p>
      </td>
      <td><ul>
       <li>Testo su riga singola</li>
       <li>Paragrafo</li>
       </ul></td>
    </tr>
    <tr>
    <td>Tipo di visualizzazione</td>
    <td>Passa da un campo di testo su riga singola a un campo di testo paragrafo e viceversa.</td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Collegamento ipertestuale</td>
    <td> Se desideri applicare un collegamento ipertestuale al testo descrittivo digitato, aggiungilo qui. Il testo descrittivo viene visualizzato come collegamento sugli oggetti a cui è associato il modulo.</td>
    <td><ul><li>Testo descrittivo</li></ul></td>
    </tr>
    <tr>
     <td>Attivo</td>
     <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     <td><ul>
     <li>Testo su riga singola</li>
     <li>Paragrafo</li>
     <li>Testo formattato</li>
     <li>Testo descrittivo</li></ul></td>
    </tr>
    <tr> 
      <td>Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Paragrafo</li>
    <li>Testo formattato</li>
    </ul></td> 
    </tr> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere campi calcolati

In un modulo personalizzato, quando associato a un oggetto, puoi aggiungere un campo personalizzato calcolato che utilizza i dati esistenti per generarne dei nuovi.

Per aggiungere un campo calcolato, consulta [Aggiungere campi calcolati con il designer dei moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Aggiungere pulsanti di scelta, gruppi di caselle di controllo e menu a discesa

A un modulo personalizzato, puoi aggiungere pulsanti di scelta, gruppi di caselle di controllo, menu a discesa e menu a discesa a selezione multipla.

+++ Espandi per visualizzare la descrizione dei campi disponibili.

* **Pulsanti di scelta**: richiede agli utenti di selezionare una sola opzione.
* **Gruppo di caselle di controllo**: consente agli utenti di selezionare più opzioni.
* **Menu a discesa a selezione singola**: fornisce un elenco di opzioni a discesa.
* **Menu a discesa a selezione multipla**: consente agli utenti di selezionare più opzioni da un elenco a discesa.

+++

>[!NOTE]
>
>I campi che consentono selezioni multiple, come i gruppo di caselle di controllo e il menu a discesa a selezione multipla, sono difficili da rappresentare nei grafici e da raggruppare nei rapporti. Per semplificare la creazione di grafici e il raggruppamento nei rapporti, puoi creare campi separati per ciascuna scelta, ad esempio un campo di testo a riga singola.

Per aggiungere pulsanti di scelta, gruppi di caselle di controllo e menu a discesa:

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro:

   * Pulsanti di scelta
   * Gruppo di caselle di controllo
   * Elenco a discesa a selezione singola
   * Elenco a discesa a selezione multipla

   ![Trascinare un campo nell’area di lavoro](assets/drag-field-to-section.png)

1. Sul lato a destra della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Input in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr> 
     <td role="rowheader">Etichetta</td> 
     <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td> 
     <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nome API</td> 
     <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p> 
    <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sui nomi e le etichette dei campi</a>.</p> </td>
     <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Istruzioni</td> 
    <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formato</td> 
    <td> <p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p> <p><b>Nota</b>:   
     <ul> 
    <li>Questo campo non può essere modificato dopo il salvataggio del modulo. Se intendi utilizzare il campo in calcoli matematici, assicurati di selezionare il formato Numero o Valuta.<br></li> 
    <li>Quando selezioni Numero o Valuta, il sistema tronca automaticamente i numeri che iniziano con 0.</li>
    <li>Il limite di caratteri per i campi Numero è 16. Inoltre puoi utilizzare un campo Testo per inserire numeri ed evitare il limite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
    </tr> 
    <tr>
      <td>Tipo di autorizzazione finanziaria</td>
      <td><p>Selezionare il tipo di autorizzazione per la contabilità che gli utenti devono avere prima di poter visualizzare o modificare questo campo personalizzato. Selezionare il formato Valuta.</p>
      <ul>
      <li><p><strong>Nessuna autorizzazione richiesta:</strong> Tutti gli utenti possono visualizzare questo campo</p></li>
      <li><p><strong>Generale:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le informazioni di contabilità generale</p></li>
      <li><p><strong>Fatturazione:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe di fatturazione</p></li>
      <li><p><strong>Costo:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe</p></li>
      </ul>
      <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md">Limitare l'accesso ai dati finanziari nei campi personalizzati</a>.</p>
      </td>
      <td><ul>
       <li>Pulsanti di scelta</li>
       <li>Gruppo di caselle di controllo</li>
       <li>Elenco a discesa a selezione singola</li>
       <li>Elenco a discesa a selezione multipla</li>
       </ul></td>
    </tr>
    <tr> 
     <td role="rowheader">Tipo di visualizzazione</td> 
    <td>Passa da un pulsante di scelta all’altro, da un gruppo di caselle di controllo all’’altro, da un elenco a discesa a selezione singola o da un elenco a discesa a selezione multipla per il campo.</td> 
    <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
    </tr> 
    <td role="rowheader">Scelte </td> 
    <td> 
    <p>Seleziona una delle opzioni seguenti:</p> 
    <ul> 
    <li><strong>Mostra valori</strong>: mostra i valori di ciascuna opzione nel campo. L’etichetta di ciascuna opzione viene mostrata per impostazione predefinita.</li>
   <li><strong>Ordina scelte dalla A alla Z</strong>: ordina in ordine alfabetico le scelte aggiunte nel campo.</li>
    </ul>
     <p>Per ciascuna scelta aggiunta per l’utente, fai clic sull’icona a forma di ingranaggio <img src="assets/gear-icon-settings.png">, quindi seleziona una delle opzioni seguenti:</p> 
    <ul> 
    <li><strong>Seleziona per impostazione predefinita</strong>: seleziona la scelta per impostazione predefinita nel campo.</li> 
    <li> <p><strong>Nascondi scelta</strong>: nascondi la scelta nel campo. Le scelte nascoste rimangono accessibili nei rapporti.</p> </li> 
    <li> <p><strong>Rimuovi scelta</strong>: rimuovi la scelta dal campo.</p> <p><b>Avvertenza</b>: se sono presenti oggetti correnti che utilizzano questa scelta, non rimuoverla dal campo. Rimuovendola, i dati storici andranno persi. In alternativa, seleziona l’opzione per nasconderla per impedire agli utenti di selezionarla in futuro.</p> </li> 
    </ul>   
    <p><b>Nota:</b> non esiste alcun limite al numero di scelte selezionabili. </p>    
    </td> 
    <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul>
    </td>
     </tr>
    <tr>
     <td>Attivo</td>
     <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     <td><ul>
     <li>Pulsanti di scelta</li>
     <li>Gruppo di caselle di controllo</li>
     <li>Elenco a discesa a selezione singola</li>
     <li>Elenco a discesa a selezione multipla</li></ul></td>
    </tr>
    <tr> 
    <td role="rowheader">Rendi il campo obbligatorio</td> 
    <td>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
    <td><ul>
    <li>Pulsanti di scelta</li>
    <li>Gruppo di caselle di controllo</li>
    <li>Elenco a discesa a selezione singola</li>
    <li>Elenco a discesa a selezione multipla</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![Icona Copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

<!--

### Add typeahead and date fields

 You can add typeahead and date fields to a custom form.

+++ Expand to see descriptions of available fields.

* **Typeahead**: Allows users to type the name of an object that exists in Workfront. A list of suggestions appears when the user starts typing. This field type supports the following objects:
    * User
    * Group
    * Job Role
    * Portfolio
    * Program
    * Project
    * Team
    * Template
    * Company
* **Date**: Displays a calendar where users can select a date and time.

+++

To add typeahead and date fields:

1. In the **New field** tab on the left side of the screen, find one of the following fields and drag it to a section on the canvas.

    * Typeahead
    * Date

    ![Drag field to section](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

    <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Field setting</td>
    <td>Description</td>
    <td>Available for </td>
    </tr>
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the custom field. You can change the label at any time.</p> <p><b>Important</b>: Avoid using special characters in this label as they don't display correctly in reports. For more information, see <a href="design-a-form.md#notes-on-field-names-and-labels">Notes on field names and labels</a>.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Required) This name is how the system identifies the field. When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. The Label and Name fields are not synchronized. This gives you the option to change the label that your users see without having to change the name that the system sees.</p> 
      <p>For more information, see <a href="design-a-form.md#notes-on-field-names-and-labels">Notes on field names and labels</a>.</p> </td>
    <td><ul>
    <li>Typeahead</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the custom field. When users fill out the custom form, they can hover over the question mark icon to view a tooltip containing the information you type here.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Display Time of Day</td> 
      <td>Select this option if you want to show the time of day along with the date in the field.</td> 
         <td><ul>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Referenced Object Type</td> 
      <td> <p>Select the object type that you want to associate with the field.</p> <p>Once you have clicked <b>Apply</b> or <b>Save and Close</b>, you can't change the object type for the field.</p> <p><b>Note</b>:   
        <ul> 
         <li>If your Workfront administrator customized the name for Portfolios, Programs, or Projects in the Workfront user interface, the default Workfront name for the object appears in this drop-down list, not the customized name. See your Workfront administrator if you need help with this.<br></li> 
         <li>The following object types are supported in the iOS and Android Workfront Mobile Apps: User, Company, Group, Job Role, Portfolio, Program, Project, and Template.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Add Filter</td>
      <td><p>Add a filter for an object type to limit the objects users can choose when they are using the field. </p> <p>For example, you could limit a field so that usernames can be selected only if they meet the following criteria:</p> 
       <ul> 
        <li>They belong to a group or groups that you specify.</li> 
        <li>They are associated with a role or job title you specify.</li> 
        <li>They belong to the same group as the person using the field.</li> 
       </ul>
       <p>You must define the filter for the object type you selected using Text Mode syntax. For information about creating a filter using Text Mode, see <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Edit a filter using text mode</a>.</p>
       <p><b>Tip:</b> You can create a report to test your filter before adding the filter directly to the typeahead field. This will help you verify that the filter returns the correct objects. Then you can switch to text mode in the report, copy the text mode statement, and add it to the typeahead filter.</p>
       <p><b>Note</b>:
       <ul> 
        <li>If you are editing an existing custom form, adding a filter to a typeahead field does not remove any objects (outside the scope of the filter) that users have already added using the field.</li> 
        <li>This filter is not available on mobile devices. If you use the filter for a typeahead field, the field will appear on users' mobile devices unaffected by the filter.</li> 
        </ul></p>
      </td>  
      <td>
       <ul>
       <li>Typeahead</li>
       </ul>
      </td>
     </tr>
     <tr>
      <td>Active</td>
      <td><p>This option is turned on by default.<p><p>When you set a field as Inactive, it is excluded from reports, filters, and views, and is no longer available in the custom forms field library.</p></td>
      <td><ul>
      <li>Typeahead</li>
      <li>Date</li></ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Make a required field</td> 
      <td>Select this option if you want the field to be required in order for the user to complete the custom form. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Date</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat the previous step to add any other fields or widgets. 

    Or

    To copy a field, hover over a field, and click the copy icon.

    ![copy icon](assets/copy-field.png)

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    Or

    Click **Save and Close**.

-->

### Aggiungi campi data

Un campo data visualizza un calendario in cui gli utenti possono selezionare una data e un’ora.

Per aggiungere campi data:

1. Nella scheda **Nuovo campo** sul lato sinistro dello schermo, individua **Data** e trascinalo in una sezione dell&#39;area di lavoro.

   ![Trascina il campo nella sezione](assets/drag-field-to-section.png)

1. Sul lato a destra dello schermo, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p> <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Visualizza ora del giorno</td>
      <td><p>Seleziona questa opzione se desideri visualizzare l’ora del giorno insieme alla data nel campo.</p></td>
     </tr> 
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere campi di ricerca esterni

Un campo di ricerca esterna richiama un’API esterna e restituisce i valori come opzioni in un campo a discesa. Gli utenti che utilizzano l’oggetto a cui è associato il modulo personalizzato possono selezionare una o più di queste opzioni dall’elenco a discesa, a seconda che il campo di ricerca esterna sia a selezione singola o multipla. I campi di ricerca esterna sono disponibili anche negli elenchi e nei rapporti.

Per esempi sull’utilizzo del campo di ricerca esterna per chiamare la stessa istanza di Workfront o un’API pubblica, consulta [Esempi di campo di ricerca esterna in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* I campi di ricerca esterna non sono disponibili negli elenchi quando il campo dipende da un altro campo.

Per aggiungere una ricerca esterna:

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua **Ricerca esterna** o **Ricerca esterna a selezione multipla** e trascinala in una sezione dell’area di lavoro.
1. Sul lato a destra dello schermo, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome API non sono sincronizzati: ciò ti offre la possibilità di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p>
      <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note su etichette e nomi dei campi</a>.</p> </td>
     </tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td>
      <td><p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato.</p>
      <p><strong>Nota:</strong></p>
      <ul><li>Puoi modificare il tipo di formato dopo il salvataggio del modulo, con unico limite: tutti i valori esistenti negli oggetti devono poter essere convertiti al nuovo tipo. Ad esempio, se il tipo di formato è Testo e un oggetto memorizza il valore "abc", non è possibile convertire il campo e viene visualizzato un errore che indica che il sistema non può convertire "abc" in numero/valuta. Se intendi utilizzare il campo in calcoli matematici, assicurati di selezionare il formato Numero o Valuta.</li>
      <li>Quando selezioni Numero o Valuta, il sistema tronca automaticamente i numeri che iniziano con 0.</li>
      <li>Il limite di caratteri per i campi Numero è 16. Inoltre puoi utilizzare un campo Testo per inserire numeri ed evitare il limite.</li>
      </ul></td>
     </tr> 
     <tr>
      <td>Tipo di autorizzazione finanziaria</td>
      <td><p>Selezionare il tipo di autorizzazione per la contabilità che gli utenti devono avere prima di poter visualizzare o modificare questo campo personalizzato. Selezionare il formato Valuta.</p>
      <ul>
      <li><p><strong>Nessuna autorizzazione richiesta:</strong> Tutti gli utenti possono visualizzare questo campo</p></li>
      <li><p><strong>Generale:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le informazioni di contabilità generale</p></li>
      <li><p><strong>Fatturazione:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe di fatturazione</p></li>
      <li><p><strong>Costo:</strong> gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe</p></li>
      </ul>
      <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md">Limitare l'accesso ai dati finanziari nei campi personalizzati</a>.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">URL API base</td> 
      <td><p>Digita o incolla l’URL per l’API.</p><p>L’URL dell’API deve restituire il contenuto JSON delle opzioni che desideri visualizzare nel menu a discesa. Puoi utilizzare il campo Percorso JSON per selezionare i valori specifici dal JSON restituito da utilizzare come opzioni del menu a discesa.</p><p>Quando inserisci l’URL dell’API, puoi facoltativamente passare i seguenti valori nell’URL:</p>
      <ul>
      <li>$$HOST: rappresenta l’host corrente di Workfront e può essere utilizzato per effettuare/cercare chiamate API verso l’API di Workfront. Quando si utilizza questo carattere jolly, l’autenticazione viene gestita automaticamente e gli utenti non devono inviare intestazioni di autenticazione. Gli utenti, ad esempio, possono cercare le attività utilizzando l’URL di base <code>$$HOST/attask/api/task/search</code>; questo consentirà di effettuare la ricerca e di selezionare i valori da un elenco di attività restituito.</li>
      <li><p>$$QUERY: rappresenta il testo di ricerca digitato dall’utente finale nel campo e ti consente di implementare il filtro delle query per i tuoi utenti. L’utente cercherà il valore nel menu a discesa.</p>
      <p>Se l’API a cui stai facendo riferimento lo consente, puoi anche includere dei modificatori nella query di ricerca per definire le modalità di esecuzione della ricerca stessa. Ad esempio, puoi utilizzare quanto segue come URL API di base per consentire agli utenti di cercare qualsiasi progetto Workfront contenente testo specifico: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Ulteriori informazioni sui modificatori di ricerca Workfront sono disponibili nella sezione <a href="/help/quicksilver/wf-api/general/api-basics.md">Nozioni di base sulle API</a>.</p>
      <p><strong>Nota:</strong> se non utilizzi $$QUERY e l’utente digita del testo nella casella di ricerca, le opzioni già disponibili verranno ridotte. Tuttavia, se utilizzi $$QUERY e l’utente digita qualsiasi carattere, viene eseguita una nuova chiamata di rete all’API. Pertanto, se l’API contiene più di 2000 valori e l’API supporta l’esecuzione di query, puoi utilizzare $$QUERY per effettuare ricerche non solo tra i 2000 valori esistenti, ma dall’API originale con le opzioni ridotte.</p></li>
      <li><p>{fieldName}: dove fieldName è un campo personalizzato o nativo in Workfront. In questo modo puoi implementare i filtri a cascata per le opzioni a discesa, passando il valore di un campo già selezionato al campo di ricerca esterna per filtrare le opzioni. Ad esempio, il campo Area geografica esiste già nel modulo e stai restringendo un elenco di paesi provenienti dall’API solo a quelli che si trovano in un’area geografica specifica.</p>
      <p>Per un campo di ricerca esterna che dipende da altri campi (utilizzando la sintassi {fieldName}), le opzioni restituite dall’API sono limitate a quelle che corrispondono a eventuali stringhe o valori inseriti negli altri campi. Questa funzionalità non è supportata negli elenchi e nei rapporti.</p></li>
      <li>{referenceObject}.{fieldName} - Dove il campo fa parte di un oggetto. Questa sintassi è simile alle espressioni personalizzate. (ad esempio, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>Suggerimento:</strong> rivedi la documentazione dell’API che stai utilizzando per le query specifiche che puoi definire.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Metodo HTTP</td> 
      <td>Seleziona <strong>GET</strong>, <strong>POST</strong> o <strong>PUT</strong> come metodo.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Percorso JSON</td>
      <td><p>Inserisci o incolla il percorso JSON per l’API.</p> <p>Questa opzione consente di estrarre i dati dal JSON restituito dall’URL dell’API. Serve come metodo per selezionare quali valori dall’interno del JSON appariranno tra le opzioni del menu a discesa.</p><p>Ad esempio, se l’URL API restituisce JSON nel seguente formato, puoi utilizzare "$.data[*].name" per selezionare Stati Uniti e Canada come opzioni a discesa:</br>
      <pre>
      {
       dati: {
         { name: "USA"},
         { name: "Canada"}
       }
      }
      </pre>
      </p>
     <p>Per ulteriori informazioni sul percorso JSON e per assicurarti che la scrittura del percorso JSON sia corretta, visita il sito <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Intestazioni</td>
      <td><p>Fai clic su <strong>Aggiungi intestazione</strong>, quindi digita o incolla la coppia chiave-valore richiesta per l’autenticazione con l’API.</p><p><strong>Nota:</strong> i campi Intestazione non sono un luogo sicuro in cui memorizzare le credenziali. Presta attenzione a ciò che inserisci e salvi.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Elenco a discesa a selezione multipla</td>
      <td><p>Seleziona questa opzione per consentire all’utente di selezionare più di un valore nel menu a discesa.</p></td>
     </tr>
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr>       
    </tbody>
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

>[!NOTE]
>
>Gli elementi seguenti rappresentano limitazioni tecniche della chiamata all’API esterna:
>
>* Numero massimo di opzioni: 2000 (vengono visualizzate solo le prime 2000 opzioni univoche del JSON restituito)
>* Timeout: 30 secondi
>* Numero di nuovi tentativi: 3
>* Durata dell’attesa tra nuovi tentativi: 500 ms
>* Stati di risposta previsti: 2xx



### Aggiungere campi di ricerca interni

Un campo di ricerca interno consente agli utenti di digitare il nome di un oggetto esistente in Workfront. Quando l’utente inizia a digitare, viene visualizzato un elenco di suggerimenti. Ad esempio, se l’utente digita un nome utente, viene visualizzato un elenco di nomi corrispondenti. Il tipo di campo di ricerca interno è supportato nei seguenti oggetti:

* Utente
* Gruppo
* Mansione
* Portfolio
* Programma
* Progetto
* Team
* Modello
* Azienda
* Attività
* Problema
* Documento
* Posizione

Per aggiungere una ricerca interna:

1. Nella scheda **Nuovo campo** sul lato sinistro dello schermo, individua **Ricerca interna** o **Ricerca interna a selezione multipla** e trascinala in una sezione dell&#39;area di lavoro.
1. Sul lato a destra dello schermo, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome API non sono sincronizzati: ciò ti offre la possibilità di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p>
      <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note su etichette e nomi dei campi</a>.</p> </td>
     </tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto di riferimento</td>
      <td><p>Seleziona il tipo di oggetto da associare al campo.</p> <p>Non puoi modificare il tipo di oggetto per il campo dopo aver fatto clic su <strong>Applica</strong> o <strong>Salva e chiudi</strong>.</p>
      <p><strong>Nota:</strong></p>
      <ul><li>Se l’amministratore Workfront ha personalizzato il nome di Portfolio, Programmi o Progetti nell’interfaccia utente di Workfront, in questo elenco a discesa viene visualizzato il nome predefinito di Workfront per l’oggetto e non il nome personalizzato. Se hai bisogno di assistenza, rivolgiti al tuo amministratore Workfront.</li>
      <li>Nelle app Workfront per dispositivi mobili iOS e Android sono supportati i seguenti tipi di oggetti: Utente, Azienda, Gruppo, Mansione, Portfolio, Programma, Progetto e Modello.</li>
      </ul></td>
     </tr> 
     <tr>
      <td>Aggiungi filtro</td>
      <td><p>Aggiungi un filtro per un tipo di oggetto per limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul> 
        <li>Appartengono a uno o più gruppi specificati.</li> 
        <li>Sono associati a un ruolo o a una mansione specifica.</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo.</li> 
       </ul>
       <p>È necessario definire il filtro per il tipo di oggetto selezionato utilizzando la sintassi della modalità testo. Per informazioni sulla creazione di un filtro utilizzando la modalità testo, consulta <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modifica un filtro in modalità testo</a>.</p>
       <p><b>Suggerimento:</b> è possibile creare un report per testare il filtro prima di aggiungerlo direttamente al campo di ricerca interno. Questo ti consentirà di verificare che il filtro restituisca gli oggetti corretti. Quindi puoi passare alla modalità testo nel rapporto, copiare l’istruzione della modalità testo e aggiungerla al filtro di ricerca interno.</p>
       <p><b>Nota</b>:
       <ul> 
        <li>Se si sta modificando un modulo personalizzato esistente, l'aggiunta di un filtro a un campo di ricerca interno non rimuove gli oggetti già aggiunti dagli utenti utilizzando il campo (al di fuori dell'ambito del filtro).</li> 
        <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo di ricerca interno, il campo verrà visualizzato sui dispositivi mobili degli utenti che non sono interessati dal filtro.</li> 
        </ul></p>
      </td>  
     </tr>
     <tr> 
      <td role="rowheader">Elenco a discesa a selezione multipla</td>
      <td><p>Seleziona questa opzione per consentire all’utente di selezionare più di un valore nel menu a discesa.</p></td>
     </tr>
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr>       
    </tbody>
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere immagini, PDF e video

Puoi aggiungere immagini, PDF e video a un modulo personalizzato. Gli utenti che utilizzano l’oggetto a cui è associato il modulo personalizzato possono visualizzare l’immagine, il PDF o il video solo nelle seguenti aree:

* L’area Dettagli degli oggetti (ad esempio, per un progetto, l’area Dettagli progetto).
* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività).

<!--
 Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app
-->

+++ Espandi per visualizzare la descrizione dei campi disponibili.

* **Immagine**: consente agli utenti di aggiungere file di immagine.
* **PDF**: consente agli utenti di aggiungere PDF
* **Video**: consente agli utenti di aggiungere file video.

+++

Per aggiungere immagini, PDF o video:

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Immagine
   * PDF
   * Video

   ![Trascina campo nella sezione](assets/drag-field-to-section.png)

1. Digita o modifica una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Dimensioni</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p> <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla l’URL del widget nel punto in cui è memorizzato su Internet.</p> 
      <p>Se stai aggiungendo un widget video, al momento puoi farlo inserendo quanto segue nella casella dell’URL:</p> 
      <ul> 
      <li> <p>Collegamento YouTube o Vimeo</p> </li> 
      <li> <p>Collegamento video Google Drive</p> </li> 
      <li> <p>Collegamento a video con estensione MP4 e MOV</p> </li> 
      <li> <p>Collegamento a video già caricati nell’area Documenti della tua istanza di Workfront. Per istruzioni, consulta <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Aggiungere un widget video a un modulo personalizzato dall’area Documenti</a> in questo articolo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
    </tbody> 
   </table>

   >[!NOTE]
   >Per i PDF, si consiglia di utilizzare Grande come dimensione di visualizzazione del widget.
   >Il visualizzatore PDF del browser influisce sulla visualizzazione per gli utenti, che potrebbero dover regolare le dimensioni della finestra e la percentuale di zoom del browser se la visualizzazione del PDF non è ottimale.

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

#### Aggiungere un video a un modulo personalizzato dall’area Documenti{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Quando aggiungi un video a un modulo personalizzato in questo modo, le autorizzazioni impostate nell’area Documenti vengono applicate al video quando gli utenti accedono al modulo da un oggetto.

1. Passa al video nell’area Documenti e genera una bozza per esso, come descritto in [Creare una bozza interattiva per un sito web o altri contenuti web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Apri la bozza.
1. Fai clic con il pulsante destro del mouse in un punto qualsiasi del video, quindi seleziona **Copia indirizzo video**.
1. Nel modulo personalizzato in cui stai aggiungendo il widget video, incolla l’indirizzo copiato nella casella **URL**.
1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere campi nativi Workfront

Puoi aggiungere campi nativi di Workfront ai moduli personalizzati. Quando il modulo personalizzato viene associato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, il campo Descrizione in un modulo personalizzato associato a un progetto acquisirà direttamente la descrizione del progetto. Il campo può mostrare “N/D” se non sono disponibili dati.

+++ Espandi per visualizzare l’elenco dei campi nativi supportati.

In questa tabella sono elencati i campi nativi disponibili per gli oggetti specifici di Workfront in un modulo personalizzato.

| Nome campo | Progetto | Attività | Problema | Modello | Attività modello | Portfolio | Programma | Gruppo |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Vantaggio corrente | ✓ |   |   |   |   |   |   |   |
| Data di completamento effettiva | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durata effettiva | ✓ |   |   |   |   |   |   |   |
| Ore effettive | ✓ |   | ✓ |   |   |   |   |   |
| Data di inizio effettiva | ✓ | ✓ | ✓ |   |   |   |   |   |
| Budget | ✓ |   |   | ✓ |   | ✓ |   |   |
| Azienda | ✓ |   |   | ✓ |   |   |   |   |
| Condizione | ✓ | ✓ | ✓ |   |   |   |   |   |
| Tipo di condizione | ✓ |   |   | ✓ |   |   |   |   |
| Valuta | ✓ |   |   | ✓ |   |   |   |   |
| Descrizione | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Durata |   | ✓ |   |   | ✓ |   |   |   |
| Tipo di durata |   | ✓ |   |   | ✓ |   |   |   |
| Unità di durata |   | ✓ |   |   | ✓ |   |   |   |
| Inserito da | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Data inserimento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Data tasso di cambio | ✓ |   |   |   |   |   |   |   |
| Costi fissi | ✓ |   |   | ✓ |   |   |   |   |
| Reddito Fisso | ✓ |   |   | ✓ |   |   |   |   |
| Gruppo | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Ultimo aggiornamento di | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Data ultimo aggiornamento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Nome | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Proprietario | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Metodo indice prestazioni | ✓ |   |   | ✓ |   |   |   |   |
| Beneficio pianificato | ✓ |   |   | ✓ |   |   |   |   |
| Data di completamento pianificata | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durata pianificata | ✓ |   |   | ✓ |   |   |   |   |
| Lavoro Necessario | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Data di inizio pianificata | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Priorità | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programma | ✓ |   |   | ✓ |   |   |   |   |
| Data di completamento prevista | ✓ | ✓ |   |   |   |   |   |   |
| Durata prevista in minuti |   | ✓ |   |   |   |   |   |   |
| Data di inizio prevista | ✓ | ✓ |   |   |   |   |   |   |
| Numero di riferimento | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Modalità pianificazione | ✓ |   |   | ✓ |   |   |   |   |
| Gravità |   |   | ✓ |   |   |   |   |   |
| Sponsor | ✓ |   |   | ✓ |   |   |   |   |
| Stato | ✓ | ✓ |   |   |   |   |   |   |
| Punti storia |   | ✓ |   |   |   |   |   |   |
| Modello | ✓ |   |   |   |   |   |   |   |
| Costo totale stimato | ✓ |   |   | ✓ |   |   |   |   |
| Ricavi totali stimati | ✓ |   |   | ✓ |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

Questi tipi di oggetto modulo personalizzati aggiuntivi supportano anche riferimenti a campi nativi.

* Record fatturazione: campo Reddito fisso
* Documento: campi Nome, Descrizione
* Società: campi Nome, Gruppo
* Scheda tariffa: campi Nome, Descrizione, Società, Gruppo
* Mansione: campi Nome, Descrizione

<!--
Non-Labor Resource: Name, Description, Home Group, Non-labor Category, Non-labor Group, Unique Identifier fields
Staffing Plan: Name, Description, Owner, Group, Company, Currency, Schedule, Start Date, End Date, Available Estimated Hours, Total Estimated Hours, Reference Number, Entered By, Entry Date, Last Updated By, Last Updated Date, Total Estimated Cost, Total Estimated Revenue fields
Staffing Plan Resource: Total Estimated Cost, Total Estimated Revenue fields
-->

+++

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua **Riferimento di campo nativo** e trascinalo in una sezione dell’area di lavoro.
1. Sul lato a destra dello schermo, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Dimensioni</td> 
      <td>(Facoltativo) Modifica le dimensioni di visualizzazione del campo in base alle esigenze.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td>
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p>
      <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo di riferimento</td> 
      <td><p>(Obbligatorio) Seleziona un campo nativo di Workfront.<p><p>Sono disponibili solo campi nativi per gli oggetti del modulo. Ad esempio, se l’elenco Tipi di oggetto nella parte superiore del designer dei moduli mostra Progetto, potrai selezionare campi nativi per i progetti ma non campi specifici delle attività.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Aggiungi filtro</td>
      <td><p>Aggiungi un filtro per il campo di riferimento per limitare l’elenco di elementi tra cui gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul>
        <li>Appartengono a uno o più gruppi specificati.</li> 
        <li>Sono associati a un ruolo o a una mansione specifica.</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo.</li> 
       </ul>
       <p>Se nel campo è presente un filtro di sistema, viene applicato per impostazione predefinita se non si aggiunge un filtro personalizzato. Un filtro personalizzato sostituisce il filtro di sistema.</p>
       <p>È necessario definire il filtro per il campo di riferimento selezionato utilizzando la sintassi della modalità testo. Per informazioni, consulta <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modificare un filtro utilizzando la modalità testo</a>.</p>
       <p>Utilizza la sintassi del filtro dinamico per restringere l’elenco di elementi in questo campo in base al valore di un altro campo. Se, ad esempio, si utilizza <code>?portfolioID={portfolio}.{ID}</code> in un filtro di campi di Project e un campo nativo di Portfolio si trova nel modulo personalizzato, nel campo Project vengono visualizzati solo i progetti inclusi nel portfolio selezionato. Se il campo Portfolio viene lasciato vuoto, tutti i progetti saranno disponibili nel campo Progetto.</p>
       <p><b>Nota</b>:
       <ul> 
        <li>L’opzione filtro è disponibile solo quando si fa riferimento a un campo di ricerca nativo typeahead o interno, ad esempio Portfolio, Company o Owner.</li>
        <li>Se stai modificando un modulo personalizzato esistente, l’aggiunta di un filtro a un campo nativo non rimuove gli oggetti (al di fuori dell’ambito del filtro) che gli utenti hanno già aggiunto utilizzando quel campo.</li> 
        <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo nativo, il campo verrà visualizzato sui dispositivi mobili degli utenti non interessati dal filtro.</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td>
      <td><p>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere file Adobe XD

Puoi aggiungere un prototipo Adobe XD direttamente a un modulo personalizzato. Gli utenti che utilizzano l’oggetto a cui è associato il modulo personalizzato possono visualizzare il file Adobe XD solo nelle seguenti aree:

* L’area Dettagli degli oggetti (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica dell’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio le caselle Modifica progetto e Modifica attività)

Per aggiungere un file Adobe XD:

1. Nella scheda **Nuovo campo** sul lato a sinistra dello schermo, individua **Adobe XD** e trascinalo in una sezione dell’area di lavoro.
1. Digita o modifica una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Dimensioni</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali nelle etichette in quanto non vengono visualizzati correttamente nei rapporti. Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il widget. Quando configuri il widget per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p>
    <p>Per ulteriori informazioni, consulta <a href="design-a-form.md#notes-on-field-names-and-labels">Note sulle etichette e sui nomi dei campi</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla un collegamento valido per il prototipo XD.</p> 
      <p><b>Nota</b>: l’impostazione Accesso al collegamento nella scheda Condividi di Adobe XD deve essere impostata su Chiunque abbia il collegamento. In caso contrario, gli utenti non potranno visualizzare il prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Digita eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr>
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere campi per pianificare una connessione

>[!IMPORTANT]
>
>Le informazioni contenute in questa sezione si riferiscono alla Pianificazione di Workfront di Adobe, una funzionalità aggiuntiva di Adobe Workfront.
>
>Per accedere a Pianificazione di Workfront è necessario disporre di pacchetti aggiuntivi.
>
>Per un elenco completo dei requisiti per accedere a Pianificazione di Workfront, consulta [Panoramica sull’accesso a Pianificazione di Workfront di Adobe](/help/quicksilver/planning/access/access-overview.md).
> 
>Per ulteriori informazioni su Pianificazione di Workfront, consulta [Introduzione a Pianificazione di Workfront di Adobe](/help/quicksilver/planning/general/planning-overview.md).

Puoi visualizzare i record connessi da Pianificazione di Workfront in un campo personalizzato di un oggetto Workfront aggiungendo un campo personalizzato di tipo Pianificazione connessione al modulo personalizzato di un oggetto.

Puoi aggiungere il campo di tipo Pianificazione connessione ai moduli personalizzati di tutti gli oggetti. Tuttavia, è possibile visualizzare i record connessi solo nei moduli personalizzati associati agli oggetti di Workfront che possono essere connessi da Pianificazione di Workfront.

>[!NOTE]
>
>Gli utenti che visualizzano le informazioni nel campo personalizzato devono avere accesso a Pianificazione di Workfront e alle aree di lavoro che contengono i tipi di record connessi agli oggetti di Workfront.

Per aggiungere un campo di tipo Pianificazione connessione:

1. Nella scheda **Nuovo campo** sul lato a sinistra della schermata, individua **Pianificazione connessione** e trascinala in una sezione dell’area di lavoro.
1. Sul lato a destra dello schermo, configura le opzioni per il campo personalizzato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Dimensioni</td> 
      <td>(Facoltativo) Modifica la dimensione di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo. Puoi modificare le etichette in qualsiasi momento.</p> <p><b>Importante</b>: evita di utilizzare caratteri speciali per le etichette.</p> 
      <p>È consigliabile scegliere un’etichetta che consenta di identificare facilmente la provenienza del record di pianficazione. Aggiungi informazioni quali il nome dell’area di lavoro o il nome del tipo di record. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome API</td>
      <td> <p>(Obbligatorio) Il nome indica il modo in cui il sistema identifica il campo. Quando configuri il campo per la prima volta e digiti l’etichetta, il campo Nome API si popola automaticamente in modo che corrisponda a esso. I campi Etichetta e Nome API non sono sincronizzati. Questo ti permette di modificare l’etichetta visualizzata dagli utenti senza dover cambiare il nome riconosciuto dal sistema.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>(Consigliato) Digita eventuali informazioni aggiuntive sul campo. Quando gli utenti compilano il modulo personalizzato, possono passare il puntatore sull’icona a forma di punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p>
      <p>Qui puoi aggiungere informazioni dettagliate sul record e sugli oggetti che stai connettendo. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto</td> 
      <td><p>(Obbligatorio) Seleziona un tipo di oggetto Workfront connesso a un tipo di record in Pianificazione di Workfront.</p>
      Puoi selezionare uno dei seguenti tipi di oggetto:
      <ul><li> Progetto</li>
      <li> Portfolio</li><li> Programma</li><li> Azienda</li><li> Gruppo</li></ul>
       <p>Sono disponibili solo i tipi di oggetto Workfront per i tipi di oggetto del modulo.</p> <p> Ad esempio, se l’elenco Tipi di oggetto nella parte superiore del designer dei moduli mostra Progetto, in questo campo potrai selezionare solo Progetto e non Portfolio, sebbene i portfolio possono essere collegati anche ai tipi di record.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Area di lavoro</td> 
      <td> <p>(Obbligatorio) Seleziona l’area di lavoro di pianificazione da cui provengono i record che desideri visualizzare in Workfront.</p> <p> Vengono visualizzate solo le aree di lavoro collegate ai tipi di oggetto selezionati nel campo Tipo di oggetto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di record</td> 
      <td><p>(Obbligatorio) Seleziona il tipo di record in Pianificazione di Workfront che presenta un collegamento con il tipo di oggetto Workfront.</p><p>Vengono visualizzati solo i tipi di record con collegamenti al tipo di oggetto selezionato nel campo Tipo oggetto. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Campo connessione</td> 
      <td><p>(Obbligatorio) Seleziona il campo di connessione tra il tipo di record Planning selezionato che desideri visualizzare sugli oggetti Workfront e il tipo di oggetto Workfront. </p> <p> <b>Nota</b>: è possibile disporre di più campi di connessione tra lo stesso oggetto e tipi di record, ma è possibile selezionare un solo campo.</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">Campi del tipo di record</td> 
      <td><p>(Facoltativo) Seleziona fino a 7 campi di ricerca dal tipo di record connesso da visualizzare nel modulo personalizzato. Il campo principale è selezionato per impostazione predefinita e non può essere modificato. </p> <p> I campi dei record collegati selezionati vengono visualizzati in una vista tabella sul modulo personalizzato. Quando il modulo viene associato a un oggetto Workfront, la vista tabella è di sola lettura. </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
     <tr>
      <td>Attivo</td>
      <td><p>Questa opzione è disabilitata per impostazione predefinita.<p><p>Quando imposti un campo come Inattivo, questo viene escluso dai rapporti, dai filtri e dalle viste e non è più disponibile nella libreria dei campi dei moduli personalizzati.</p></td>
     </tr>
      </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere eventuali altri campi.

   Oppure

   Per copiare un campo, passa il puntatore su un campo e fai clic sull’icona Copia.

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passa a un’altra sezione per continuare a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

   Ora puoi allegare il modulo a un oggetto connesso da Pianificazione di Workfront ed eseguire una delle operazioni seguenti:

   * Visualizzare i tipi di record in Pianificazione di Workfront connessi all’oggetto Workfront, se presenti.
   * Collegare o scollegare i record dall’oggetto Workfront.

   Per ulteriori informazioni, consulta [Gestire i collegamenti dei record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

### Aggiungere estensioni interfaccia utente

Un’app può essere incorporata in un modulo personalizzato Workfront utilizzando il tipo di campo Estensioni interfaccia utente. Per creare le estensioni interfaccia utente, devi disporre dell’accesso a Adobe App Builder in Adobe Developer Console. Per informazioni, consulta [Incorporare un’app utilizzando un modulo personalizzato Workfront](/help/quicksilver/app-builder/app-builder.md#embed-an-app-using-a-workfront-custom-form) nell’articolo [Creare applicazioni personalizzate per Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Organizzare e visualizzare in anteprima un modulo con il designer dei moduli

Per informazioni su come organizzare un modulo personalizzato con interruzioni di sezione e visualizzare un’anteprima del modulo, consulta [Organizzare e visualizzare in anteprima un modulo con il designer dei moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
