---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]
description: Il tuo [!DNL Adobe Workfront Fusion] Gli scenari possono contenere i tipi di elementi elencati di seguito in un bundle.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '708'
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

## Tipi di dati degli elementi

Puoi contenere in un bundle i tipi di elementi elencati di seguito.

Per informazioni sui tipi di elementi [!DNL Workfront Fusion] consente la conversione tra di loro, vedi [Tipo di coercizione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Testo</p> </td> 
   <td> <p>Il tipo di elemento più comune. Per alcuni elementi di testo, [!DNL Adobe Workfront Fusion] controlla se la lunghezza massima o minima consentita è rispettata o se l'elemento esegue la convalida del formato (e-mail, URL o nome file).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Numero</p> </td> 
   <td> <p>Per alcuni elementi numerici, [!DNL Workfront Fusion] può convalidare l’input per un intervallo specificato (il valore minimo o massimo consentito).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booleano (sì/no)</p> </td> 
   <td> <p>Questo tipo viene utilizzato per gli elementi con solo due valori possibili: true o false. </p> <p>Quando si impostano i moduli, il tipo booleano può apparire in due forme diverse:</p> 
    <ul> 
     <li> <p>La casella di controllo obbligatoria viene visualizzata se il campo è obbligatorio e deve essere compilato.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>I campi facoltativi che possono essere lasciati vuoti vengono visualizzati come una casella di selezione che consente di selezionare tre valori: <code>Yes</code>, <code>No</code>, e <code>Not defined</code> (impostazione predefinita).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Puoi fare clic su <strong>[!UICONTROL Map]</strong> se devi mappare il valore su un elemento da un altro modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Data</p> </td> 
   <td> <p>Le date vengono immesse nel formato data ISO 8601, ad esempio <code>2015-09-18T11:58Z</code>. È possibile modificare il fuso orario nelle impostazioni del profilo, come spiegato in <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modificare le impostazioni del profilo in [!DNL Adobe Workfront Fusion]</a>. </p> <p>Se fai clic su un campo che richiede una data, nelle impostazioni del modulo viene visualizzato un calendario a comparsa. L'ora non è richiesta per alcuni elementi.</p> <p>I valori degli elementi Data vengono formattati utilizzando il fuso orario locale e Web selezionato nel profilo. Puoi visualizzare la versione ISO 8601 del valore di un elemento data passando il cursore sopra l’elemento.</p> <p>Nota: se il valore ISO non viene visualizzato, l’elemento è probabilmente un testo, non una data.</p> <p>L’ora viene immessa nel <code>hours:minutes:seconds</code> ad esempio,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (dati binari)</p> </td> 
   <td> <p>Il contenuto del file viene in genere inviato come contenuto di tipo buffer (contenuto immagine, file video e altri). In alcuni casi, i dati di testo sono inclusi in questo tipo (ad esempio, un file di testo). [!DNL Workfront Fusion] è in grado di convertire automaticamente dati di testo nel codice binario in testo e testo in dati di testo nel codice binario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Informazioni sulla mappatura dei file in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Raccolta</p> </td> 
   <td> <p>Una raccolta è un elemento costituito da più elementi secondari. L'elemento Sender in un messaggio e-mail è un esempio di raccolta: contiene il nome del mittente (tipo di testo) e l'indirizzo e-mail del mittente (tipo di testo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Seleziona (menu)</p> </td> 
   <td> <p>Quando configuri le impostazioni del modulo come descritto in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configurare le impostazioni di un modulo in [!DNL Adobe Workfront Fusion]</a>, è possibile selezionare tra più elementi dello stesso tipo. Un esempio è il menu di selezione delle cartelle nelle impostazioni per [!DNL Dropbox] moduli. </p> <p>Quando si impostano i moduli, il menu di selezione può essere visualizzato in due forme:</p> <p> <p>Se è possibile selezionare più elementi, vengono visualizzati diversi elementi con caselle di controllo.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Se è disponibile una sola opzione, viene visualizzato un menu a discesa.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Se devi mappare un elemento da un altro modulo, utilizza <strong>Mappa</strong> pulsante. Questo pulsante consente di aprire un campo di testo anziché il menu di selezione. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>Puoi utilizzare il tipo di array per lavorare con diversi valori dello stesso tipo, incluse le raccolte. Un esempio è rappresentato dai moduli [!UICONTROL E-mail]: restituiscono una matrice di allegati e ogni allegato contiene nome, contenuto, dimensione e così via. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mappare un array in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Convalida</p> </td> 
   <td> <p>[!DNL Workfront Fusion] potrebbe eseguire la convalida per ogni tipo di elemento. Se un elemento non supera la convalida, l’elaborazione del modulo verrà interrotta a causa di un errore di dati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Errore di elaborazione in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
