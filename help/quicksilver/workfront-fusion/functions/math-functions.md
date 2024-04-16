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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Funzioni matematiche in [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

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
   <p>Corrente: No [!DNL Workfront Fusion] requisito di licenza.</p> 
   <p>Oppure</p> 
   <p>Legacy: qualsiasi </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Prodotto</td>  
   <td> 
   <p>Nuovo:</p> <ul><li>[!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront] Piano: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Piano: [!DNL Workfront Fusion] è incluso.</li></ul> 
   <p>Oppure</p> 
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## [!UICONTROL max ([array di valori]), max(valore1;valore2; ...)]

Restituisce il numero più grande in una matrice specificata o il numero più grande tra i numeri immessi singolarmente.

## [!UICONTROL min ([array di valori]), min(valore1; valore2; ...)]

Restituisce il numero più piccolo di una matrice specificata o il numero più piccolo tra i numeri immessi singolarmente.

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

## [!UICONTROL parseNumber (numero; separatore decimale)]

Analizza una stringa con un numero e restituisce il numero. Ad esempio, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (numero; decimalPOINTS; [decimalSeparator]; [migliaiaSeparatore])]

Restituisce un numero nel formato richiesto. Per impostazione predefinita, il punto decimale è una virgola (,) e il separatore delle migliaia è un punto (.).

>[!INFO]
>
>**Esempio:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Restituisce 123.456.789.000
