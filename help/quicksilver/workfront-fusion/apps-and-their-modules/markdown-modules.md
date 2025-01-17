---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Markdown
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 9e810302-4897-494a-9b50-667d87ce9cb7
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# [!UICONTROL Moduli Markdown]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli Markdown](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/markdown-modules.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In uno scenario [!DNL Adobe Workfront Fusion], è possibile utilizzare i moduli [!UICONTROL Markdown] per convertire Markdown in HTML e HTML in Markdown.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
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

## [!UICONTROL Markdown a HTML]

Questo modulo converte Markdown in HTML.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Immetti il testo normale formattato per Markdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>Abilita questa opzione per convertire GitHub Flavored Markdown in HTML.</p> <p>Per ulteriori informazioni, vedere la scheda di riferimento del Mar[!DNL ] nella documentazione di [!DNL GitHub].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sanitize]</td> 
   <td>Selezionare un'opzione per indicare se si desidera rimuovere i tag HTML dal testo o dal HTML escape.</td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL HTML a Markdown]

Questo modulo converte il codice HTML in Markdown.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Immetti il codice HTML da convertire in Markdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>Abilitare questa opzione per convertire il HTML in [!DNL GitHub Flavored Markdown].</p> <p>Per ulteriori informazioni, vedere la scheda di riferimento Markdown nella documentazione di [!DNL GitHub].</p> </td> 
  </tr> 
 </tbody> 
</table>
