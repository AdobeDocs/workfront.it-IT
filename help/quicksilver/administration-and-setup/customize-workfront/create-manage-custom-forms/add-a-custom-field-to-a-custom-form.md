---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Aggiungere un campo personalizzato a un modulo personalizzato con il generatore di moduli legacy
description: Quando si lavora su un modulo personalizzato, è possibile creare un nuovo campo personalizzato e aggiungerlo a un modulo personalizzato. È inoltre possibile aggiungere un campo personalizzato già aggiunto a un altro modulo personalizzato.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: db362bd73e51b30090708822876ad02f7804d064
workflow-type: tm+mt
source-wordcount: '2313'
ht-degree: 2%

---

# Aggiungere un campo personalizzato a un modulo personalizzato con il generatore di moduli legacy

<!-- Audited: 02/2024 -->

Quando si lavora su un modulo personalizzato, è possibile creare un nuovo campo personalizzato e aggiungerlo a un modulo personalizzato.

È inoltre possibile aggiungere un campo personalizzato già aggiunto a un altro modulo personalizzato. Per istruzioni, consulta [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Per informazioni sull’aggiunta di un widget di risorse a un modulo personalizzato, processo simile all’aggiunta di un campo personalizzato, consulta [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>In un modulo personalizzato contenente molti campi personalizzati o molte opzioni a selezione multipla nei campi personalizzati, gli utenti potrebbero notare un rallentamento delle prestazioni quando aggiungono o modificano valori in tali campi. Ad esempio, un modulo contenente 100 campi personalizzati o più campi personalizzati selezionati con più di 200 opzioni potrebbe risultare più lento quando gli utenti interagiscono con esso.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td>Accesso amministrativo ai moduli personalizzati </td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aggiungere un campo personalizzato a un modulo personalizzato {#add-custom-field-to-custom-form}

1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Seleziona la **Aggiungi un campo** scheda.

   ![Aggiungi una scheda campo](assets/add-a-field.jpg)

1. Con **Nuovo campo** ![Icona Nuovo campo](assets/new-field.jpg) selezionato, selezionare uno dei seguenti tipi di campo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Campo di testo con una riga</td> 
      <td>Consente agli utenti di digitare una singola riga di testo nel campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo di testo paragrafo</td> 
      <td>Consente di digitare più righe di testo nel campo.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Campo di testo con formattazione</td> 
      <td>Consente agli utenti di digitare più righe di testo nel campo e formattare il testo con grassetto, corsivo, sottolineato, punti elenco, numerazione, collegamenti ipertestuali e virgolette. È disponibile in Home, nell’area Aggiornamenti, negli elenchi e nell’area Dettagli per gli oggetti Workfront. Un limite di caratteri di 15.000 consente di inserire testo e formattazione in modo molto ampio.</p> <p>Per informazioni sull’accesso a questo campo tramite l’API, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Archiviazione di campi in formato Rich Text nell’API</a>.</p> <p><b>NOTA</b>: i campi di testo con formattazione non sono disponibili per le app Workfront per dispositivi mobili. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">A discesa</td> 
      <td>Fornisce un elenco di scelte a discesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatico </td> 
      <td>Consente di digitare il nome di un oggetto esistente in Workfront. Quando l’utente inizia a digitare, viene visualizzato un elenco di suggerimenti.
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
      <td>Consente di definire un'espressione e di visualizzare il risultato nel modulo personalizzato. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Aggiungere dati calcolati a un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data</td> 
      <td>Visualizza un calendario in cui gli utenti possono selezionare una data e un'ora.</td> 
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
      <td>Un'interruzione di sezione non è in realtà un campo. È possibile utilizzare un'interruzione di sezione per organizzare i campi personalizzati e i widget in sezioni e, se necessario, configurare diverse autorizzazioni di visualizzazione e modifica per ogni sezione. Per informazioni sull'aggiunta e la configurazione delle interruzioni di sezione, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Aggiungere un’interruzione di sezione a un modulo personalizzato</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >I campi che consentono selezioni multiple, come la casella di controllo e il menu a discesa, sono difficili da tracciare e raggruppare nei rapporti. Per semplificare la creazione di grafici e il raggruppamento nei report, è possibile creare campi separati per ogni scelta, ad esempio un campo di testo a riga singola.

1. Il giorno **Impostazioni campo** , configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td> <p>(Obbligatorio) Digita un’etichetta descrittiva da visualizzare sopra il campo personalizzato. Puoi modificare l’etichetta in qualsiasi momento.</p> <p><b>IMPORTANTE</b>: evita di utilizzare caratteri speciali in questa etichetta. Non vengono visualizzati correttamente nei rapporti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obbligatorio) Questo nome indica il modo in cui il sistema identifica il campo personalizzato quando lo si aggiunge a varie aree in Workfront, ad esempio report, Home e interazioni API.</p> <p>Quando configuri il campo personalizzato per la prima volta e digiti l’etichetta, il campo Nome si popola automaticamente in modo che corrisponda a esso. Tuttavia, i campi Etichetta e Nome non sono sincronizzati. In questo modo è possibile modificare l'etichetta visualizzata dagli utenti senza dover cambiare il nome visualizzato dal sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Sebbene sia possibile farlo, si consiglia di non modificare questo nome dopo che l’utente o altri utenti hanno iniziato a utilizzare il modulo personalizzato in Workfront. In questo caso, il sistema non riconoscerà più il campo personalizzato a cui potrebbe ora fare riferimento in altre aree di Workfront. <p>Ad esempio, se aggiungi il campo personalizzato a un rapporto e successivamente ne modifichi il nome, Workfront non lo riconosce nel rapporto e non funzionerà più correttamente a meno che non lo aggiungi nuovamente al rapporto utilizzando il nuovo nome.</p> </li>
      <li> <p>È consigliabile non digitare un nome già utilizzato per i campi Workfront incorporati.</p> </li>
      <li><p>È consigliabile non utilizzare il carattere punto/punto nel nome del campo personalizzato, per evitare errori quando si utilizza il campo in aree diverse di Workfront.</p></li>
      </ul> <p>Ogni nome di campo personalizzato deve essere univoco nell’istanza Workfront della tua organizzazione. In questo modo, è possibile riutilizzare un modulo già creato per un altro modulo personalizzato. Per ulteriori informazioni, consulta <a href="#add-a-custom-field-to-a-custom-form">Aggiungere un campo personalizzato a un modulo personalizzato</a> in questo articolo.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Istruzioni</td> 
      <td> <p>Inserisci eventuali informazioni aggiuntive sul campo personalizzato. Quando gli utenti compilano il modulo personalizzato, possono passare il cursore sull’icona del punto interrogativo per visualizzare una descrizione comando contenente le informazioni digitate qui.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Seleziona il tipo di dati che verranno acquisiti nel campo personalizzato. È possibile modificare la selezione del formato dopo il salvataggio del modulo, ma il nuovo formato deve supportare il valore immesso.</p>

   <p><strong>Esempio:</strong> Se si salva un valore numerico per un campo con formato Testo in almeno un oggetto e successivamente si modifica il formato in Numerico o Valuta, non si verificherà alcun errore. </p>
      <p>Tuttavia, se si salva un valore alfanumerico in un campo con formato Testo in almeno un oggetto e si tenta di modificare il formato in Numerico o Valuta, si verificherà un errore perché il valore alfanumerico salvato non è compatibile con i formati Numerico o Valuta. </p>

   <p><strong>Nota:</strong> Il limite di caratteri per i campi Numero è 16. È inoltre possibile utilizzare un campo Testo per immettere numeri ed evitare il limite.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Disposizione</td> 
      <td>(Solo a discesa, caselle di controllo e pulsanti di scelta) Consente di cambiare il tipo di selezione delle opzioni desiderata per il campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensione</td> 
      <td>(Solo campi di testo) Selezionare una larghezza per il campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza ora del giorno</td> 
      <td>(Solo campi data) Seleziona questa opzione se desideri visualizzare nel campo l’ora del giorno e la data.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di oggetto di riferimento</td> 
      <td> <p>(Solo campi typeahead) Selezionare il tipo di oggetto da associare al campo.</p> <p>Dopo aver fatto clic su Applica o su Salva+Chiudi, non è possibile modificare il tipo di oggetto per il campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se l'amministratore di Workfront ha personalizzato il nome di Portfoli, programmi o progetti nell'interfaccia utente di Workfront, in questo elenco a discesa viene visualizzato il nome Workfront predefinito per l'oggetto e non il nome personalizzato. Se hai bisogno di assistenza, rivolgiti all’amministratore di Workfront.<br></li> 
         <li>Nelle app mobili iOS e Android Workfront sono supportati i seguenti tipi di oggetti: Utente, Società, Gruppo, Mansione, Portfolio, Programma, Progetto e Modello.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aggiungi filtro</td> 
      <td> <p>(Solo campi di completamento automatico) Aggiungi un filtro per un tipo di oggetto per limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. </p> <p>Ad esempio, puoi limitare un campo in modo che i nomi utente possano essere selezionati solo se soddisfano i seguenti criteri:</p> 
       <ul> 
        <li>Appartengono a uno o più gruppi specificati</li> 
        <li>Sono associati a un ruolo o a una mansione specificata</li> 
        <li>Appartengono allo stesso gruppo della persona che utilizza il campo</li> 
       </ul> <p>È necessario definire il filtro per il tipo di oggetto selezionato utilizzando la sintassi della modalità testo. Per informazioni sulla creazione di un filtro in modalità testo, vedere <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p>
       <p><b>NOTA</b>:   
        <ul> 
         <li>Se si sta modificando un modulo personalizzato esistente, l'aggiunta di un filtro a un campo automatico non rimuove gli oggetti già aggiunti dagli utenti utilizzando il campo al di fuori dell'ambito del filtro.</li> 
         <li>Questo filtro non è disponibile sui dispositivi mobili. Se utilizzi il filtro per un campo Typeahead, il campo verrà visualizzato sui dispositivi mobili degli utenti che non sono interessati dal filtro.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testo descrittivo</td> 
      <td>(Solo campi Testo descrittivo) Digitare il testo da visualizzare per fornire istruzioni o un collegamento nel modulo personalizzato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Collegamento ipertestuale</td> 
      <td>(Solo campi Testo descrittivo) Se si desidera applicare un collegamento ipertestuale al Testo descrittivo digitato, aggiungerlo qui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi il campo obbligatorio</td> 
      <td>Seleziona questa opzione se desideri che il campo sia obbligatorio per consentire all’utente di completare il modulo personalizzato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Traccia le modifiche dei campi nei feed di aggiornamento</td> 
      <td><p>Fai clic sull’elenco a discesa, quindi seleziona i tipi di oggetto in cui desideri tenere traccia automaticamente delle modifiche al valore del campo.</p> 
      <p><b>NOTA</b>: questa opzione non è disponibile per:</p> 
      <ul> 
      <li>Moduli personalizzati associati ai seguenti tipi di oggetti: Spesa, Società, Iterazione, Record fatturazione e Gruppo.</li> 
      <li>I seguenti tipi di campo: Calcolato, Testo descrittivo e Interruzione di sezione</li> 
      </ul>
      <p><b>IMPORTANTE</b>: la selezione o deselezione di un tipo di oggetto influisce su tutti i moduli personalizzati associati al tipo di oggetto selezionato e che contengono questo campo. Ad esempio, se deselezioni un tipo di oggetto e salvi il modulo personalizzato, le modifiche al valore del campo non vengono più tracciate per quel tipo di oggetto in nessun modulo personalizzato che contiene il campo.</p>
       <p>Dopo aver selezionato qui un tipo di oggetto per un campo e aver salvato il modulo personalizzato, il campo viene visualizzato nella scheda Campi personalizzati dell’area Aggiorna feed di Configurazione.</p> 
       <p>Al contrario, se questo campo viene eliminato nell’area Aggiorna feed di Configurazione, il tipo di oggetto per questa impostazione viene deselezionato in tutti i moduli personalizzati associati al tipo di oggetto e che contengono questo campo.</p> 
       <p>Per ulteriori informazioni, consulta la sezione <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Aggiungi i campi di cui vuoi tenere traccia in Workfront</a> nell’articolo <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Configurare gli aggiornamenti di sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td>
      <td>Specificare i campi da visualizzare nel modulo in base alle selezioni effettuate dagli utenti nei campi esistenti. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scelte </td> 
      <td> <p>(solo pulsanti a discesa, caselle di controllo o pulsanti di scelta; facoltativo)</p> 
       <ol> 
        <li> <p>Clic <b>Opzioni</b>, quindi attiva uno dei seguenti elementi:</p> 
           <ul> 
            <li><strong>Mostra valori</strong>: mostra i valori di ciascuna scelta nel campo. L’etichetta di ciascuna scelta viene visualizzata per impostazione predefinita.</li> 
            <li><strong>Ordina le scelte dalla A alla Z</strong>: Ordina le scelte aggiunte in ordine alfabetico nel campo.</li> 
           </ul> 
        </li> 
        <li> <p>Per ogni scelta aggiunta per l’utente, fai clic sull’icona a forma di ingranaggio <img src="assets/gear-icon-settings.png">, quindi seleziona una delle seguenti opzioni:</p> 
           <ul> 
            <li><strong>Seleziona per impostazione predefinita</strong>: seleziona la scelta per impostazione predefinita nel campo.</li> 
            <li> <p><strong>Nascondi scelta</strong>: nasconde la scelta nel campo. Le scelte nascoste rimangono accessibili nei rapporti.</p> </li> 
            <li> <p><strong>Rimuovi scelta</strong>: rimuovi la scelta dal campo.</p> <p><b>AVVISO</b>: se gli oggetti correnti utilizzano questa scelta, non rimuoverla dal campo. Rimuovendola, i dati storici andranno perduti. Al contrario, seleziona l’opzione per nasconderlo, impedendo agli utenti di selezionarlo in futuro.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Per modificare il tipo di visualizzazione di un campo nel modulo personalizzato, fai clic sul pulsante **Tipo di visualizzazione** quindi fare clic sul tipo desiderato.

   Puoi passare dai seguenti tipi di visualizzazione dei campi:

   * **Campi di tipo selezione**: Caselle Di Controllo, Elenco A Discesa, Pulsanti Di Scelta.
   * **Campi di testo**: Campo Testo A Riga Singola, Campo Testo Paragrafo. Non è possibile impostare un tipo di visualizzazione diverso per un campo di testo con formattazione. È tuttavia possibile rimuoverlo e aggiungere un altro tipo di campo.)

   Se ad esempio è stato creato un campo Caselle di controllo, è possibile modificarlo in un campo a discesa o in un campo Pulsanti di scelta. In alternativa, se è stato creato un campo di testo a riga singola, è possibile modificarlo in un campo di testo paragrafo.

   >[!NOTE]
   >
   >Quando si desidera modificare il tipo di visualizzazione di un campo da un campo casella di controllo o da un campo a discesa a selezione multipla (un elenco a discesa che consente di selezionare più opzioni) a un tipo di campo a selezione singola, tenere presente quanto segue:
   >
   >* Se si passa a Pulsanti di opzione, Workfront mantiene i valori a selezione multipla eventualmente immessi nel campo fino a quando l&#39;utente non cambia e salva i dati in qualsiasi parte del modulo. A questo punto, tutti i valori selezionati utilizzando il campo di tipo a selezione multipla vengono sostituiti dal valore del pulsante di opzione selezionato.
   >* Se passi a un elenco a discesa a selezione singola, Workfront mantiene eventuali valori a selezione multipla immessi da un utente nel campo fino a quando l’utente non cambia e salva i valori nel campo. A questo punto, tutti i valori selezionati utilizzando il campo a selezione multipla vengono sostituiti dal valore a discesa selezionato.

1. (Facoltativo) Ripeti i passaggi 3-5 per aggiungere altri campi personalizzati.

   Oppure

   Aggiungi campi già creati per la tua organizzazione, come spiegato in [Riutilizzare un campo personalizzato o un widget in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, il calo delle prestazioni può verificarsi quando in un modulo esistono più di 100 moduli, a seconda della complessità. Esempi di moduli complessi includono moduli con parametri a catena, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Clic **Applica**.
1. Se si desidera continuare a creare il modulo personalizzato in altri modi, passare a uno dei seguenti articoli:

   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Aggiungere un’interruzione di sezione a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
