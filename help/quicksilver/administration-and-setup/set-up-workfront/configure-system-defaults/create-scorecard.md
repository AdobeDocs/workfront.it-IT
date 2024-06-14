---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare una scorecard
description: Una scorecard misura il grado di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.I responsabili di Portfolio solitamente definiscono le domande e le risposte della scorecard per garantire che siano significative e utili durante la definizione delle priorità e la selezione del progetto. Un [!DNL Adobe Workfront] L’amministratore crea le scorecard in base ai consigli dei gestori di portfolio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Creare una scorecard

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Una scorecard misura il grado di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.

I responsabili di Portfolio solitamente definiscono le domande e le risposte delle scorecard per garantire che siano significative e utili durante la definizione delle priorità e la selezione dei progetti. Un [!DNL Adobe Workfront] L’amministratore crea le scorecard in base ai consigli dei gestori di portfolio.

Le domande e le risposte scelte per una scorecard devono essere quantificabili in modo da fornire un valore di allineamento per confrontare progetti diversi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Corrente: [!UICONTROL Business] o versione successiva</p> 
   Oppure
   <p>Nuovo: [!UICONTROL Prime] o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td><p>Corrente: [!UICONTROL Plan]</p>
   Oppure
   <p>Nuovo: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

+++

## Creare una scorecard

{{step-1-to-setup}}

1. Clic **[!UICONTROL Scorecard]**, quindi fai clic su **[!UICONTROL Nuova scorecard]** per avviare il generatore di scorecard e crearne una.

1. Specifica un **[!UICONTROL Nome Scorecard]** e un **[!UICONTROL Descrizione]**.

   Il nome viene visualizzato quando si associa la scorecard al progetto. La descrizione viene visualizzata accanto al nome della scorecard nell’elenco delle scorecard.

1. Fai clic su **[!UICONTROL Aggiungi domanda]** menu a discesa per aprire [!UICONTROL domanda scorecard] , quindi specificare le seguenti informazioni per la domanda:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domanda]</td> 
      <td>Digitare la domanda da includere nella scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Punti]</td> 
      <td>Digitare il numero massimo di punti possibile per questa domanda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL punti negativi]</td> 
      <td>Selezionare questa opzione per indicare che [!DNL Workfront] devono sottrarre dal totale i punti possibili. Non è possibile aggiungere punteggi negativi al numero massimo di punti possibile di una scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di visualizzazione [!UICONTROL]</td> 
      <td>Seleziona <strong>[!UICONTROL Valore(0-100)]</strong> se desideri visualizzare un campo numerico nella scorecard in cui gli utenti possono specificare un valore compreso tra 0 e 100.<p>Oppure, seleziona <strong>[!UICONTROL A Discesa]</strong> o <strong>[!UICONTROL Pulsanti Di Scelta]</strong> per creare una risposta, gli utenti possono specificare utilizzando tale controllo. Clic <strong>[!UICONTROL Aggiungi risposta]</strong>, quindi digita il <strong>Valore [!UICONTROL]</strong> in punti percentuali per la risposta, nel caso in cui sia soddisfatta. Se si sceglie 100%, il numero di punti assegnati per questa domanda viene raggiunto completamente. Se si desidera indicare che la risposta contiene solo una parte del totale di punti assegnati a questa domanda, selezionare un valore percentuale inferiore. Ad esempio, se la domanda è valutata a 10 punti e si desidera che la risposta contenga 5 di tali punti, scegliere 50% per il valore.</p>
      <p>Seleziona <strong>[!UICONTROL predefinito]</strong> se si desidera indicare che questa risposta è quella predefinita.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Aggiungi domanda]** per aggiungere ulteriori domande e risposte alla scorecard, seguendo gli stessi passaggi.

   >[!NOTE]
   >
   >Puoi riordinare le domande nella scorecard trascinandole nell’ordine corretto.

1. Clic **[!UICONTROL Salva]** dopo aver immesso tutte le informazioni.

   In questo modo, la scorecard viene creata e i project manager possono collegarla al proprio caso aziendale di progetto.

## Applicare una scorecard a un progetto

Un utente con [!UICONTROL gestire] le autorizzazioni di un progetto possono applicare una scorecard a un progetto, dopo che questa è stata creata da [!DNL Workfront] amministratore.

Una scorecard viene aggiunta a un progetto nell’ambito della creazione di un business case per il progetto. Per ulteriori informazioni sull’aggiunta di una scorecard a un progetto, consulta [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Per ulteriori informazioni sulle autorizzazioni per i progetti, consulta [Condividere un progetto in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
