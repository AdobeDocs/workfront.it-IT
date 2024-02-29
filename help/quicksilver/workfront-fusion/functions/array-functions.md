---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni array in Adobe Workfront Fusion
description: Nel pannello di mappatura di Adobe Workfront Fusion sono disponibili le seguenti funzioni di array.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 5860e75d0a6521abbe082668749f78058fe7a114
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Funzioni array in Adobe Workfront Fusion

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
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL aggiungi (matrice; valore1; valore2; ...)]

Aggiunge i valori specificati nei parametri a un array e restituisce tale array.

## [!UICONTROL contiene (array; valore)]

Verifica se un array contiene il valore.

## [!UICONTROL distinct (array; [chiave])]

Rimuove i duplicati all&#39;interno di un array. Utilizza la &quot;[!UICONTROL chiave]&quot; per accedere alle proprietà all&#39;interno di oggetti complessi. Per accedere alle proprietà nidificate, utilizza la notazione del punto. Il primo elemento di un array è l&#39;indice 1.

>[!INFO]
>
>**Esempio:** `distinct(Contacts[];name)`
>
>Rimuove i duplicati in un array di contatti confrontando la proprietà &quot;name&quot;

## [!UICONTROL appiattisci (array)]

Crea un nuovo array con tutti gli elementi sub-array concatenati in esso, in modo ricorsivo, fino alla profondità specificata.


## [!UICONTROL join (array; separatore)]

Concatena tutti gli elementi di un array in una stringa utilizzando il separatore specificato tra ogni elemento.

## [!UICONTROL tasti (oggetto)]

Restituisce una matrice delle proprietà di un determinato oggetto o matrice.

## [!UICONTROL lunghezza (array)]

Restituisce il numero di elementi in una matrice.

## [!UICONTROL mappa (array complesso; chiave;[chiave per il filtro];[valori possibili per il filtro])]

Restituisce una matrice primitiva contenente i valori di una matrice complessa. Questa funzione consente di filtrare i valori. Utilizza nomi di variabili non elaborati per le chiavi.

>[!INFO]
>
>**Esempi:**
>
>* `map(Emails[];email)`
>
>  Restituisce un array primitivo con le e-mail
>
>* `map(Emails[];email;label;work;home)`
>
>  Restituisce un array primitivo con e-mail aventi un’etichetta uguale a lavoro o casa

Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (matrice1; matrice2; ...)]

Unisce uno o più array in un unico array.

## [!UICONTROL rimuovere (matrice; valore1; valore2; ...)]

Rimuove i valori specificati nei parametri di un array. Questa funzione è efficace solo su array primitivi di testo o numeri.

## [!UICONTROL inverso (array)]

Il primo elemento dell’array diventa l’ultimo elemento, il secondo diventa il successivo-ultimo e così via.

## [!UICONTROL slice (array; start; [fine])]

Restituisce una nuova matrice contenente solo gli elementi selezionati.

## [!UICONTROL sort (array; [ordine]; [chiave])]

Ordina i valori di un array. I valori validi della proprietà `order` I parametri sono:

* `asc`

  (impostazione predefinita) - Ordine crescente: 1, 2, 3, ... per il tipo Numero. A, B, C, a, b, c, ... per il tipo Testo

* `desc`

  ordine decrescente: ..., 3, 2, 1 per il tipo Numero. ..., c, b, a, C, B, A per il tipo Testo.

* `asc ci`

  ordine crescente senza distinzione tra maiuscole e minuscole: A, a, B, b, C, c, ... per il tipo Testo.

* `desc ci`

  ordine decrescente senza distinzione tra maiuscole e minuscole: ..., C, c, B, b, A, a per il tipo Testo.

Utilizza il `key` per accedere alle proprietà all&#39;interno di oggetti complessi.

Utilizza nomi di variabili non elaborati per le chiavi.

Per accedere alle proprietà nidificate, utilizza la notazione del punto.

Il primo elemento di un array è l&#39;indice 1.

>[!INFO]
>
>**Esempi:**
>
>* `sort(Contacts[];name)`
>
>    Ordina un array di contatti in base alla proprietà &quot;name&quot; in ordine crescente predefinito
>
>* `sort(Contacts[];desc;name)`
>
>   Ordina un array di contatti in base alla proprietà &quot;name&quot; in ordine decrescente
>
>* `sort(Contacts[];asc ci;name)`
>
>    Ordina un array di contatti in base alla proprietà &quot;name&quot;, in ordine crescente senza distinzione tra maiuscole e minuscole
>
>* `sort(Emails[];sender.name)`
>
>    Ordina un array di e-mail in base alla proprietà &quot;sender.name&quot;

## [!UICONTROL arrayDifference [array1, array2, modalità]]

Restituisce la differenza tra due array.

Immetti uno dei seguenti valori per `mode` parametro.

* `classic`: restituisce un nuovo array che contiene tutti gli elementi di `array1` che non esistono in `array2`.

* `symmetric`: restituisce una matrice di elementi che non sono comuni a entrambe le matrici.

  In altre parole, la funzione restituisce un array che contiene tutti gli elementi di `array1` che non esistono in `array2`, e tutti gli elementi di `array2` che non esistono in `array1`.

  >[!INFO]
  >
  >**Esempi:**
  >
  >Considerati i seguenti array:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Restituisce `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Restituisce `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Restituisce `[1,2,6,7]`

## toArray

Questa funzione converte una raccolta in un array di coppie chiave-valore.

>[!INFO]
>
>**Esempi:**
>
>Data la raccolta
>
>`{ key1: "value1", key2: "value2:}`
>
>La funzione
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Restituisce la matrice di coppie chiave-valore
>
>`[{ key1: "value1"}, { key2: "value2"}]`
