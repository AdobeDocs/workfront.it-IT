---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Strumenti
description: La sezione  [!DNL Adobe Workfront Fusion Tools]  include diversi moduli utili che possono migliorare il tuo scenario.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2283'
ht-degree: 0%

---

# [!UICONTROL Strumenti]

La sezione [!DNL Adobe Workfront Fusion Tools] include diversi moduli utili che possono migliorare il tuo scenario.

I moduli [!UICONTROL Tools] sono disponibili dall&#39;elenco delle app o dall&#39;icona ![](assets/tools-icon-small.png) di [!UICONTROL Tools] nella parte inferiore dello schermo.

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
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Strumenti] e relativi campi

* [Triggers](#triggers)
* [Azioni](#actions)
* [Aggregatori](#aggregators)
* [Trasformatori](#transformers)

### Triggers

#### [!UICONTROL Trigger di base]

Questo modulo consente di creare un trigger personalizzato e definirne i bundle di input.

Puoi utilizzare questo modulo, ad esempio, per i contatti o qualsiasi altro elenco pianificato per l&#39;invio a un indirizzo e-mail specificato (ad esempio [!UICONTROL E-mail] >[!UICONTROL Invia un messaggio e-mail] o [!DNL Gmail] >[!UICONTROL Invia un messaggio e-mail] moduli) oppure come semplice promemoria da attivare ogni volta che desideri.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Crea bundle personalizzati aggiungendo elementi array. L’array è costituito dalle coppie nome - valore.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Ottieni più variabili]](#get-multiple-variables)
* [[!UICONTROL Ottieni variabile]](#get-variable)
* [[!UICONTROL Funzione di incremento]](#increment-function)
* [[!UICONTROL Imposta più variabili]](#set-multiple-variables)
* [[!UICONTROL Imposta variabile]](#set-variable)
* [[!UICONTROL Sospendi]](#sleep)

#### [!UICONTROL Ottieni più variabili]

Questo modulo recupera i valori creati in precedenza dal modulo [!UICONTROL Imposta variabile] o [!UICONTROL Imposta più variabili].

Questo modulo può leggere le variabili impostate in qualsiasi punto dello scenario, anche se la variabile è stata impostata in un percorso diverso da quello in cui si trova il modulo [!UICONTROL Ottieni più variabili]. L&#39;unico requisito è che il modulo [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] o [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile multipla] venga eseguito prima del modulo [!UICONTROL Strumenti] > [!UICONTROL Ottieni variabili multiple]. Per ulteriori informazioni sull&#39;ordine di esecuzione dei moduli, vedere [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Aggiungi le variabili che desideri ottenere dal modulo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nome variabile]</td>
        <td>Per ogni variabile aggiunta, mappare il nome della variabile che si desidera ottenere.</td>
    </tr>
</table>

>[!INFO]
>
>**Esempi:** Di seguito sono riportati i possibili utilizzi dei moduli [!UICONTROL Set]/[!UICONTROL Get (multiple) variable]:
>
>* Per memorizzare un valore calcolato per un utilizzo successivo, anche in un percorso diverso. Ciò è utile nei casi in cui il valore viene utilizzato in più moduli e la formula per calcolare il valore è eccessivamente complessa.
>* Eseguire il debug di una formula. Se una formula utilizzata in un modulo non fornisce un risultato corretto, copiarla e incollarla in un modulo [!UICONTROL Imposta variabile] inserito prima del modulo appropriato. Disconnetti i moduli dopo il modulo [!UICONTROL Imposta variabile] ed esegui lo scenario. Verificare l&#39;output del modulo [!UICONTROL Imposta variabile], regolare o semplificare la formula, eseguire nuovamente lo scenario e continuare a farlo fino alla risoluzione del problema.


#### [!UICONTROL Ottieni variabile]

Questo modulo recupera un valore creato in precedenza dal modulo [!UICONTROL Imposta variabile] o [!UICONTROL Imposta più variabili].

Questo modulo può leggere le variabili impostate in qualsiasi punto dello scenario, anche se la variabile è stata impostata in un percorso diverso da quello in cui si trova il modulo [!UICONTROL Ottieni variabile]. L&#39;unico requisito è che il modulo [!UICONTROL Strumenti] > [!UICONTROL Imposta variabile] o [!UICONTROL Strumenti] > [!UICONTROL Imposta più variabili] venga eseguito prima del modulo [!UICONTROL Strumenti] > [!UICONTROL Ottieni variabile]. Per ulteriori informazioni sull&#39;ordine di esecuzione dei moduli, vedere [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome variabile]</td> 
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
     <li>[!UICONTROL Dopo l'esecuzione di uno scenario]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:**
>
>Uno degli utilizzi del modulo consiste nell’implementare un’assegnazione &quot;round robin&quot; di attività, lead, e-mail e così via, agli utenti di un gruppo. L&#39;algoritmo sceglie gli assegnatari da un gruppo in un certo ordine razionale, di solito andando dall&#39;alto alla fine di un elenco. Quando l’algoritmo raggiunge la fine dell’elenco, assegna l’assegnazione successiva all’utente in cima all’elenco e continua a effettuare assegnazioni in fondo all’elenco.
>
>Lo scenario seguente invia un’e-mail al primo destinatario dopo ogni esecuzione dello scenario con numero dispari e al secondo destinatario dopo ogni esecuzione dello scenario con numero pari.
>
>![](assets/example-email-350x246.gif)
>
>1. Per creare questo scenario:
>1. Impostare il campo **[!UICONTROL Reimposta un valore]** del modulo su Mai.
>1. Impostare la route per i valori dispari. Impostare il filtro per questa route utilizzando la funzione matematica del modulo che è uguale a `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Nota**: non dimenticare di modificare l&#39;operatore [!UICONTROL Uguale a] dall&#39;operatore [!UICONTROL Testo] predefinito all&#39;operatore [!UICONTROL Numerico].
>
>1. Impostare la route per i valori pari utilizzando la funzione matematica del modulo che è uguale a `0`:
>
>La funzione di incremento ne aggiunge uno ogni volta che viene eseguito lo scenario. I filtri controllano l’incremento e agiscono sul suo valore, garantendo che le e-mail siano distribuite in modo uniforme.

#### [!UICONTROL Imposta più variabili]

Questo modulo crea variabili che possono essere mappate da altri moduli nel percorso. La variabile può anche essere mappata ai moduli [!UICONTROL Get Variable] o [!UICONTROL Get Multiple Variables] per qualsiasi route nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Aggiungi le variabili che desideri che vengano impostate dal modulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome variabile] </td> 
   <td>Per ogni variabile, inserisci il nome della variabile. Questo nome verrà visualizzato quando si esegue la mappatura della variabile in altri moduli. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore variabile] </td> 
   <td>Per ogni variabile, immetti il valore per la variabile. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata variabile] </td> 
   <td> <p>Seleziona per quanto tempo le variabili devono rimanere valide (mantieni lo stesso valore).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: la variabile è valida per un ciclo. Utile quando vengono ricevuti più webhook in un’esecuzione dello scenario (più webhook = più cicli). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: la variabile è valida per l'esecuzione di uno scenario. Un’esecuzione può contenere uno o più cicli.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Imposta variabile]

Questo modulo crea una variabile che può essere mappata da altri moduli nel percorso. La variabile può anche essere mappata ai moduli [!UICONTROL Get Variable] o [!UICONTROL Get Multiple Variables] per qualsiasi route nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome variabile] </td> 
   <td>Immetti il nome della variabile. Questo nome verrà visualizzato quando si esegue la mappatura della variabile in altri moduli. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata variabile] </td> 
   <td> <p>Seleziona per quanto tempo le variabili devono rimanere valide (mantieni lo stesso valore).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: la variabile è valida per un ciclo. Utile quando vengono ricevuti più webhook in un’esecuzione dello scenario (più webhook = più cicli). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: la variabile è valida per l'esecuzione di uno scenario. Un’esecuzione può contenere uno o più cicli.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore variabile] </td> 
   <td>Immetti o mappa il valore per la variabile. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sospendi]

Questo modulo ti consente di ritardare il flusso dello scenario fino a 300 secondi (5 minuti).

Questa funzione può essere utile, ad esempio, se si desidera ridurre il carico del server del servizio [!DNL target] o imitare il comportamento umano durante l&#39;invio di SMS o e-mail in blocco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>Immetti per quanti secondi verrà messo in pausa lo scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Se desideri sospendere il flusso per periodi di tempo più lunghi, ti consigliamo di suddividere lo scenario in due scenari:
>
>* Il primo scenario conterrà la parte prima della pausa.
>* Il secondo scenario conterrà la parte successiva.
>
>Il primo scenario si concluderebbe con l’archiviazione di tutte le informazioni necessarie in un archivio dati insieme alla marca temporale corrente. Il secondo scenario controlla periodicamente l’archivio dati per individuare i record con una marca temporale precedente al ritardo previsto, recupera i record, finalizza l’elaborazione dei dati e rimuove i record dall’archivio dati.
>
>Per ulteriori informazioni sugli archivi dati, vedere [Archivi dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Per ulteriori informazioni su moduli di archivio dati specifici, vedere [[!UICONTROL Moduli di archivio dati]](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Aggregatori

* [[!UICONTROL Aggregatore numerico]](#numeric-aggregator)
* [[!UICONTROL Aggregatore tabella]](#table-aggregator)
* [[!UICONTROL Aggregatore di testo]](#text-aggregator)

#### [!UICONTROL Aggregatore numerico]

Questo modulo consente di recuperare i valori numerici, applicare una delle funzioni selezionate (SUM, AVG, COUNT, MAX, MIN) e restituire il risultato in un bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo Source]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Funzione di aggregazione [!UICONTROL]</p> </td> 
   <td> <p>Selezionare la funzione da utilizzare per aggregare i valori.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Raggruppa per]</p> </td> 
   <td> <p>Definire un'espressione in base alla quale raggruppare l'output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati vengono quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l’espressione valutata) e un valore (il valore aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td> 
   <td>Abilita questa opzione per interrompere lo scenario quando non ci sono risultati.</td> 
  </tr> 
  <tr> 
   <td> <p>Valore [!UICONTROL]</p> </td> 
   <td> <p>Immettere o mappare il valore da aggregare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggregatore tabella]

Questo modulo unisce i valori dei campi selezionati dei bundle ricevuti in un singolo bundle utilizzando un separatore di colonna e riga specificato (che consente di creare una tabella).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo Source]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campi aggregati]</td> 
   <td> <p> Seleziona dal modulo selezionato qui sopra i campi che contengono i valori da aggregare nel bundle uno.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore colonne]</p> </td> 
   <td> <p>Seleziona o immetti il tipo di separatore che separerà le colonne del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere che si desidera utilizzare per separare i valori nel campo separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore di righe]</p> </td> 
   <td> <p>Seleziona o immetti il tipo di separatore che separerà le righe del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere che si desidera utilizzare per separare i valori nel campo separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Raggruppa per]</p> </td> 
   <td> <p>Definire un'espressione in base alla quale raggruppare l'output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati verranno quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l’espressione valutata) e un valore (il valore aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario quando non sono presenti risultati.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggregatore di testo]

Questo modulo unisce in un singolo bundle i valori dei campi selezionati dei bundle ricevuti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo Source]</p> </td> 
   <td> <p>Seleziona il modulo da cui desideri aggregare i campi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separatore di righe]</p> </td> 
   <td> <p>Seleziona o immetti il tipo di separatore che separerà le righe del valore del campo nel bundle risultante. Se si seleziona [!UICONTROL Altro], immettere il carattere che si desidera utilizzare per separare i valori nel campo separatore.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Raggruppa per]</p> </td> 
   <td> <p>Definisci un’espressione contenente uno o più elementi mappati. I dati aggregati vengono separati in Gruppi con il valore della stessa espressione. Ogni gruppo restituisce come bundle separato contenente una Chiave con l’espressione valutata e il testo aggregato. In questo modo, puoi utilizzare la Chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> Inserisci o mappa il testo che desideri aggregare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario quando non sono presenti risultati.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** è possibile utilizzare l&#39;aggregatore di testo per inserire più valori (ad esempio, nomi di clienti o note) in un singolo bundle e inviare un messaggio e-mail contenente tutti i valori nel corpo o nell&#39;oggetto dell&#39;e-mail.

### Trasformatori

* [[!UICONTROL Componi una stringa]](#compose-a-string)
* [[!UICONTROL Convertire la codifica del testo]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Opzione]](#switch)

#### [!UICONTROL Componi una stringa]

Converte qualsiasi valore in un tipo di dati stringa (testo). Semplifica la mappatura quando si mappano, ad esempio dati binari.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>Immettere o mappare i dati da convertire in testo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertire la codifica del testo]

Converte il testo immesso (o i dati binari) nella codifica selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Dati di input]</p> </td> 
   <td> <p>Immetti o mappa il contenuto da convertire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Selezionare il tipo di codifica dei dati di input. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>Seleziona il tipo di codifica dei dati di destinazione (output).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Opzione]

Verifica se il valore immesso corrisponde all’elenco di valori fornito. Restituisce l’output in base al risultato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Immettere l'espressione che si desidera valutare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizza espressioni regolari da trovare]</td> 
   <td> <p>Abilita questa opzione per utilizzare espressioni regolari. Il modulo determina i casi in base all’espressione regolare, anziché a una corrispondenza esatta.</p> 
    <div> 
     <p>Un’espressione regolare è una sequenza di caratteri in cui ogni carattere è un metacarattere, con un significato speciale, o un carattere regolare con un significato letterale. Questi caratteri e metacaratteri identificano un pattern che può essere utilizzato per la ricerca di testo. Ad esempio, se si desidera cercare i nomi, è possibile impostare un'espressione regolare per cercare un motivo costituito da due parole consecutive che iniziano con lettere maiuscole. Le espressioni regolari sono uno strumento utile per la ricerca e la manipolazione del testo.</p> 
     <p>Una discussione sulle espressioni regolari va oltre lo scopo di questo articolo. Si consiglia di utilizzare le risorse seguenti:</p> 
     <ul> 
      <li>Per l'elenco completo dei metacaratteri, vedere <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Espressioni regolari</a> nei documenti Web MDN.</li> 
      <li>Per un'esercitazione sulla creazione di espressioni regolari, consigliamo <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Per la sperimentazione con espressioni regolari, consigliamo il sito Web <a href="https://regex101.com/">Espressioni regolari 101</a>. Selezionare ECMAScript (JavaScript) FLAVOR nel pannello sinistro.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Casi] </td> 
   <td> <p>Se l'input contiene un valore immesso nel campo [!UICONTROL Pattern], viene restituito il valore immesso nel campo [!UICONTROL Output].</p> <p>Se l'input non corrisponde a nessuno dei valori impostati in un campo [!UICONTROL Pattern], si verifica una delle situazioni seguenti:</p> 
    <ul> 
     <li>Viene restituito il valore del campo [!UICONTROL Else]</li> 
     <li>Se nel campo [!UICONTROL Else] non è presente alcun valore, non viene restituito alcun output.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Immettere il valore restituito quando i criteri impostati nel campo Casi non sono soddisfatti. </p> </td> 
  </tr> 
 </tbody> 
</table>
