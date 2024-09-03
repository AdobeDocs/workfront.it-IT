---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni generali di Adobe Workfront Fusion
description: Nel pannello di mappatura di Adobe Workfront Fusion sono disponibili le seguenti funzioni generali.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 4cca9738ad9537247234faa0b1c441163d4e315f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Funzioni generali in [!DNL Adobe Workfront Fusion]

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL get (oggetto o array; percorso)]

Restituisce il percorso del valore di un oggetto o di una matrice. Per accedere agli oggetti nidificati, utilizzare la notazione del punto. Il primo elemento di un array è l&#39;indice 1.

>[!INFO]
>
>**Esempi:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (espressione; valore1; valore2)]

Restituisce `value1` se l&#39;espressione viene valutata come true, altrimenti restituisce `value2`.

Per creare un&#39;istruzione if che restituisca un valore solo se due o più espressioni vengono valutate come true, utilizzare la parola chiave `and`.

Per combinare `if` istruzioni, utilizzare gli operatori `and` e `or`.

![e operatore](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Esempi:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Restituisce Un
>
>* `if( 1 = 2 ; A ; B )`
>
>   Restituisce B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Restituisce B
>   

## [!UICONTROL ifempty (valore1; valore2)]

Restituisce `value1` se questo valore non è vuoto, altrimenti restituisce `value2`.

>[!INFO]
>
>**Esempi:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Restituisce Un
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Restituisce B
>
>* `ifempty(` `""` `;` `B` )
>
>   Restituisce B

## [!UICONTROL opzione (espressione; valore1; risultato1; [valore2; risultato2; ...]; [altro])]

Valuta un valore (denominato espressione) rispetto a un elenco di valori; restituisce il risultato corrispondente al primo valore corrispondente. Per includere un valore `else`, aggiungerlo dopo l&#39;espressione o il valore finale.

>[!INFO]
>
>**Esempi:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Restituisce 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Restituisce 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   Restituisce 4
>   
>   In questa funzione, 4 è il valore da restituire se non viene applicata alcuna espressione (il valore `else`).

## [!UICONTROL omit(object; key1; [key2; ...])]

Omette le chiavi specificate dell&#39;oggetto e restituisce il resto.

>[!INFO]
>
>**Esempio:**
>
>`omit(` Utente `;` password `)`
>
>Restituisce una raccolta delle informazioni dell&#39;utente, esclusa la password.

## [!UICONTROL scegli(oggetto; chiave1; [chiave2; ...])]

Seleziona dall’oggetto solo le chiavi specificate.

>[!INFO]
>
>**Esempio:**
>
>`pick(` Utente `;` password `;` e-mail `)`
>
>Restituisce una raccolta contenente solo la password e l&#39;indirizzo e-mail dell&#39;utente.
