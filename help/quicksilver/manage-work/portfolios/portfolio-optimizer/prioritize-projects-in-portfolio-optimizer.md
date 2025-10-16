---
title: Assegnare la priorità ai progetti in Portfolio Optimizer
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Puoi assegnare la priorità ai progetti in Portfolio Optimizer per stabilire l’ordine in cui devono essere completati.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Assegna priorità ai progetti in [!UICONTROL Portfolio Optimizer]

Puoi assegnare la priorità ai progetti in [!UICONTROL Portfolio Optimizer] per stabilire l&#39;ordine in cui devono essere completati.

Quando si utilizza [!UICONTROL Portfolio Optimizer], tenere presente quanto segue:

* I progetti nella parte superiore di [!UICONTROL Portfolio Optimizer] sono considerati più importanti di quelli elencati nella parte inferiore. Per ottimizzare Portfolio, è necessario completare i progetti in base alla loro priorità in [!UICONTROL Portfolio Optimizer].
* La priorità dei progetti in [!UICONTROL Portfolio Optimizer] non è correlata al campo [!UICONTROL Priority] nella scheda [!UICONTROL Project Details] di un progetto.

  Il campo [!UICONTROL Priority] nella scheda [!UICONTROL Project Details] è un contrassegno visivo specificato manualmente per comprendere l&#39;importanza di un progetto.

* La priorità dei progetti in Portfolio Optimizer è visibile in [!DNL Resource Planner], se è abilitato. In [!DNL Resource Planner], i progetti ricevono le risorse in base all&#39;ordine della priorità [!UICONTROL Pianificazione risorse] e non a quello della priorità [!UICONTROL Portfolio].

  Per informazioni sull&#39;assegnazione delle priorità ai progetti nella [!UICONTROL Programmazione risorse], vedere l&#39;articolo [Assegnazione delle priorità ai progetti nella [!UICONTROL Programmazione risorse]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Per impostazione predefinita, nell&#39;area **[!UICONTROL Assegnazione priorità progetto]** di [!UICONTROL Portfolio Optimizer] i progetti vengono visualizzati nell&#39;ordine di [!UICONTROL Date inizio pianificate] e [!UICONTROL Valore netto].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td> 
   <td> <p>Workfront Prime o versione successiva</p>
      <p>Prime flusso di lavoro o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di [!UICONTROL Edit] ai progetti [!UICONTROL Portfolio] e </p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di [!UICONTROL Manage] per il portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso per la documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Modifica la priorità dei progetti in [!UICONTROL Portfolio Optimizer]

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **[!UICONTROL Portfolio]**.
1. (Facoltativo) Seleziona il filtro corretto nel menu a discesa **[!UICONTROL Filtro]**, per visualizzare l&#39;elenco corretto dei portfolio.
1. Fai clic sul nome di un portfolio per aprirlo.
1. Fai clic su **[!UICONTROL Ottimizzazione Portfolio]** nel pannello a sinistra.
1. Nell&#39;area [!UICONTROL ottimizzazione del progetto], modifica la priorità dei progetti trascinando i progetti in ordine di priorità e rilasciandoli nella posizione di visualizzazione desiderata.

   ![Ottimizzatore Portfolio con progetti](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Fare clic su **[!UICONTROL Imposta priorità]** nell&#39;area di ottimizzazione del progetto al termine della ridisposizione dei progetti. I progetti riceveranno un nuovo numero in base al nuovo ordine.

1. Fai clic su **[!UICONTROL Salva]** per salvare la priorità del nuovo progetto in [!UICONTROL Portfolio Optimizer]. La priorità è elencata come numero nella colonna numero **#**.

   >[!TIP]
   >
   >Ciò non modifica necessariamente l&#39;ordine dei progetti in [!UICONTROL Portfolio Optimizer], poiché l&#39;elenco dei progetti potrebbe essere ordinato in base a una colonna diversa da **#**. Fare clic sull&#39;intestazione di colonna **#** per ordinare l&#39;elenco in base alla priorità del progetto.

   È possibile visualizzare la priorità del progetto così come appare in [!UICONTROL Portfolio Optimizer] nella Programmazione delle risorse, abilitando l&#39;impostazione **[!UICONTROL Visualizza priorità Portfolio]** nella Programmazione delle risorse.

   Per informazioni sull&#39;assegnazione delle priorità ai progetti nella [!UICONTROL Programmazione risorse], vedere l&#39;articolo [Assegnazione delle priorità ai progetti nella [!UICONTROL Programmazione risorse]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
