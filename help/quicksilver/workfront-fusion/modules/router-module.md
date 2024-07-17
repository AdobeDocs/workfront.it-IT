---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo router in Adobe Workfront Fusion
description: Il modulo Router consente di diramare il flusso in più route ed elaborare i dati all'interno di ciascuna route in modo diverso. Una volta che un modulo Router riceve un bundle, lo inoltra a ogni route connessa nell'ordine in cui le route sono state collegate al modulo Router.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Modulo [!UICONTROL Router] in [!DNL Adobe Workfront Fusion]

Il modulo [!UICONTROL Router] ti consente di diramare il flusso in più route ed elaborare i dati all&#39;interno di ogni route in modo diverso. Quando un modulo [!UICONTROL Router] riceve un bundle, lo inoltra a ogni route connessa nell&#39;ordine in cui le route sono state collegate al modulo [!UICONTROL Router].

>[!NOTE]
>
>* Per verificare l&#39;ordine delle route, è possibile fare clic sull&#39;icona [!UICONTROL Allineamento automatico], che disporrà le route in base all&#39;ordine dall&#39;alto verso il basso.
>
>  Per modificare l&#39;ordine, rimuovere il modulo [!UICONTROL Router] e ricollegare le route nell&#39;ordine desiderato.
>
>* Le route vengono elaborate in sequenza, non in parallelo. Un bundle viene inviato alla route successiva solo dopo che è stato completamente elaborato dalla route precedente.
>



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

## Aggiunta di un modulo [!UICONTROL Router] a uno scenario

È possibile aggiungere un [!UICONTROL router] a uno scenario in uno dei modi seguenti:

* Se desideri connettere il modulo [!UICONTROL Router] dopo un modulo, fai clic sull&#39;handle destro del modulo, inizia a digitare **[!UICONTROL router]** per cercarlo, quindi scegli **[!UICONTROL Controllo flusso]** > **[!UICONTROL Router]** nell&#39;elenco dei moduli visualizzati.

  ![](assets/connect-the-router-350x108.png)

* Se si desidera inserire il modulo [!UICONTROL Router] tra due moduli, fare clic sull&#39;icona a forma di chiave inglese sotto la route che collega i due moduli (oppure fare clic con il pulsante destro del mouse sulla route) e scegliere **[!UICONTROL Aggiungi router]** dal menu.

  ![](assets/insert-router-350x191.png)

* È possibile inserire automaticamente un modulo [!UICONTROL Router]. Ad esempio, nell’immagine seguente, per collegare il modulo nell’angolo inferiore destro a quello nell’angolo superiore sinistro (che è già collegato a quello nell’angolo superiore destro), trascina la maniglia sinistra del modulo inferiore destro e rilascialo sul modulo superiore sinistro.

  ![](assets/insert-router-automatically-350x379.png)

## Filtri

È possibile inserire un filtro in una route dopo il modulo [!UICONTROL Router] per filtrare i bundle come in qualsiasi altra route:

1. Fare clic su uno dei punti del percorso.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Nella casella **[!UICONTROL Configura un filtro]** visualizzato, aggiungi le condizioni, quindi fai clic su **[!UICONTROL OK]** per salvare la configurazione del filtro.

   ![](assets/set-up-a-filter-2-350x242.png)

Per ulteriori informazioni, vedere [Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Route di fallback

La configurazione del filtro su una route dopo un modulo [!UICONTROL Router] contiene un&#39;opzione speciale: Route di fallback:

![](assets/fallback-route-350x260.png)

Se abilitata, questa route viene utilizzata nel caso in cui un bundle non possa continuare dal modulo [!UICONTROL Router] tramite qualsiasi altra route perché i filtri sulle altre route l&#39;hanno filtrata.

La route di fallback si distingue con un segno di freccia diverso all&#39;interno del modulo [!UICONTROL Router]:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Un caso d’uso tipico della route di fallback consiste nel continuare il flusso con una route se la condizione è soddisfatta e con un’altra route in caso contrario, come nei passaggi seguenti:

1. Inserisci un modulo [!UICONTROL Router] nello scenario.
1. Connetti entrambe le route al modulo [!UICONTROL Router].
1. Fai clic sulla prima route e specifica una condizione:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Fare clic sulla seconda route e abilitare l&#39;opzione [!UICONTROL route di fallback]:

   ![](assets/enable-fallback-route-option-350x238.png)
