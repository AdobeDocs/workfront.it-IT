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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 3%

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

Restituisce il valore `value1` se l’espressione viene valutata come true; in caso contrario restituisce il `value2`.

>[!INFO]
>
>**Esempi:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Restituisce Un
>
>* `if( = 2 ; A ; B )`
>
>   Restituisce B

## [!UICONTROL ifempty (valore1; valore2)]

Restituisce il valore `value1` se questo valore non è vuoto, altrimenti restituisce il `value2`.

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

## [!UICONTROL switch (espressione; valore1; risultato1; [valore2; risultato2; ...]; [else])]

Valuta un valore (denominato espressione) rispetto a un elenco di valori; restituisce il risultato corrispondente al primo valore corrispondente.

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

Omette le chiavi specificate dell&#39;oggetto e restituisce il resto.

>[!INFO]
>
>**Esempio:**
>
>`omit(` Utente `;` password `)`
>
>Restituisce una raccolta delle informazioni dell&#39;utente, escludendo >la password.

## [!UICONTROL pick(object; key1; [key2; ...])]

Seleziona dall’oggetto solo le chiavi specificate.

>[!INFO]
>
>**Esempio:**
>
>`pick(` Utente `;` password `;` email `)`
>
>Restituisce una raccolta contenente solo la password e l&#39;indirizzo e-mail dell&#39;utente.
