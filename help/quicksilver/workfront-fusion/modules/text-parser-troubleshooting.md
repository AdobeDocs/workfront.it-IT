---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Risoluzione dei problemi del parser di testo in [!DNL Adobe Workfront Fusion]
description: Utilizzare queste informazioni se non è possibile ottenere il parser di testo per produrre alcun output.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Risoluzione dei problemi del parser di testo in [!DNL Adobe Workfront Fusion]

Utilizza queste informazioni se non riesci a ottenere un parser di testo per produrre alcun output.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Risoluzione dei problemi

Esempio di caso, si desidera analizzare il tipo di file di un documento di file &quot;filename.docx&quot; e l’estensione del nome del file varia sempre da DOCX a PDF a CSV.

L&#39;espressione che è possibile scegliere di utilizzare in questo caso è [!DNL \..+]

Se doveste utilizzare questo su espressione regex su regex101.com otterrete una corrispondenza completa.

![](assets/regex-expression-350x130.png)

Sull&#39;immagine precedente, l&#39;estensione del file era corretta. Se si prende questo e si tenta di implementarlo nel parser di testo:

![](assets/text-parser-350x602.png)

non otterrete una corrispondenza:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

Il motivo è che il &quot;i&quot; mostra solo il numero di corrispondenze per corrispondenza, quindi in questo caso abbiamo 2 corrispondenze, quindi dopo il &quot;i&quot; c&#39;è un valore numerico 1 e 2. In questo caso, se devi far corrispondere o trasmettere dati attraverso un filtro solo il secondo valore corrispondente, puoi specificare quale valore è rappresentato dal valore numerico.

![](assets/text-parser-matches-350x355.png)

Per ottenere i valori di corrispondenza necessari per aggiungere parentesi alla parte che si desidera analizzare (ad esempio, per estrarre da &quot;filename.docx&quot; - solo &quot;docx&quot;), quindi, in base all&#39;espressione regex che utilizziamo per questo scenario di caso, le parentesi devono essere applicate su \.(.+)

Questo acquisisce il DOCX, lo inserisce in un gruppo e lascia il &quot;&quot;. fuori.

![](assets/text-parser-get-matches-350x592.png)

Nell&#39;output mostrato nell&#39;immagine seguente, il gruppo di acquisizione corrisponderà a qualsiasi carattere (ad eccezione dei terminatori di riga).

![](assets/text-parser-output-350x389.png)

Un&#39;altra soluzione che incorpora anche regex sta utilizzando la funzione di sostituzione

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Quindi sostituisci `abcdefghijklmno pqr stuvw xyz.docx` con la variabile del nome del file effettivo.
