---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni matematiche in Adobe Workfront Fusion
description: Nel pannello di mappatura di Adobe Workfront Fusion sono disponibili le seguenti funzioni matematiche.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# Funzioni matematiche in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL media ([array di valori]) media(valore1; [value2], ...)]

Restituisce il valore medio dei valori numerici in una matrice specifica o il valore medio dei valori numerici immessi singolarmente.

## [!UICONTROL ceil (number)]

Restituisce il numero intero più piccolo maggiore o uguale a un numero specificato.

>[!INFO]
>
>**Esempi:**
>
>* `ceil(` `1.2` `)`
>
>   Restituisce 2
>
>* `ceil(` `4` `)`
>
>   Restituisce 4

## [!UICONTROL floor (number)]

Restituisce il numero intero più grande minore o uguale a un numero specificato.

>[!INFO]
>
>**Esempi:**
>
>* `floor(` `1.2` `)`
>
>   Restituisce 1
>
>* `floor(` `1.9` `)`
>
>   Restituisce 1
>
>* `floor(` `4` `)`
>
>   Restituisce 4

## [!UICONTROL formatNumber (numero; decimalPOINTS; [decimalSeparator]; [migliaiaSeparatore])]

Restituisce un numero nel formato richiesto. Per impostazione predefinita, il punto decimale è una virgola (,) e il separatore delle migliaia è un punto (.).

>[!INFO]
>
>**Esempio:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Restituisce 123.456.789.000

## [!UICONTROL max ([array di valori]), max(valore1;valore2; ...)]

Restituisce il numero più grande in una matrice specificata o il numero più grande tra i numeri immessi singolarmente.

## [!UICONTROL min ([array di valori]), min(valore1; valore2; ...)]

Restituisce il numero più piccolo di una matrice specificata o il numero più piccolo tra i numeri immessi singolarmente.

## [!UICONTROL parseNumber (numero; separatore decimale)]

Analizza una stringa con un numero e restituisce il numero. Ad esempio, parseNumber(1 756,456;,)

## [!UICONTROL round (numero)]

Arrotonda un valore numerico al numero intero più vicino.

>[!INFO]
>
>**Esempi:**
>
>* `round(` `1.2` `)`
>
>   Restituisce 1
>
>* `round(` `1.5` `)`
>
>   Restituisce 2
>
>* `round(` `1.7` `)`
>
>   Restituisce 2
> 
>* `round(` `2` `)`
>
>   Restituisce 2

## [!UICONTROL sum ([array di valori]), sum(value1; value2; ...)]

Restituisce la somma dei valori in una matrice specificata o la somma dei numeri immessi singolarmente.
