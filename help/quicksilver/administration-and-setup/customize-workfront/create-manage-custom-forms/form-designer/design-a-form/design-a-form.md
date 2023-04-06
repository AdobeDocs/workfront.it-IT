---
title: Progettazione di un modulo con la struttura del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato con la struttura del modulo.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '3803'
ht-degree: 4%

---


# Progettazione di un modulo con la struttura del modulo

È possibile progettare un modulo personalizzato con la struttura del modulo. È possibile allegare moduli personalizzati a diversi oggetti Workfront per acquisire i dati relativi a tali oggetti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
   <p>Piano attuale: Standard</p>
   <p>oppure</p>
   <p>Piano legacy: Pianificare</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Iniziare a progettare un modulo personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Fai clic su **Nuovo modulo personalizzato.**
1. Selezionare i tipi di oggetto a cui si desidera associare il modulo personalizzato, quindi fare clic su **Continua**.

   ![](assets/choose-object-type.jpg)

1. In **Titolo obbligatorio** area, digitare il titolo del modulo personalizzato.
1. (Facoltativo) Per aggiungere altri tipi di oggetto al modulo in modo che possa essere allegato a più oggetti, fare clic sul pulsante **Aggiungi** icona ![](assets/add-objects-icon.png) dopo **Tipi di oggetti**, quindi seleziona il tipo desiderato nel menu visualizzato. È possibile ripetere questa operazione per aggiungere tutti i tipi di oggetto desiderati.

   È inoltre possibile fare clic sulla X di un tipo di oggetto per eliminarla dal modulo.

   >[!CAUTION]
   >
   >L’eliminazione di un modulo personalizzato comporta anche l’eliminazione di tutti i dati personalizzati presenti negli oggetti associati al modulo. Impossibile recuperare i dati eliminati. È consigliabile disattivare un modulo personalizzato, se si disattiva un modulo personalizzato non più utilizzato, conservare tutti i dati storici associati.
   >
   >Per ulteriori informazioni, consulta [Eliminare i tipi di oggetto in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. È quindi possibile iniziare ad aggiungere campi al modulo personalizzato. Consulta le sezioni seguenti:
   * [Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Aggiungi campi di testo](#add-text-fields)
   * [Aggiungi campi calcolati](#add-calculated-fields)
   * [Aggiungere pulsanti di scelta, gruppi di caselle di controllo e menu a discesa](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Aggiungere campi tipo di data e data](#add-typeahead-and-date-fields)
   * [Aggiungere immagini, PDF e video](#add-images-pdfs-and-videos)
   * [Aggiungere file Adobe XD](#add-adobe-xd-files)

## Aggiungere campi nuovi o esistenti al modulo personalizzato

Durante la progettazione del modulo personalizzato è possibile utilizzare campi nuovi o esistenti.

## Riutilizzare un campo o un widget esistente già utilizzato in un altro modulo personalizzato

1. In alto a sinistra nella schermata, fai clic su **Libreria campi**.

1. Trascina il campo o il widget nel modulo personalizzato desiderato.
1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, è possibile che si verifichi un peggioramento delle prestazioni in presenza di più di 100 moduli, a seconda della complessità del modulo.
   >
   >
   >Esempi di moduli complessi includono moduli con parametri a cascata, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

### Aggiungi campi di testo

È possibile aggiungere diversi campi di testo a un modulo personalizzato.

+++ **Espandi per visualizzare le descrizioni dei campi di testo disponibili**

* **Campo di testo a riga singola**: Consente agli utenti di digitare una singola riga di testo nel campo .
* **Campo testo paragrafo**: Consente agli utenti di digitare più righe di testo nel campo.
* **Campo di testo con formattazione**: Consente agli utenti di digitare più righe di testo nel campo e formattarlo con grassetto, corsivo, sottolineato, punti elenco, numerazione, collegamenti ipertestuali e virgolette di blocco. Un limite di caratteri di 15.000 consente l&#39;uso di testo e formattazione numerosi.

   Per informazioni sull’accesso a questo campo tramite l’API, consulta Archiviazione di campi RTF nell’API.

   >[!NOTE]
   >
   >I campi di testo con formattazione non sono disponibili per le app mobili Workfront (disponibili nelle prossime versioni).

* **Testo descrittivo**: Consente di includere istruzioni e collegamenti a pagine esterne a Workfront.

+++

Per aggiungere un campo di testo:

1. Sul lato sinistro dello schermo, trova uno dei seguenti campi di testo e trascinalo in una sezione dell’area di lavoro:

   * Testo a riga singola:
   * Testo paragrafo
   * Campo di testo con formattazione
   * Testo descrittivo

   ![](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che si sta aggiungendo:

   <table>
    <tr>
    <td>Ingresso in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr>
    <td>Dimensione</td>
    <td><p>Modificare le dimensioni dei campi di testo nel modulo.<p>
   </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    <li>Testo con formattazione</li>
    <li>Testo descrittivo - Disponibile a breve</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etichetta</td>
    <td><p>Digita un’etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.<p>
    <p>IMPORTANTE: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p></td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    <li>Testo con formattazione</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nome</td>
    <td><p>(Obbligatorio) Questo nome indica in che modo il sistema identifica il campo. Quando si configura il widget per la prima volta e si digita l’etichetta, il campo Nome viene compilato automaticamente in modo da corrispondere a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati, in quanto consentono di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p>
    <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti avete iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato in cui ora potrebbe essere fatto riferimento in altre aree di Workfront. <p>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e smette di funzionare correttamente, a meno che non lo aggiungi nuovamente al rapporto con il nuovo nome.</p> </li>
      <li> <p>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.</p> </li>
      <li><p>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori durante l’utilizzo del campo in aree diverse di Workfront.</p></li>
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    <li>Testo con formattazione</li>
    <li>Testo descrittivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Istruzioni</td>
    <td>Inserisci eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    <li>Testo con formattazione</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formato</td>
    <td><p>Seleziona il tipo di dati da acquisire nel campo personalizzato.</p> <p><b>NOTA</b>:   
    <ul> 
    <li>Impossibile modificare il campo dopo il salvataggio del modulo. Se si desidera utilizzare il campo in calcoli matematici, assicurarsi di selezionare un formato Numero o Valuta.<br></li> 
    <li>Quando si seleziona Numero o Valuta, i numeri che iniziano con 0 vengono troncati automaticamente dal sistema.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Tipo di Disposizione</td>
    <td>Passa dai campi di testo a riga singola a quelli a paragrafo singolo.</td>
    <td><ul>
    <li>Testo su riga singola</li>
    <li>Testo paragrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Collegamento ipertestuale</td>
    <td> Se si desidera applicare un collegamento ipertestuale al testo descrittivo digitato, aggiungerlo qui. Il testo descrittivo viene visualizzato come un collegamento sugli oggetti a cui è allegato il modulo.</td>
    <td><ul><li>Testo descrittivo</li></ul></td>
    </tr>
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, passa il puntatore del mouse su un campo e fai clic sull’icona Copia .

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

### Aggiungi campi calcolati

In un modulo personalizzato è possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato è associato a un oggetto.

Per aggiungere un campo calcolato, vedi [Aggiunta di campi calcolati con la finestra di progettazione del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Aggiungere pulsanti di scelta, caselle di controllo e menu a discesa

È possibile aggiungere pulsanti di scelta, caselle di controllo e elenchi a discesa a un modulo personalizzato.

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Pulsanti di scelta**: Richiede agli utenti di selezionare una sola scelta.
* **Gruppo di caselle di selezione**: Consente agli utenti di selezionare più scelte.
* **Elenco a discesa**: Fornisce un elenco di scelte a discesa.

+++

Per aggiungere pulsanti di scelta e caselle di controllo:

1. Sul lato sinistro dello schermo, trova uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Pulsanti di opzione
   * Gruppo di caselle di controllo
   * A discesa

   ![](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che si sta aggiungendo:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Ingresso in</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
    <tr> 
     <td role="rowheader">Etichetta</td> 
     <td> <p>(Obbligatorio) Immetti un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nome</td> 
     <td> <p>(Obbligatorio) Questo nome indica in che modo il sistema identifica il campo personalizzato quando lo si aggiunge a varie aree in Workfront, come report, home e interazioni API.</p> <p>Quando si configura il campo personalizzato per la prima volta e si digita l’etichetta, il campo Nome viene compilato automaticamente in modo da corrispondere a tale campo. Tuttavia, i campi Etichetta e Nome non sono sincronizzati, in quanto consentono di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p> 
    <p><b>IMPORTANTE</b>:   
     <ul> 
    <li>Anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti avete iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato in cui ora potrebbe essere fatto riferimento in altre aree di Workfront. <p>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e smette di funzionare correttamente, a meno che non lo aggiungi nuovamente al rapporto con il nuovo nome.</p> </li>
    <li> <p>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.</p> </li>
     <li><p>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori durante l’utilizzo del campo in aree diverse di Workfront.</p></li>
     </ul> <p>Ogni nome di campo personalizzato deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo è possibile riutilizzare uno già creato per un altro modulo personalizzato. Per ulteriori informazioni, consulta <a href="#Add" class="MCXref xref">Aggiungere un campo personalizzato a un modulo personalizzato</a> in questo articolo.</p> </td>
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Istruzioni</td> 
    <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formato</td> 
    <td> <p>Seleziona il tipo di dati da acquisire nel campo personalizzato.</p> <p><b>NOTA</b>:   
     <ul> 
    <li>Impossibile modificare il campo dopo il salvataggio del modulo. Se si desidera utilizzare il campo in calcoli matematici, assicurarsi di selezionare un formato Numero o Valuta.<br></li> 
    <li>Quando si seleziona Numero o Valuta, i numeri che iniziano con 0 vengono troncati automaticamente dal sistema.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Tipo di Disposizione</td> 
    <td>Passa da pulsanti di scelta, gruppi di caselle di controllo o menu a discesa del campo.</td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Rendi il campo obbligatorio</td> 
    <td>Selezionare questa opzione se si desidera che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Scelte </td> 
    <td> 
    <ol> 
    <li> <p>Fai clic su <b>Opzioni</b>, quindi attiva una delle seguenti opzioni:</p> 
    <ul> 
    <li><strong>Mostra valori</strong>: Mostra i valori di ogni scelta nel campo . L’etichetta di ogni scelta viene visualizzata per impostazione predefinita.</li> 
     <li><strong>Opzioni di ordinamento A-Z</strong>: Ordina le opzioni aggiunte in ordine alfabetico nel campo.</li> 
    </ul> 
    </li> 
    <li> <p>Per ogni scelta aggiunta per l’utente, fai clic sull’icona a forma di ingranaggio <img src="assets/gear-icon-settings.png">, quindi seleziona una delle seguenti opzioni:</p> 
    <ul> 
    <li><strong>Seleziona per impostazione predefinita</strong>: Seleziona l’opzione per impostazione predefinita nel campo .</li> 
    <li> <p><strong>Nascondi scelta</strong>: Nasconde la scelta nel campo . Le scelte nascoste rimangono accessibili nei rapporti.</p> </li> 
    <li> <p><strong>Rimuovi scelta</strong>: Rimuovi la scelta dal campo.</p> <p><b>AVVISO</b>: Se si utilizzano oggetti correnti con questa opzione, non rimuoverli dal campo. La sua rimozione provocherà la perdita di dati storici. Invece, seleziona l’opzione per nasconderlo, impedendo agli utenti di selezionarlo in futuro.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Pulsanti di opzione</li>
    <li>Gruppo di caselle di controllo</li>
    <li>A discesa</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, passa il puntatore del mouse su un campo e fai clic sull’icona Copia .

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere campi tipo di data e data

È possibile aggiungere campi tipo di data e data a un modulo personalizzato.

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Tipo**: Consente agli utenti di digitare il nome di un oggetto esistente in Workfront. Quando l’utente inizia a digitare, viene visualizzato un elenco di suggerimenti. Questo tipo di campo supporta i seguenti oggetti:
   * Utente
   * Gruppo
   * Ruolo
   * Portfolio
   * Programma
   * Progetto
   * Team
   * Modello
   * Azienda
* **Campo data**: Visualizza un calendario in cui gli utenti possono selezionare una data e un’ora.

+++

Per aggiungere campi data tipo precedente:

1. Sul lato sinistro dello schermo, trova uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Automatico
   * Campo Data

   ![](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che si sta aggiungendo:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Impostazione campo</td>
    <td>Descrizione</td>
    <td>Disponibile per </td>
    </tr>
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Immetti un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
       <td><ul>
    <li>Automatico</li>
    <li>Campo Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica in che modo il sistema identifica il campo personalizzato quando lo si aggiunge a varie aree in Workfront, come report, home e interazioni API.</p> <p>Quando si configura il campo personalizzato per la prima volta e si digita l’etichetta, il campo Nome viene compilato automaticamente in modo da corrispondere a tale campo. Tuttavia, i campi Etichetta e Nome non sono sincronizzati, in quanto consentono di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti avete iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato in cui ora potrebbe essere fatto riferimento in altre aree di Workfront. <p>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e smette di funzionare correttamente, a meno che non lo aggiungi nuovamente al rapporto con il nuovo nome.</p> </li>
      <li> <p>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.</p> </li>
      <li><p>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori durante l’utilizzo del campo in aree diverse di Workfront.</p></li>
      </ul> <p>Ogni nome di campo personalizzato deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo è possibile riutilizzare uno già creato per un altro modulo personalizzato. Per ulteriori informazioni, consulta <a href="#Add" class="MCXref xref">Aggiungere un campo personalizzato a un modulo personalizzato</a> in questo articolo.</p> </td>
         <td><ul>
    <li>Automatico</li>
    <li>Campo Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Automatico</li>
    <li>Campo Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza ora del giorno</td> 
      <td>Seleziona questa opzione se desideri visualizzare l’ora del giorno insieme alla data nel campo .</td> 
         <td><ul>
    <li>Campo Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto di riferimento</td> 
      <td> <p>Selezionare il tipo di oggetto che si desidera associare al campo.</p> <p>Dopo aver fatto clic su Applica o su Salva+Chiudi, non è possibile modificare il tipo di oggetto del campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se l’amministratore di Workfront ha personalizzato il nome per Portfoli, programmi o progetti nell’interfaccia utente di Workfront, il nome Workfront predefinito per l’oggetto viene visualizzato in questo elenco a discesa, non nel nome personalizzato. Per assistenza, rivolgiti al tuo amministratore Workfront.<br></li> 
         <li>I seguenti tipi di oggetti sono supportati nelle app mobili iOS e Android Workfront: Utente, azienda, gruppo, ruolo del lavoro, Portfolio, programma, progetto e modello.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Automatico</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td> 
      <td>Selezionare questa opzione se si desidera che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
       <td><ul>
    <li>Automatico</li>
    <li>Campo Data</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, passa il puntatore del mouse su un campo e fai clic sull’icona Copia .

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere immagini, PDF e video

È possibile aggiungere immagini, PDF e video a un modulo personalizzato. Gli utenti che lavorano con l’oggetto a cui è allegato il modulo personalizzato possono visualizzare l’immagine, PDF o il video solo nelle aree seguenti:

* Area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica per l’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, le caselle Modifica progetto e Modifica attività)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Espandi per visualizzare le descrizioni dei campi disponibili**

* **Immagine**: Consente agli utenti di aggiungere file di immagine ______.
* **PDF**: Consente agli utenti di aggiungere PDF
* **Video**: Consente agli utenti di aggiungere file video ____.

+++

Per aggiungere immagini, PDF o video:

1. Sul lato sinistro dello schermo, trova uno dei campi seguenti e trascinalo in una sezione dell’area di lavoro.

   * Immagine
   * PDF
   * Video

   ![](assets/drag-field-to-section.png)

1. Digita o modifica una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Immetti un'etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome è il modo in cui il sistema identifica il widget.</p> <p>Quando si configura il widget per la prima volta e si digita l’etichetta, il campo Nome viene compilato automaticamente in modo da corrispondere a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati, in quanto consentono di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p> <p><b>IMPORTANTE</b>: Anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti iniziate a utilizzare il modulo personalizzato in widget. In questo caso, il sistema non riconoscerà più il widget dove potrebbe ora essere referenziato in altre aree di Workfront. </p> <p>Ogni nome di widget deve essere univoco nell'istanza Workfront della tua organizzazione. In questo modo è possibile riutilizzare uno già creato per un altro modulo personalizzato. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digita o incolla l'URL del widget in cui è memorizzato su Internet.</p> 
      <p>Se stai aggiungendo un widget video, al momento puoi farlo aggiungendo quanto segue nella casella URL:</p> 
      <ul> 
      <li> <p>Collegamento YouTube o Vimeo</p> </li> 
      <li> <p>Collegamento video a Google Drive</p> </li> 
      <li> <p>Collegamento a video con estensione MP4 e MOV</p> </li> 
      <li> <p>Collega a video già caricato nell’area Documenti nella tua istanza Workfront. Per istruzioni, consulta <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Aggiungere un widget video a un modulo personalizzato dall’area Documenti</a> in questo articolo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>Modifica le dimensioni di visualizzazione del widget in base alle esigenze.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, passa il puntatore del mouse su un campo e fai clic sull’icona Copia .

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

#### **Aggiungere un widget video a un modulo personalizzato dall’area Documenti**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Quando si aggiunge un video a un modulo personalizzato in questo modo, solo le autorizzazioni impostate per il modulo personalizzato vengono applicate al video quando gli utenti accedono al modulo su un oggetto e non alle autorizzazioni impostate per il video nell’area Documenti.

1. Passa al video nell’area Documenti e genera una bozza per esso, come descritto in [Creare una bozza interattiva per un sito web o altro contenuto web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Apri la bozza.
1. Fai clic con il pulsante destro del mouse in un punto qualsiasi del video, quindi seleziona **Copia indirizzo video**.
1. Nel modulo personalizzato in cui si sta aggiungendo il widget video, incolla l’indirizzo copiato nel **URL** scatola.
1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

### Aggiungere file Adobe XD

È possibile aggiungere un prototipo Adobe XD direttamente a un modulo personalizzato. Gli utenti che utilizzano l’oggetto a cui è allegato il modulo personalizzato possono visualizzare il file Adobe XD solo nelle aree seguenti:

* Area Dettagli dell’oggetto (ad esempio, per un progetto, l’area Dettagli progetto)
* La casella Modifica per l’oggetto, se presenta il nuovo aspetto dell’esperienza Adobe Workfront (ad esempio, le caselle Modifica progetto e Modifica attività)

Per aggiungere un file Adobe XD:

1. Sul lato sinistro dello schermo, trova **Adobe XD** e trascinarlo in una sezione dell&#39;area di lavoro.
1. Digita o modifica una delle seguenti proprietà per il widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Immetti un'etichetta descrittiva da visualizzare sopra il widget. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome è il modo in cui il sistema identifica il widget. Quando si configura il widget per la prima volta e si digita l’etichetta, il campo Nome viene compilato automaticamente in modo da corrispondere a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati, in quanto consentono di modificare l’etichetta visualizzata dagli utenti senza dover modificare il nome visualizzato dal sistema.</p>
    <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Anche se è possibile farlo, ti consigliamo di non modificare questo nome dopo che tu o altri utenti avete iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato in cui ora potrebbe essere fatto riferimento in altre aree di Workfront. <p>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e smette di funzionare correttamente, a meno che non lo aggiungi nuovamente al rapporto con il nuovo nome.</p> </li>
      <li> <p>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.</p> </li>
      <li><p>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori durante l’utilizzo del campo in aree diverse di Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obbligatorio) Digitare o incollare un collegamento XD prototipo valido.</p> 
      <p>Nota: L’impostazione Accesso collegamento nella scheda Condividi di Adobe XD deve essere impostata su Chiunque disponga del collegamento. In caso contrario, gli utenti non potranno visualizzare il prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul widget. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Facoltativo) Se necessario, modifica le dimensioni di visualizzazione del widget.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi o widget.

   oppure

   Per copiare un campo, passa il puntatore del mouse su un campo e fai clic sull’icona Copia .

   ![icona copia](assets/copy-field.png)

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

## Organizzazione e visualizzazione in anteprima di un modulo con la struttura del modulo

Per informazioni su come organizzare e visualizzare un’anteprima del modulo, vedere [Organizzazione e visualizzazione in anteprima di un modulo con la struttura del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).