---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]
description: Le [!DNL Adobe Workfront Fusion] Gli scenari possono contenere i tipi di elementi elencati di seguito in un bundle.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]

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

## Tipi di dati elemento

Puoi contenere i tipi di elementi elencati di seguito in un bundle.

Per informazioni su quali tipi di elementi [!DNL Workfront Fusion] consente la conversione tra gli altri, vedi [Tipo di coercizione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Testo</p> </td> 
   <td> <p>Il tipo di elemento più comune. Per alcuni elementi di testo, [!DNL Adobe Workfront Fusion] controlla se la lunghezza massima o minima consentita è soddisfatta o se l’elemento esegue la convalida del formato (e-mail, URL o nome del file).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Numero</p> </td> 
   <td> <p>Per alcuni elementi numerici, [!DNL Workfront Fusion] può convalidare l’input per un intervallo specificato (il valore minimo o massimo consentito).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booleano (Sì/No)</p> </td> 
   <td> <p>Questo tipo viene utilizzato per gli elementi con solo due possibili valori: true o false. </p> <p>Quando si impostano i moduli, il tipo booleano può essere visualizzato in due moduli diversi:</p> 
    <ul> 
     <li> <p>La casella di controllo obbligatoria è visualizzata nel caso in cui il campo sia obbligatorio e deve essere compilato.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>I campi facoltativi che possono essere lasciati vuoti vengono visualizzati come una casella di selezione, consentendo la selezione tra tre valori: <code>Yes</code>, <code>No</code>e <code>Not defined</code> (predefinito).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Puoi fare clic su <strong>[!UICONTROL Map]</strong> se devi mappare il valore a un elemento da un altro modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Data</p> </td> 
   <td> <p>Le date vengono immesse nel formato di data ISO 8601, ad esempio: <code>2015-09-18T11:58Z</code>. Puoi modificare il fuso orario nelle impostazioni del profilo, come spiegato in <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modifica le impostazioni del profilo in [!DNL Adobe Workfront Fusion]</a>. </p> <p>Se si fa clic su un campo che richiede una data, nelle impostazioni del modulo viene visualizzato un calendario a comparsa. Il tempo non è necessario per alcuni elementi.</p> <p>I valori degli elementi Data vengono formattati utilizzando il fuso orario locale e Web selezionato nel profilo. Per visualizzare la versione ISO 8601 del valore di un elemento data, posiziona il puntatore del mouse sopra l’elemento.</p> <p>Nota: Se il valore ISO non viene visualizzato, l'elemento è probabilmente testo, non una data.</p> <p>L’ora viene immessa nel <code>hours:minutes:seconds</code> formato, ad esempio,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (dati binari)</p> </td> 
   <td> <p>Il contenuto del file viene in genere inviato come contenuto di tipo buffer (contenuto immagine, file video e altri). In alcuni casi, i dati di testo sono inclusi in questo tipo (ad esempio, un file di testo). [!DNL Workfront Fusion] è in grado di convertire automaticamente i dati di testo nel codice binario in testo e testo in dati di testo nel codice binario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Informazioni sulla mappatura di file in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Raccolta</p> </td> 
   <td> <p>Una raccolta è un elemento costituito da più elementi secondari. L’elemento Mittente in un messaggio e-mail è un esempio di raccolta: contiene il nome del mittente (tipo di testo) e l’indirizzo e-mail del mittente (tipo di testo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Seleziona (menu)</p> </td> 
   <td> <p>Quando configuri le impostazioni del modulo come descritto in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configura le impostazioni di un modulo in [!DNL Adobe Workfront Fusion]</a>, puoi selezionare diversi elementi dello stesso tipo. Un esempio è il menu di selezione della cartella nelle impostazioni per [!DNL Dropbox] moduli. </p> <p>Quando si impostano i moduli, il menu di selezione può essere visualizzato in due moduli:</p> <p> <p>Se è possibile selezionare più elementi, vengono visualizzati diversi elementi con le caselle di controllo.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Se è possibile utilizzare una sola opzione, viene visualizzato un menu a discesa.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Se hai bisogno di mappare un elemento da un altro modulo, utilizza il <strong>Mappa</strong> pulsante . Questo pulsante apre un campo di testo invece del menu di selezione. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>È possibile utilizzare il tipo di matrice per lavorare con più valori dello stesso tipo, incluse le raccolte. Un esempio sono i moduli [!UICONTROL Email]: restituiscono una matrice di allegati e ogni allegato contiene nome, contenuto, dimensioni e così via. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mappare un array in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Convalida</p> </td> 
   <td> <p>[!DNL Workfront Fusion] potrebbe eseguire la convalida per ogni tipo di elemento. Se un elemento non supera la convalida, il modulo interromperà l’elaborazione a causa di un errore di dati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Errore di elaborazione in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
