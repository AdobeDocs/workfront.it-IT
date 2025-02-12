---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Creare un portfolio
description: Un Portfolio è una raccolta di progetti in competizione per le stesse risorse, budget e pianificazione. I progetti in un Portfolio sono abbastanza simili da utilizzare lo stesso Pool di Risorse e venire misurati sulla stessa scorecard.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---

# Creare un portfolio

<!--Audited: 7/2024-->

Un Portfolio è una raccolta di progetti in competizione per le stesse risorse, budget e pianificazione. I progetti in un Portfolio sono abbastanza simili da utilizzare lo stesso Pool di Risorse e venire misurati sulla stessa scorecard.

È possibile utilizzare i portafogli per raggruppare progetti appartenenti alle stesse linee di prodotti, divisioni, reparti, società o altre unità aziendali.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p>
   <p>Corrente:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di [!UICONTROL Edit] ai portfolio</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Dopo aver creato un portfolio, per impostazione predefinita disponi delle autorizzazioni di gestione</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modi per creare i portfolio

Puoi creare un portfolio in Workfront utilizzando uno dei seguenti metodi:

* Crea un portfolio da zero a partire dall’area Portfolio del menu principale. Questo articolo descrive come creare un portfolio da zero.

* Importa un portfolio utilizzando le funzioni di avvio.

  In qualità di amministratore di Workfront, puoi importare i portfolio con una procedura di avvio.

  Per informazioni sull&#39;importazione di dati tramite Kick-Start in Workfront, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Aggiungere i portfolio quando vengono collegati da un tipo di record in Workfront Planning.

  È necessario disporre di una nuova licenza Workfront e di una licenza Workfront Planning aggiuntiva per Workfront Planning.

  Per informazioni sull&#39;accesso a Workfront Planning, vedere [Panoramica dell&#39;accesso](/help/quicksilver/planning/access/access-overview.md).

  Per informazioni sulla creazione di portafogli tramite l&#39;aggiunta di tali portafogli ai record, vedere la sezione &quot;Creare record durante la connessione&quot; nell&#39;articolo [Creare record](/help/quicksilver/planning/records/create-records.md).


## Creare un portfolio

{{step1-click-main-menu}}

1. Fai clic su **[!UICONTROL Portfolio]**.
1. Fare clic su **[!UICONTROL Nuovo Portfolio]**.
1. Sostituisci **[!UICONTROL Portfolio senza titolo]** con il nome desiderato per il portfolio.

   Il nome può contenere fino a 255 caratteri.

1. (Facoltativo) Fai clic sul nome in **[!UICONTROL Portfolio Manager]** nell&#39;intestazione nella parte superiore della pagina per assegnare un manager diverso per il portfolio.

   ![Nome manager Portfolio](assets/portfolio-manager-name-350x51.jpg)

   In qualità di creatore del portfolio, per impostazione predefinita ti viene assegnato il ruolo di gestore del portfolio.

1. Fai clic su **[!UICONTROL Dettagli Portfolio]** nel pannello a sinistra.
1. Nell&#39;area **[!UICONTROL Panoramica]**, modificare una delle seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td> <p>Digita una descrizione per Portfolio per indicare cosa c’è di univoco. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Inizia a digitare il nome di un utente che desideri indicare come gestore del portfolio, quindi selezionalo quando viene visualizzato nell’elenco. È lo stesso del [!UICONTROL Portfolio Owner]. Questa è la persona che può supervisionare il lavoro definito nei progetti del portfolio e può approvare il Business Case.</p> <p>Importante: quando si designa un utente come [!UICONTROL Portfolio Manager], questi ottiene automaticamente le autorizzazioni [!UICONTROL Manage] per il portfolio, i programmi e i progetti in esso contenuti. </p> <p>Suggerimento: è inoltre possibile aggiornare [!UICONTROL Portfolio Manager] nell'intestazione nella parte superiore della pagina.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Gruppo </td> 
      <td> <p>Aggiungi il nome di un singolo gruppo se il gruppo possiede il portfolio o ha la responsabilità di completarlo. </p> <p>Per assicurarsi di selezionare il gruppo corretto, posizionare il puntatore del mouse su di esso e fare clic sull'icona [!UICONTROL information] <img src="assets/info-icon.png"> visualizzata accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic nella casella **[!UICONTROL Aggiungi modulo personalizzato]** nell&#39;angolo superiore destro della pagina [!UICONTROL Dettagli Portfolio] per selezionare un modulo personalizzato per il portfolio e aggiornare i campi personalizzati.

   >[!TIP]
   >
   >Per allegare i moduli personalizzati del portfolio è necessario averli già creati.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
1. (Facoltativo) Fai clic su **[!UICONTROL Programmi]** nel pannello a sinistra, quindi su **[!UICONTROL Aggiungi programmi]** per aggiungere programmi al portfolio.

   Per ulteriori informazioni sulla creazione di programmi, vedere [Creare un programma](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Facoltativo) Fai clic su **[!UICONTROL Progetti]** nel pannello a sinistra, quindi su **[!UICONTROL Aggiungi progetti]** per aggiungere progetti al portfolio.

   Per ulteriori informazioni sull&#39;aggiunta di progetti a un Portfolio, vedere [Aggiungere progetti a un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
