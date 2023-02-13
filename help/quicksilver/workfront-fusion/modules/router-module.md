---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo router in Adobe Workfront Fusion
description: Il modulo Router consente di suddividere il flusso in più percorsi ed elaborare i dati all'interno di ogni percorso in modo diverso. Una volta che un modulo Router riceve un bundle, lo inoltra a ogni route connessa nell'ordine in cui le route sono state collegate al modulo Router.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!UICONTROL Router] modulo in [!DNL Adobe Workfront Fusion]

La [!UICONTROL Router] Il modulo ti consente di suddividere il flusso in più percorsi ed elaborare i dati all’interno di ogni percorso in modo diverso. Una volta [!UICONTROL Router] Il modulo riceve un bundle, lo inoltra a ogni rotta collegata nell&#39;ordine in cui le rotte sono state collegate al [!UICONTROL Router] modulo .

>[!NOTE]
>
>* Per verificare l&#39;ordine delle route, puoi fare clic sul pulsante [!UICONTROL Allineamento automatico] icona, che organizza i percorsi in base all&#39;ordine dall&#39;alto verso il basso.
>
>  Per modificare l’ordine, rimuovere la [!UICONTROL Router] e ricollega le route nell&#39;ordine desiderato.
>
>* I percorsi vengono elaborati in sequenza, non in parallelo. Un bundle viene inviato alla route successiva solo dopo essere stato completamente elaborato dalla route precedente.
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

## Aggiunta di un [!UICONTROL Router] modulo a uno scenario

A [!UICONTROL Router] può essere aggiunto a uno scenario in uno dei seguenti modi:

* Se desideri collegare il [!UICONTROL Router] modulo dopo un modulo, fare clic sulla maniglia destra del modulo, iniziare a digitare **[!UICONTROL router]** per cercare, quindi scegliere **[!UICONTROL Controllo del flusso]** > **[!UICONTROL Router]** nell’elenco dei moduli visualizzati.

   ![](assets/connect-the-router-350x108.png)

* Se desideri inserire il [!UICONTROL Router] modulo tra due moduli, fare clic sull&#39;icona chiave sotto la rotta che collega i due moduli (o fare clic con il pulsante destro del mouse sulla rotta) e scegliere **[!UICONTROL Aggiungere un router]** dal menu.

   ![](assets/insert-router-350x191.png)

* È possibile inserire un [!UICONTROL Router] modulo automaticamente. Ad esempio, nell’immagine seguente, per collegare il modulo nell’angolo in basso a destra a quello nell’angolo in alto a sinistra (già collegato a quello nell’angolo in alto a destra), trascina la maniglia sinistra del modulo in basso a destra e rilasciala sul modulo in alto a sinistra.

   ![](assets/insert-router-automatically-350x379.png)

## Filtri

Puoi inserire un filtro su una route dopo la [!UICONTROL Router] modulo per filtrare i bundle come su qualsiasi altro percorso:

1. Fare clic su uno dei punti del percorso.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. In **[!UICONTROL Impostare un filtro]** casella visualizzata, aggiungere condizioni, quindi fare clic su **[!UICONTROL OK]** per salvare la configurazione del filtro.

   ![](assets/set-up-a-filter-2-350x242.png)

Per ulteriori informazioni, consulta [Aggiungi un filtro a uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Il percorso di fallback

Impostazione del filtro su una route dopo un [!UICONTROL Router] il modulo contiene un&#39;opzione speciale: Il percorso di fallback:

![](assets/fallback-route-350x260.png)

Quando abilitato, questo percorso viene utilizzato nel caso in cui un bundle non possa continuare dal [!UICONTROL Router] modulo tramite qualsiasi altra route perché i filtri sugli altri percorsi l&#39;hanno filtrata.

Il percorso di fallback si distingue con un segno di freccia diverso all’interno del [!UICONTROL Router] modulo:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Un caso d’uso tipico della rotta di fallback è quello di continuare il flusso con una rotta se la condizione è soddisfatta e con un’altra rotta se non lo è, come nei seguenti passaggi:

1. Inserisci un [!UICONTROL Router] nel tuo scenario.
1. Collegare entrambe le rotte al [!UICONTROL Router] modulo .
1. Fai clic sul primo percorso e specifica una condizione:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Fai clic sul secondo percorso e abilita [!UICONTROL percorso di fallback] opzione:

   ![](assets/enable-fallback-route-option-350x238.png)
