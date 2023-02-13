---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni stringa in Adobe Workfront Fusion
description: Le seguenti funzioni stringa sono disponibili nel pannello di mappatura di Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# Funzioni stringa in [!DNL Adobe Workfront Fusion]

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (testo; [rimuovere la diacritica])]

Rimuove tutti i caratteri non ascii da una stringa di testo.

>[!INFO]
>
>**Esempi:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   Restituisce: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   Restituisce: [!UICONTROL escrz]


## [!UICONTROL base64 (testo)]

Trasforma il testo in base64.

>[!INFO]
>
>**Esempio:**
>
>`base64( workfront )`
>
>Restituisce: d29ya2Zyb250===

## [!UICONTROL maiuscola (testo)]

Converte il primo carattere di una stringa di testo in maiuscolo.

>[!INFO]
>
>**Esempio:**
>
>`capitalize( workfront )`
>
>Restituisce: [!DNL Workfront]

## contiene (testo; stringa di ricerca)

Verifica se il testo contiene la stringa di ricerca.

>[!INFO]
>
>**Esempi:**
>
>* `contains( Hello World ; Hello )`
   >
   >   Restituisce: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   Restituisce: [!UICONTROL false]


## [!UICONTROL decodeURL (testo)]

Decodifica caratteri speciali in un URL in testo.

>[!INFO]
>
>**Esempio:**
>`decodeURL( Automate%20your%20workflow )`
>
>Restituisce: [!UICONTROL Automatizzare il flusso di lavoro]

## [!UICONTROL encodeURL (testo)]

Codifica caratteri speciali in un testo in un indirizzo URL valido.

## [!UICONTROL escapeHTML (testo)]

Elimina tutti i tag di HTML nel testo.

>[!INFO]
>
>**Esempio:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Restituisce: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Elimina tutti i tag Markdown nel testo.

>[!INFO]
>
>**Esempio:**
>
>`escapeMarkdown( # Header )`
>
>Restituisce: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

Restituisce la posizione della prima occorrenza di un valore specificato in una stringa. Questo metodo restituisce &#39;-1&#39; se il valore ricercato non è presente. Il valore iniziale indica dove deve iniziare la ricerca nella stringa.

>[!INFO]
>
>**Esempi:**
>
>* `indexOf( Workfront ; o )`
   >
   >   Restituisce: 1
>
>* `indexOf( Workfront ; x )`
   >
   >   Restituisce: -1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   Restituisce: 6


## [!UICONTROL lunghezza (testo o buffer)]

Restituisce la lunghezza della stringa di testo (numero di caratteri) o del buffer binario (dimensione del buffer in byte).

>[!INFO]
>
>**Esempio:**
>
>`length( hello )`
>
>Restituisce: 5

## [!UICONTROL Lower (testo)]

Converte tutti i caratteri alfabetici di una stringa di testo in minuscolo.

>[!INFO]
>
>**Esempio:**
>
>`lower( Hello )`
>
>Restituisce: hello

## [!UICONTROL md5 (testo)]

Calcola l’hash md5 di una stringa.

>[!INFO]
>
>**Esempio:**
>
>`md5( Workfront )`
>
>Restituisce: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sostituire (testo;stringa di ricerca; stringa sostitutiva)]

Sostituisce la stringa di ricerca con la nuova stringa.

>[!INFO]
>
>**Esempio:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Restituisce: [!UICONTROL Hi World]

Espressioni regolari (racchiuse in `/.../`) può essere utilizzata come stringa di ricerca con una combinazione di flag (ad esempio `g`, `i`, `m`) aggiunta:

>[!INFO]
>
>**Esempio:**
>
>![](assets/replace---1-350x31.png)
>
>Tutti questi numeri X X X X sono sostituiti con X

La stringa di sostituzione può includere i seguenti pattern di sostituzione speciali:

* `$&` Inserisce la sottostringa corrispondente.
* `$n` Se n è un numero intero positivo inferiore a 100, inserisce l’ennesima stringa di sottocorrispondenza tra parentesi. Questo è indicizzato a 1.

