---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Risoluzione dei problemi relativi al parser di testo in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Risoluzione dei problemi relativi al parser di testo in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Parser di testo](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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

## Risoluzione dei problemi

Ad esempio, si desidera analizzare il tipo di file di un documento &quot;filename.docx&quot; e l&#39;estensione del nome file varia sempre da DOCX a PDF a CSV.

L&#39;espressione che si può scegliere di utilizzare in questo caso è [!DNL \..+]

Se dovessi utilizzarlo su un’espressione regex su regex101.com otterrai una corrispondenza completa.

![](assets/regex-expression-350x130.png)

Nell’immagine precedente, l’estensione del file corrispondeva correttamente. Se prendi questo e tenti di implementarlo nel parser di testo:

![](assets/text-parser-350x602.png)

non riceverai un risultato:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

Il motivo è che la &quot;i&quot; mostra solo il numero di corrispondenze per partita, quindi in questo caso abbiamo 2 corrispondenze, quindi dopo la &quot;i&quot; c&#39;è un valore numerico 1 e 2. Il caso d’uso prevede che, se dovesse essere necessario far corrispondere o trasmettere dati attraverso un filtro, solo il secondo valore corrispondente sia possibile specificare quale valore è rappresentato dal valore numerico.

![](assets/text-parser-matches-350x355.png)

Per ottenere i valori di corrispondenza necessari per aggiungere parentesi alla parte che si desidera analizzare, ad esempio per estrarre da &quot;filename.docx&quot; - solo &quot;docx&quot;, in base all&#39;espressione regex utilizzata per questo scenario, le parentesi devono essere applicate a \.(.+)

Questo acquisisce il DOCX, lo inserisce in un gruppo e lascia il &quot;.&quot; fuori di esso.

![](assets/text-parser-get-matches-350x592.png)

Nell&#39;output mostrato nell&#39;immagine seguente, il gruppo di cattura corrisponderà a qualsiasi carattere (ad eccezione dei terminatori di riga).

![](assets/text-parser-output-350x389.png)

Un’altra soluzione alternativa che incorpora anche regex è l’utilizzo della funzione replace

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Quindi sostituisci `abcdefghijklmno pqr stuvw xyz.docx` con la tua effettiva variabile di nome file.
