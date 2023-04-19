---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Aggiunta di un campo personalizzato a un modulo personalizzato con il modulo precedente
description: Quando si lavora su un modulo personalizzato, è possibile creare un nuovo campo personalizzato e aggiungerlo a un modulo personalizzato. È inoltre possibile aggiungere un campo personalizzato già aggiunto a un altro modulo personalizzato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: f9fce2715cad3e2ea2bf16de5f4ba457f981725c
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 3%

---

# Aggiunta di un campo personalizzato a un modulo personalizzato con il modulo precedente

Quando si lavora su un modulo personalizzato, è possibile creare un nuovo campo personalizzato e aggiungerlo a un modulo personalizzato.

È inoltre possibile aggiungere un campo personalizzato già aggiunto a un altro modulo personalizzato. Per istruzioni, consulta [Riutilizzare un campo o un widget personalizzato in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Per informazioni sull’aggiunta di un widget risorse a un modulo personalizzato, che è un processo simile all’aggiunta di un campo personalizzato, consulta [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>In un modulo personalizzato contenente molti campi personalizzati o numerose opzioni di selezione multipla in campi personalizzati, le prestazioni potrebbero essere più lente quando si aggiungono o si modificano valori in tali campi. Ad esempio, un modulo contenente 100 campi personalizzati, o campi personalizzati con più di 200 opzioni, potrebbe risultare più lento quando gli utenti interagiscono con esso.

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
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Aggiungere un campo personalizzato a un modulo personalizzato

1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Apri **Aggiungi un campo** scheda .

   ![](assets/add-a-field.jpg)

1. Con **Nuovo campo** ![](assets/new-field.jpg) seleziona uno dei tipi di campo elencati di seguito:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Campo di testo con una riga</td> 
      <td>Consente agli utenti di digitare una singola riga di testo nel campo .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo di testo paragrafo</td> 
      <td>Consente agli utenti di digitare più righe di testo nel campo.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Campo di testo con formattazione</td> 
      <td>Consente agli utenti di digitare più righe di testo nel campo e formattarlo con grassetto, corsivo, sottolineato, punti elenco, numerazione, collegamenti ipertestuali e virgolette di blocco. È disponibile in Home, nell’area Aggiornamenti, negli elenchi e nell’area Dettagli per gli oggetti Workfront. Un limite di caratteri di 15.000 consente l'uso di testo e formattazione numerosi.</p> <p>Per informazioni sull’accesso a questo campo tramite l’API, vedi <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Archiviazione di campi RTF nell’API</a>.</p> <p><b>NOTA</b>: I campi di testo con formattazione non sono disponibili per le app mobili Workfront (disponibili nelle prossime versioni). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">A discesa</td> 
      <td>Fornisce un elenco di scelte a discesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatico </td> 
      <td>Consente agli utenti di digitare il nome di un oggetto esistente in Workfront. Quando l’utente inizia a digitare, viene visualizzato un elenco di suggerimenti.
      Questo tipo di campo supporta i seguenti oggetti:
      <ul><li>Utente</li>
      <li>Gruppo</li>
      <li>Ruolo</li>
      <li>Portfolio</li>
      <li>Programma</li>
      <li>Progetto</li>
      <li>Team</li>
      <li>Modello</li>
      <li>Azienda</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calcolato</td> 
      <td>Consente di definire un’espressione e visualizzare il risultato sul modulo personalizzato. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Aggiungere dati calcolati a un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data</td> 
      <td>Visualizza un calendario in cui gli utenti possono selezionare una data e un’ora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Checkboxe</td> 
      <td>Consente agli utenti di selezionare più scelte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bottoni Circolari</td> 
      <td>Richiede agli utenti di selezionare una sola scelta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testo descrittivo</td> 
      <td>Consente di includere istruzioni e collegamenti a pagine esterne a Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interruzione di sezione</td> 
      <td>Un'interruzione di sezione in realtà non è un campo. È possibile utilizzare un’interruzione di sezione per organizzare campi e widget personalizzati in sezioni e, se necessario, configurare diverse autorizzazioni di visualizzazione e modifica per ogni sezione. Per informazioni sull’aggiunta e la configurazione delle interruzioni di sezione, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Aggiungere un’interruzione di sezione a un modulo personalizzato</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Sulla **Impostazioni campo** configura le opzioni disponibili per il tipo di campo personalizzato che si sta aggiungendo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Immetti un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: Evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
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
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comandi contenente le informazioni digitate qui.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Seleziona il tipo di dati da acquisire nel campo personalizzato. È possibile modificare la selezione del formato dopo aver salvato il modulo, ma il nuovo formato deve supportare il valore immesso.</p>

   <p><strong>Esempio:</strong> Se si salva un valore numerico per un campo con formato testo su almeno un oggetto e successivamente si modifica il formato in Numero o Valuta, non si verificherà un errore. </p>
      <p>Tuttavia, se si salva un valore alfanumerico in un campo con formato Testo su almeno un oggetto e si tenta di modificare il formato in Numero o Valuta, si verificherà un errore perché il valore alfanumerico salvato non è compatibile con i formati Numero o Valuta. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Disposizione</td> 
      <td>(Solo menu a discesa, caselle di controllo e pulsanti di scelta) Consente di cambiare il tipo di selezione di opzioni desiderato per il campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Solo campi di testo) Selezionare una larghezza per il campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza ora del giorno</td> 
      <td>(Solo campi data) Selezionare questa opzione se si desidera visualizzare l’ora del giorno insieme alla data nel campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto di riferimento</td> 
      <td> <p>(Solo per i campi di tipo precedente) Selezionare il tipo di oggetto che si desidera associare al campo.</p> <p>Dopo aver fatto clic su Applica o su Salva+Chiudi, non è possibile modificare il tipo di oggetto del campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se l’amministratore di Workfront ha personalizzato il nome per Portfoli, programmi o progetti nell’interfaccia utente di Workfront, il nome Workfront predefinito per l’oggetto viene visualizzato in questo elenco a discesa, non nel nome personalizzato. Per assistenza, rivolgiti al tuo amministratore Workfront.<br></li> 
         <li>I seguenti tipi di oggetti sono supportati nelle app mobili iOS e Android Workfront: Utente, azienda, gruppo, ruolo del lavoro, Portfolio, programma, progetto e modello.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aggiungi filtro</td> 
      <td> <p>(Solo per i campi di tipo precedente) Aggiungi un filtro per un tipo di oggetto per limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul> 
        <li>Appartengono a uno o più gruppi specificati</li> 
        <li>Sono associati a un ruolo o a un titolo di lavoro specificato</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo</li> 
       </ul> <p>È necessario definire il filtro per il tipo di oggetto selezionato utilizzando la sintassi Modalità testo. Per informazioni sulla creazione di un filtro utilizzando la modalità di testo, consulta la sezione . <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">Modificare la modalità testo in un filtro</a> nell'articolo <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Panoramica della modalità testo</a>. </p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se si sta modificando un modulo personalizzato esistente, l’aggiunta di un filtro a un campo di tipo precedente non rimuove gli oggetti (al di fuori dell’ambito del filtro) che gli utenti hanno già aggiunto utilizzando il campo.</li> 
         <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo Typeahead, il campo verrà visualizzato sui dispositivi mobili degli utenti non interessati dal filtro.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testo descrittivo</td> 
      <td>(Solo per campi di testo descrittivo) Digitare il testo da visualizzare per fornire istruzioni o un collegamento al modulo personalizzato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Collegamento ipertestuale</td> 
      <td>(Solo campi di testo descrittivo) Se si desidera applicare un collegamento ipertestuale al testo descrittivo digitato, aggiungerlo qui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td> 
      <td>Selezionare questa opzione se si desidera che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Traccia le modifiche dei campi nei feed di aggiornamento</td> 
      <td><p>Fare clic sull’elenco a discesa, quindi selezionare i tipi di oggetto in cui si desidera tenere traccia automaticamente delle modifiche al valore del campo.</p> 
      <p><b>NOTA</b>: Questa opzione non è disponibile per i seguenti elementi:</p> 
      <ul> 
      <li>Moduli personalizzati associati ai seguenti tipi di oggetti: Spese, Società, Iterazione, Record fatturazione e Gruppo.</li> 
      <li>I seguenti tipi di campi: Calcolato , Testo descrittivo e Interruzione sezione</li> 
      </ul>
      <p><b>IMPORTANTE</b>: La selezione o la deselezione di un tipo di oggetto in questo campo ha effetto su tutti i moduli personalizzati associati al tipo di oggetto selezionato e contenenti tale campo. Ad esempio, se si deseleziona qui un tipo di oggetto e si salva il modulo personalizzato, le modifiche al valore del campo non saranno più tracciate per quel tipo di oggetto in alcun modulo personalizzato contenente il campo.</p>
       <p>Dopo aver selezionato qui un tipo di oggetto per un campo e aver salvato il modulo personalizzato, il campo viene visualizzato nella scheda Campi personalizzati dell’area Aggiorna feed in Configurazione.</p> 
       <p>Viceversa, se questo campo viene eliminato nell’area Feed aggiornamento in Configurazione, il tipo di oggetto per questa impostazione viene deselezionato in tutti i moduli personalizzati associati al tipo di oggetto e che contengono questo campo.</p> 
       <p>Per ulteriori informazioni, consulta la sezione . <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Aggiungi i campi da tracciare in Workfront</a> nell'articolo <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">Configurare gli aggiornamenti di sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td> 
      <td>Specificare i campi da visualizzare nel modulo in base alle selezioni effettuate dagli utenti nei campi esistenti. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scelte </td> 
      <td> <p>(Solo menu a discesa, caselle di controllo o pulsanti di scelta; opzionale)</p> 
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
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Per modificare il tipo di visualizzazione di un campo nel modulo personalizzato, fare clic sul pulsante **Tipo di visualizzazione** dal menu a discesa, quindi fare clic sul tipo desiderato.

   È possibile scegliere tra i seguenti tipi di visualizzazione dei campi:

   * **Campi di tipo selezione**: Caselle Di Controllo, Menu A Discesa, Pulsanti Di Scelta.
   * **Campi di testo**: Campo Di Testo A Riga Singola, Campo Di Testo Paragrafo. (Non è possibile impostare un campo di testo con formattazione su un tipo di visualizzazione diverso. Tuttavia, è possibile rimuoverlo e aggiungere un altro tipo di campo.)

   Ad esempio, se è stato creato un campo Caselle di selezione, è possibile modificarlo in un campo a discesa o in un campo Pulsanti di scelta. In alternativa, se è stato creato un campo di testo a riga singola, è possibile modificarlo in un campo Testo paragrafo.

   >[!NOTE]
   >
   >Quando si desidera modificare il tipo di visualizzazione di un campo da un campo casella di controllo o da un campo a discesa con selezione multipla (un menu a discesa che consente di selezionare più di un’opzione) a un tipo di campo con selezione singola, tenere presente quanto segue:
   >
   >* Se si passa a Pulsanti di scelta, Workfront conserva tutti i valori di selezione multipla che un utente può aver immesso nel campo finché l’utente non cambia e salva i dati in qualsiasi parte del modulo. A questo punto, tutti i valori selezionati utilizzando il campo di tipo a selezione multipla vengono sostituiti dal valore Pulsante di scelta selezionato.
   >* Se si passa a un menu a discesa a selezione singola, Workfront mantiene tutti i valori di selezione multipla che un utente può aver immesso nel campo finché l’utente non cambia e salva i valori nel campo. A questo punto, tutti i valori selezionati utilizzando il campo di tipo a selezione multipla vengono sostituiti dal valore a discesa selezionato.


1. (Facoltativo) Ripeti i passaggi 2-6 per aggiungere altri campi personalizzati.

   Oppure

   Aggiungi campi già creati per la tua organizzazione, come spiegato in [Riutilizzare un campo o un widget personalizzato in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, è possibile che si verifichi un peggioramento delle prestazioni in presenza di più di 100 moduli, a seconda della complessità del modulo. Esempi di moduli complessi includono moduli con parametri a cascata, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Fai clic su **Applica**.
1. Per continuare a creare il modulo personalizzato in altri modi, procedere con uno dei seguenti articoli:

   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e compilazione di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