>[!INFO]
>
>**Esempi:**
>
>![](assets/variable-value-350x63.png)
>
>Restituisce: Numero di telefono `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>Restituisce: Numero di telefono: `+420777111222`

>[!CAUTION]
Non utilizzare gruppi di acquisizione denominati quali `/ is (?<number>\d+)/` nell&#39;argomento della stringa di sostituzione. In questo modo si verifica un errore.

Per ulteriori informazioni sulle espressioni regolari, consulta [Analizzatore di testo](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (testo; [encoding]; [key])]

Calcola l’hash sha1 di una stringa. Se viene specificato l’argomento chiave, viene restituito invece l’hash HMAC sha1. Codifiche supportate: &quot;esadecimale&quot; (predefinito), &quot;base64&quot; o &quot;latin1&quot;.

>[!INFO]
**Esempio:**
`sha1( workfront )`
Restituisce: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (testo; [encoding]; [key])]

Calcola l’hash sha256 di una stringa. Se viene specificato l’argomento chiave, viene restituito l’hash HMAC sha256. Codifiche supportate: &quot;esadecimale&quot; (predefinito), &quot;base64&quot; o &quot;latin1&quot;.>

>[!INFO]
**Esempio:**
`sha256( workfront )`
Restituisce: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (testo; [codifica output]; [key]; [codifica chiave])]

Calcola l’hash sha512 di una stringa. Se viene specificato l&#39;argomento chiave, viene restituito invece l&#39;hash HMAC sha512.

Codifiche supportate:

* &quot;[!UICONTROL esasperare]&quot; (predefinito)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codifiche chiave supportate:

* &quot;[!UICONTROL text]&quot; (predefinito)
* &quot;[!UICONTROL esasperare]&quot;
* &quot;[!UICONTROL base64]&quot; o &quot;[!UICONTROL binario]&quot;

Quando si utilizza &quot;[!UICONTROL binario]&quot; codifica chiave, una chiave deve essere un buffer, non una stringa.

>[!INFO]
**Esempio:**
`sha512(workfront)`
Restituisce: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b8 5e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL divisione (testo; separatore)]

Divide una stringa in una matrice di stringhe separando la stringa in sottostringhe.

>[!INFO]
**Esempio:**
`split( John, George, Paul ; , )`

## [!UICONTROL startcase (testo)]

Comprende la prima lettera di ogni parola e le lettere minuscole di tutte le altre lettere.

>[!INFO]
**Esempio:**
`startcase( hello WORLD )`
Restituisce: [!UICONTROL Hello World]

## [!UICONTROL stripHTML (testo)]

Rimuove dal testo tutti i tag HTML.

>[!INFO]
**Esempio:**
`stripHTML( <b>Hello</b> )`
Restituisce: Ciao

## [!UICONTROL sottostringa (testo; inizio;fine)]

Restituisce una parte di una stringa di testo tra la posizione &quot;start&quot; e la posizione &quot;end&quot;.

>[!INFO]
**Esempi:**
* `substring( Hello ; 0 ; 3)`

   Restituisce: Alza
* `substring( Hello ; 1 ; 3 )`

   Restituisce: el


## [!UICONTROL toBinary (valore)]

Converte qualsiasi valore in dati binari.

È inoltre possibile specificare la codifica come secondo argomento per applicare conversioni binarie da esadecimali o base64 a dati binari.

>[!INFO]
**Esempi:**
* `toBinary( Workfront )`

   Restituisce: 57 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   Restituisce: 57 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString (valore)]

Converte qualsiasi valore in una stringa.

## [!UICONTROL trim (testo)]

Rimuove gli spazi all’inizio o alla fine del testo.

## [!UICONTROL superiore (testo)]

Converte tutti i caratteri alfabetici di una stringa di testo in caratteri maiuscoli.

>[!INFO]
**Esempio:**
`upper( Hello )`
Restituisce: [!UICONTROL CIAO]
