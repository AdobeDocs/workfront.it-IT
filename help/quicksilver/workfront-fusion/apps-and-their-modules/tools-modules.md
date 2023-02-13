---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Strumenti
description: La [!DNL Adobe Workfront Fusion Tools] La sezione include diversi moduli utili che possono migliorare il tuo scenario.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# [!UICONTROL Strumenti]

La [!DNL Adobe Workfront Fusion Tools] La sezione include diversi moduli utili che possono migliorare il tuo scenario.

[!UICONTROL Strumenti] i moduli sono disponibili dall’elenco delle app o dal [!UICONTROL Strumenti] icona ![](assets/tools-icon-small.png) nella parte inferiore dello schermo.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Strumenti] e i relativi campi

* [Triggers](#triggers)
* [Azioni](#actions)
* [Aggregatori](#aggregators)
* [Trasformatori](#transformers)

### Triggers

#### [!UICONTROL Trigger di base]

Questo modulo ti consente di creare un trigger personalizzato e definirne i bundle di input.

È possibile utilizzare questo modulo, ad esempio, per contatti o qualsiasi altro elenco che è previsto venga inviato a un indirizzo e-mail specifico (ad esempio [!UICONTROL E-mail] >[!UICONTROL Invia un messaggio e-mail]oppure [!DNL Gmail] >[!UICONTROL Invia un messaggio e-mail] moduli) o come semplice promemoria da attivare ogni volta che lo desideri.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Crea bundle personalizzati aggiungendo elementi array. La matrice è costituita dalle coppie nome-valore.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Ottieni variabili multiple]](#get-multiple-variables)
* [[!UICONTROL Get Variable]](#get-variable)
* [[!UICONTROL Funzione di incremento]](#increment-function)
* [[!UICONTROL Imposta variabili multiple]](#set-multiple-variables)
* [[!UICONTROL Imposta variabile]](#set-variable)
* [[!UICONTROL Sonno]](#sleep)

#### [!UICONTROL Ottieni variabili multiple]

Questo modulo recupera i valori creati in precedenza da [!UICONTROL Imposta variabile] o [!UICONTROL Imposta variabili multiple] modulo .

Questo modulo è in grado di leggere le variabili impostate in qualsiasi punto dello scenario, anche se la variabile è stata impostata in un percorso diverso rispetto a dove [!UICONTROL Ottieni variabili multiple] il modulo si trova. L&#39;unico requisito è che la [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] o [!UICONTROL Strumenti] > [!UICONTROL Imposta più variabili] il modulo viene eseguito prima del [!UICONTROL Strumenti] > [!UICONTROL Ottieni variabili multiple] modulo . Per ulteriori informazioni sull’ordine di esecuzione dei moduli, vedi [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Aggiungi le variabili che desideri ottenere dal modulo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>Per ogni variabile aggiunta, mappa il nome della variabile che desideri ottenere.</td>
    </tr>
</table>

>[!INFO]
>
>**Esempi:**  Di seguito sono riportati i possibili utilizzi del [!UICONTROL Imposta]/[!UICONTROL Ottieni (più) variabili] moduli:
>
>* Memorizzare un valore calcolato per un uso successivo, anche in un percorso diverso. Ciò è utile nei casi in cui il valore viene utilizzato in più moduli e la formula per calcolare il valore è eccessivamente complessa.
>* Per eseguire il debug di una formula. Se una formula utilizzata in un modulo sembra non fornire un risultato corretto, copiarla e incollarla in un [!UICONTROL Imposta variabile] modulo inserito prima del modulo pertinente. Scollega i moduli dopo la [!UICONTROL Imposta variabile] ed esegui lo scenario. Verifica la [!UICONTROL Imposta variabile] output del modulo, regolare o semplificare la formula, eseguire nuovamente lo scenario e continuare a farlo fino a quando il problema non è stato risolto.



#### [!UICONTROL Get Variable]

Questo modulo recupera un valore creato in precedenza da [!UICONTROL Imposta variabile] o [!UICONTROL Imposta variabili multiple] modulo .

Questo modulo è in grado di leggere le variabili impostate in qualsiasi punto dello scenario, anche se la variabile è stata impostata in un percorso diverso rispetto a dove [!UICONTROL Get Variable] il modulo si trova. L&#39;unico requisito è che la [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] o [!UICONTROL Strumenti] > [!UICONTROL Imposta variabili multiple] il modulo viene eseguito prima del [!UICONTROL Strumenti] > [!UICONTROL Get Variable] modulo . Per ulteriori informazioni sull’ordine di esecuzione dei moduli, vedi [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable name]</td> 
   <td> <p>Mappa il nome della variabile che desideri ottenere dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Funzione di incremento]

Questo modulo restituisce un valore incrementato di 1 dopo il funzionamento di ciascun modulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reimposta un valore]</td> 
   <td> <p>Seleziona quando desideri che il modulo incrementi il valore. </p> 
    <ul> 
     <li>[!UICONTROL Dopo un ciclo]</li> 
     <li>[!UICONTROL Dopo un'esecuzione di scenario]</li> 
     <li>[!UICONTROL Mai]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:**
>
>Uno degli utilizzi del modulo è quello di implementare un’assegnazione &quot;round robin&quot; di attività, lead, e-mail e così via, agli utenti di un gruppo. L&#39;algoritmo sceglie gli assegnatari da un gruppo in un certo ordine razionale, di solito andando dall&#39;alto in fondo a un elenco. Quando l’algoritmo raggiunge la fine dell’elenco, assegna l’assegnazione successiva all’utente in cima all’elenco e continua a effettuare assegnazioni in basso nell’elenco.
>
>Lo scenario seguente invia un’e-mail al primo destinatario dopo ogni esecuzione di scenari dispari e al secondo destinatario dopo ogni esecuzione di scenari pari.
>
>![](assets/example-email-350x246.gif)
>
>1. Per creare questo scenario:
>1. Imposta il **[!UICONTROL Reimpostare un valore]** campo per mai.
>1. Impostare il percorso per i valori dispari. Impostare il filtro per questa route utilizzando la funzione matematica del modulo uguale a `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **Nota**: Non dimenticare di modificare le [!UICONTROL Uguale a] dall’impostazione predefinita [!UICONTROL Testo] all&#39;operatore [!UICONTROL Numerico] operatore.
>
>1. Imposta la route per i valori pari utilizzando la funzione matematica del modulo che è uguale a `0`:
>
>La funzione di incremento ne aggiunge una ogni volta che lo scenario viene eseguito. I filtri controllano l’incremento e agiscono sul suo valore, garantendo che le e-mail siano distribuite in modo uniforme.

#### [!UICONTROL Imposta variabili multiple]

Questo modulo crea variabili che possono essere mappate da altri moduli della route. La variabile può anche essere mappata alla variabile [!UICONTROL Get Variable] o [!UICONTROL Ottieni variabili multiple] moduli per qualsiasi route nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Aggiungi le variabili che desideri impostare nel modulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Per ogni variabile, immetti il nome della variabile. Questo nome verrà visualizzato quando mappi la variabile in altri moduli. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore della variabile] </td> 
   <td>Per ogni variabile, immetti il valore della variabile . </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata della variabile] </td> 
   <td> <p>Seleziona per quanto tempo vuoi che le variabili rimangano valide (mantieni lo stesso valore).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: La variabile è valida per un ciclo. Utile quando vengono ricevuti più webhook in un'esecuzione di scenario (più webhook = più cicli). </li> 
     <li><strong>[!UICONTROL Un'esecuzione]</strong>: La variabile è valida per un'esecuzione di scenario. Una esecuzione può contenere uno o più cicli.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Imposta variabile]

Questo modulo crea una variabile che può essere mappata da altri moduli della route. La variabile può anche essere mappata alla variabile [!UICONTROL Get Variable] o [!UICONTROL Ottieni variabili multiple] moduli per qualsiasi route nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Immetti il nome della variabile. Questo nome verrà visualizzato quando mappi la variabile in altri moduli. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata della variabile] </td> 
   <td> <p>Seleziona per quanto tempo vuoi che le variabili rimangano valide (mantieni lo stesso valore).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: La variabile è valida per un ciclo. Utile quando vengono ricevuti più webhook in un'esecuzione di scenario (più webhook = più cicli). </li> 
     <li><strong>[!UICONTROL Un'esecuzione]</strong>: La variabile è valida per un'esecuzione di scenario. Una esecuzione può contenere uno o più cicli.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore della variabile] </td> 
   <td>Immetti o mappa il valore della variabile. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sonno]

Questo modulo consente di ritardare il flusso dello scenario per un massimo di 300 secondi (5 minuti).

Questa funzione può essere utile, ad esempio, se desideri abbassare il [!DNL target] caricamento del server di servizio o per imitare il comportamento umano durante l’invio in massa di SMS o e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Ritardo]</p> </td> 
   <td> <p>Immettere il numero di secondi per i quali lo scenario verrà messo in pausa.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Se desideri mettere in pausa il flusso per periodi di tempo più lunghi, ti consigliamo di suddividere lo scenario in due scenari:
>
>* Il primo scenario conterrebbe la parte prima della pausa.
>* Il secondo scenario conterrebbe la parte successiva.
>
>Il primo scenario termina con l&#39;archiviazione di tutte le informazioni necessarie in un archivio dati insieme alla marca temporale corrente. Il secondo scenario controlla periodicamente l’archiviazione dei dati per i record con una marca temporale precedente al ritardo previsto, recupera i record, finalizza l’elaborazione dei dati e rimuovi i record dall’archivio dati.
>
>Per ulteriori informazioni sugli archivi dati, consulta [Archivia dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Per ulteriori informazioni su moduli di archiviazione dati specifici, consulta [[!UICONTROL Archiviazione dati] moduli](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Aggregatori

* [[!UICONTROL Aggregatore numerico]](#numeric-aggregator)
* [[!UICONTROL Aggregatore tabella]](#table-aggregator)
* [[!UICONTROL Aggregatore di testo]](#text-aggregator)

#### [!UICONTROL Aggregatore numerico]

Questo modulo consente di recuperare i valori numerici, quindi applicare una delle funzioni selezionate (SUM, AVG, COUNT, MAX, MIN) e restituire il risultato in un unico bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo di origine]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Seleziona la funzione da utilizzare per aggregare i valori.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definire un’espressione per la quale si desidera raggruppare l’output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati vengono quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l'espressione valutata) e un valore (il valore aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Abilita questa opzione per interrompere lo scenario in assenza di risultati.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>Immetti o mappa il valore da aggregare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggregatore tabella]

Questo modulo unisce i valori dai campi selezionati dei bundle ricevuti in un singolo bundle utilizzando un separatore di colonna e riga specificato (che consente di creare una tabella).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo di origine]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td> <p> Seleziona dal modulo selezionato in precedenza i campi che contengono i valori che desideri aggregare nell’unico bundle.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore di colonna]</p> </td> 
   <td> <p>Selezionare o immettere il tipo di separatore che separerà le colonne del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere da utilizzare per separare i valori nel campo del separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore di riga]</p> </td> 
   <td> <p>Selezionare o immettere il tipo di separatore che separerà le righe del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere da utilizzare per separare i valori nel campo del separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definire un’espressione per la quale si desidera raggruppare l’output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati saranno quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l'espressione valutata) e un valore (il valore aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario in assenza di risultati.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggregatore di testo]

Questo modulo unisce i valori dai campi selezionati dei bundle ricevuti in un unico bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo di origine]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore di riga]</p> </td> 
   <td> <p>Selezionare o immettere il tipo di separatore che separerà le righe del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere da utilizzare per separare i valori nel campo del separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Definisci un'espressione contenente uno o più elementi mappati. I dati aggregati sono separati in Gruppi con lo stesso valore dell'espressione. Ogni gruppo produce come bundle separato contenente una Chiave con l'espressione valutata e il testo aggregato. In questo modo, puoi utilizzare la Chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testo]</td> 
   <td> <p> Immettere o mappare il testo che si desidera aggregare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario in assenza di risultati.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Puoi utilizzare l’aggregatore di testo per inserire più valori (ad esempio, nomi o note dei clienti) in un singolo bundle e inviare un’e-mail contenente tutti i valori nel corpo dell’e-mail o nell’oggetto dell’e-mail.

### Trasformatori

* [[!UICONTROL Componi una stringa]](#compose-a-string)
* [[!UICONTROL Convertire la codifica del testo]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Interruttore]](#switch)

#### [!UICONTROL Componi una stringa]

Converte qualsiasi valore in un tipo di dati stringa (testo). Semplifica la mappatura, ad esempio, quando si mappano dati binari.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo]</td> 
   <td> <p>Immetti o mappa i dati da convertire in testo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertire la codifica del testo]

Converte il testo di input immesso (o dati binari) nella codifica selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>Immetti o mappa il contenuto da convertire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Seleziona il tipo di codifica dei dati di input. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Pagina del codice dei dati di output]</p> </td> 
   <td> <p>Seleziona il tipo di codifica dei dati di destinazione (output).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Interruttore]

Verifica la presenza di una corrispondenza con l’elenco di valori fornito. Restituisce l&#39;output in base al risultato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Immettere l'espressione da valutare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usa espressioni regolari per trovare corrispondenza]</td> 
   <td> <p>Abilita questa opzione per utilizzare espressioni regolari. Il modulo determina i casi in base all’espressione regolare, anziché a una corrispondenza esatta.</p> 
    <div> 
     <p>Un'espressione regolare è una sequenza di caratteri in cui ogni carattere è un metacarattero, con un significato speciale, o un carattere regolare con un significato letterale. Questi caratteri e metacaratteri identificano un pattern che può essere utilizzato per la ricerca di testo. Ad esempio, se si desidera cercare i nomi, è possibile impostare un'espressione regolare per cercare un pattern composto da due parole consecutive che iniziano con lettere maiuscole. Le espressioni regolari sono uno strumento potente per la ricerca e la manipolazione del testo.</p> 
     <p>Una discussione sulle espressioni regolari va oltre l'ambito di applicazione di questo articolo. Consigliamo le seguenti risorse:</p> 
     <ul> 
      <li>Per l'elenco completo dei metacaratteri, vedi <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Espressioni regolari</a> nei documenti web MDN.</li> 
      <li>Per un'esercitazione su come creare espressioni regolari, si consiglia di <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Per la sperimentazione con espressioni regolari, si consiglia l’ <a href="https://regex101.com/">Espressioni regolari 101</a> sito web. Selezionare ECMAScript (JavaScript) FLAVOR nel pannello a sinistra.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Casi [!UICONTROL] </td> 
   <td> <p>Se l’input contiene un valore inserito nel campo [!UICONTROL Pattern], viene restituito il valore inserito nel campo [!UICONTROL Output] .</p> <p>Se l’input non corrisponde a nessuno dei valori impostati in un campo [!UICONTROL Pattern], si verifica una delle seguenti situazioni:</p> 
    <ul> 
     <li>Viene restituito il valore del campo [!UICONTROL Else]</li> 
     <li>Se nel campo [!UICONTROL Else] non è presente alcun valore, non viene restituito alcun output.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Immetti il valore restituito quando i criteri impostati nel campo Casi non sono soddisfatti. </p> </td> 
  </tr> 
 </tbody> 
</table>
