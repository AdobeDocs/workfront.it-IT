---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare una scorecard
description: Una scorecard misura se un progetto è in linea con i criteri precedentemente stabiliti di un portfolio. Una scheda di valutazione spesso riflette la missione, i valori e gli obiettivi strategici di un'organizzazione.I responsabili di Portfolio solitamente definiscono le domande e le risposte della scorecard per assicurarsi che siano significative e preziose durante la definizione delle priorità e la selezione del progetto. Un [!DNL Adobe Workfront] L’amministratore crea le scorecard in base alle raccomandazioni dei gestori di portfolio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Creare una scorecard

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Una scorecard misura se un progetto è in linea con i criteri precedentemente stabiliti di un portfolio. Una scheda di valutazione spesso riflette la missione, i valori e gli obiettivi strategici di un&#39;organizzazione.

I manager di Portfolio definiscono di solito le domande e le risposte della scorecard per assicurarsi che siano significative e preziose durante la definizione delle priorità e la selezione del progetto. Un [!DNL Adobe Workfront] L’amministratore crea le scorecard in base alle raccomandazioni dei gestori di portfolio.

Le domande e le risposte scelte per una scheda di valutazione devono essere quantificabili al fine di fornire un valore di allineamento per confrontare progetti diversi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>[!UICONTROL Business] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
 </tbody> 
</table>

## Creare una scorecard

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Scorecard]**, quindi fai clic su **[!UICONTROL Nuova scorecard]** per creare una nuova scorecard e avviare il generatore di scorecard.

1. Specifica una **[!UICONTROL Nome della scorecard]** e **[!UICONTROL Descrizione]**.

   Il nome viene visualizzato quando si associa la scorecard al progetto. La descrizione viene visualizzata accanto al nome della scorecard nell’elenco della scorecard.

1. Fai clic sul pulsante **[!UICONTROL Aggiungi domanda]** menu a discesa per aprire [!UICONTROL domanda scorecard] , quindi specifica le seguenti informazioni per la domanda:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domanda]</td> 
      <td>Digita la domanda da includere nella scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Digita i punti massimi possibili per questa domanda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Punti negativi]</td> 
      <td>Seleziona questa opzione per indicare che [!DNL Workfront] devono sottrarre dal totale dei punti possibili. Non è possibile aggiungere punteggi negativi ai punti massimi possibili di una scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Seleziona <strong>[!UICONTROL Value(0-100)]</strong> se desideri visualizzare un campo numerico nella scorecard dove gli utenti possono specificare un valore compreso tra 0 e 100.<p>Oppure, seleziona <strong>Menu a discesa [!UICONTROL]</strong> o <strong>[!UICONTROL Pulsanti di scelta]</strong> per creare una risposta che gli utenti possono specificare utilizzando tale controllo. Fai clic su <strong>[!UICONTROL Aggiungi risposta]</strong>, quindi digita il <strong>[!UICONTROL Value]</strong> in punti percentuali per la risposta, qualora sia soddisfatta. Se scegli 100%, il numero di punti assegnati per questa domanda è pienamente raggiunto. Se si desidera indicare che questa risposta contiene solo una parte della quantità totale di punti assegnati a questa domanda, selezionare un valore percentuale inferiore. Ad esempio, se la domanda viene valutata a 10 punti e desideri che questa risposta contenga 5 di questi punti, scegli 50% per il tuo valore.</p>
      <p>Seleziona <strong>[!UICONTROL Predefinito]</strong> per indicare che questa è la risposta predefinita.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Aggiungi domanda]** per aggiungere ulteriori domande e risposte alla scorecard, seguendo gli stessi passaggi.

   >[!NOTE]
   >
   >Puoi riordinare le domande nella scorecard trascinando e rilasciando le domande nell’ordine corretto.

1. Fai clic su **[!UICONTROL Salva]** al termine dell’immissione dei dati.

## Applicare una scorecard a un progetto

Un utente con [!UICONTROL gestire] le autorizzazioni per un progetto possono applicare una scorecard a un progetto, dopo che la scorecard è stata creata da [!DNL Workfront] amministratore.

Una scorecard viene aggiunta a un progetto come parte della creazione di un business case per il progetto. Per ulteriori informazioni sull’aggiunta di una scorecard a un progetto, consulta [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Per ulteriori informazioni sulla creazione di scorecard, consulta [Creare una scorecard](#create-a-scorecard).

Per ulteriori informazioni sulle autorizzazioni del progetto, consulta [Condividi un progetto in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
