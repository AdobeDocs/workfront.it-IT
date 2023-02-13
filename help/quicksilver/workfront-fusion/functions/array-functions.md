---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni dell'array in Adobe Workfront Fusion
description: Le seguenti funzioni dell'array sono disponibili nel pannello di mappatura di Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Funzioni dell&#39;array in Adobe Workfront Fusion

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

## [!UICONTROL add (array; valore1; value2; ...]

Aggiunge a una matrice i valori specificati nei parametri e restituisce tale array.

## [!UICONTROL contiene (array; valore)]

Verifica se una matrice contiene il valore.

## [!UICONTROL distinto (array; [key])]

Rimuove i duplicati all’interno di una matrice. Utilizza il &quot;[!UICONTROL key]&quot; argomento per accedere alle proprietà all’interno di oggetti complessi. Per accedere alle proprietà nidificate, utilizza la notazione del punto. Il primo elemento di una matrice è l&#39;indice 1.

>[!INFO]
>
>**Esempio:** `distinct(Contacts[];name)`
>
>Rimuove i duplicati all&#39;interno di una matrice di contatti confrontando la proprietà &quot;name&quot;

## [!UICONTROL flatten (array)]

Crea un nuovo array con tutti gli elementi di sottoarray concatenati, in modo ricorsivo, fino alla profondità specificata.


## [!UICONTROL join (array; separatore)]

Concatena tutti gli elementi di un array in una stringa utilizzando il separatore specificato tra ciascun elemento.

## [!UICONTROL keys (oggetto)]

Restituisce una matrice delle proprietà di un oggetto o array specificato.

## [!UICONTROL length (array)]

Restituisce il numero di elementi in una matrice.

## [!UICONTROL mappa (matrice complessa; chiave;[chiave per il filtro];[possibili valori di filtro])]

Restituisce una matrice primitiva contenente i valori di una matrice complessa. Questa funzione consente di filtrare i valori. Utilizza i nomi delle variabili non elaborate per le chiavi.

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
>  Restituisce un array primitivo con e-mail con un&#39;etichetta uguale a lavoro o a casa

Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (array1); array2; ...]

Unisce uno o più array in un unico array.

## [!UICONTROL remove (array; valore1; value2; ...]

Rimuove i valori specificati nei parametri di una matrice. Questa funzione è efficace solo su array primitivi di testo o numeri.

## [!UICONTROL reverse (array)]

Il primo elemento dell’array diventa l’ultimo, il secondo diventa il successivo all’ultimo e così via.

## [!UICONTROL sezione (matrice); inizio; [end])]

Restituisce una nuova matrice contenente solo gli elementi selezionati.

## [!UICONTROL sort (array; [ordine]; [key])]

Ordina i valori di una matrice. I valori validi della `order` sono:

* `asc`

   (predefinito) - Ordine crescente: 1, 2, 3, ... per il tipo Numero. A, B, C, a, b, c, ... per tipo Testo

* `desc`

   ordine decrescente: ..., 3, 2, 1 per il tipo Numero. ..., c, b, a, C, B, A per il tipo Testo.

* `asc ci`

   ordine crescente senza distinzione tra maiuscole e minuscole: A, a, B, b, C, c, ... per il tipo Testo.

* `desc ci`

   ordine decrescente senza distinzione tra maiuscole e minuscole: ..., C, c, B, b, A, a per il tipo Testo.

Utilizza la `key` per accedere alle proprietà all’interno di oggetti complessi.

Utilizza i nomi delle variabili non elaborate per le chiavi.

Per accedere alle proprietà nidificate, utilizza la notazione del punto.

Il primo elemento di una matrice è l&#39;indice 1.

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
   >    Ordina una matrice di contatti in base alla proprietà &quot;name&quot; in ordine crescente senza distinzione tra maiuscole e minuscole
>
>* `sort(Emails[];sender.name)`
   >
   >    Ordina una matrice di e-mail dalla proprietà &quot;sender.name&quot;


## [!UICONTROL arrayDifference [array1, array2, modalità]]

Restituisce la differenza tra due array.

Immettere uno dei seguenti valori per il `mode` parametro .

* `classic`: Restituisce un nuovo array contenente tutti gli elementi di `array1` che non esistono in `array2`.

* `symmetric`: Restituisce una matrice di elementi non comuni a entrambi gli array.

   In altre parole, la funzione restituisce un array che contiene tutti gli elementi di `array1` che non esistono in `array2`e tutti gli elementi `array2` che non esistono in `array1`.

   >[!INFO]
   >
   >**Esempi:**
   >
   >Dati i seguenti array:
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
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

