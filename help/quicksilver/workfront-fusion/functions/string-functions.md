---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni stringa in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Funzioni stringa in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Funzioni stringa](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/string-functions.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] piano</td>  
   <td> <p>Qualsiasi</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td>  
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td>  
   <td> 
   <p>Corrente: nessun requisito di licenza [!DNL Workfront Fusion].</p> 
   <p>Oppure</p> 
   <p>Legacy: qualsiasi </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Prodotto</td>  
   <td> 
   <p>Nuovo:</p> <ul><li>Piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Il piano [!DNL Workfront Fusion] è incluso.</li></ul> 
   <p>Oppure</p> 
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL lunghezza (testo o buffer)]

Restituisce la lunghezza della stringa di testo (numero di caratteri) o del buffer binario (dimensione del buffer in byte).

>[!INFO]
>
>**Esempio:**
>
>`length( hello )`
>
>Restituisce: 5

## [!UICONTROL inferiore (testo)]

Converte tutti i caratteri alfabetici di una stringa di testo in minuscolo.

>[!INFO]
>
>**Esempio:**
>
>`lower( Hello )`
>
>Restituisce: hello

## [!UICONTROL maiuscole (testo)]

Converte il primo carattere di una stringa di testo in maiuscolo.

>[!INFO]
>
>**Esempio:**
>
>`capitalize( workfront )`
>
>Restituisce: [!DNL Workfront]

## [!UICONTROL startcase (testo)]

Usa la maiuscola per la prima lettera di ogni parola e le minuscole per tutte le altre lettere.

>[!INFO]
>
>**Esempio:**
>`startcase( hello WORLD )`
>
>Restituisce: [!UICONTROL Hello World]

## [!UICONTROL ascii (testo; [rimuovere segni diacritici])]

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



## [!UICONTROL sostituisci (testo;stringa di ricerca; stringa di sostituzione)]

sostituisce la stringa di ricerca con la nuova stringa.

>[!INFO]
>
>**Esempio:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Restituisce: [!UICONTROL Salve mondo]

Le espressioni regolari (racchiuse in `/.../`) possono essere utilizzate come stringa di ricerca con una combinazione di flag (ad esempio `g`, `i`, `m`) aggiunti:

>[!INFO]
>
>**Esempio:**
>
>![](assets/replace---1-350x31.png)
>
>Tutti questi numeri X X X X sono sostituiti da X

La stringa di sostituzione può includere i seguenti modelli di sostituzione speciali:

* `$&` Inserisce la sottostringa corrispondente.
* `$n` Dove n è un numero intero positivo minore di 100, inserisce l&#39;ennesima stringa tra parentesi. È indicizzato 1.

>[!INFO]
>
>**Esempi:**
>
>![](assets/variable-value-350x63.png)
>
>Restituisce: numero di telefono `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Restituisce: numero di telefono: `+420777111222`

>[!CAUTION]
>
>Non utilizzare gruppi di acquisizione denominati come `/ is (?<number>\d+)/` nell&#39;argomento della stringa di sostituzione. In questo caso si verifica un errore.

Per ulteriori informazioni sulle espressioni regolari, vedere [Parser di testo](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL ritaglio (testo)]

Rimuove gli spazi all&#39;inizio o alla fine del testo.

## [!UICONTROL superiore (testo)]

Converte tutti i caratteri alfabetici in maiuscolo in una stringa di testo.

>[!INFO]
>
>**Esempio:**
>
>`upper( Hello )`
>
>Restituisce: [!UICONTROL CIAO]

## [!UICONTROL sottostringa (testo; inizio;fine)]

Restituisce una parte di una stringa di testo tra la posizione &quot;start&quot; e la posizione &quot;end&quot;.

>[!INFO]
>
>**Esempi:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Restituisce: Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Restituisce: el

## [!DNL indexOf (string; value; [start])]

Restituisce la posizione della prima occorrenza di un valore specificato in una stringa. Questo metodo restituisce &#39;-1&#39; se il valore ricercato non è presente. Il valore iniziale indica la posizione nella stringa da cui deve iniziare la ricerca.

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

## [!UICONTROL toBinary (valore)]

Converte qualsiasi valore in dati binari.

È inoltre possibile specificare la codifica come secondo argomento per applicare le conversioni binarie da hex o base64 ai dati binari.

>[!INFO]
>
>**Esempi:**
>
>* `toBinary( Workfront )`
>
>   Restituisce: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Restituisce: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (valore)]

Converte qualsiasi valore in una stringa.

## [!UICONTROL encodeURL (testo)]

Codifica i caratteri speciali in un testo in un indirizzo URL valido.

## [!UICONTROL decodeURL (testo)]

Decodifica caratteri speciali in un URL in testo.

>[!INFO]
>
>**Esempio:**
>`decodeURL( Automate%20your%20workflow )`
>
>Restituisce: [!UICONTROL Automatizza il flusso di lavoro]

## [!UICONTROL escapeHTML (testo)]

Esclude tutti i tag HTML nel testo.

>[!INFO]
>
>**Esempio:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Restituisce: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Evita tutti i tag Markdown nel testo.

>[!INFO]
>
>**Esempio:**
>
>`escapeMarkdown( # Header )`
>
>Restituisce: `&#35; Header`

## [!UICONTROL stripHTML (testo)]

Rimuove tutti i tag HTML dal testo.

>[!INFO]
>
>**Esempio:**
>
>`stripHTML( <b>Hello</b> )`
>
>Restituisce: Hello

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

## [!UICONTROL split (testo; separatore)]

Divide una stringa in una matrice di stringhe separandola in sottostringhe.

>[!INFO]
>
>**Esempio:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (testo)]

Calcola l’hash MD5 di una stringa.

>[!INFO]
>
>**Esempio:**
>
>`md5( Workfront )`
>
>Restituisce: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (testo; [codifica]; [chiave])]

Calcola l’hash sha1 di una stringa. Se l&#39;argomento chiave è specificato, viene restituito l&#39;hash HMAC sha1. Codifiche supportate: &quot;hex&quot; (impostazione predefinita), &quot;base64&quot; o &quot;latin1&quot;.

>[!INFO]
>
>**Esempio:**
>
>`sha1( workfront )`
>
>Restituisce: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (testo; [codifica]; [chiave])]

Calcola l’hash sha256 di una stringa. Se l&#39;argomento chiave è specificato, viene restituito l&#39;hash sha256 HMAC. Codifiche supportate: &quot;hex&quot; (impostazione predefinita), &quot;base64&quot; o &quot;latin1&quot;.>

>[!INFO]
>
>**Esempio:**
>
>`sha256( workfront )`
>
>Restituisce: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (testo; [codifica output]; [chiave]; [codifica chiave])]

Calcola l’hash sha512 di una stringa. Se l&#39;argomento chiave è specificato, viene restituito l&#39;hash HMAC sha512.

Codifiche supportate

* &quot;[!UICONTROL esadecimale]&quot; (impostazione predefinita)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codifiche chiave supportate:

* &quot;[!UICONTROL testo]&quot; (impostazione predefinita)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; o &quot;[!UICONTROL binario]&quot;

Quando si utilizza la codifica di chiave &quot;[!UICONTROL binary]&quot;, una chiave deve essere un buffer, non una stringa.

>[!INFO]
>
>**Esempio:**
>
>`sha512(workfront)`
>
>Restituisce: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (testo)]

Trasforma il testo in base64.

>[!INFO]
>
>**Esempio:**
>
>`base64( workfront )`
>
>Restituisce: d29ya2Zyb250==
