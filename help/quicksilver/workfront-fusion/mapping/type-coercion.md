---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Coerenza del tipo in Adobe Workfront Fusion
description: Questo documento descrive come [!DNL Adobe Workfront Fusion] si comporta in situazioni in cui riceve valori nei formati dati previsti e imprevisti.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Tipo di coercizione in [!DNL Adobe Workfront Fusion]

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

### Tipo di coercizione

Questo documento descrive come [!DNL Adobe Workfront Fusion] si comporta in situazioni in cui riceve valori nei formati dati previsti e imprevisti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Previsto</th> 
   <th>Ricevuto</th> 
   <th> <p>Descrizione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>array </td> 
   <td>array </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>altro </td> 
   <td> <p>Se il valore ricevuto non è del tipo di matrice, [!DNL Workfront Fusion] crea un array e il primo (e l’unico) elemento sarà il valore ricevuto.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>booleano </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>numero </td> 
   <td> <p>Il valore viene convertito in logico Sì, anche se il valore è 0.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>text </td> 
   <td> <p>Se il valore è uguale a false o il valore è vuoto, viene convertito in No logico. In caso contrario, viene convertito in logico Sì.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>altro </td> 
   <td> <p>Il valore viene convertito in logico Sì ogni volta che il valore ricevuto esiste (non è nullo).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>Il valore viene consegnato invariato solo se la pagina di codice è come previsto. Se la pagina del codice è diversa, [!DNL Workfront Fusion] cercherà di convertire il valore ricevuto nella pagina di codice richiesta. Se questa conversione non è supportata, [!DNL Workfront Fusion] restituirà un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>booleano </td> 
   <td> <p>Il valore viene convertito in testo (true/false) e quindi in dati binari seguendo i passaggi indicati in precedenza per la conversione in testo.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
   <td> <p>Il valore viene convertito in testo ISO 8601 e quindi in dati binari seguendo i passaggi indicati per la conversione in testo.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>numero </td> 
   <td> <p>Il valore viene convertito in testo e quindi in dati binari seguendo i passaggi indicati in precedenza per la conversione in testo.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>Il valore viene convertito in dati binari e codificato come previsto. Se la codifica prevista non è specificata, verrà utilizzata la codifica utf8.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>raccolta </td> 
   <td>raccolta </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>raccolta </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] cercherà di convertire il testo in una data. Se la conversione non riesce, verrà restituito un errore di convalida. La data deve contenere giorno, mese e anno. La data può contenere il fuso orario e il fuso orario. Il fuso orario predefinito è basato sulle impostazioni. Esempi:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>numero </td> 
   <td>numero </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>numero </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] cercherà di convertire il testo in un numero. Se la conversione non riesce, verrà restituito un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>numero </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>Se l’array specificato supporta la conversione in testo, il valore viene convertito. In caso contrario, [!DNL Workfront Fusion] restituirà un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>booleano </td> 
   <td> <p>Il valore viene convertito in testo (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Se per i dati binari è specificata la codifica del testo, il valore verrà convertito in testo. In caso contrario, [!DNL Workfront Fusion] restituirà un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
   <td> <p>Il valore viene convertito in testo ISO 8601.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>numero </td> 
   <td> <p>Il valore viene convertito in testo.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>tempo </td> 
   <td>tempo </td> 
   <td> <p>Il valore viene consegnato invariato.</p> </td> 
  </tr> 
  <tr> 
   <td>tempo </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] cercherà di convertire il tempo in ore:minutes:formato secondi. Se la conversione non riesce, verrà restituito un errore di convalida.</p> </td> 
  </tr> 
  <tr> 
   <td>tempo </td> 
   <td>altro </td> 
   <td> <p>[!DNL Workfront Fusion] restituisce un errore di convalida.</p> </td> 
  </tr> 
 </tbody> 
</table>
