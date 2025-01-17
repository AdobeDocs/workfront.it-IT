---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funzioni matematiche in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 1%

---

# Funzioni matematiche in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Funzioni matematiche](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-functions.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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

## [!UICONTROL media ([matrice di valori]) media(valore1; [valore2], ...)]

Restituisce il valore medio dei valori numerici in una matrice specifica o il valore medio dei valori numerici immessi singolarmente.

## [!UICONTROL ceil (numero)]

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

## [!UICONTROL piano (numero)]

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

## [!UICONTROL max ([matrice di valori]), max(valore1;valore2; ...)]

Restituisce il numero più grande in una matrice specificata o il numero più grande tra i numeri immessi singolarmente.

## [!UICONTROL min ([matrice di valori]), min(valore1; valore2; ...)]

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

## [!UICONTROL somma ([matrice di valori]), somma(valore1; valore2; ...)]

Restituisce la somma dei valori in una matrice specificata o la somma dei numeri immessi singolarmente.

## [!UICONTROL parseNumber (numero; separatore decimale)]

Analizza una stringa con un numero e restituisce il numero. Ad esempio, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (numero; separatore decimale; [separatore decimale]; [migliaiaSeparatore])]

Restituisce un numero nel formato richiesto. Per impostazione predefinita, il punto decimale è una virgola (,) e il separatore delle migliaia è un punto (.).

>[!INFO]
>
>**Esempio:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Restituisce 123.456.789.000
