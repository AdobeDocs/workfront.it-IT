---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni generali in Adobe Workfront Fusion
description: Le seguenti funzioni generali sono disponibili nel pannello di mappatura di Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

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

## [!UICONTROL get (oggetto o array; percorso)]

Restituisce il percorso del valore di un oggetto o di una matrice. Per accedere agli oggetti nidificati, utilizzare la notazione del punto. Il primo elemento di una matrice è l&#39;indice 1.

>[!INFO]
>
>**Esempi:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if (espressione; valore1; value2)]

Restituisce il `value1` se l’espressione è valutata come true; altrimenti restituisce il `value2`.

>[!INFO]
>
>**Esempi:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    Restituisce A
>
>* `if( = 2 ; A ; B )`
   >
   >   Restituisce B


## [!UICONTROL ifempty (valore1; value2)]

Restituisce il `value1` se questo valore non è vuoto; altrimenti restituisce il `value2`.

>[!INFO]
>
>**Esempi:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   Restituisce A
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   Restituisce B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   Restituisce B


## [!UICONTROL switch (espressione; valore1; risultato1; [value2; risultato2; ...]; [else])]

valuta un valore (denominato espressione) rispetto a un elenco di valori; restituisce il risultato corrispondente al primo valore corrispondente.

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
>  Restituisce 4

## [!UICONTROL omit(object; key1; [key2; ...])]

omette le chiavi specificate dell&#39;oggetto e restituisce il resto.

>[!INFO]
>
>**Esempio:**
>
>`omit(` Utente `;` password `)`
>
>Restituisce un insieme di informazioni dell&#39;utente, escludendo >la password.

## [!UICONTROL pick(object; key1; [key2; ...])]

Seleziona dall’oggetto solo le chiavi specificate.

>[!INFO]
>
>**Esempio:**
>
>`pick(` Utente `;` password `;` email `)`
>
>Restituisce un insieme solo della password e dell&#39;indirizzo e-mail dell&#39;utente.
