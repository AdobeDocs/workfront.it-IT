---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare una scorecard
description: Una scorecard misura il grado di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un'organizzazione.I responsabili di Portfolio solitamente definiscono le domande e le risposte della scorecard per garantire che siano significative e utili durante la definizione delle priorità e la selezione del progetto. Un amministratore  [!DNL Adobe Workfront]  crea le scorecard in base ai consigli dei gestori di portfolio.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 1%

---

# Creare una scorecard

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Una scorecard misura il grado di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.

In qualità di gestore di portfolio, puoi definire le domande e le risposte delle scorecard per garantirne il significato e il valore durante la definizione delle priorità e la selezione dei progetti.

In qualità di amministratore [!DNL Adobe Workfront], puoi creare scorecard in base ai consigli dei gestori di portfolio.

Le domande e le risposte scelte per una scorecard devono essere quantificabili in modo da fornire un valore di allineamento per confrontare progetti diversi.

Puoi creare una scorecard nel modo seguente:

* Da zero
* Copiandone uno esistente

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Nuovo: [!UICONTROL Prime] o versione successiva</p>
   <p>Corrente: [!UICONTROL Business] o versione successiva</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una scorecard da zero

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Scorecard]**, quindi su **[!UICONTROL Nuova scorecard]**.

   Viene visualizzata la casella **Nuova scorecard**.

   ![Nuova casella scorecard](assets/new-scorecard-350x173.png)

1. Specifica un nome **[!UICONTROL scorecard]** e una **[!UICONTROL descrizione]**.

   Il nome viene visualizzato quando si associa la scorecard al progetto. La descrizione viene visualizzata accanto al nome della scorecard nell’elenco delle scorecard.

1. Fai clic sul menu a discesa **[!UICONTROL Aggiungi domanda]** per aprire la sezione [!UICONTROL domanda scorecard], quindi specifica le seguenti informazioni per la domanda:

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
      <td>Selezionare questa opzione per indicare che [!DNL Workfront] deve sottrarre dal totale dei punti possibili. Non è possibile aggiungere punteggi negativi al numero massimo di punti possibile di una scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di visualizzazione [!UICONTROL]</td> 
      <td>Selezionare <strong>[!UICONTROL Value(0-100)]</strong> per visualizzare un campo numerico nella scorecard in cui gli utenti possono specificare un valore compreso tra 0 e 100.<p>In alternativa, selezionare <strong>[!UICONTROL elenco a discesa]</strong> o <strong>[!UICONTROL pulsanti di scelta]</strong> per creare una risposta che gli utenti possono specificare utilizzando tale controllo. Fare clic su <strong>[!UICONTROL Add Answer]</strong>, quindi digitare il <strong>[!UICONTROL Value]</strong> in punti percentuali per questa risposta, nel caso che sia soddisfatta. Se si sceglie 100%, il numero di punti assegnati per questa domanda viene raggiunto completamente. Se si desidera indicare che la risposta contiene solo una parte del totale di punti assegnati a questa domanda, selezionare un valore percentuale inferiore. Ad esempio, se la domanda è valutata a 10 punti e si desidera che la risposta contenga 5 di tali punti, scegliere 50% per il valore.</p>
      <p>Selezionare <strong>[!UICONTROL Predefinito]</strong> se si desidera indicare che questa risposta è quella predefinita.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Aggiungi domanda]** per aggiungere altre domande e risposte alla scorecard, seguendo gli stessi passaggi.

   >[!NOTE]
   >
   >Puoi riordinare le domande nella scorecard trascinandole nell’ordine corretto.

1. Fai clic su **[!UICONTROL Salva]**.

   In questo modo viene creata la scorecard e i project manager possono collegarla al proprio caso aziendale di progetto.

## Copiare una scorecard esistente

Puoi creare una scorecard copiandone e modificandone una esistente.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Scorecard]** nel pannello a sinistra.
1. Seleziona una scorecard nell&#39;elenco, quindi fai clic sull&#39;icona **Copia** ![Copia scorecard](assets/copy-scorecard-icon.png) nella parte superiore dell&#39;elenco delle scorecard.

   Viene visualizzata la casella **Copia scorecard**.

   ![Copia casella scorecard](assets/copy-scorecard-box.png)

1. Specifica le seguenti informazioni:

   * **Scorecard**: aggiorna il nome della scorecard.  Per impostazione predefinita, il nome viene aggiornato automaticamente in base al seguente formato:

     `Original scorecard name (Copy)`
   * **Descrizione**: digitare ulteriori informazioni sulla scorecard.
1. Fai clic su **Salva**.

   In questo modo viene creata una nuova scorecard con le stesse informazioni di quella originale. Ora i project manager possono allegarlo al proprio caso aziendale di progetto.

## Applicare una scorecard a un progetto

Un utente con autorizzazioni [!UICONTROL manage] per un progetto può applicare una scorecard a un progetto dopo che l&#39;amministratore [!DNL Workfront] ha creato la scorecard.

Una scorecard viene aggiunta a un progetto nell’ambito della creazione di un business case per il progetto. Per ulteriori informazioni sull&#39;aggiunta di una scorecard a un progetto, vedere [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Per ulteriori informazioni sulle autorizzazioni del progetto, vedere [Condividere un progetto in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


